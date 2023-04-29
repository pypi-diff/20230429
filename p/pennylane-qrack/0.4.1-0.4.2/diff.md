# Comparing `tmp/pennylane-qrack-0.4.1.tar.gz` & `tmp/pennylane-qrack-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-qrack-0.4.1.tar", last modified: Tue Feb 14 11:45:11 2023, max compression
+gzip compressed data, was "pennylane-qrack-0.4.2.tar", last modified: Sat Apr 29 12:07:48 2023, max compression
```

## Comparing `pennylane-qrack-0.4.1.tar` & `pennylane-qrack-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2022-04-22 20:03:22.000000 pennylane-qrack-0.4.1/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4437 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3363 2023-02-14 11:13:39.000000 pennylane-qrack-0.4.1/README.rst
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/pennylane_qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2023-02-14 11:13:39.000000 pennylane-qrack-0.4.1/pennylane_qrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2023-02-14 11:14:25.000000 pennylane-qrack-0.4.1/pennylane_qrack/_version.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    14575 2023-02-14 11:42:59.000000 pennylane-qrack-0.4.1/pennylane_qrack/qrack_device.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     4437 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      417 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/entry_points.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       44 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2023-02-14 11:45:11.000000 pennylane-qrack-0.4.1/pennylane_qrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2280 2023-02-14 11:31:02.000000 pennylane-qrack-0.4.1/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-02-14 11:45:11.579066 pennylane-qrack-0.4.1/tests/
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)    17160 2023-02-14 11:27:48.000000 pennylane-qrack-0.4.1/tests/test_apply.py
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1715 2023-02-14 11:28:19.000000 pennylane-qrack-0.4.1/tests/test_integration.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3780 2023-02-14 11:28:49.000000 pennylane-qrack-0.4.1/tests/test_units.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2022-04-22 20:03:22.000000 pennylane-qrack-0.4.2/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     4437 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3363 2023-02-14 11:13:39.000000 pennylane-qrack-0.4.2/README.rst
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/pennylane_qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2023-02-14 11:13:39.000000 pennylane-qrack-0.4.2/pennylane_qrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2023-04-29 12:06:12.000000 pennylane-qrack-0.4.2/pennylane_qrack/_version.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    14588 2023-04-29 12:00:06.000000 pennylane-qrack-0.4.2/pennylane_qrack/qrack_device.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     4437 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      417 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/entry_points.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       44 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2023-04-29 12:07:48.000000 pennylane-qrack-0.4.2/pennylane_qrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2280 2023-02-14 11:31:02.000000 pennylane-qrack-0.4.2/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-29 12:07:48.864655 pennylane-qrack-0.4.2/tests/
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)    17241 2023-04-29 12:01:31.000000 pennylane-qrack-0.4.2/tests/test_apply.py
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1715 2023-02-14 11:28:19.000000 pennylane-qrack-0.4.2/tests/test_integration.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3783 2023-04-29 12:03:05.000000 pennylane-qrack-0.4.2/tests/test_units.py
```

### Comparing `pennylane-qrack-0.4.1/LICENSE` & `pennylane-qrack-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-qrack-0.4.1/PKG-INFO` & `pennylane-qrack-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.4.1
+Version: 0.4.2
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pennylane-qrack-0.4.1/README.rst` & `pennylane-qrack-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pennylane-qrack-0.4.1/pennylane_qrack/__init__.py` & `pennylane-qrack-0.4.2/pennylane_qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pennylane-qrack-0.4.1/pennylane_qrack/_version.py` & `pennylane-qrack-0.4.2/pennylane_qrack/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `pennylane-qrack-0.4.1/pennylane_qrack/qrack_device.py` & `pennylane-qrack-0.4.2/pennylane_qrack/qrack_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         # translate op wire labels to consecutive wire labels used by the device
         device_wires = self.map_wires(op.wires)
         par = op.parameters
 
         if len(par[0]) != 2 ** len(device_wires):
             raise ValueError("Unitary matrix must be of shape (2**wires, 2**wires).")
 
-        if op.inverse:
+        if isinstance(op, Adjoint):
             par[0] = par[0].conj().T
 
         matrix = par[0].flatten().tolist()
         self._state.mtrx(matrix, device_wires.labels[0])
 
     def analytic_probability(self, wires=None):
         """Return the (marginal) analytic probability of each computational basis state."""
```

### Comparing `pennylane-qrack-0.4.1/pennylane_qrack.egg-info/PKG-INFO` & `pennylane-qrack-0.4.2/pennylane_qrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.4.1
+Version: 0.4.2
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pennylane-qrack-0.4.1/setup.py` & `pennylane-qrack-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pennylane-qrack-0.4.1/tests/test_apply.py` & `pennylane-qrack-0.4.2/tests/test_apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
     def test_invalid_qubit_state_vector(self):
         """Test that an exception is raised if the state
         vector is the wrong size"""
         dev = QrackDevice(2)
         state = np.array([0, 123.432])
 
-        with pytest.raises(ValueError, match=r"State vector must be of length 2\*\*wires"):
+        with pytest.raises(ValueError, match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\)."):
             op = qml.QubitStateVector(state, wires=[0, 1])
             dev.apply([op])
 
     @pytest.mark.parametrize("op,mat", single_qubit)
     def test_single_qubit_no_parameters(self, init_state, op, mat, tol):
         """Test PauliX application"""
         dev = QrackDevice(1)
@@ -419,15 +419,15 @@
     def test_apply_errors_qubit_state_vector(self):
         """Test that apply fails for incorrect state preparation."""
         dev = QrackDevice(2)
 
         with pytest.raises(ValueError, match="Sum of amplitudes-squared does not equal one."):
             dev.apply([qml.QubitStateVector(np.array([1, -1]), wires=[0])])
 
-        with pytest.raises(ValueError, match=r"State vector must be of length 2\*\*wires."):
+        with pytest.raises(ValueError, match="State vector must have shape \\(2\\*\\*wires,\\) or \\(batch_size, 2\\*\\*wires\\)."):
             p = np.array([1, 0, 1, 1, 0]) / np.sqrt(3)
             dev.reset()
             dev.apply([qml.QubitStateVector(p, wires=[0, 1])])
 
     def test_apply_errors_basis_state(self):
         """Test that apply fails for incorrect basis state preparation."""
         dev = QrackDevice(2)
```

### Comparing `pennylane-qrack-0.4.1/tests/test_integration.py` & `pennylane-qrack-0.4.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pennylane-qrack-0.4.1/tests/test_units.py` & `pennylane-qrack-0.4.2/tests/test_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         state = np.array((0, 1, 0, 1))
         op = qml.BasisState(state, wires=[0, 1, 2, 3])
         dev.apply([op])
         dev.reset()
 
         expected = [0.0] * 16
         expected[0] = 1.0
-        actual = dev._state.dump()
+        actual = dev._state.out_ket()
         for i in range(16):
             actual[i] = actual[i] * np.conjugate(actual[i])
         assert np.allclose(actual, expected)
 
     @pytest.mark.parametrize("obs,args,wires,supported", [
         (qml.PauliX, [], [0], True),
         (qml.Hadamard, [], [0], False),
```

