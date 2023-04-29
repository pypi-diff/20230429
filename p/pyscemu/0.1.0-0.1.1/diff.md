# Comparing `tmp/pyscemu-0.1.0.tar.gz` & `tmp/pyscemu-0.1.1.tar.gz`

## Comparing `pyscemu-0.1.0.tar` & `pyscemu-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.0/pyproject.toml
--rw-r--r--   0     1000     1000    22868 2023-04-29 13:13:41.000000 pyscemu-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-04-28 22:05:08.000000 pyscemu-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 pyscemu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000     9611 2023-04-29 18:27:14.000000 pyscemu-0.1.1/README.md
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.1/examples/xloader_dexor.py
+-rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.1/examples/xloader_keygen.py
+-rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.1/pyproject.toml
+-rw-r--r--   0     1000     1000    24020 2023-04-29 18:27:36.000000 pyscemu-0.1.1/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-04-29 18:27:36.000000 pyscemu-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     9937 1970-01-01 00:00:00.000000 pyscemu-0.1.1/PKG-INFO
```

### Comparing `pyscemu-0.1.0/src/lib.rs` & `pyscemu-0.1.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 #[pyclass]
 struct Emu {
     emu: libscemu::emu::Emu,
 }
 
 #[pymethods]
 impl Emu {
+
+    /// reset the instruction counter to zero.
+    fn reset_pos(&mut self) {
+        self.emu.pos = 0;
+    }
    
     /// check if the emulator is in 64bits mode
     fn is_64bits(&self) -> PyResult<bool> {
         return Ok(self.emu.cfg.is_64bits);
     }
 
     /// check if the emulator is in 32bits mode
@@ -88,28 +93,30 @@
     }
 
 
     /// when the execution reached a specified amount of steps will spawn an interactive console.
     fn spawn_console_at_pos(&mut self, position:u64) {
         //self.emu.cfg.console = true;
         //self.emu.cfg.console_num = position;
+        self.emu.cfg.console_enabled = true;
         self.emu.spawn_console_at(position);
     }
 
     /// when the execution reached a specified address will spawn an interactive console.
     fn spawn_console_at_addr(&mut self, addr:u64) {
         self.emu.cfg.console2 = true;
         self.emu.cfg.console_addr = addr;
     }
 
     /// disable the console spawning.
     fn disable_spawn_console_at_pos(&mut self) {
         self.emu.cfg.console_num = 0;
     }
-    
+   
+    /// allow to enable the console if its needed.
     fn enable_console(&mut self) {
         self.emu.cfg.console_enabled = true;
     }
 
     fn disable_console(&mut self) {
         self.emu.cfg.console_enabled = false;
     }
@@ -297,15 +304,14 @@
     }*/
 
     /// start emulating the binary after finding the first return.
     fn run_until_return(&mut self) {
         self.emu.run_until_ret();
     }
 
-
     /// emulate a single step, this is slower than run(address) or run(0)
     fn step(&mut self) -> PyResult<bool> {
         return Ok(self.emu.step());
     }
 
     /// start emulating the binary until reach the provided end_addr. Use run(0) for emulating forever.
     fn run(&mut self, end_addr:u64) {
@@ -313,14 +319,41 @@
     }
 
     /// read the number of instructions emulated since now.
     fn get_position(&mut self) -> PyResult<u64> {
         return Ok(self.emu.pos);
     }
 
+    /// call a 32bits function, internally pushes params in reverse order.
+    fn call32(&mut self, address:u64, params:Vec<u32>) -> PyResult<u32> {
+        for i in (0..params.len()).rev() {
+            self.emu.stack_push32(params[i]);
+        }
+        let ret_addr = self.emu.regs.get_eip();
+        self.emu.stack_push32(ret_addr as u32);
+        self.emu.regs.set_eip(address);
+        //self.emu.set_eip(address, false);
+        self.emu.run(ret_addr);
+        return Ok(self.emu.regs.get_eax() as u32);
+    }
+
+    /// call a 64bits function, internally pushes params in reverse order.
+    fn call64(&mut self, address:u64, params:Vec<u64>) -> PyResult<u64> {
+        for i in (0..params.len()).rev() {
+            self.emu.stack_push64(params[i]);
+        }
+        let ret_addr = self.emu.regs.rip;
+        //self.emu.stack_push64(ret_addr);
+        self.emu.set_eip(address, false);
+        self.emu.run(ret_addr);
+        return Ok(self.emu.regs.rax);
+    }
+
+    // registers
+
     /// read register value ie get_reg('rax')
     fn get_reg(&mut self, reg:&str) -> PyResult<u64> {
         if self.emu.regs.is_reg(reg) {
             return Ok(self.emu.regs.get_by_name(reg));
         }
         return Err(PyValueError::new_err("invalid register name"));
     }
@@ -482,26 +515,24 @@
     }
 
     /// write a wide string on memory.
     pub fn write_wide_string(&mut self, to:u64, from:&str) {
         self.emu.maps.write_wide_string(to, from);
     }
 
-    /// write a python bytearray to the emulator memory.
+    /// write a python list of bytes to the emulator memory.
     pub fn write_buffer(&mut self, to:u64, from:&[u8]) {
         self.emu.maps.write_buffer(to, from);
     }
 
-    /// read a buffer from the emulator memory to a python bytearray.
+    /// read a buffer from the emulator memory to a python list of bytes.
     pub fn read_buffer(&mut self, from:u64, sz:usize) -> PyResult<Vec<u8>> {
-        //TODO: test the type of data returned
         return Ok(self.emu.maps.read_buffer(from, sz));
     }
 
-
     /// print all the maps that match a substring of the keyword provided.
     pub fn print_maps_by_keyword(&self, kw:&str) {
         self.emu.maps.print_maps_keyword(kw);
     }
 
     /// print all the memory maps on the process address space.
     pub fn print_maps(&self) {
```

### Comparing `pyscemu-0.1.0/Cargo.lock` & `pyscemu-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

