# Comparing `tmp/SAPsim-1.0.2.tar.gz` & `tmp/SAPsim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.2.tar", last modified: Wed Apr 26 02:07:09 2023, max compression
+gzip compressed data, was "SAPsim-1.0.3.tar", last modified: Sat Apr 29 00:55:03 2023, max compression
```

## Comparing `SAPsim-1.0.2.tar` & `SAPsim-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 02:07:00.000000 SAPsim-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 02:07:09.522108 SAPsim-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-26 02:07:00.000000 SAPsim-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 02:07:00.000000 SAPsim-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:07:09.522108 SAPsim-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-26 02:07:00.000000 SAPsim-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:55:03.534177 SAPsim-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 00:54:53.000000 SAPsim-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-29 00:55:03.530177 SAPsim-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-29 00:54:53.000000 SAPsim-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:55:03.526178 SAPsim-1.0.3/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:55:03.530177 SAPsim-1.0.3/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-29 00:54:53.000000 SAPsim-1.0.3/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:55:03.526178 SAPsim-1.0.3/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-29 00:55:03.000000 SAPsim-1.0.3/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-29 00:55:03.000000 SAPsim-1.0.3/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:55:03.000000 SAPsim-1.0.3/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 00:55:03.000000 SAPsim-1.0.3/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 00:55:03.000000 SAPsim-1.0.3/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-29 00:54:53.000000 SAPsim-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:55:03.534177 SAPsim-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-29 00:54:53.000000 SAPsim-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:55:03.530177 SAPsim-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/test_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-29 00:54:53.000000 SAPsim-1.0.3/tests/test_run.py
```

### Comparing `SAPsim-1.0.2/LICENSE` & `SAPsim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.2/PKG-INFO` & `SAPsim-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -28,42 +28,39 @@
 
 <p align="center">
     <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
-Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
+`pip install SAPsim`
 
-Next, install SAPsim.
-
-```sh
-pip install SAPsim
-```
+Your Python version needs to be 3.9+. Check with `python --version`. If `python` doesn't work, try `python3`.
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
 Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
-from SAPsim import run
-
-run("path/to/your/SAP/program.csv")                 # run at full speed (default)
-run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+>>> from SAPsim import run
+>>> run("path/to/your/SAP/program.csv")                 # run at full speed (default)
+...
+>>> run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+...
 ```
 
 Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easy to just mimic the example programs [above](#usage).
+It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog).
 But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.2/README.md` & `SAPsim-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,42 +8,39 @@
 
 <p align="center">
     <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
-Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
+`pip install SAPsim`
 
-Next, install SAPsim.
-
-```sh
-pip install SAPsim
-```
+Your Python version needs to be 3.9+. Check with `python --version`. If `python` doesn't work, try `python3`.
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
 Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
-from SAPsim import run
-
-run("path/to/your/SAP/program.csv")                 # run at full speed (default)
-run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+>>> from SAPsim import run
+>>> run("path/to/your/SAP/program.csv")                 # run at full speed (default)
+...
+>>> run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+...
 ```
 
 Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easy to just mimic the example programs [above](#usage).
+It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog).
 But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.2/SAPsim/__init__.py` & `SAPsim-1.0.3/SAPsim/__init__.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.2/SAPsim/utils/exceptions.py` & `SAPsim-1.0.3/SAPsim/utils/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 """Custom exceptions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
+from pathlib import Path
 import SAPsim.utils.helpers as helpers
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 
 
 def print_debug_info() -> None:
     """When most Exceptions (not DroppedOffBottom) occur, this function is called to print the instruction that caused the Exception and program state (RAM and registers and flags)"""
-    curr_instruction = globs.RAM[globs.PC]
+    curr_instruction = global_vars.RAM[global_vars.PC]
     print(
-        f"Exception raised during execution of {globs.OPCODE_TO_MNEMONIC[helpers.parse_opcode(curr_instruction)]} {helpers.parse_arg(curr_instruction)} at address {globs.PC}"
+        f"Exception raised during execution of {global_vars.MNEMONIC_TO_OPCODE.inverse[helpers.parse_opcode(curr_instruction)]} {helpers.parse_arg(curr_instruction)} at address {global_vars.PC}"
     )
     helpers.print_RAM(dispPC=True)
     helpers.print_info()
 
 
 class ARegisterNotEnoughBits(Exception):
     """The unsigned value in register A can't be stored in NUM_BITS_IN_REGISTERS bits."""
 
     def __init__(self):
-        self.message = f"The unsigned value in register A can't be stored in {globs.NUM_BITS_IN_REGISTERS} bits."
+        self.message = f"The unsigned value in register A can't be stored in {global_vars.NUM_BITS_IN_REGISTERS} bits."
         print_debug_info()
         super().__init__(self.message)
 
 
 class BRegisterNotEnoughBits(Exception):
     """The unsigned value in register B can't be stored in NUM_BITS_IN_REGISTERS bits."""
 
     def __init__(self):
-        self.message = f"The unsigned value in register B can't be stored in {globs.NUM_BITS_IN_REGISTERS} bits."
+        self.message = f"The unsigned value in register B can't be stored in {global_vars.NUM_BITS_IN_REGISTERS} bits."
         print_debug_info()
         super().__init__(self.message)
 
 
 class ARegisterNegativeInt(Exception):
     """There's somehow a negative number in unsigned register A."""
 
     def __init__(self):
         self.message = (
-            f"There's somehow a negative number {globs.A} in unsigned register A."
+            f"There's somehow a negative number {global_vars.A} in unsigned register A."
         )
         print_debug_info()
         super().__init__(self.message)
 
 
 class BRegisterNegativeInt(Exception):
     """There's somehow a negative number in unsigned register B."""
 
     def __init__(self):
         self.message = (
-            f"There's somehow a negative number {globs.B} in unsigned register B."
+            f"There's somehow a negative number {global_vars.B} in unsigned register B."
         )
         print_debug_info()
         super().__init__(self.message)
 
 
 class DroppedOffBottom(Exception):
     """Raised if ``PC`` > max address in ``RAM``."""
@@ -69,33 +70,34 @@
         super().__init__(self.message)
 
 
 class LoadFromUnmappedAddress(Exception):
     """Raised if attempting to Mem(addr), but Addr is not mapped."""
 
     def __init__(self):
-        self.message = f"Attempted to load from unmapped address {globs.PC}."
+        self.message = f"Attempted to load from unmapped address {global_vars.PC}."
         print_debug_info()
         super().__init__(self.message)
 
 
 class JumpToNegativeAddress(Exception):
     def __init__(self, message=f"Attempted to jump to a negative address."):
         self.message = message
         print_debug_info()
         super().__init__(self.message)
 
 
-class InvalidFileExtension(Exception):
+class FileNotCSV(Exception):
     def __init__(
         self,
-        path,
-        message=f"Invalid file extension for prog positional argument. Must be .csv",
+        path: Path,
+        message=f"Invalid filepath provided. Extension must be .csv",
     ):
         self.message = message
+        self.message += f"\nYou provided the filepath: {path}"
         super().__init__(self.message)
 
 
 class RowWithNoAddress(Exception):
     def __init__(self, row):
         self.message = f"There's a row with no address value in row {row} of your program!\nNote: In Excel, this row might just appear empty, which is normally fine. But open up the .csv in a text editor and you'll see that there is a row with 2 commas but no address value."
         super().__init__(self.message)
@@ -121,23 +123,27 @@
 
 class DuplicateAddress(Exception):
     def __init__(self, address):
         self.message = f"Address {address} is duplicated in your program!"
         super().__init__(self.message)
 
 
-class MnemonicButNoArg(Exception):
+class NoSecondHexit(Exception):
     def __init__(self, address):
-        self.message = f"Address {address} of your program has a Mnemonic but no Arg!"
+        self.message = (
+            f"Address {address} of your program has a First Hexit but no Second Hexit!"
+        )
         super().__init__(self.message)
 
 
-class ArgButNoMnemonic(Exception):
+class NoFirstHexit(Exception):
     def __init__(self, address):
-        self.message = f"Address {address} of your program has an Arg but no Mnemonic!"
+        self.message = (
+            f"Address {address} of your program has an Second Hexit but no First Hexit!"
+        )
         super().__init__(self.message)
 
 
 class FirstHexitNegative(Exception):
     def __init__(self, address):
         self.message = (
             f"The first hexit at address {address} of your program must be positive!"
@@ -163,33 +169,27 @@
     def __init__(self, address):
         self.message = f"The second hexit at address {address} of your program must be less than 16!"
         super().__init__(self.message)
 
 
 class InvalidFirstHexit(Exception):
     def __init__(self, address):
-        self.message = f"The first hexit at address {address} is not valid! Must be a hexit 0 to f or a base-10 integer 0 to 15 representing a hexit. You typed one letter in this field, so I assume you meant to put a hexit here, not a Mnemonic."
-        super().__init__(self.message)
-
-
-class InvalidMnemonic(Exception):
-    def __init__(self, address):
-        self.message = f"The mnemonic given at address {address} is invalid. See SAP instruction set for list of supported mnemonics. The mnemonic field can also be a hexit 0 to f if representing data."
+        self.message = f"The First Hexit given at address {address} is invalid. See SAP instruction set for list of supported mnemonics. The First Hexit field can also be a hexit 0 to f if representing data."
         super().__init__(self.message)
 
 
-class InvalidArg(Exception):
+class InvalidSecondHexit(Exception):
     def __init__(self, address):
-        self.message = f"The arg at address {address} is invalid. It must be a hexit 0 to f or a base-10 integer 0 to 15 representing a hexit."
+        self.message = f"The Second Hexit at address {address} is invalid. It must be a hexit 0 to f or a base-10 integer 0 to 15 representing a hexit."
         super().__init__(self.message)
 
 
 class MoreThan16MappedAddresses(Exception):
     def __init__(self):
-        self.message = f"A SAP program can have at most 16 addresses! In this simulation, a skipped address doesn't count toward that count. Excluding skipped addresses, you have {len(globs.RAM)} mapped addresses."
+        self.message = f"A SAP program can have at most 16 addresses! In this simulation, a skipped address doesn't count toward that count. Excluding skipped addresses, you have {len(global_vars.RAM)} mapped addresses."
         super().__init__(self.message)
 
 
 class InstructionRequiresArg(Exception):
     def __init__(self, instruction: str):
         self.message = f"You typed: {instruction}. Only NOP, OUT, and HLT strings have an unnecessary Arg (but there's still a hexit for the arg)."
         super().__init__(self.message)
```

### Comparing `SAPsim-1.0.2/SAPsim/utils/execute.py` & `SAPsim-1.0.3/SAPsim/utils/execute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 """Execute instructions in RAM."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from pathlib import Path
 from typing import Any
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 import SAPsim.utils.instructions as instructions
 import SAPsim.utils.helpers as helpers
 from SAPsim.utils.helpers import is_documented_by
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.parser as parser
 
 
 def execute_full_speed() -> None:
     """Execute instructions in ``RAM`` at full speed until ``EXECUTING`` is ``False`` or ``PC > max addr``."""
     max_addr: int = 0
-    if globs.RAM.keys():
-        max_addr = max(globs.RAM.keys())
-    while globs.EXECUTING:
+    if global_vars.RAM.keys():
+        max_addr = max(global_vars.RAM.keys())
+    while global_vars.EXECUTING:
         # Check that RAM is non-empty.
-        if globs.RAM.keys() and globs.PC > max_addr:
-            globs.EXECUTING = False
+        if global_vars.RAM.keys() and global_vars.PC > max_addr:
+            global_vars.EXECUTING = False
             raise exceptions.DroppedOffBottom
 
         # If we're executing an empty address but it's not a DroppedOffBottom, just skip and don't execute
-        if globs.PC not in globs.RAM:
-            globs.PC += 1
+        if global_vars.PC not in global_vars.RAM:
+            global_vars.PC += 1
             continue
 
         instructions.OPCODE_TO_INSTR_PROCEDURE[
-            helpers.parse_opcode(globs.RAM[globs.PC])
-        ](helpers.parse_arg(globs.RAM[globs.PC]))
+            helpers.parse_opcode(global_vars.RAM[global_vars.PC])
+        ](helpers.parse_arg(global_vars.RAM[global_vars.PC]))
 
 
 def execute_next() -> None:
     """Execute a single instruction at the current ``PC`` value if ``EXECUTING``. If attempting to execute an empty address, ``PC += 1`` (i.e., doesn't skip to next filled address)."""
-    if globs.EXECUTING:
-        if globs.RAM.keys() and globs.PC > max(globs.RAM.keys()):
-            globs.EXECUTING = False
+    if global_vars.EXECUTING:
+        if global_vars.RAM.keys() and global_vars.PC > max(global_vars.RAM.keys()):
+            global_vars.EXECUTING = False
             raise exceptions.DroppedOffBottom
 
         # If executing an empty address, just skip and don't execute
-        if globs.PC not in globs.RAM:
-            globs.PC += 1
+        if global_vars.PC not in global_vars.RAM:
+            global_vars.PC += 1
         else:
             instructions.OPCODE_TO_INSTR_PROCEDURE[
-                helpers.parse_opcode(globs.RAM[globs.PC])
-            ](helpers.parse_arg(globs.RAM[globs.PC]))
+                helpers.parse_opcode(global_vars.RAM[global_vars.PC])
+            ](helpers.parse_arg(global_vars.RAM[global_vars.PC]))
 
 
 def run(prog_path: str, **kwargs) -> None:
     r"""Run given .csv program in SAPsim format.
 
     :param prog_path:
         .csv file in SAPsim format.
@@ -64,67 +64,78 @@
             * Default is full speed
         * *change* (``str``) --
             * Comma-separated list of changes to RAM
             * Format: <addr>:<base-10 value>,<addr>:<base-10 value>,...
             * The value at each address will be overwritten to that base-10 value
             * Useful for debugging programs (edit a value without changing CSV)
             * Also useful for autograding programs (overwrite a reserved instruction/data value)
-        * *table_fmt* (``str``) --
+        * *table_format* (``str``) --
             * Table format
             * Options: https://github.com/astanin/python-tabulate#table-format
             * Default value is "simple_outline"
         * *bits* (``int``) --
             * Number of bits in unsigned registers
             * Default 8
     :return: ``None``
     """
+    if not isinstance(prog_path, str):
+        raise TypeError("Required parameter prog_path must be a str.")
+    if "debug" in kwargs and not isinstance(kwargs["debug"], bool):
+        raise TypeError("Keyword argument debug must be a bool.")
+    if "change" in kwargs and not isinstance(kwargs["change"], str):
+        raise TypeError("Keyword argument change must be a str.")
+    if "table_format" in kwargs and not isinstance(kwargs["table_format"], str):
+        raise TypeError("Keyword argument table_format must be a str.")
+    if "bits" in kwargs and not isinstance(kwargs["bits"], int):
+        raise TypeError("Keyword argument bits must be an int.")
+
     path: Path = Path(prog_path)
-    assert path.suffix == ".csv"
+    if not path.suffix == ".csv":
+        raise exceptions.FileNotCSV(path)
     helpers.setup_8bit()
     parser.parse_csv(path)
     if "bits" in kwargs:
-        assert int(kwargs["bits"]) > 1
-        globs.NUM_BITS_IN_REGISTERS = int(kwargs["bits"])
-        globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**globs.NUM_BITS_IN_REGISTERS - 1
+        assert kwargs["bits"] > 1
+        global_vars.NUM_BITS_IN_REGISTERS = kwargs["bits"]
     if "change" in kwargs:
         changes = kwargs["change"].split(",")
         for change in changes:
             if change.count(":") != 1:
                 print(
-                    "Invalid syntax for --c option, correct format is <addr>:<base-10 value>,<addr>:<base-10 value>, ..."
+                    "Invalid syntax for change parameter, correct format is <addr>:<base-10 value>, <addr>:<base-10 value>, ..."
                 )
                 exit(1)
             change = change.strip()
             colon_position = change.find(":")
             addr = int(change[:colon_position])
-            if addr not in globs.RAM:
+            if addr not in global_vars.RAM:
                 print(
                     f"You can apply a change only to an address that's already mapped (not skipped). Address {addr} is not mapped."
                 )
                 exit(1)
             value = int(change[colon_position + 1 :])
-            if value < 0 or value > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
+            if value < 0 or value > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
                 print(
                     f"Invalid base-10 value for change: {value}. Negative or overflows registers."
                 )
                 exit(1)
-            globs.RAM[addr] = value
-    if "table_fmt" in kwargs:
-        globs.table_fmt = kwargs["table_fmt"]
+            global_vars.RAM[addr] = value
+    if "table_format" in kwargs:
+        global_vars.table_format = kwargs["table_format"]
     if "debug" in kwargs and kwargs["debug"]:
         print(f"Initial state of simulation of {prog_path}")
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Debug mode: press Enter to execute next instruction ( > ).")
         input()
-        while globs.EXECUTING:
+        while global_vars.EXECUTING:
             # Special case so that you don't have to press Enter twice to halt on a HLT instruction
             if (
-                globs.PC in globs.RAM
-                and helpers.parse_opcode(globs.RAM[globs.PC]) == 0xF
+                global_vars.PC in global_vars.RAM
+                and helpers.parse_opcode(global_vars.RAM[global_vars.PC]) == 0xF
             ):
                 execute_next()
                 break
             execute_next()
             helpers.print_RAM(dispPC=True)
             helpers.print_info()
             input()
```

### Comparing `SAPsim-1.0.2/SAPsim/utils/globs.py` & `SAPsim-1.0.3/SAPsim/utils/global_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Global variables.
 
 If changing anything in this file, also modify SAPsim/__init__.py."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
+from bidict import bidict
+
 RAM = {}
 """``dict[int, int]`` mapping ``PC``:``byte``, where ``byte`` can be instruction or data (indistinguishable, mostly)"""
 PC: int = 0
 """Program counter that indexes into ``RAM``, default value 0"""
 A: int = 0
 """Register A, default value 0"""
 B: int = 0
@@ -20,46 +22,37 @@
 Lab 3's ALU has default value True (1) for FlagZ because the results register is initially 0.
 
 However, it makes more sense in the simulation to set it to False by default."""
 # Number of bits in registers
 # Same as number of full adders
 # This affects how FLAG_C, FLAG_Z, and result register work
 NUM_BITS_IN_REGISTERS: int = 8
-"""IMPORTANT NOTE: If changing this value, then also change ``MAX_UNSIGNED_VAL_IN_REGISTERS``!!! This variable is the #bits in registers and affects how everything works. Default is 8."""
-MAX_UNSIGNED_VAL_IN_REGISTERS = 2**NUM_BITS_IN_REGISTERS - 1
-"""This value needs to be changed whenever NUM_BITS_IN_REGISTERS is changed!"""
+"""This variable is the #bits in registers and affects how ``add``, ``sub``, ``ldi``, and ``lda`` work.
+Default value is 8."""
 EXECUTING: bool = True
 """Is the program executing? Set to ``False`` by ``hlt()``"""
 
-MNEMONIC_TO_OPCODE = {
-    "NOP": 0,
-    "LDA": 1,
-    "ADD": 2,
-    "SUB": 3,
-    "STA": 4,
-    "LDI": 5,
-    "JMP": 6,
-    "JC": 7,
-    "JZ": 8,
-    "OUT": 14,
-    "HLT": 15,
-}
-"""Maps ``str mnemonic : int opcode``. All mnemonics in this dict are in all caps."""
-
-OPCODE_TO_MNEMONIC = {
-    0: "NOP",
-    1: "LDA",
-    2: "ADD",
-    3: "SUB",
-    4: "STA",
-    5: "LDI",
-    6: "JMP",
-    7: "JC",
-    8: "JZ",
-    14: "OUT",
-    15: "HLT",
-}
-"""Maps ``int opcode : str mnemonic``"""
+MNEMONIC_TO_OPCODE: bidict = bidict(
+    {
+        "NOP": 0,
+        "LDA": 1,
+        "ADD": 2,
+        "SUB": 3,
+        "STA": 4,
+        "LDI": 5,
+        "JMP": 6,
+        "JC": 7,
+        "JZ": 8,
+        "OUT": 14,
+        "HLT": 15,
+    }
+)
+
+"""Bidirectional dictionary mapping ``str mnemonic : int opcode``.
+
+Use ``MNEMONIC_TO_OPCODE.inverse[opcode]`` to get mnemonic from opcode.
+
+All mnemonics in this dict are in all caps."""
 
-table_fmt: str = "simple_outline"
+table_format: str = "simple_outline"
 """Tabulate ``table_fmt`` arg to customize pretty-printing. Defaults to ``simple_outline``, see all options: https://github.com/astanin/python-tabulate#table-
                         format"""
```

### Comparing `SAPsim-1.0.2/SAPsim/utils/helpers.py` & `SAPsim-1.0.3/SAPsim/utils/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Miscellaneous helper functions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 
 from tabulate import tabulate
 from typing import Any
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 import SAPsim.utils.exceptions as exceptions
 
 
 def is_documented_by(
     original, lines_to_remove: int = 0, prepend: str = "", append: str = ""
 ):
     r"""Use for wrapper functions that should have the original function's docstring.
@@ -72,28 +72,28 @@
 
     For NOP, OUT, and HLT, if an Arg is not given, then the right hexit will just be 0.
 
     Haven't yet tested exception handling."""
     if " " not in instruction:
         if len(instruction) != 3 or instruction.upper() not in {"NOP", "OUT", "HLT"}:
             raise exceptions.InstructionRequiresArg(instruction)
-        return globs.MNEMONIC_TO_OPCODE[instruction.upper()] << 4
+        return global_vars.MNEMONIC_TO_OPCODE[instruction.upper()] << 4
     space_position = instruction.find(" ")
     if len(instruction) != (space_position + 2) and len(instruction) != (
         space_position + 3
     ):
         raise exceptions.InvalidInstructionString(instruction)
     if (
         int(instruction[space_position + 1 :]) < 0
         or int(instruction[space_position + 1 :]) >= 16
     ):
         raise exceptions.InvalidInstructionString(instruction)
-    return (globs.MNEMONIC_TO_OPCODE[instruction[:space_position].upper()] << 4) | int(
-        instruction[space_position + 1 :]
-    )
+    return (
+        global_vars.MNEMONIC_TO_OPCODE[instruction[:space_position].upper()] << 4
+    ) | int(instruction[space_position + 1 :])
 
 
 @is_documented_by(
     instruction_to_byte,
     0,
     ""
     r"""
@@ -103,55 +103,55 @@
 def i2b(instruction: str) -> int:
     return instruction_to_byte(instruction)
 
 
 def print_RAM(**kwargs):
     """Pretty print the contents of RAM, sorted by address. | <PC (optional)> | Addr | Instruction | Dec | Hex | (since we can't distinguish instructions from data). Display arrow on current PC value if ``dispPC=True`` in kwargs. Set ``format=`` to set tabulate pretty-print format."""
     table = []
-    for addr in sorted(globs.RAM.keys()):
-        byte = globs.RAM[addr]
+    for addr in sorted(global_vars.RAM.keys()):
+        byte = global_vars.RAM[addr]
         opcode = parse_opcode(byte)
         arg = parse_arg(byte)
         instruction_str = (
-            (globs.OPCODE_TO_MNEMONIC[opcode] + " " + str(arg))
-            if opcode in globs.OPCODE_TO_MNEMONIC
+            (global_vars.MNEMONIC_TO_OPCODE.inverse[opcode] + " " + str(arg))
+            if opcode in global_vars.MNEMONIC_TO_OPCODE.inverse
             else "Invalid Opcode"
         )
         table_row = []
         if "dispPC" in kwargs and kwargs["dispPC"]:
-            table_row.append(">" if globs.PC == addr else "")
+            table_row.append(">" if global_vars.PC == addr else "")
         table_row.extend([addr, instruction_str, byte, pad_hex(hex(byte), 2)])
         table.append(table_row)
     headers = []
     if "dispPC" in kwargs and kwargs["dispPC"]:
         headers.append("PC")
     headers.extend(["Addr", "Instruction", "Dec", "Hex"])
-    print(tabulate(table, headers=headers, tablefmt=globs.table_fmt))
+    print(tabulate(table, headers=headers, tablefmt=global_vars.table_format))
 
 
 def print_info(**kwargs):
     """Print the values of everything in global_vars.py except RAM. Set optional parameter ``bool=True`` to print flags as ``bool`` instead of ``int``. Set ``format=`` for tabulate pretty-print format."""
     table = [
-        ["PC", globs.PC],
-        ["Reg A", globs.A],
-        ["Reg B", globs.B],
+        ["PC", global_vars.PC],
+        ["Reg A", global_vars.A],
+        ["Reg B", global_vars.B],
         [
             "FlagC",
-            globs.FLAG_C
+            global_vars.FLAG_C
             if ("bool" in kwargs and kwargs["bool"])
-            else int(globs.FLAG_C),
+            else int(global_vars.FLAG_C),
         ],
         [
             "FlagZ",
-            globs.FLAG_Z
+            global_vars.FLAG_Z
             if ("bool" in kwargs and kwargs["bool"])
-            else int(globs.FLAG_Z),
+            else int(global_vars.FLAG_Z),
         ],
     ]
-    print(tabulate(table, tablefmt=globs.table_fmt))
+    print(tabulate(table, tablefmt=global_vars.table_format))
 
 
 def pad_hex(hex: str, width: int):
     """Pad given hex str with 0x prefix to width hexits. That is, 0x prefix not included in the width."""
     return "0x" + hex[2:].zfill(width)
 
 
@@ -161,83 +161,80 @@
     for key in dict:
         rv[key] = dict[key]
     return rv
 
 
 def setup_4bit():
     """Sets up the 4-bit environment and resets global variables to default values."""
-    globs.NUM_BITS_IN_REGISTERS = 4
-    globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**4 - 1
+    global_vars.NUM_BITS_IN_REGISTERS = 4
     reset_globals()
 
 
 def setup_8bit():
     """Sets up the 8-bit environment and resets global variables to default values."""
-    globs.NUM_BITS_IN_REGISTERS = 8
-    globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**8 - 1
+    global_vars.NUM_BITS_IN_REGISTERS = 8
     reset_globals()
 
 
 def setup_n_bit(n: int):
     """Sets up the n-bit environment and resets global variables to default values."""
     assert n > 1
-    globs.NUM_BITS_IN_REGISTERS = n
-    globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**n - 1
+    global_vars.NUM_BITS_IN_REGISTERS = n
     reset_globals()
 
 
 def reset_globals():
-    """Reset global variables (not ``NUM_BITS_IN_REGISTERS`` and ``MAX_UNSIGNED_VAL_IN_REGISTERS`` to default values."""
-    globs.RAM = {}
-    globs.PC = 0
-    globs.A = 0
-    globs.B = 0
-    globs.FLAG_C = False
-    globs.FLAG_Z = False
-    globs.EXECUTING = True
+    """Reset global variables (not ``NUM_BITS_IN_REGISTERS``) to default values."""
+    global_vars.RAM = {}
+    global_vars.PC = 0
+    global_vars.A = 0
+    global_vars.B = 0
+    global_vars.FLAG_C = False
+    global_vars.FLAG_Z = False
+    global_vars.EXECUTING = True
 
 
 def get_state() -> dict[str, Any]:
     """Return a dict of global variables and their values.
     Mostly used in testing functions."""
     return {
-        "RAM": globs.RAM,
-        "PC": globs.PC,
-        "A": globs.A,
-        "B": globs.B,
-        "FLAG_C": globs.FLAG_C,
-        "FLAG_Z": globs.FLAG_Z,
-        "EXECUTING": globs.EXECUTING,
+        "RAM": global_vars.RAM,
+        "PC": global_vars.PC,
+        "A": global_vars.A,
+        "B": global_vars.B,
+        "FLAG_C": global_vars.FLAG_C,
+        "FLAG_Z": global_vars.FLAG_Z,
+        "EXECUTING": global_vars.EXECUTING,
     }
 
 
 def check_state_all(
     RAM, PC: int, A: int, B: int, FLAG_C: bool, FLAG_Z: bool, EXECUTING: bool
 ):
     """Compare all current state variables to expected values. Mostly used in testing functions."""
-    assert RAM == globs.RAM
-    assert PC == globs.PC
-    assert A == globs.A
-    assert B == globs.B
-    assert FLAG_C == globs.FLAG_C
-    assert FLAG_Z == globs.FLAG_Z
-    assert EXECUTING == globs.EXECUTING
+    assert RAM == global_vars.RAM
+    assert PC == global_vars.PC
+    assert A == global_vars.A
+    assert B == global_vars.B
+    assert FLAG_C == global_vars.FLAG_C
+    assert FLAG_Z == global_vars.FLAG_Z
+    assert EXECUTING == global_vars.EXECUTING
 
 
 def check_state(**kwargs):
     """Compare the current state to expected values. Mostly used in testing functions.
 
     Optional parameters RAM=, PC=, A=, B=, FLAG_C=, FLAG_Z=, EXECUTING="""
     if "RAM" in kwargs:
-        assert kwargs["RAM"] == globs.RAM
+        assert kwargs["RAM"] == global_vars.RAM
     if "PC" in kwargs:
-        assert kwargs["PC"] == globs.PC
+        assert kwargs["PC"] == global_vars.PC
     if "A" in kwargs:
-        assert kwargs["A"] == globs.A
+        assert kwargs["A"] == global_vars.A
     if "B" in kwargs:
-        assert kwargs["B"] == globs.B
+        assert kwargs["B"] == global_vars.B
     if "FLAG_C" in kwargs:
-        assert kwargs["FLAG_C"] == globs.FLAG_C
+        assert kwargs["FLAG_C"] == global_vars.FLAG_C
     if "FLAG_Z" in kwargs:
-        assert kwargs["FLAG_Z"] == globs.FLAG_Z
+        assert kwargs["FLAG_Z"] == global_vars.FLAG_Z
     if "EXECUTING" in kwargs:
-        assert kwargs["EXECUTING"] == globs.EXECUTING
+        assert kwargs["EXECUTING"] == global_vars.EXECUTING
```

### Comparing `SAPsim-1.0.2/SAPsim/utils/instructions.py` & `SAPsim-1.0.3/SAPsim/utils/instructions.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 This DOES NOT exist in actual SAP but for implementation purposes, instructions that don't need an arg (i.e. NOP, OUT, HLT) get a default parameter so that they can still be called with an argument. In actual SAP, all instructions (byte) have a required Arg, not a default or optional arg.
 
 INSTRUCTIONS dict for using an opcode to call a specific function is defined at the bottom."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from tabulate import tabulate
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.helpers as helpers
 
 
 def nop(arg: int = 0) -> None:
     """Nop
 
     Opcode 0"""
-    globs.PC += 1
+    global_vars.PC += 1
 
 
 def lda(arg: int) -> None:
     """``A = Mem(arg)``
 
     Opcode 1"""
-    if arg not in globs.RAM:
+    if arg not in global_vars.RAM:
         raise exceptions.LoadFromUnmappedAddress
-    globs.A = globs.RAM[arg]
-    if globs.A > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
+    global_vars.A = global_vars.RAM[arg]
+    if global_vars.A > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
         raise exceptions.ARegisterNotEnoughBits
-    if globs.A < 0:
+    if global_vars.A < 0:
         raise exceptions.ARegisterNegativeInt
-    globs.PC += 1
+    global_vars.PC += 1
 
 
 def add(arg: int, **kwargs) -> None:
     """``A = A + Mem(arg)``. Accounts for ``NUM_BITS_IN_REGISTERS`` to set ``FLAG_C`` and ``FLAG_Z``. Handles overflow.
 
     Opcode 2
 
@@ -46,35 +46,35 @@
         memory address, usually
     kwarg
         ``direct_add``: bool
             Set to ``True`` to directly add ``arg`` (i.e. ``A = A + arg`` instead of ``A = A + Mem(arg)``), for testing purposes and use in ``sub``.
 
             This behavior does not exist in actual SAP."""
     if "direct_add" in kwargs and kwargs["direct_add"]:
-        globs.B = arg
+        global_vars.B = arg
     else:
-        if arg not in globs.RAM:
+        if arg not in global_vars.RAM:
             raise exceptions.LoadFromUnmappedAddress
-        globs.B = globs.RAM[arg]
+        global_vars.B = global_vars.RAM[arg]
 
-    if globs.B > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
+    if global_vars.B > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
         raise exceptions.BRegisterNotEnoughBits
-    if globs.B < 0:
+    if global_vars.B < 0:
         raise exceptions.BRegisterNegativeInt
 
-    globs.A += globs.B
+    global_vars.A += global_vars.B
 
-    if globs.A > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
-        globs.FLAG_C = 1
-        globs.A -= 2**globs.NUM_BITS_IN_REGISTERS
+    if global_vars.A > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
+        global_vars.FLAG_C = 1
+        global_vars.A -= 2**global_vars.NUM_BITS_IN_REGISTERS
     else:
-        globs.FLAG_C = 0
-    globs.FLAG_Z = globs.A == 0
+        global_vars.FLAG_C = 0
+    global_vars.FLAG_Z = global_vars.A == 0
 
-    globs.PC += 1
+    global_vars.PC += 1
 
 
 def sub(arg: int, **kwargs) -> None:
     """``A = A - Mem(arg)``. Accounts for ``NUM_BITS_IN_REGISTERS`` to set ``FLAG_C`` and ``FLAG_Z``. Calls ``add()`` twice to perform 2's complement subtraction.
 
     Opcode 3
 
@@ -84,115 +84,117 @@
         memory address, usually
     kwarg
         direct_sub: bool
             set to ``True`` to directly sub ``arg`` (i.e. ``A = A - arg`` instead of ``A = A - Mem(arg)``), for testing purposes.
 
             This behavior does not exist in actual SAP."""
     if "direct_sub" in kwargs and kwargs["direct_sub"]:
-        globs.B = arg
+        global_vars.B = arg
     else:
-        if arg not in globs.RAM:
+        if arg not in global_vars.RAM:
             raise exceptions.LoadFromUnmappedAddress
-        globs.B = globs.RAM[arg]
+        global_vars.B = global_vars.RAM[arg]
 
-    if globs.B > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
+    if global_vars.B > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
         raise exceptions.BRegisterNotEnoughBits
-    if globs.B < 0:
+    if global_vars.B < 0:
         raise exceptions.BRegisterNegativeInt
 
     # Clone A and B for use later in setting FlagC.
-    A_clone = globs.A
-    B_clone = globs.B
+    A_clone = global_vars.A
+    B_clone = global_vars.B
 
-    inverse_B = B_clone ^ globs.MAX_UNSIGNED_VAL_IN_REGISTERS
+    inverse_B = B_clone ^ (2**global_vars.NUM_BITS_IN_REGISTERS - 1)
 
     add(inverse_B, direct_add=True)
     add(1, direct_add=True)
 
     # add() modified globs.B, reset it
-    globs.B = B_clone
+    global_vars.B = B_clone
 
     # FLAG_Z is correct at this point.
     # FLAG_C is not correct so is explicitly handled.
     # This uses the unsigned comparison table FlagC = A >= B (compare their values before A changed)
-    globs.FLAG_C = A_clone >= B_clone
+    global_vars.FLAG_C = A_clone >= B_clone
 
     # Subtract 1 from PC since there were 2 adds that each did PC += 1
     # Net effect is globs.PC += 1
-    globs.PC -= 1
+    global_vars.PC -= 1
 
 
 def sta(arg: int) -> None:
     """``Mem(Arg) = A``. CAN store to unmapped addr, which will simply map the addr in RAM.
 
     Opcode 4"""
-    globs.RAM[arg] = globs.A
-    globs.PC += 1
+    global_vars.RAM[arg] = global_vars.A
+    global_vars.PC += 1
 
 
 def ldi(arg: int) -> None:
     """``A = arg``
 
     Opcode 5"""
-    globs.A = arg
-    if arg > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
+    global_vars.A = arg
+    if arg > (2**global_vars.NUM_BITS_IN_REGISTERS - 1):
         raise exceptions.ARegisterNotEnoughBits
     if arg < 0:
         raise exceptions.ARegisterNegativeInt
-    globs.PC += 1
+    global_vars.PC += 1
 
 
 def jmp(arg: int) -> None:
     """``PC = arg``
 
     Opcode 6"""
     if arg < 0:
         raise exceptions.JumpToNegativeAddress
-    globs.PC = arg
+    global_vars.PC = arg
 
 
 def jc(arg: int) -> None:
     """If ``FC=1`` then ``PC=arg``; else go on
 
     Opcode 7"""
-    if globs.FLAG_C:
+    if global_vars.FLAG_C:
         if arg < 0:
             raise exceptions.JumpToNegativeAddress
-        globs.PC = arg
+        global_vars.PC = arg
     else:
-        globs.PC += 1
+        global_vars.PC += 1
 
 
 def jz(arg: int) -> None:
     """If ``FZ=1`` then ``PC=arg``; else go on
 
     Opcode 8"""
-    if globs.FLAG_Z:
+    if global_vars.FLAG_Z:
         if arg < 0:
             raise exceptions.JumpToNegativeAddress
-        globs.PC = arg
+        global_vars.PC = arg
     else:
-        globs.PC += 1
+        global_vars.PC += 1
 
 
 def out(arg: int = 0) -> None:
     """``Display = OUT = A``. Prints | PC | A (dec) | A (hex) |
 
     Opcode 14"""
-    arg = helpers.parse_arg(globs.RAM[globs.PC])
-    table = [[globs.PC, globs.A, helpers.pad_hex(hex(globs.A), 2)]]
-    print(tabulate(table, headers=["PC", "Dec", "Hex"], tablefmt=globs.table_fmt))
-    globs.PC += 1
+    arg = helpers.parse_arg(global_vars.RAM[global_vars.PC])
+    table = [[global_vars.PC, global_vars.A, helpers.pad_hex(hex(global_vars.A), 2)]]
+    print(
+        tabulate(table, headers=["PC", "Dec", "Hex"], tablefmt=global_vars.table_format)
+    )
+    global_vars.PC += 1
 
 
 def hlt(arg: int = 0) -> None:
     """Halt
 
     Opcode 15"""
-    globs.EXECUTING = False
+    global_vars.EXECUTING = False
 
 
 OPCODE_TO_INSTR_PROCEDURE = {
     0: nop,
     1: lda,
     2: add,
     3: sub,
```

### Comparing `SAPsim-1.0.2/SAPsim/utils/parser.py` & `SAPsim-1.0.3/SAPsim/utils/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Parses a SAP program in the CSV format given in ``template.csv`` into ``globs.RAM``."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from csv import DictReader
 from pathlib import Path
 import SAPsim.utils.exceptions as exceptions
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 
 
 def parse_csv(file_path: Path):
     """Takes a ``.csv`` file path in ``template.csv`` format and parses it into ``RAM``."""
     prog = DictReader(open(file_path))
     num_rows = 1
     addresses = set()
@@ -30,68 +30,68 @@
             raise exceptions.NegativeAddress(num_rows)
         num_rows += 1
 
         if address in addresses:
             raise exceptions.DuplicateAddress(address)
         addresses.add(address)
 
-        # If there's an Address and no Mnemonic and no Arg in a row, insert a NOP 0 and continue parsing
-        if not row["Mnemonic"] and not row["Arg"]:
-            globs.RAM[address] = 0x00
+        # If there's an Address and no First Hexit and no Second Hexit in a row, insert a NOP 0 and continue parsing
+        if not row["First Hexit"] and not row["Second Hexit"]:
+            global_vars.RAM[address] = 0x00
             continue
-        # But if there's an Address and either only an Mnemonic or only an Arg, exception
-        elif row["Mnemonic"] and not row["Arg"]:
-            raise exceptions.MnemonicButNoArg(address)
-        elif not row["Mnemonic"] and row["Arg"]:
-            raise exceptions.ArgButNoMnemonic(address)
+        # But if there's an Address and either only an First Hexit or only an Second Hexit, exception
+        elif row["First Hexit"] and not row["Second Hexit"]:
+            raise exceptions.NoSecondHexit(address)
+        elif not row["First Hexit"] and row["Second Hexit"]:
+            raise exceptions.NoFirstHexit(address)
 
         first_hexit = 0
-        # Need to determine if the field is a base-10 int or one-letter hexit str or Mnemonic str.
-        # int() will cause a ValueError if it's a one-letter hexit str or Mnemonic str.
+        # Need to determine if the field is a base-10 int or one-letter hexit str or First Hexit str.
+        # int() will cause a ValueError if it's a one-letter hexit str or First Hexit str.
         try:
             # int() strips the str
-            first_hexit = int(row["Mnemonic"])
+            first_hexit = int(row["First Hexit"])
             # Must be a valid base-10 integer here
             if first_hexit < 0:
                 raise exceptions.FirstHexitNegative(address)
             elif first_hexit > 0xF:
                 raise exceptions.FirstHexitGreaterThan15(address)
         except ValueError:
-            # Must be a string, mnemonic or hexit
+            # Must be a string, First Hexit or hexit
             # Use strip() and upper() for some safety
-            mnemonic = row["Mnemonic"].strip().upper()
+            first_hexit = row["First Hexit"].strip().upper()
             # Must be a hex value if length is 1
-            if len(mnemonic) == 1:
+            if len(first_hexit) == 1:
                 try:
-                    first_hexit = int(mnemonic, 16)
+                    first_hexit = int(first_hexit, 16)
                 except ValueError:
                     raise exceptions.InvalidFirstHexit(address)
-            # Otherwise must be Mnemonic
+            # Otherwise must be First Hexit
             else:
-                if mnemonic not in globs.MNEMONIC_TO_OPCODE:
-                    raise exceptions.InvalidMnemonic(address)
-                first_hexit = globs.MNEMONIC_TO_OPCODE[mnemonic]
+                if first_hexit not in global_vars.MNEMONIC_TO_OPCODE:
+                    raise exceptions.InvalidFirstHexit(address)
+                first_hexit = global_vars.MNEMONIC_TO_OPCODE[first_hexit]
 
         second_hexit = 0
         try:
-            second_hexit = int(row["Arg"])
+            second_hexit = int(row["Second Hexit"])
             # Must be a base-10 integer here
             if second_hexit < 0:
                 raise exceptions.SecondHexitNegative(address)
             elif second_hexit > 0xF:
                 raise exceptions.SecondHexitGreaterThan15(address)
         except ValueError:
             # Must be a str here
             # Use strip() and upper() for some safety for a string field
-            arg = row["Arg"].strip().upper()
+            arg = row["Second Hexit"].strip().upper()
             if len(arg) != 1:
-                raise exceptions.InvalidArg(address)
+                raise exceptions.InvalidSecondHexit(address)
             try:
                 second_hexit = int(arg, 16)
             except ValueError:
-                raise exceptions.InvalidArg(address)
+                raise exceptions.InvalidSecondHexit(address)
 
         byte = first_hexit << 4 | second_hexit
-        globs.RAM[address] = byte
+        global_vars.RAM[address] = byte
 
-    if len(globs.RAM) > 16:
+    if len(global_vars.RAM) > 16:
         raise exceptions.MoreThan16MappedAddresses
```

### Comparing `SAPsim-1.0.2/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.3/SAPsim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -28,42 +28,39 @@
 
 <p align="center">
     <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
 </p>
 
 ## Install
 
-Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
+`pip install SAPsim`
 
-Next, install SAPsim.
-
-```sh
-pip install SAPsim
-```
+Your Python version needs to be 3.9+. Check with `python --version`. If `python` doesn't work, try `python3`.
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
 Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
-from SAPsim import run
-
-run("path/to/your/SAP/program.csv")                 # run at full speed (default)
-run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+>>> from SAPsim import run
+>>> run("path/to/your/SAP/program.csv")                 # run at full speed (default)
+...
+>>> run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
+...
 ```
 
 Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easy to just mimic the example programs [above](#usage).
+It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog).
 But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.2/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.3/SAPsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 SAPsim.egg-info/SOURCES.txt
 SAPsim.egg-info/dependency_links.txt
 SAPsim.egg-info/requires.txt
 SAPsim.egg-info/top_level.txt
 SAPsim/utils/__init__.py
 SAPsim/utils/exceptions.py
 SAPsim/utils/execute.py
-SAPsim/utils/globs.py
+SAPsim/utils/global_vars.py
 SAPsim/utils/helpers.py
 SAPsim/utils/instructions.py
 SAPsim/utils/parser.py
 tests/__init__.py
 tests/test_example_progs.py
 tests/test_exceptions.py
 tests/test_helpers.py
```

### Comparing `SAPsim-1.0.2/pyproject.toml` & `SAPsim-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.2/setup.py` & `SAPsim-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
+# Don't need to install pathlib because pathlib is in the standard library in 3.4+
 install_requires: list[str] = [
     "setuptools",
     "tabulate",
+    "bidict",
 ]
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
-    version="1.0.2",
+    # Check https://pypi.org/project/SAPsim/ for latest version number
+    version="1.0.3",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.2/tests/test_example_progs.py` & `SAPsim-1.0.3/tests/test_example_progs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 This code should be the same (or mostly the same, in case it's updated) as the code that autogrades Lab 4.
 If you have any questions about RESERVED/RETURN VALUE, they can be answered by reading through this.
 If you don't know the test cases your program is failing, you can very easily write a function to check it yourself. It'd probably be exactly the same as what I wrote.
 """
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-from SAPsim.utils import globs
+from pathlib import Path
+from SAPsim.utils import global_vars
 from SAPsim.utils import parser
 from SAPsim.utils.execute import execute_full_speed
 from SAPsim.utils.helpers import setup_8bit
 
 
 def clone_dict(dict):
     """Returns a deep clone of `dict`. Used to clone `RAM`."""
@@ -24,60 +25,60 @@
     """Test ex1.csv.
     RESERVED:
         14: Input 0 to 255
     RETURN VALUE:
         15: 1 if x == 3 else 0
     """
     setup_8bit()
-    parser.parse_csv("tests/public_prog/ex1.csv")
+    parser.parse_csv(Path("tests/public_prog/ex1.csv"))
     # Clone student's program
-    ram_copy = clone_dict(globs.RAM)
+    ram_copy = clone_dict(global_vars.RAM)
     for num in range(256):
         setup_8bit()
-        globs.RAM = clone_dict(ram_copy)
+        global_vars.RAM = clone_dict(ram_copy)
         # Overwrite RESERVED address with test input
-        globs.RAM[14] = num
+        global_vars.RAM[14] = num
         # We've chosen not to overwrite RETURN VALUE address to a wrong value before execution, which we could have done to prevent hardcoding
         # ex1.csv doesn't take advantage of this
         # Is there a way to take advantage of this in your flags.csv program?
-        # globs.RAM[15] = 0x42
+        # global_vars.RAM[15] = 0x42
         try:
             execute_full_speed()
         except Exception:
             # Note when an Exception occurs, the rest of the tests don't run. The break is for performance reasons.
             break
         # The autograder has a tests_passed variable and adds 1 to it if the RETURN VALUE is correct
-        assert int(num == 3) == globs.RAM[15]
+        assert int(num == 3) == global_vars.RAM[15]
 
     # score = tests_passed / total_tests
 
 
 def test_ex2():
     """Test ex2.csv.
     RESERVED:
         15: Input 0 to 255
     RETURN VALUE:
         Register A: See ex2_rv() function
     """
     setup_8bit()
-    parser.parse_csv("tests/public_prog/ex2.csv")
+    parser.parse_csv(Path("tests/public_prog/ex2.csv"))
     # Clone student's program
-    ram_copy = clone_dict(globs.RAM)
+    ram_copy = clone_dict(global_vars.RAM)
     for num in range(256):
         setup_8bit()
-        globs.RAM = clone_dict(ram_copy)
+        global_vars.RAM = clone_dict(ram_copy)
         # Overwrite RESERVED address with test input
-        globs.RAM[15] = num
+        global_vars.RAM[15] = num
         try:
             execute_full_speed()
         except Exception:
             # Note when an Exception occurs, the rest of the tests don't run. The break is for performance reasons.
             break
         # The autograder has a tests_passed variable and adds 1 to it if the RETURN VALUE is correct
-        assert ex2_rv(num) == globs.A
+        assert ex2_rv(num) == global_vars.A
 
     # score = tests_passed / total_tests
 
 
 def ex2_rv(X):
     """Helper function for testing ex2.csv. Just the example pseudocode to be replicated.
     Can make it not use a loop and instead use an if < 16 and then a mod operation but I don't have time for that.
```

### Comparing `SAPsim-1.0.2/tests/test_exceptions.py` & `SAPsim-1.0.3/tests/test_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Test exception handling."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
+from pathlib import Path
 import pytest
 import SAPsim.utils.exceptions as exceptions
 from SAPsim.utils.helpers import setup_4bit, setup_8bit
 from SAPsim.utils import parser
 
 
 def test_16MappedAddresses():
     setup_8bit()
-    parser.parse_csv("tests/malformed_csv/16_mapped_addresses.csv")
+    parser.parse_csv(Path("tests/malformed_csv/16_mapped_addresses.csv"))
 
 
 def test_19MappedAddresses():
     setup_8bit()
     with pytest.raises(exceptions.MoreThan16MappedAddresses):
-        parser.parse_csv("tests/malformed_csv/19_mapped_addresses.csv")
+        parser.parse_csv(Path("tests/malformed_csv/19_mapped_addresses.csv"))
```

### Comparing `SAPsim-1.0.2/tests/test_helpers.py` & `SAPsim-1.0.3/tests/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Test helpers.py."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 import pytest
 from SAPsim.utils.helpers import *
-from SAPsim.utils.globs import *
+from SAPsim.utils.global_vars import *
 import SAPsim.utils.exceptions as exceptions
 
 
 def test_instruction_to_byte_returns_correct_byte():
     """Generate all possible instructions in byte form. Test that `instruction_to_byte` returns the correct byte given the string representation <Mnemonic> <Arg>."""
     # Instructions 0x00 to 0x8f (inclusive)
     for i in range(0x90):
         assert i == instruction_to_byte(
-            f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}"
+            f"{MNEMONIC_TO_OPCODE.inverse[(i & 0xF0) >> 4]} {i & 0xF}"
         )
     # Instructions 0xe0 to 0xff (inclusive)
     for i in range(0xE0, 0xFF):
         assert i == instruction_to_byte(
-            f"{OPCODE_TO_MNEMONIC[(i & 0xF0) >> 4]} {i & 0xF}"
+            f"{MNEMONIC_TO_OPCODE.inverse[(i & 0xF0) >> 4]} {i & 0xF}"
         )
 
 
 def test_instruction_to_byte_NOP_OUT_HLT():
     """Test that instruction to byte returns correct opcode and Arg 0 for NOP, OUT, HLT without an arg."""
     assert 0 == instruction_to_byte("NOP")
     assert 0xE << 4 == instruction_to_byte("OUT")
```

### Comparing `SAPsim-1.0.2/tests/test_instructions.py` & `SAPsim-1.0.3/tests/test_instructions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 """Test instructions."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import SAPsim.utils.globs as globs
+import SAPsim.utils.global_vars as global_vars
 from SAPsim.utils.execute import execute_full_speed, execute_next
 from SAPsim.utils.helpers import check_state, check_state_all
 from SAPsim.utils.exceptions import (
     DroppedOffBottom,
     ARegisterNotEnoughBits,
     LoadFromUnmappedAddress,
 )
 from SAPsim.utils.helpers import setup_4bit
 
 
 def test_nop():
     setup_4bit()
-    globs.RAM[0] = 0x00
-    globs.RAM[1] = 0x01
-    globs.RAM[2] = 0x02
-    globs.RAM[4] = 0x0F
+    global_vars.RAM[0] = 0x00
+    global_vars.RAM[1] = 0x01
+    global_vars.RAM[2] = 0x02
+    global_vars.RAM[4] = 0x0F
     try:
         execute_full_speed()
         assert False
     except DroppedOffBottom:
         pass
     check_state_all({0: 0x00, 1: 0x01, 2: 0x02, 4: 0x0F}, 5, 0, 0, False, False, False)
 
 
 def test_lda():
     setup_4bit()
-    globs.RAM[0] = 0x1F
-    globs.RAM[1] = 0x1E
-    globs.RAM[14] = 0x3
-    globs.RAM[15] = 0x4
+    global_vars.RAM[0] = 0x1F
+    global_vars.RAM[1] = 0x1E
+    global_vars.RAM[14] = 0x3
+    global_vars.RAM[15] = 0x4
     execute_next()
     check_state_all({0: 0x1F, 1: 0x1E, 14: 0x3, 15: 0x4}, 1, 4, 0, False, False, True)
     execute_next()
     check_state_all({0: 0x1F, 1: 0x1E, 14: 0x3, 15: 0x4}, 2, 3, 0, False, False, True)
 
 
 def test_lda_raises_ARegisterOverflow():
     setup_4bit()
-    globs.RAM[0] = 0x1F
-    globs.RAM[15] = 0x10
+    global_vars.RAM[0] = 0x1F
+    global_vars.RAM[15] = 0x10
     try:
         execute_next()
         assert False
     except ARegisterNotEnoughBits:
         pass
 
 
 def test_lda_from_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x1F
+    global_vars.RAM[0] = 0x1F
     try:
         execute_next()
         assert False
     except LoadFromUnmappedAddress:
         pass
 
 
 def test_add():
     setup_4bit()
-    globs.RAM[0] = 0x2F
-    globs.RAM[1] = 0x2E
-    globs.RAM[14] = 0xF
-    globs.RAM[15] = 0xF
+    global_vars.RAM[0] = 0x2F
+    global_vars.RAM[1] = 0x2E
+    global_vars.RAM[14] = 0xF
+    global_vars.RAM[15] = 0xF
     execute_next()
     check_state(
         RAM={0: 0x2F, 1: 0x2E, 14: 0xF, 15: 0xF}, A=0xF, FLAG_C=False, FLAG_Z=False
     )
     execute_next()
     check_state(
         RAM={0: 0x2F, 1: 0x2E, 14: 0xF, 15: 0xF}, A=14, FLAG_C=True, Flag_Z=False
@@ -79,103 +79,103 @@
         assert False
     except DroppedOffBottom:
         pass
 
 
 def test_add_from_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2F
+    global_vars.RAM[0] = 0x2F
     try:
         execute_next()
         assert False
     except LoadFromUnmappedAddress:
         pass
 
 
 def test_sub():
     setup_4bit()
-    globs.RAM[0] = 0x3F
-    globs.RAM[1] = 0x3E
-    globs.RAM[14] = 0x1
-    globs.RAM[15] = 0xF
+    global_vars.RAM[0] = 0x3F
+    global_vars.RAM[1] = 0x3E
+    global_vars.RAM[14] = 0x1
+    global_vars.RAM[15] = 0xF
     execute_next()
     check_state(
         RAM={0: 0x3F, 1: 0x3E, 14: 0x1, 15: 0xF}, A=1, FLAG_C=False, FLAG_Z=False
     )
     execute_next()
     check_state(RAM={0: 0x3F, 1: 0x3E, 14: 0x1, 15: 0xF}, A=0, FLAG_C=True, FLAG_Z=True)
 
 
 def test_sta_to_unmapped_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2F
-    globs.RAM[1] = 0x4E
-    globs.RAM[15] = 0xF
+    global_vars.RAM[0] = 0x2F
+    global_vars.RAM[1] = 0x4E
+    global_vars.RAM[15] = 0xF
     execute_next()
     execute_next()
     check_state(
         RAM={0: 0x2F, 1: 0x4E, 0xE: 0xF, 0xF: 0xF},
         A=0xF,
         FLAG_C=False,
         FLAG_Z=False,
         PC=2,
         EXECUTING=True,
     )
 
 
 def test_sta_overwrites_addr():
     setup_4bit()
-    globs.RAM[0] = 0x2E
-    globs.RAM[1] = 0x4F
-    globs.RAM[14] = 2
-    globs.RAM[15] = 1
+    global_vars.RAM[0] = 0x2E
+    global_vars.RAM[1] = 0x4F
+    global_vars.RAM[14] = 2
+    global_vars.RAM[15] = 1
     try:
         execute_full_speed()
         assert False
     except DroppedOffBottom:
         pass
     check_state_all({0: 0x2E, 1: 0x4F, 14: 2, 15: 2}, 16, 2, 2, False, False, False)
 
 
 def test_ldi():
     setup_4bit()
-    globs.RAM[0] = 0x59
+    global_vars.RAM[0] = 0x59
     execute_next()
     check_state_all({0: 0x59}, 1, 9, 0, False, False, True)
 
 
 def test_ldi_overwrites_A():
     setup_4bit()
-    globs.A = 15
-    globs.RAM[0] = 0x55
+    global_vars.A = 15
+    global_vars.RAM[0] = 0x55
     execute_next()
     check_state_all({0: 0x55}, 1, 5, 0, False, False, True)
 
 
 def test_ldi_doesnt_modify_flags():
     setup_4bit()
-    globs.RAM[0] = 0x5A
-    globs.FLAG_C = True
-    globs.FLAG_Z = True
+    global_vars.RAM[0] = 0x5A
+    global_vars.FLAG_C = True
+    global_vars.FLAG_Z = True
     execute_next()
     check_state_all({0: 0x5A}, 1, 0xA, 0, True, True, True)
 
 
 def test_jmp():
     setup_4bit()
-    globs.RAM[0] = 0x67
+    global_vars.RAM[0] = 0x67
     execute_next()
     check_state_all({0: 0x67}, 7, 0, 0, False, False, True)
 
 
 def test_jmp_executes_instruction():
     setup_4bit()
-    globs.RAM[0] = 0x64
-    globs.RAM[4] = 0x55
-    globs.RAM[5] = 0x47
+    global_vars.RAM[0] = 0x64
+    global_vars.RAM[4] = 0x55
+    global_vars.RAM[5] = 0x47
     execute_next()
     check_state_all({0: 0x64, 4: 0x55, 5: 0x47}, 4, 0, 0, False, False, True)
     execute_next()
     check_state_all({0: 0x64, 4: 0x55, 5: 0x47}, 5, 5, 0, False, False, True)
     execute_next()
     check_state_all({0: 0x64, 4: 0x55, 5: 0x47, 7: 5}, 6, 5, 0, False, False, True)
     execute_next()
@@ -185,16 +185,16 @@
         assert False
     except DroppedOffBottom:
         pass
 
 
 def test_hlt():
     setup_4bit()
-    globs.RAM[0] = 0xFF
-    globs.RAM[15] = 0x10
+    global_vars.RAM[0] = 0xFF
+    global_vars.RAM[15] = 0x10
     execute_next()
     check_state_all({0: 0xFF, 15: 0x10}, 0, 0, 0, False, False, False)
     for i in range(100):
         execute_next()
     check_state_all({0: 0xFF, 15: 0x10}, 0, 0, 0, False, False, False)
     for i in range(1000):
         execute_full_speed()
```

### Comparing `SAPsim-1.0.2/tests/test_run.py` & `SAPsim-1.0.3/tests/test_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 def test_run_ex1() -> None:
     """Test ex1.csv"""
     f = open(TEMP_FILE_PATH, "w")
     sys.stdout = f
     # Use plain table_fmt to avoid special characters that aren't the same on Ubuntu and Windows (unit tests)
-    run("tests/public_prog/ex1.csv", table_fmt="plain")
+    run("tests/public_prog/ex1.csv", table_format="plain")
     f.close()
 
     f2 = open(TEMP_FILE_PATH, "r")
     expected = open("tests/data/public_prog/ex1_plain.txt", "r")
 
     assert f2.readlines() == expected.readlines()
 
@@ -54,15 +54,15 @@
     expected.close()
 
 
 def test_run_ex2() -> None:
     f = open(TEMP_FILE_PATH, "w")
     sys.stdout = f
     # Use plain table_fmt to avoid special characters that aren't the same on Ubuntu and Windows (unit tests)
-    run("tests/public_prog/ex2.csv", table_fmt="plain")
+    run("tests/public_prog/ex2.csv", table_format="plain")
     f.close()
 
     f2 = open(TEMP_FILE_PATH, "r")
     expected = open("tests/data/public_prog/ex2_plain.txt", "r")
 
     assert f2.readlines() == expected.readlines()
```

