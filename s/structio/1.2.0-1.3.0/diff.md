# Comparing `tmp/structio-1.2.0.tar.gz` & `tmp/structio-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.2.0.tar", last modified: Sun Apr 23 00:07:15 2023, max compression
+gzip compressed data, was "structio-1.3.0.tar", last modified: Sat Apr 29 05:49:12 2023, max compression
```

## Comparing `structio-1.2.0.tar` & `structio-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:07:15.913372 structio-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-23 00:07:15.913372 structio-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-04-23 00:06:41.000000 structio-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 00:06:41.000000 structio-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:07:15.913372 structio-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:07:15.913372 structio-1.2.0/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 00:07:15.000000 structio-1.2.0/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-23 00:06:41.000000 structio-1.2.0/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:49:12.972128 structio-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-29 05:49:12.972128 structio-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-04-29 05:48:52.000000 structio-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-29 05:48:52.000000 structio-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:49:12.972128 structio-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:49:12.972128 structio-1.3.0/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 05:49:12.000000 structio-1.3.0/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-29 05:48:52.000000 structio-1.3.0/structio.py
```

### Comparing `structio-1.2.0/PKG-INFO` & `structio-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -17,16 +17,16 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> import structio
->>> stream = structio.StructIO(endian='little')
+>>> from structio import StructIO
+>>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
@@ -84,29 +84,29 @@
 
 Converts byte *b* into an list of integers representing the individual bits of the byte. First element in the list is the LSB in the byte.
 
 **pack_bits(bits)**
 
 Converts a list of integers into a byte.
 
-**unpack_int(b, endian, signed=False)**
+**unpack_int(b, endian=None, signed=False)**
 
-Converts bytes object *b* into an integer. The endian is specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
+Converts bytes object *b* into an integer. The endian can be specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
 
-**pack_int(number, numbytes, endian, signed=False)**
+**pack_int(number, numbytes, endian=None, signed=False)**
 
 Converts *number* into a bytes object with length *numbytes* and endian *endian*. The *signed* argument is used to specify whether the integer is signed or not.
 
-**unpack_float(b, numbytes, endian)**
+**unpack_float(b, numbytes, endian=None)**
 
-Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
-**pack_float(number, numbytes, endian)**
+**pack_float(number, numbytes, endian=None)**
 
-Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
 **unpack_str(b)**
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
@@ -118,19 +118,19 @@
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
 **unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
-Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
+Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string can be specified with the *endian* argument.
 
 **unpack_7bint(b, start=0)**
 
 Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
@@ -190,15 +190,15 @@
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
 **delete(length)**
 
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+Deletes *length* bytes from the object starting from the current position.
 
 **find(bytes_sequence, n=1)**
 
 Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
 
 **index(bytes_sequence, n=1)**
 
@@ -280,29 +280,45 @@
 
 Same as *write_cstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_cstr(string)**
 
 Deletes the null-terminated string existing at the current location, then writes *string* as a null-terminated string in it's place.  Raises a *ValueError* if it fails to find a null termination.
 
+**skip_cstr()**
+
+Skips the null-terminated string at the current position.
+
+**delete_cstr()**
+
+Deletes the null-terminated string at the current position.
+
 **read_pstr(numbytes, endian=None)**
 
 Reads a Pascal string from the object and returns it. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
 
 **write_pstr(string, numbytes, endian=None)**
 
-Writes *string* to the object as a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
+Writes *string* to the object as a Pascal string.
 
 **append_pstr(string, numbytes, endian=None)**
 
-Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes. The endian of the length of the string can be specified with the *endian* argument.
+Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_pstr(string, numbytes, endian=None)**
 
-Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place. *numbytes* is used to specify how many bytes are used for the integer holding the string's length. The endian of the length of the string can be specified with the *endian* argument.
+Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place.
+
+**skip_pstr(numbytes, endian=None)**
+
+Skips the null-terminated string at the current position.
+
+**delete_pstr(numbytes, endian=None)**
+
+Deletes the null-terminated string at the current position.
 
 **read_7bint()**
 
 Reads the bytes representing a 7 bit integer from the object at the current position and converts them into an integer.
 
 **write_7bint(number)**
 
@@ -312,19 +328,27 @@
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
 Overwrites the 7 bit integer at the current position with *number*.
 
+**skip_7bint()**
+
+Skips the 7 bit integer at the current position.
+
+**delete_7bint()**
+
+Deletes the 7 bit integer at the current position.
+
 -----
 
 ### Extending StructIO
 
-You can add your own types by inheriting from the two base objects:
+You can add your own types by inheriting from the base Struct object:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
         str_len, int_len = self.unpack_7bint(b, start)
@@ -334,15 +358,19 @@
         str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         return string, int_len + str_len
         
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
-        
+```
+
+As well as the stream object:
+
+```python
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
         return self._read(self._struct.unpack_7bstr, ())
         
@@ -350,8 +378,14 @@
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
+		 
+    def skip_7bstr(self):
+        return self._skip(self._struct._get_7bstr_len, ())
+        
+    def delete_7bstr(self):
+        return self._delete(self._struct._get_7bstr_len, ())
 ```
```

### Comparing `structio-1.2.0/README.md` & `structio-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> import structio
->>> stream = structio.StructIO(endian='little')
+>>> from structio import StructIO
+>>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
@@ -76,29 +76,29 @@
 
 Converts byte *b* into an list of integers representing the individual bits of the byte. First element in the list is the LSB in the byte.
 
 **pack_bits(bits)**
 
 Converts a list of integers into a byte.
 
-**unpack_int(b, endian, signed=False)**
+**unpack_int(b, endian=None, signed=False)**
 
-Converts bytes object *b* into an integer. The endian is specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
+Converts bytes object *b* into an integer. The endian can be specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
 
-**pack_int(number, numbytes, endian, signed=False)**
+**pack_int(number, numbytes, endian=None, signed=False)**
 
 Converts *number* into a bytes object with length *numbytes* and endian *endian*. The *signed* argument is used to specify whether the integer is signed or not.
 
-**unpack_float(b, numbytes, endian)**
+**unpack_float(b, numbytes, endian=None)**
 
-Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
-**pack_float(number, numbytes, endian)**
+**pack_float(number, numbytes, endian=None)**
 
-Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
 **unpack_str(b)**
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
@@ -110,19 +110,19 @@
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
 **unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
-Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
+Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string can be specified with the *endian* argument.
 
 **unpack_7bint(b, start=0)**
 
 Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
@@ -182,15 +182,15 @@
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
 **delete(length)**
 
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+Deletes *length* bytes from the object starting from the current position.
 
 **find(bytes_sequence, n=1)**
 
 Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
 
 **index(bytes_sequence, n=1)**
 
@@ -272,29 +272,45 @@
 
 Same as *write_cstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_cstr(string)**
 
 Deletes the null-terminated string existing at the current location, then writes *string* as a null-terminated string in it's place.  Raises a *ValueError* if it fails to find a null termination.
 
+**skip_cstr()**
+
+Skips the null-terminated string at the current position.
+
+**delete_cstr()**
+
+Deletes the null-terminated string at the current position.
+
 **read_pstr(numbytes, endian=None)**
 
 Reads a Pascal string from the object and returns it. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
 
 **write_pstr(string, numbytes, endian=None)**
 
-Writes *string* to the object as a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
+Writes *string* to the object as a Pascal string.
 
 **append_pstr(string, numbytes, endian=None)**
 
-Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes. The endian of the length of the string can be specified with the *endian* argument.
+Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_pstr(string, numbytes, endian=None)**
 
-Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place. *numbytes* is used to specify how many bytes are used for the integer holding the string's length. The endian of the length of the string can be specified with the *endian* argument.
+Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place.
+
+**skip_pstr(numbytes, endian=None)**
+
+Skips the null-terminated string at the current position.
+
+**delete_pstr(numbytes, endian=None)**
+
+Deletes the null-terminated string at the current position.
 
 **read_7bint()**
 
 Reads the bytes representing a 7 bit integer from the object at the current position and converts them into an integer.
 
 **write_7bint(number)**
 
@@ -304,19 +320,27 @@
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
 Overwrites the 7 bit integer at the current position with *number*.
 
+**skip_7bint()**
+
+Skips the 7 bit integer at the current position.
+
+**delete_7bint()**
+
+Deletes the 7 bit integer at the current position.
+
 -----
 
 ### Extending StructIO
 
-You can add your own types by inheriting from the two base objects:
+You can add your own types by inheriting from the base Struct object:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
         str_len, int_len = self.unpack_7bint(b, start)
@@ -326,15 +350,19 @@
         str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         return string, int_len + str_len
         
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
-        
+```
+
+As well as the stream object:
+
+```python
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
         return self._read(self._struct.unpack_7bstr, ())
         
@@ -342,8 +370,14 @@
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
-```
+		 
+    def skip_7bstr(self):
+        return self._skip(self._struct._get_7bstr_len, ())
+        
+    def delete_7bstr(self):
+        return self._delete(self._struct._get_7bstr_len, ())
+```
```

### Comparing `structio-1.2.0/structio.egg-info/PKG-INFO` & `structio-1.3.0/structio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -17,16 +17,16 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> import structio
->>> stream = structio.StructIO(endian='little')
+>>> from structio import StructIO
+>>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14)
 4
 >>> stream.write_cstr('Hello')
 6
 >>> stream.write_pstr('World!', 1)
@@ -84,29 +84,29 @@
 
 Converts byte *b* into an list of integers representing the individual bits of the byte. First element in the list is the LSB in the byte.
 
 **pack_bits(bits)**
 
 Converts a list of integers into a byte.
 
-**unpack_int(b, endian, signed=False)**
+**unpack_int(b, endian=None, signed=False)**
 
-Converts bytes object *b* into an integer. The endian is specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
+Converts bytes object *b* into an integer. The endian can be specified with the *endian* argument. The *signed* argument is used to specify whether the integer is signed or not.
 
-**pack_int(number, numbytes, endian, signed=False)**
+**pack_int(number, numbytes, endian=None, signed=False)**
 
 Converts *number* into a bytes object with length *numbytes* and endian *endian*. The *signed* argument is used to specify whether the integer is signed or not.
 
-**unpack_float(b, numbytes, endian)**
+**unpack_float(b, numbytes, endian=None)**
 
-Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts bytes object *b* into a float. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
-**pack_float(number, numbytes, endian)**
+**pack_float(number, numbytes, endian=None)**
 
-Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian is specified with the *endian* argument.
+Converts *number* into a bytes object. *numbytes* can be 2 for half precision, 4 for single precision, or 8 for double precision. The endian can be specified with the *endian* argument.
 
 **unpack_str(b)**
 
 Convert bytes object *b* into a string.
 
 **pack_str(string)**
 
@@ -118,19 +118,19 @@
 
 **pack_cstr(string)**
 
 Converts *string* into a bytes object representing a null-terminated string.
 
 **unpack_pstr(b, numbytes, endian=None, start=0)**
 
-Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string is specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
+Converts bytes object *b* into a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument. *b* will only be converted up to the length specified in the bytes object. If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_pstr(string, numbytes, endian=None)**
 
-Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string is specified with the *endian* argument.
+Converts *string* into a bytes object in the Pascal string format. *numbytes* is used to specify how many bytes are used for the string's length. The endian of the length of the string can be specified with the *endian* argument.
 
 **unpack_7bint(b, start=0)**
 
 Converts bytes representing a 7 bit integer (Variable Length Quantity) into an integer.  If *start* is specified, then the bytes object will be converted starting from position *start*. Returns a tuple containing both the value and the length of the type.
 
 **pack_7bint(number)**
 
@@ -190,15 +190,15 @@
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
 **delete(length)**
 
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+Deletes *length* bytes from the object starting from the current position.
 
 **find(bytes_sequence, n=1)**
 
 Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
 
 **index(bytes_sequence, n=1)**
 
@@ -280,29 +280,45 @@
 
 Same as *write_cstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_cstr(string)**
 
 Deletes the null-terminated string existing at the current location, then writes *string* as a null-terminated string in it's place.  Raises a *ValueError* if it fails to find a null termination.
 
+**skip_cstr()**
+
+Skips the null-terminated string at the current position.
+
+**delete_cstr()**
+
+Deletes the null-terminated string at the current position.
+
 **read_pstr(numbytes, endian=None)**
 
 Reads a Pascal string from the object and returns it. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
 
 **write_pstr(string, numbytes, endian=None)**
 
-Writes *string* to the object as a Pascal string. *numbytes* is used to specify how many bytes are used for the string's length in the object. The endian of the length of the string can be specified with the *endian* argument.
+Writes *string* to the object as a Pascal string.
 
 **append_pstr(string, numbytes, endian=None)**
 
-Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes. The endian of the length of the string can be specified with the *endian* argument.
+Same as *write_pstr* but appends the value to the object at the current position instead of overwriting existing bytes.
 
 **overwrite_pstr(string, numbytes, endian=None)**
 
-Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place. *numbytes* is used to specify how many bytes are used for the integer holding the string's length. The endian of the length of the string can be specified with the *endian* argument.
+Deletes the existing Pascal string at the current position and writes *string* as a Pascal string in it's place.
+
+**skip_pstr(numbytes, endian=None)**
+
+Skips the null-terminated string at the current position.
+
+**delete_pstr(numbytes, endian=None)**
+
+Deletes the null-terminated string at the current position.
 
 **read_7bint()**
 
 Reads the bytes representing a 7 bit integer from the object at the current position and converts them into an integer.
 
 **write_7bint(number)**
 
@@ -312,19 +328,27 @@
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
 Overwrites the 7 bit integer at the current position with *number*.
 
+**skip_7bint()**
+
+Skips the 7 bit integer at the current position.
+
+**delete_7bint()**
+
+Deletes the 7 bit integer at the current position.
+
 -----
 
 ### Extending StructIO
 
-You can add your own types by inheriting from the two base objects:
+You can add your own types by inheriting from the base Struct object:
 
 ```python
 from structio import Struct, StructIO
 
 class ExtendedStruct(Struct):
     def _get_7bstr_len(self, b, start=0):
         str_len, int_len = self.unpack_7bint(b, start)
@@ -334,15 +358,19 @@
         str_len, int_len = self.unpack_7bint(b, start)
         string = self.unpack_str(b[(start + int_len):(start + int_len + str_len)])
         return string, int_len + str_len
         
     def pack_7bstr(self, string):
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
-        
+```
+
+As well as the stream object:
+
+```python
 class ExtendedStructIO(StructIO):
     def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
         super().__init__(b, endian, struct=struct)
         
     def read_7bstr(self):
         return self._read(self._struct.unpack_7bstr, ())
         
@@ -350,8 +378,14 @@
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
         return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
+		 
+    def skip_7bstr(self):
+        return self._skip(self._struct._get_7bstr_len, ())
+        
+    def delete_7bstr(self):
+        return self._delete(self._struct._get_7bstr_len, ())
 ```
```

### Comparing `structio-1.2.0/structio.py` & `structio-1.3.0/structio.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,34 +15,32 @@
             return self.endian
         else:
             return endian
             
     def unpack_bool(self, b):
         if isinstance(b, int):
             return b != 0
-            
+        elif len(b) == 1:
+            return b != b'\x00'
         else:
-            if len(b) == 1:
-                return b != b'\x00'
-            else:
-                raise ValueError('expected bytes object of length 1')
-                
+            raise ValueError('expected int or bytes object of length 1')
+            
     def pack_bool(self, boolean):
         if boolean:
             return b'\x01'
         else:
             return b'\x00'
             
     def unpack_bits(self, b):
         if isinstance(b, int):
             number = b
         elif len(b) == 1:
             number = self.unpack_int(b)
         else:
-            raise ValueError('expected bytes object of length 1')
+            raise ValueError('expected int or bytes object of length 1')
             
         return [number >> i & 1 for i in range(8)]
         
     def pack_bits(self, bits):
         return self.pack_int(sum(bits[i] << i for i in range(8)), 1)
         
     def unpack_int(self, b, endian=None, signed=False):
@@ -123,15 +121,15 @@
             
         number |= byte << (7 * i)
         length = i + 1
         
         return number, length
         
     def pack_7bint(self, number):
-        b = bytearray()
+        b = b''
         
         while number > 127:
             b += self.pack_int(number & 0b01111111 | 0b10000000, 1) 
             number >>= 7
             
         b += self.pack_int(number, 1)
         return b
@@ -211,22 +209,21 @@
         length = self.write(b)
         self.write(buffer)
         self.truncate()
         self.seek(start + length)
         return length
         
     def delete(self, length):
-        current_position = self.tell()
+        start = self.tell()
+        object_length = len(self)
         
-        if current_position - length < 0:
-            length = current_position
+        if start + length > object_length:
+            length = object_length - start
             
-        start = current_position - length
-        self.overwrite(start, current_position, b'')
-        
+        self.overwrite(start, start + length , b'')
         return length
         
     def find(self, bytes_sequence, n=1):
         start = self.tell()
         content = self.getvalue()
         location = content.find(bytes_sequence, start)
         
@@ -235,31 +232,37 @@
             
             if location == -1:
                 break
                 
         return location
         
     def index(self, bytes_sequence, n=1):
-        end = self.find(bytes_sequence, n)
+        location = self.find(bytes_sequence, n)
         
-        if end == -1:
+        if location == -1:
             raise ValueError('{} not found'.format(bytes_sequence))
             
-        return end
+        return location
         
     def _read(self, unpack_func, unpack_args):
         value, length = unpack_func(self.getvalue(), *unpack_args, start=self.tell())
         self.seek(length, 1)
         return value
         
     def _overwrite(self, len_func, len_args, pack_func, pack_args):
         start = self.tell()
         length = len_func(self.getvalue(), *len_args, start=start)
         return self.overwrite(start, start + length, pack_func(*pack_args))
         
+    def _skip(self, len_func, len_args):
+        return self.seek(len_func(self.getvalue(), *len_args, start=self.tell()), 1)
+        
+    def _delete(self, len_func, len_args):
+        return self.delete(len_func(self.getvalue(), *len_args, start=self.tell()))
+        
     def read_bool(self):
         return self._struct.unpack_bool(self.read(1))
         
     def write_bool(self, boolean):
         return self.write(self._struct.pack_bool(boolean))
         
     def append_bool(self, boolean):
@@ -312,30 +315,48 @@
         
     def append_cstr(self, string):
         return self.append(self._struct.pack_cstr(string))
         
     def overwrite_cstr(self, string):
         return self._overwrite(self._struct._get_cstr_len, (), self._struct.pack_cstr, (string,))
         
+    def skip_cstr(self):
+        return self._skip(self._struct._get_cstr_len, ())
+        
+    def delete_cstr(self):
+        return self._delete(self._struct._get_cstr_len, ())
+        
     def read_pstr(self, numbytes, endian=None):
         return self._read(self._struct.unpack_pstr, (numbytes, endian))
         
     def write_pstr(self, string, numbytes, endian=None):
         return self.write(self._struct.pack_pstr(string, numbytes, endian))
         
     def append_pstr(self, string, numbytes, endian=None):
         return self.append(self._struct.pack_pstr(string, numbytes, endian))
         
     def overwrite_pstr(self, string, numbytes, endian=None):
         return self._overwrite(self._struct._get_pstr_len, (numbytes, endian), self._struct.pack_pstr, (string, numbytes, endian))
         
+    def skip_pstr(self, numbytes, endian=None):
+        return self._skip(self._struct._get_pstr_len, (numbytes, endian))
+        
+    def delete_pstr(self, numbytes, endian=None):
+        return self._delete(self._struct._get_pstr_len, (numbytes, endian))
+        
     def read_7bint(self):
         return self._read(self._struct.unpack_7bint, ())
         
     def write_7bint(self, number):
         return self.write(self._struct.pack_7bint(number))
         
     def append_7bint(self, number):
         return self.append(self._struct.pack_7bint(number))
         
     def overwrite_7bint(self, number):
-        return self._overwrite(self._struct._get_7bint_len, (), self._struct.pack_7bint, (number,))
+        return self._overwrite(self._struct._get_7bint_len, (), self._struct.pack_7bint, (number,))
+        
+    def skip_7bint(self):
+        return self._skip(self._struct._get_7bint_len, ())
+        
+    def delete_7bint(self):
+        return self._delete(self._struct._get_7bint_len, ())
```

