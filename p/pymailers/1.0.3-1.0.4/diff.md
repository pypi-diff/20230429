# Comparing `tmp/pymailers-1.0.3.tar.gz` & `tmp/pymailers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymailers-1.0.3.tar", last modified: Sat Apr 29 08:05:22 2023, max compression
+gzip compressed data, was "pymailers-1.0.4.tar", last modified: Sat Apr 29 08:09:17 2023, max compression
```

## Comparing `pymailers-1.0.3.tar` & `pymailers-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:05:22.439000 pymailers-1.0.3/
--rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 08:05:22.423000 pymailers-1.0.3/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)     1107 2023-04-29 08:03:18.000000 pymailers-1.0.3/README.md
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:05:22.247000 pymailers-1.0.3/pymailers/
--rw-rw----   0 root         (0) permagrp2  (9997)      938 2023-04-29 08:01:54.000000 pymailers-1.0.3/pymailers/PyMailer.py
--rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-28 19:23:29.000000 pymailers-1.0.3/pymailers/__init__.py
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:05:22.399000 pymailers-1.0.3/pymailers.egg-info/
--rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 08:05:21.000000 pymailers-1.0.3/pymailers.egg-info/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-29 08:05:21.000000 pymailers-1.0.3/pymailers.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-29 08:05:21.000000 pymailers-1.0.3/pymailers.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-29 08:05:21.000000 pymailers-1.0.3/pymailers.egg-info/top_level.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-29 08:05:22.443000 pymailers-1.0.3/setup.cfg
--rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-29 08:03:44.000000 pymailers-1.0.3/setup.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:09:17.667000 pymailers-1.0.4/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 08:09:17.643000 pymailers-1.0.4/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)     1107 2023-04-29 08:03:18.000000 pymailers-1.0.4/README.md
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:09:17.455000 pymailers-1.0.4/pymailers/
+-rw-rw----   0 root         (0) permagrp2  (9997)      926 2023-04-29 08:08:27.000000 pymailers-1.0.4/pymailers/PyMailer.py
+-rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-28 19:23:29.000000 pymailers-1.0.4/pymailers/__init__.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 08:09:17.555000 pymailers-1.0.4/pymailers.egg-info/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 08:09:16.000000 pymailers-1.0.4/pymailers.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-29 08:09:17.000000 pymailers-1.0.4/pymailers.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-29 08:09:16.000000 pymailers-1.0.4/pymailers.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-29 08:09:16.000000 pymailers-1.0.4/pymailers.egg-info/top_level.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-29 08:09:17.671000 pymailers-1.0.4/setup.cfg
+-rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-29 08:07:50.000000 pymailers-1.0.4/setup.py
```

### Comparing `pymailers-1.0.3/PKG-INFO` & `pymailers-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.0.3
+Version: 1.0.4
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

### Comparing `pymailers-1.0.3/README.md` & `pymailers-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymailers-1.0.3/pymailers/PyMailer.py` & `pymailers-1.0.4/pymailers/PyMailer.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     msg['Subject'] = self.subject
     
     with smtplib.SMTP(self.smtp_host, self.smtp_port) as smtp:
       smtp.starttls()
       smtp.login(self.email, self.password)
       smtp.send_message(msg)
       if self.display:
-        print(f"""SMTP Host : {self.smtp_host}\n
-SMTP Port : {self.smtp_port}\n
-Email : {self.email}\n
-Password : {self.password}\n
-To : {self.to}\n
-Subject : {self.subject}\n
+        print(f"""SMTP Host : {self.smtp_host}
+SMTP Port : {self.smtp_port}
+Email : {self.email}
+Password : {self.password}
+To : {self.to}
+Subject : {self.subject}
 Body : {self.body}\n\n
 Email sent successfully.""")
```

### Comparing `pymailers-1.0.3/pymailers.egg-info/PKG-INFO` & `pymailers-1.0.4/pymailers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.0.3
+Version: 1.0.4
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

### Comparing `pymailers-1.0.3/setup.py` & `pymailers-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pymailers',
-    version='1.0.3',
+    version='1.0.4',
     description='The classic email sending library for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Rio Agung Purnomo',
     author_email='rioagungpurnomo.ak@gmail.com',
     url='https://github.com/rioagungpurnomo/pymailers',
     packages=['pymailers'],
```

