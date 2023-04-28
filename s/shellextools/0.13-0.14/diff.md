# Comparing `tmp/shellextools-0.13.tar.gz` & `tmp/shellextools-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellextools-0.13.tar", last modified: Mon Apr 24 01:09:09 2023, max compression
+gzip compressed data, was "shellextools-0.14.tar", last modified: Fri Apr 28 23:03:09 2023, max compression
```

## Comparing `shellextools-0.13.tar` & `shellextools-0.14.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.351475 shellextools-0.13/
--rw-rw-rw-   0        0        0     1148 2023-04-24 01:08:53.000000 shellextools-0.13/LICENSE.rst
--rw-rw-rw-   0        0        0      209 2023-04-24 01:08:52.000000 shellextools-0.13/MANIFEST.in
--rw-rw-rw-   0        0        0     3804 2023-04-24 01:09:09.351475 shellextools-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     3154 2023-04-24 01:07:11.000000 shellextools-0.13/README.md
--rw-rw-rw-   0        0        0       85 2023-04-24 01:09:09.352472 shellextools-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-04-24 01:09:06.000000 shellextools-0.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.344459 shellextools-0.13/shellextools/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.13/shellextools/LICENSE
--rw-rw-rw-   0        0        0     3154 2023-04-24 01:07:11.000000 shellextools-0.13/shellextools/README.md
--rw-rw-rw-   0        0        0    50720 2023-04-24 01:03:11.000000 shellextools-0.13/shellextools/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-23 18:11:16.000000 shellextools-0.13/shellextools/getmultifiles.py
--rw-rw-rw-   0        0        0     2555 2023-04-23 18:11:16.000000 shellextools-0.13/shellextools/loggax3.py
--rw-rw-rw-   0        0        0      248 2023-04-24 01:09:06.000000 shellextools-0.13/shellextools/requirements.txt
--rw-rw-rw-   0        0        0     9983 2023-04-24 01:09:06.000000 shellextools-0.13/shellextools/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.350478 shellextools-0.13/shellextools.egg-info/
--rw-rw-rw-   0        0        0     3804 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-24 01:09:09.000000 shellextools-0.13/shellextools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.932038 shellextools-0.14/
+-rw-rw-rw-   0        0        0     1148 2023-04-28 23:02:53.000000 shellextools-0.14/LICENSE.rst
+-rw-rw-rw-   0        0        0      209 2023-04-28 23:02:51.000000 shellextools-0.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     3804 2023-04-28 23:03:09.932038 shellextools-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3154 2023-04-24 01:10:31.000000 shellextools-0.14/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-28 23:03:09.933036 shellextools-0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-04-28 23:03:08.000000 shellextools-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.928049 shellextools-0.14/shellextools/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.14/shellextools/LICENSE
+-rw-rw-rw-   0        0        0     3154 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/README.md
+-rw-rw-rw-   0        0        0    51326 2023-04-28 23:02:03.000000 shellextools-0.14/shellextools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/getmultifiles.py
+-rw-rw-rw-   0        0        0     2555 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/loggax3.py
+-rw-rw-rw-   0        0        0      248 2023-04-28 23:03:08.000000 shellextools-0.14/shellextools/requirements.txt
+-rw-rw-rw-   0        0        0     9983 2023-04-28 23:03:08.000000 shellextools-0.14/shellextools/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.931041 shellextools-0.14/shellextools.egg-info/
+-rw-rw-rw-   0        0        0     3804 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/top_level.txt
```

### Comparing `shellextools-0.13/LICENSE.rst` & `shellextools-0.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/PKG-INFO` & `shellextools-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.13
+Version: 0.14
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

### Comparing `shellextools-0.13/README.md` & `shellextools-0.14/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/setup.py` & `shellextools-0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.13'''
+VERSION = '''0.14'''
 DESCRIPTION = '''Adds Python functions/methods to the Windows context menu'''
 
 # Setting up
 setup(
     name="shellextools",
     version=VERSION,
     license='MIT',
```

### Comparing `shellextools-0.13/shellextools/LICENSE` & `shellextools-0.14/shellextools/LICENSE`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/shellextools/README.md` & `shellextools-0.14/shellextools/README.md`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/shellextools/__init__.py` & `shellextools-0.14/shellextools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1465,56 +1465,68 @@
     mainmenuitem,
     submenu,
     futurnameofcompiledexe,
     filetypes,
     additional_arguments="",
     loopnumber=0,
 ):
+    filetypes=[x.strip() for x in filetypes]
     fileswritten = []
     if check_if_admin() == False:
         return 1
 
     dataf, cmdtools, myfile, newpath, newpathescaped, newpathuninstall = get_new_file_vars(
         folderinprogramdata, futurnameofcompiledexe
     )
     addtocommand0=r'\"'
     addtocommand1=r'\"'
     additional_arguments = additional_arguments.strip()
     if additional_arguments:
         additional_arguments = f" {additional_arguments}"
+
     commandsraw = [
         rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}" /v "MUIVerb" /t REG_SZ /d "{mainmenuitem}" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}" /v "SubCommands" /t REG_SZ /d "" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}\shell" /v "MUIVerb" /t REG_SZ /d "{submenu}" /f""",
+        rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}\shell\{submenu}" /f""",
+        rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}\shell\{submenu}\command" /ve /t REG_SZ /d "{newpathescaped} \"%1\"{additional_arguments}" /f""",
+
         rf"""%systemroot%\system32\Reg.exe add "HKCR\.FTYPE\shell\{mainmenuitem}\shell\{submenu}\command" /ve /t REG_SZ /d "{newpathescaped} \"%1\"{additional_arguments}" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}" /v "MUIVerb" /t REG_SZ /d "{mainmenuitem}" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}" /v "SubCommands" /t REG_SZ /d "" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}\shell" /v "MUIVerb" /t REG_SZ /d "{submenu}" /f""",
         rf"""%systemroot%\system32\Reg.exe add "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}\shell\{submenu}\command" /ve /t REG_SZ /d "\"{newpath}\" --path {addtocommand0}%1{addtocommand1}{additional_arguments}" /f""",
     ]
+
     commandsrawdelete = [
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\.FTYPE\shell\{mainmenuitem}" /f""",
-
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\.FTYPE\shell\{mainmenuitem}\shell" /f""",
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\.FTYPE\shell\{mainmenuitem}\shell\{submenu}" /f""",
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}\shell\{submenu}" /f""",
         rf"""%systemroot%\system32\Reg.exe delete "HKCR\SystemFileAssociations\.FTYPE\shell\{mainmenuitem}" /f""",
 
 
     ]
     uninstalldatalist = []
     for fi in filetypes:
         for c in commandsrawdelete:
-            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
+            if fi !='*':
+                command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
+            else:
+                command2add = c.replace(rf"\.FTYPE{os.sep}", rf"{os.sep}*{os.sep}")
+
             uninstalldatalist.append(command2add)
 
     commands = []
     for fi in filetypes:
         for c in commandsraw:
-            command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
+            if fi != '*':
+                command2add = c.replace(rf"\.FTYPE{os.sep}", rf"\.{fi.strip('. ')}{os.sep}")
+            else:
+                command2add = c.replace(rf"\.FTYPE{os.sep}", rf"{os.sep}*{os.sep}")
             commands.append(command2add)
 
     for c in commands:
         subprocess.run(c, shell=True)
 
     shutil.copy(myfile, newpath)
     fileswritten.append(newpath)
```

### Comparing `shellextools-0.13/shellextools/getmultifiles.py` & `shellextools-0.14/shellextools/getmultifiles.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/shellextools/loggax3.py` & `shellextools-0.14/shellextools/loggax3.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/shellextools/thirdparty.json` & `shellextools-0.14/shellextools/thirdparty.json`

 * *Files identical despite different names*

### Comparing `shellextools-0.13/shellextools.egg-info/PKG-INFO` & `shellextools-0.14/shellextools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.13
+Version: 0.14
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
```

