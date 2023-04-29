# Comparing `tmp/gqylpy_ssh-1.2.4-py3-none-any.whl.zip` & `tmp/gqylpy_ssh-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 19026 bytes, number of entries: 7
--rw-r--r--  2.0 unx    21410 b- defN 23-Mar-26 07:06 gqylpy_ssh/__init__.py
--rw-r--r--  2.0 unx    10187 b- defN 23-Mar-26 07:06 gqylpy_ssh/g ssh.py
--rw-r--r--  2.0 unx    26436 b- defN 23-Mar-26 07:06 gqylpy_ssh-1.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2193 b- defN 23-Mar-26 07:06 gqylpy_ssh-1.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-26 07:06 gqylpy_ssh-1.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-26 07:06 gqylpy_ssh-1.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      559 b- defN 23-Mar-26 07:06 gqylpy_ssh-1.2.4.dist-info/RECORD
-7 files, 60888 bytes uncompressed, 18042 bytes compressed:  70.4%
+Zip file size: 19056 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    21469 b- defN 23-Apr-29 01:56 gqylpy_ssh/__init__.py
+-rw-r--r--  2.0 unx    10214 b- defN 23-Apr-29 01:56 gqylpy_ssh/g ssh.py
+-rw-r--r--  2.0 unx    26436 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2192 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      559 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/RECORD
+7 files, 60973 bytes uncompressed, 18072 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gqylpy_ssh/__init__.py
 Comment: 
 
 Filename: gqylpy_ssh/g ssh.py
 Comment: 
 
-Filename: gqylpy_ssh-1.2.4.dist-info/LICENSE
+Filename: gqylpy_ssh-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: gqylpy_ssh-1.2.4.dist-info/METADATA
+Filename: gqylpy_ssh-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: gqylpy_ssh-1.2.4.dist-info/WHEEL
+Filename: gqylpy_ssh-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: gqylpy_ssh-1.2.4.dist-info/top_level.txt
+Filename: gqylpy_ssh-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gqylpy_ssh-1.2.4.dist-info/RECORD
+Filename: gqylpy_ssh-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gqylpy_ssh/__init__.py

```diff
@@ -6,15 +6,15 @@
 
     >>> from gqylpy_ssh import GqylpySSH, Command
     >>> ssh = GqylpySSH('192.168.1.7', 22, username='gqylpy', password=...)
     >>> c: Command = ssh.cmd('echo Hi, GQYLPY')
     >>> c.status_output
     (True, 'Hi, GQYLPY')
 
-    @version: 1.2.4
+    @version: 1.2.5
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-ssh
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 This file is part of gqylpy-ssh.
@@ -28,14 +28,19 @@
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License along
 with gqylpy-ssh. If not, see <https://www.gnu.org/licenses/>.
 """
 import paramiko
+import threading
+
+from typing import Union, Tuple, Generator, Any
+
+__first__: 'GqylpySSH'
 
 
 def __init__(
         hostname:        str,
         port:            int  = 22,
         *,
         username:        str  = None,
@@ -134,18 +139,20 @@
         auto_sudo          =auto_sudo,
         reconnect          =reconnect
     )
 
     if gname is None:
         return gobj
 
-    setattr(__gpack__, gname, gobj)
+    gpack = globals()
+
+    if '__first__' not in gpack:
+        gpack['__first__'] = gobj
 
-    if not hasattr(__gpack__, '__first__'):
-        __gpack__.__first__ = gobj
+    gpack[gname] = gobj
 
 
 class GqylpySSH(paramiko.SSHClient):
 
     def __init__(
         self,
         hostname:        str,
@@ -300,21 +307,21 @@
                     get_pty=get_pty,
                     environment=env
                 )
         return Command(command, stdout, stderr)
 
     def cmd_many(
             self,
-            commands: 'Union[list, tuple]',
+            commands: Union[list, tuple],
             *,
             timeout: int  = None,
             bufsize: int  = None,
             get_pty: bool = None,
             env:     dict = None
-    ) -> 'Generator':
+    ) -> Generator:
         """
         @param commands: A commands tuple or list.
         @param timeout:  Execute command timeout, default permanent.
         @param bufsize:  Buffer size, default permanent.
         @param get_pty:  Whether to enable pseudo-terminal, default False.
         @param env:      A dictionary of environment variables. Indication:
                          server may reject environment variables.
@@ -388,22 +395,22 @@
         return True if command_exitcode == 0 else False
 
     @property
     def output(self) -> str:
         return process(command_output)
 
     @property
-    def status_output(self) -> 'Tuple[bool, str]':
+    def status_output(self) -> Tuple[bool, str]:
         return self.status, self.output
 
     def output_else_raise(self) -> str:
         self.raise_if_error()
         return self.output
 
-    def output_else_define(self, define=None) -> 'Any':
+    def output_else_define(self, define=None) -> Any:
         return self.output if self.status else define
 
     def contain(self, string: str, *, ignore_case: bool = False) -> bool:
         output: str = self.output
         if ignore_case:
             string: str = string.lower()
             output: str = output.lower()
@@ -416,27 +423,27 @@
             raise SSHCommandError
 
     def output_if_contain_string_else_raise(self, string: str) -> str:
         if self.contain(string):
             return self.output
         raise SSHCommandError
 
-    def table2dict(self, *, split: str = None) -> 'Generator':
+    def table2dict(self, *, split: str = None) -> Generator:
         """Convert the titled output to dictionary."""
 
-    def line2list(self, *, split: str = None) -> 'Generator':
+    def line2list(self, *, split: str = None) -> Generator:
         """Convert to list by line."""
 
 
 def gname2gobj(func):
-    def inner(*a, gname: 'Union[str, GqylpySSH]' = None, **kw) -> Command:
+    def inner(*a, gname: Union[str, GqylpySSH] = None, **kw) -> Command:
         if gname is None:
             gobj: GqylpySSH = __first__
         elif gname.__class__ is str:
-            gobj: GqylpySSH = getattr(__gpack__, gname)
+            gobj: GqylpySSH = globals()[gname]
         elif gname.__class__ is GqylpySSH:
             gobj: GqylpySSH = gname
         else:
             raise TypeError
         return func(*a, gname=gobj, **kw)
     return inner
 
@@ -445,15 +452,15 @@
 def cmd(
         command: str,
         *,
         timeout: int  = None,
         bufsize: int  = None,
         get_pty: bool = None,
         env:     dict = None,
-        gname:  'Union[str, GqylpySSH]' = None
+        gname:   Union[str, GqylpySSH] = None
 ) -> Command:
     """
     @param command: A command string.
     @param timeout: Execute command timeout, default permanent.
     @param bufsize: Buffer size, default permanent.
     @param get_pty: Whether to enable pseudo-terminal, default False.
     @param env:     A dictionary of environment variables. Indication:
@@ -467,22 +474,22 @@
         get_pty=get_pty,
         env=env
     )
 
 
 @gname2gobj
 def cmd_many(
-        commands: 'Union[list, tuple]',
+        commands: Union[list, tuple],
         *,
         timeout: int  = None,
         bufsize: int  = None,
         get_pty: bool = None,
         env:     dict = None,
-        gname:  'Union[str, GqylpySSH]' = None
-) -> 'Generator':
+        gname:   Union[str, GqylpySSH] = None
+) -> Generator:
     """
     @param commands: A commands tuple or list.
     @param timeout:  Execute command timeout, default permanent.
     @param bufsize:  Buffer size, default permanent.
     @param get_pty:  Whether to enable pseudo-terminal, default False.
     @param env:      A dictionary of environment variables. Indication:
                      server may reject environment variables.
@@ -501,16 +508,16 @@
 def cmd_async(
         command: str,
         *,
         timeout: int  = None,
         bufsize: int  = None,
         get_pty: bool = None,
         env:     dict = None,
-        gname:  'Union[str, GqylpySSH]' = None
-) -> 'threading.Thread':
+        gname:   Union[str, GqylpySSH] = None
+) -> threading.Thread:
     """
     @param command: A command string.
     @param timeout: Execute command timeout, default permanent.
     @param bufsize: Buffer size, default permanent.
     @param get_pty: Whether to enable pseudo-terminal, default False.
     @param env:     A dictionary of environment variables. Indication:
                     server may reject environment variables.
@@ -534,26 +541,23 @@
 BadHostKeyException       = paramiko.ssh_exception.BadHostKeyException
 IncompatiblePeer          = paramiko.ssh_exception.IncompatiblePeer
 ProxyCommandFailure       = paramiko.ssh_exception.ProxyCommandFailure
 NoValidConnectionsError   = paramiko.ssh_exception.NoValidConnectionsError
 CouldNotCanonicalize      = paramiko.ssh_exception.CouldNotCanonicalize
 ConfigParseError          = paramiko.ssh_exception.ConfigParseError
 
-import sys
-import threading
-from typing import Union, Tuple, Generator, Any
-
-__first__: GqylpySSH
-__gpack__ = sys.modules[__name__]
-
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
-    __import__(f'{__name__}.g {__name__[7:]}')
-    gcode = globals()[f'g {__name__[7:]}']
+    gpack = globals()
+    gpath = f'{__name__}.g {__name__[7:]}'
+    gcode = __import__(gpath, fromlist=...)
 
-    for gname in globals():
-        if gname[0] != '_' and hasattr(gcode, gname):
+    for gname in gpack:
+        try:
+            assert gname[0] != '_' or gname == '__init__'
             gfunc = getattr(gcode, gname)
-            gfunc.__module__ = __package__
-            setattr(__gpack__, gname, gfunc)
-
-    setattr(__gpack__, '__init__', gcode.__init__)
+            assert gfunc.__module__ in (gpath, __package__)
+        except (AssertionError, AttributeError):
+            continue
+        gfunc.__module__ = __package__
+        gfunc.__doc__ = gpack[gname].__doc__
+        gpack[gname] = gfunc
```

## gqylpy_ssh/g ssh.py

```diff
@@ -30,15 +30,16 @@
 from paramiko.ssh_exception import NoValidConnectionsError
 
 from paramiko.channel import ChannelFile
 from paramiko.channel import ChannelStderrFile
 
 first: 'GqylpySSH'
 
-gpack, gcode = sys.modules[__package__], sys.modules[__name__]
+gpack = sys.modules[__package__]
+gcode = sys.modules[__name__]
 
 
 def __init__(
         hostname: str,
         port:     int = 22,
         *,
         gname:    str = None,
@@ -84,15 +85,15 @@
         params['pkey'] = pkey
         self.hostname  = hostname
         self.params    = params
 
     def __del__(self):
         try:
             self.close()
-        except AttributeError:
+        except (TypeError, AttributeError):
             pass
 
     def cmd(
             self,
             command: str,
             *,
             timeout: int  = None,
@@ -171,15 +172,15 @@
             for c in commands:
                 c: str = c.rstrip()
                 if c[-1] == '&':
                     c = c[:-1]
                     warnings.warn(
                         'note that running multiple commands '
                         'in tuple mode cannot use asynchrony "&".'
-                    )
+                    , stacklevel=2)
                 co: Command = self.cmd(c, **kw)
                 co.raise_if_error()
                 yield co
         elif commands.__class__ is list:
             yield from (self.cmd(c, **kw) for c in commands)
         else:
             raise TypeError(
```

## Comparing `gqylpy_ssh-1.2.4.dist-info/LICENSE` & `gqylpy_ssh-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gqylpy_ssh-1.2.4.dist-info/METADATA` & `gqylpy_ssh-1.2.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-ssh
-Version: 1.2.4
+Version: 1.2.5
 Summary: 在远程服务器执行命令并得到执行结果，它是对 paramiko 库的二次封装。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: LGPL
 Project-URL: Source, https://github.com/gqylpy/gqylpy-ssh
 Classifier: Environment :: Web Environment
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: paramiko (<3.0,>=2.10.4)
+Requires-Dist: paramiko (<4.0,>=3.1.0)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-ssh.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-ssh/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_ssh)](https://pypi.org/project/gqylpy_ssh)
 [![License](https://img.shields.io/pypi/l/gqylpy_ssh)](https://github.com/gqylpy/gqylpy-ssh/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_ssh/month)](https://pepy.tech/project/gqylpy_ssh)
 
@@ -38,12 +38,12 @@
 
 <kbd>pip3 install gqylpy_ssh</kbd>
 
 ```python
 >>> from gqylpy_ssh import GqylpySSH, Command
 
 >>> ssh = GqylpySSH('192.168.1.7', 22, username='gqylpy', password=...)
->>> c: Command = ssh.cmd('echo Hi, GQYLPY')
 
+>>> c: Command = ssh.cmd('echo Hi, GQYLPY')
 >>> c.status_output
 (True, 'Hi, GQYLPY')
 ```
```

## Comparing `gqylpy_ssh-1.2.4.dist-info/RECORD` & `gqylpy_ssh-1.2.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-gqylpy_ssh/__init__.py,sha256=F9rJOUhhnyhylSC-UDABJ4gLCa014abLYB_L9wGXqiI,21410
-gqylpy_ssh/g ssh.py,sha256=ww497j34VWd-WxwHZKsTASXYttYJfMy2Lu6nnL89aC0,10187
-gqylpy_ssh-1.2.4.dist-info/LICENSE,sha256=X6Jb9fOV_SbnAcLh3kyn0WKBaYbceRwi-PQiaFetG7I,26436
-gqylpy_ssh-1.2.4.dist-info/METADATA,sha256=X0VFZp9LHTp0-TymRP5_mAdMXLu_DecbioJCvF8SzcA,2193
-gqylpy_ssh-1.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gqylpy_ssh-1.2.4.dist-info/top_level.txt,sha256=y1KYztkiTUtiUdgCbFb7QvSotTeXe2iCsRw4x7SZscU,11
-gqylpy_ssh-1.2.4.dist-info/RECORD,,
+gqylpy_ssh/__init__.py,sha256=GuhtpKmtDNdX4APz5-qS5xUH6VjyK3YqlvjpBkfx-vM,21469
+gqylpy_ssh/g ssh.py,sha256=RI6GU4lmeR3j9D8VhMbDLhmaIecL5kkCcfIDkpYYPl0,10214
+gqylpy_ssh-1.2.5.dist-info/LICENSE,sha256=X6Jb9fOV_SbnAcLh3kyn0WKBaYbceRwi-PQiaFetG7I,26436
+gqylpy_ssh-1.2.5.dist-info/METADATA,sha256=9-52P_n8aO6DfXMRB9DWeunj4x_FXsPIQLFPlI97s1M,2192
+gqylpy_ssh-1.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gqylpy_ssh-1.2.5.dist-info/top_level.txt,sha256=y1KYztkiTUtiUdgCbFb7QvSotTeXe2iCsRw4x7SZscU,11
+gqylpy_ssh-1.2.5.dist-info/RECORD,,
```

