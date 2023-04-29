# Comparing `tmp/noteslib-2.1.0.tar.gz` & `tmp/noteslib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteslib-2.1.0.tar", last modified: Fri Oct 19 19:23:08 2018, max compression
+gzip compressed data, was "noteslib-2.1.1.tar", last modified: Sat Apr 29 20:17:56 2023, max compression
```

## Comparing `noteslib-2.1.0.tar` & `noteslib-2.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     5145 2018-10-18 23:46:57.674295 noteslib-2.1.0/doc/README.md
--rw-r--r--   0        0        0    13960 2018-10-19 19:22:47.108492 noteslib-2.1.0/noteslib.py
--rw-r--r--   0        0        0      718 2018-10-19 16:55:53.868403 noteslib-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 noteslib-2.1.0/setup.py
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 noteslib-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6398 2023-04-29 20:04:14.127882 noteslib-2.1.1/README.md
+-rw-r--r--   0        0        0    13960 2023-04-29 19:44:26.600883 noteslib-2.1.1/noteslib.py
+-rw-r--r--   0        0        0      733 2023-04-29 19:45:38.932194 noteslib-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6943 1970-01-01 00:00:00.000000 noteslib-2.1.1/PKG-INFO
```

### Comparing `noteslib-2.1.0/doc/README.md` & `noteslib-2.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # NotesLib
 
-NotesLib is a library of Python classes for manipulating Lotus
+NotesLib is a library of Python classes for manipulating (Lotus/IBM/HCL)
 Notes/Domino objects via COM.
 
 NotesLib was created by Robert Follek, and the current maintainer is Marcelo Huerta.
 
+*(Please don't ask Robert about NotesLib, though: he released the code in text form some
+time ago, he doesn't work with Notes any more and the whole idea of updating the code 
+and uploading it to PyPI can only be blamed on Marcelo. Who is not working actively with
+Notes at this time, so... responses can be slow.)*
+
+NotesLib **depends on a proper installation and configuration of a Notes client on a 
+Windows computer**, as it interacts with the COM server that is part of a Notes installation
+for Windows and it expects a complete local configuration in place.
+
+The Python version to be installed should be 32- or 64-bits depending on the version of 
+the underlying COM server providing the objects accessed by the library. This means that for
+a Notes client up to version 11.x, you should install a 32-bit Python. Version 12.x is the first
+of the Notes clients to be 64-bit, so the COM server is also, and you need a 64-bit Python to
+interact with it.
+
+-----
+
+**We've received information that the COM server in version 12.0 and 12.0.1 had bugs and HCL
+solved the specific problems found in version 12.0.2.** *Caveat emptor*: any underlying problems
+with the COM server are beyond the scope of this library.
+
+-----
+
 The NotesLib classes correspond to the standard LotusScript classes; they
 support all the standard properties and methods. The NotesLib classes have
 additional methods and ease-of-use features. See below the details for the
 individual classes.
 
 Classes available so far:
```

### Comparing `noteslib-2.1.0/noteslib.py` & `noteslib-2.1.1/noteslib.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Classes available so far:
     Session
     Database
     ACL
     ACLEntry
 """
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 import win32com.client
 
 # -------------------------------------------------------------------
 
 class NotesLibError(Exception): pass
 class SessionError(NotesLibError): pass
```

### Comparing `noteslib-2.1.0/pyproject.toml` & `noteslib-2.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
-requires = ["flit"]
-build-backend = "flit.buildapi"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "noteslib"
 author = "Robert Follek"
 author-email = "bfollek@gmail.com"
 maintainer = "Marcelo Huerta"
 maintainer-email = "richieadler@gmail.com"
-description-file = "doc/README.md"
-requires-python = "~=3.0"
+description-file = "README.md"
+requires-python = ">=3.7"
 requires = [
 	"pywin32",
 ]
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Environment :: Win32 (MS Windows)",
 	"Intended Audience :: Developers",
```

