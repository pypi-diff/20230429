# Comparing `tmp/torf-cli-5.0.0.tar.gz` & `tmp/torf-cli-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torf-cli-5.0.0.tar", last modified: Thu Apr 13 08:27:34 2023, max compression
+gzip compressed data, was "torf-cli-5.1.0.tar", last modified: Sat Apr 29 13:05:16 2023, max compression
```

## Comparing `torf-cli-5.0.0.tar` & `torf-cli-5.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/
--rw-------   0 ich       (1000) ich       (1000)    35147 2018-01-11 12:25:16.000000 torf-cli-5.0.0/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-13 08:27:34.511725 torf-cli-5.0.0/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     8011 2022-05-03 14:08:27.000000 torf-cli-5.0.0/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.507725 torf-cli-5.0.0/docs/
--rw-------   0 ich       (1000) ich       (1000)    16248 2023-04-10 10:11:45.000000 torf-cli-5.0.0/docs/torf.1
--rw-------   0 ich       (1000) ich       (1000)       38 2023-04-13 08:27:34.511725 torf-cli-5.0.0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1180 2022-12-17 16:14:42.000000 torf-cli-5.0.0/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/tests/
--rw-------   0 ich       (1000) ich       (1000)      999 2020-06-21 10:43:26.000000 torf-cli-5.0.0/tests/test_basics.py
--rw-------   0 ich       (1000) ich       (1000)     8204 2020-08-11 10:31:28.000000 torf-cli-5.0.0/tests/test_configfile.py
--rw-------   0 ich       (1000) ich       (1000)     2165 2020-08-11 10:31:17.000000 torf-cli-5.0.0/tests/test_configformat.py
--rw-------   0 ich       (1000) ich       (1000)    31261 2022-12-17 16:14:42.000000 torf-cli-5.0.0/tests/test_create.py
--rw-------   0 ich       (1000) ich       (1000)    19428 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_edit.py
--rw-------   0 ich       (1000) ich       (1000)     3864 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_errors.py
--rw-------   0 ich       (1000) ich       (1000)    17888 2022-06-02 14:41:48.000000 torf-cli-5.0.0/tests/test_info.py
--rw-------   0 ich       (1000) ich       (1000)     4453 2022-06-02 14:48:45.000000 torf-cli-5.0.0/tests/test_json.py
--rw-------   0 ich       (1000) ich       (1000)     8610 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_metainfo.py
--rw-------   0 ich       (1000) ich       (1000)     4335 2020-08-11 13:03:24.000000 torf-cli-5.0.0/tests/test_profiles.py
--rw-------   0 ich       (1000) ich       (1000)     5666 2020-06-21 10:43:26.000000 torf-cli-5.0.0/tests/test_progress.py
--rw-------   0 ich       (1000) ich       (1000)     8686 2023-04-10 10:22:01.000000 torf-cli-5.0.0/tests/test_reuse.py
--rw-------   0 ich       (1000) ich       (1000)     2313 2020-08-10 10:16:28.000000 torf-cli-5.0.0/tests/test_stdin.py
--rw-------   0 ich       (1000) ich       (1000)     1375 2023-04-12 14:07:26.000000 torf-cli-5.0.0/tests/test_utils.py
--rw-------   0 ich       (1000) ich       (1000)    12745 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_verify.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/torf_cli.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      717 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       37 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       24 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        8 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/top_level.txt
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/torfcli/
--rw-------   0 ich       (1000) ich       (1000)     1236 2022-03-16 17:49:06.000000 torf-cli-5.0.0/torfcli/__init__.py
--rw-------   0 ich       (1000) ich       (1000)      646 2020-06-21 10:43:26.000000 torf-cli-5.0.0/torfcli/__main__.py
--rw-------   0 ich       (1000) ich       (1000)    14028 2023-04-12 13:57:52.000000 torf-cli-5.0.0/torfcli/_config.py
--rw-------   0 ich       (1000) ich       (1000)     3533 2020-06-21 10:43:26.000000 torf-cli-5.0.0/torfcli/_errors.py
--rw-------   0 ich       (1000) ich       (1000)     9261 2022-12-17 16:14:42.000000 torf-cli-5.0.0/torfcli/_main.py
--rw-------   0 ich       (1000) ich       (1000)     3027 2022-04-30 14:21:11.000000 torf-cli-5.0.0/torfcli/_term.py
--rw-------   0 ich       (1000) ich       (1000)    23553 2022-05-05 13:04:31.000000 torf-cli-5.0.0/torfcli/_ui.py
--rw-------   0 ich       (1000) ich       (1000)    10424 2023-04-12 14:02:02.000000 torf-cli-5.0.0/torfcli/_utils.py
--rw-------   0 ich       (1000) ich       (1000)      707 2023-04-13 08:26:36.000000 torf-cli-5.0.0/torfcli/_vars.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-29 13:05:16.457057 torf-cli-5.1.0/
+-rw-------   0 ich       (1000) ich       (1000)    35147 2018-01-11 12:25:16.000000 torf-cli-5.1.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-29 13:05:16.457057 torf-cli-5.1.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     8011 2022-05-03 14:08:27.000000 torf-cli-5.1.0/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-29 13:05:16.453057 torf-cli-5.1.0/docs/
+-rw-------   0 ich       (1000) ich       (1000)    16367 2023-04-29 12:49:50.000000 torf-cli-5.1.0/docs/torf.1
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-04-29 13:05:16.457057 torf-cli-5.1.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1180 2023-04-28 10:21:16.000000 torf-cli-5.1.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-29 13:05:16.457057 torf-cli-5.1.0/tests/
+-rw-------   0 ich       (1000) ich       (1000)      999 2020-06-21 10:43:26.000000 torf-cli-5.1.0/tests/test_basics.py
+-rw-------   0 ich       (1000) ich       (1000)     8204 2020-08-11 10:31:28.000000 torf-cli-5.1.0/tests/test_configfile.py
+-rw-------   0 ich       (1000) ich       (1000)     2165 2020-08-11 10:31:17.000000 torf-cli-5.1.0/tests/test_configformat.py
+-rw-------   0 ich       (1000) ich       (1000)    31707 2023-04-29 12:45:43.000000 torf-cli-5.1.0/tests/test_create.py
+-rw-------   0 ich       (1000) ich       (1000)    20723 2023-04-29 13:03:45.000000 torf-cli-5.1.0/tests/test_edit.py
+-rw-------   0 ich       (1000) ich       (1000)     3864 2022-04-30 14:21:11.000000 torf-cli-5.1.0/tests/test_errors.py
+-rw-------   0 ich       (1000) ich       (1000)    17888 2022-06-02 14:41:48.000000 torf-cli-5.1.0/tests/test_info.py
+-rw-------   0 ich       (1000) ich       (1000)     4453 2022-06-02 14:48:45.000000 torf-cli-5.1.0/tests/test_json.py
+-rw-------   0 ich       (1000) ich       (1000)     8610 2022-04-30 14:21:11.000000 torf-cli-5.1.0/tests/test_metainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     4335 2020-08-11 13:03:24.000000 torf-cli-5.1.0/tests/test_profiles.py
+-rw-------   0 ich       (1000) ich       (1000)     5666 2020-06-21 10:43:26.000000 torf-cli-5.1.0/tests/test_progress.py
+-rw-------   0 ich       (1000) ich       (1000)     8686 2023-04-10 10:22:01.000000 torf-cli-5.1.0/tests/test_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)     2313 2020-08-10 10:16:28.000000 torf-cli-5.1.0/tests/test_stdin.py
+-rw-------   0 ich       (1000) ich       (1000)     1375 2023-04-12 14:07:26.000000 torf-cli-5.1.0/tests/test_utils.py
+-rw-------   0 ich       (1000) ich       (1000)    12745 2022-04-30 14:21:11.000000 torf-cli-5.1.0/tests/test_verify.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-29 13:05:16.457057 torf-cli-5.1.0/torf_cli.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      717 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       37 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       24 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)        8 2023-04-29 13:05:16.000000 torf-cli-5.1.0/torf_cli.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-29 13:05:16.457057 torf-cli-5.1.0/torfcli/
+-rw-------   0 ich       (1000) ich       (1000)     1236 2022-03-16 17:49:06.000000 torf-cli-5.1.0/torfcli/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)      646 2020-06-21 10:43:26.000000 torf-cli-5.1.0/torfcli/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)    14239 2023-04-29 12:45:43.000000 torf-cli-5.1.0/torfcli/_config.py
+-rw-------   0 ich       (1000) ich       (1000)     3533 2020-06-21 10:43:26.000000 torf-cli-5.1.0/torfcli/_errors.py
+-rw-------   0 ich       (1000) ich       (1000)     9351 2023-04-29 12:45:43.000000 torf-cli-5.1.0/torfcli/_main.py
+-rw-------   0 ich       (1000) ich       (1000)     3027 2022-04-30 14:21:11.000000 torf-cli-5.1.0/torfcli/_term.py
+-rw-------   0 ich       (1000) ich       (1000)    23553 2022-05-05 13:04:31.000000 torf-cli-5.1.0/torfcli/_ui.py
+-rw-------   0 ich       (1000) ich       (1000)    10424 2023-04-12 14:02:02.000000 torf-cli-5.1.0/torfcli/_utils.py
+-rw-------   0 ich       (1000) ich       (1000)      707 2023-04-29 12:50:54.000000 torf-cli-5.1.0/torfcli/_vars.py
```

### Comparing `torf-cli-5.0.0/LICENSE` & `torf-cli-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/PKG-INFO` & `torf-cli-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-cli
-Version: 5.0.0
+Version: 5.1.0
 Summary: CLI tool to create, read and edit torrent files
 Home-page: https://github.com/rndusr/torf-cli
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet file cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-cli-5.0.0/README.rst` & `torf-cli-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/docs/torf.1` & `torf-cli-5.1.0/docs/torf.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: torf
 .\"    Author: [see the "AUTHOR(S)" section]
 .\" Generator: Asciidoctor 2.0.18
-.\"      Date: 2023-04-10
+.\"      Date: 2023-04-29
 .\"    Manual: \ \&
 .\"    Source: \ \&
 .\"  Language: English
 .\"
-.TH "TORF" "1" "2023-04-10" "\ \&" "\ \&"
+.TH "TORF" "1" "2023-04-29" "\ \&" "\ \&"
 .ie \n(.g .ds Aq \(aq
 .el       .ds Aq '
 .ss \n[.ss] 0
 .nh
 .ad l
 .de URL
 \fI\\$2\fP <\\$1>\\$3
@@ -383,14 +383,19 @@
 .RS 4
 The maximum piece size when creating a torrent.  SIZE is multiplied by 1 MiB
 (1048576 bytes).  The resulting number must be a power of two (2, 4, 8, 16,
 etc.).  Numbers smaller than 1 are allowed, e.g. \(lq0.25\(rq sets the maximum piece
 size to 256 KiB.
 .RE
 .sp
+\fB\-\-creator\fP, \fB\-a\fP \fICREATOR\fP
+.RS 4
+Name and version of the application that created the torrent.
+.RE
+.sp
 \fB\-\-nocreator\fP, \fB\-A\fP
 .RS 4
 Remove the name of the application that created the torrent from an existing
 torrent.
 .RE
 .sp
 \fB\-\-yes\fP, \fB\-y\fP
```

### Comparing `torf-cli-5.0.0/setup.py` & `torf-cli-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_basics.py` & `torf-cli-5.1.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_configfile.py` & `torf-cli-5.1.0/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_configformat.py` & `torf-cli-5.1.0/tests/test_configformat.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_create.py` & `torf-cli-5.1.0/tests/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,15 +492,15 @@
     with patch.multiple('torfcli._main', _hash_pieces=DEFAULT, _write_torrent=DEFAULT):
         factor = 1.234
         exp_invalid_piece_size = int(factor * 2**20)
         with patch('sys.exit') as mock_exit:
             run([content_path, '--max-piece-size', str(factor)])
         mock_exit.assert_called_once_with(err.Code.CLI)
         cap = capsys.readouterr()
-        assert cap.err == f'{_vars.__appname__}: Piece size must be a power of 2: {exp_invalid_piece_size}\n'
+        assert cap.err == f'{_vars.__appname__}: Piece size must be divisible by 16 KiB: {exp_invalid_piece_size}\n'
 
 
 def test_default_date(capsys, mock_content):
     content_path = str(mock_content)
     exp_torrent_filename = os.path.basename(content_path) + '.torrent'
     exp_torrent_filepath = os.path.join(os.getcwd(), exp_torrent_filename)
 
@@ -644,14 +644,28 @@
     t = torf.Torrent.read(exp_torrent_filepath)
     assert t.comment is None
 
     cap = capsys.readouterr()
     assert 'Comment\t' not in cap.out
 
 
+def test_creator_option(capsys, mock_content):
+    content_path = str(mock_content)
+    exp_torrent_filename = os.path.basename(content_path) + '.torrent'
+    exp_torrent_filepath = os.path.join(os.getcwd(), exp_torrent_filename)
+
+    run([content_path, '--creator', 'Mbombo'])
+
+    t = torf.Torrent.read(exp_torrent_filepath)
+    assert t.created_by == 'Mbombo'
+
+    cap = capsys.readouterr()
+    assert 'Created By\tMbombo' in cap.out
+
+
 def test_nocreator_option(capsys, mock_content):
     content_path = str(mock_content)
     exp_torrent_filename = os.path.basename(content_path) + '.torrent'
     exp_torrent_filepath = os.path.join(os.getcwd(), exp_torrent_filename)
 
     run([content_path, '--nocreator'])
```

### Comparing `torf-cli-5.0.0/tests/test_edit.py` & `torf-cli-5.1.0/tests/test_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 from datetime import datetime
 from unittest.mock import patch
 
 import torf
 
+from torfcli import _config as config
 from torfcli import _errors as err
 from torfcli import _vars, run
 
 
 def test_nonexisting_input(capsys):
     nonexisting_path = '/no/such/file'
     with patch('sys.exit') as mock_exit:
@@ -67,14 +68,38 @@
     outfile = str(tmp_path / 'out.torrent')
     with create_torrent(created_by='The creator') as infile:
         orig = torf.Torrent.read(infile)
         run(['-i', infile, '--nocreator', '-o', outfile])
         new = torf.Torrent.read(outfile)
         assert_torrents_equal(orig, new, created_by=None)
 
+def test_remove_creator_even_when_creator_provided(create_torrent, tmp_path, assert_torrents_equal):
+    outfile = str(tmp_path / 'out.torrent')
+    with create_torrent(created_by='The creator') as infile:
+        orig = torf.Torrent.read(infile)
+        run(['-i', infile, '--nocreator', '--creator', 'A conflicting creator', '-o', outfile])
+        new = torf.Torrent.read(outfile)
+        assert_torrents_equal(orig, new, created_by=None)
+
+def test_edit_creator(create_torrent, tmp_path, assert_torrents_equal):
+    outfile = str(tmp_path / 'out.torrent')
+    with create_torrent(created_by='The creator') as infile:
+        orig = torf.Torrent.read(infile)
+        run(['-i', infile, '--creator', 'A different creator', '-o', outfile])
+        new = torf.Torrent.read(outfile)
+        assert_torrents_equal(orig, new, created_by='A different creator')
+
+def test_edit_default_creator(create_torrent, tmp_path, assert_torrents_equal):
+    outfile = str(tmp_path / 'out.torrent')
+    with create_torrent(created_by='The creator') as infile:
+        orig = torf.Torrent.read(infile)
+        run(['-i', infile, '--creator', '-o', outfile])
+        new = torf.Torrent.read(outfile)
+        assert_torrents_equal(orig, new, created_by=config.DEFAULT_CREATOR)
+
 
 def test_remove_private(create_torrent, tmp_path, assert_torrents_equal):
     outfile = str(tmp_path / 'out.torrent')
     with create_torrent(private=True) as infile:
         orig = torf.Torrent.read(infile)
         run(['-i', infile, '--noprivate', '-o', outfile])
         new = torf.Torrent.read(outfile)
```

### Comparing `torf-cli-5.0.0/tests/test_errors.py` & `torf-cli-5.1.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_info.py` & `torf-cli-5.1.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_json.py` & `torf-cli-5.1.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_metainfo.py` & `torf-cli-5.1.0/tests/test_metainfo.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_profiles.py` & `torf-cli-5.1.0/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_progress.py` & `torf-cli-5.1.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_reuse.py` & `torf-cli-5.1.0/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_stdin.py` & `torf-cli-5.1.0/tests/test_stdin.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_utils.py` & `torf-cli-5.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/tests/test_verify.py` & `torf-cli-5.1.0/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torf_cli.egg-info/PKG-INFO` & `torf-cli-5.1.0/torf_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-cli
-Version: 5.0.0
+Version: 5.1.0
 Summary: CLI tool to create, read and edit torrent files
 Home-page: https://github.com/rndusr/torf-cli
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet file cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-cli-5.0.0/torf_cli.egg-info/SOURCES.txt` & `torf-cli-5.1.0/torf_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/__init__.py` & `torf-cli-5.1.0/torfcli/__init__.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/__main__.py` & `torf-cli-5.1.0/torfcli/__main__.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/_config.py` & `torf-cli-5.1.0/torfcli/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     --tracker, -t TRACKER  List of comma-separated announce URLs; may be
                            given multiple times for multiple tiers
     --webseed, -w WEBSEED  Webseed URL; may be given multiple times
     --private, -p          Forbid clients to use DHT and PEX
     --comment, -c COMMENT  Comment that is stored in the torrent file
     --date, -d DATE        Creation date as YYYY-MM-DD[ HH:MM[:SS]], 'now'
                            or 'today' (default: 'now')
+    --creator, -a CREATOR  Name of application used to create torrent file.
+                           (default: '{DEFAULT_CREATOR}')
     --source, -s SOURCE    Add "source" field
     --xseed, -x            Randomize info hash
     --max-piece-size SIZE  Maximum piece size in multiples of 1 MiB
                            (must be a power of two)
     --notracker, -T        Remove trackers from INPUT
     --nowebseed, -W        Remove webseeds from INPUT
     --noprivate, -P        Remove private flag from INPUT
@@ -113,14 +115,15 @@
 
 _cliparser.add_argument('--name', '-n', default='')
 _cliparser.add_argument('--tracker', '-t', default=[], action='append')
 _cliparser.add_argument('--webseed', '-w', default=[], action='append')
 _cliparser.add_argument('--private', '-p', action='store_true', default=None)
 _cliparser.add_argument('--comment', '-c')
 _cliparser.add_argument('--date', '-d', default='')
+_cliparser.add_argument('--creator', '-a', nargs='?', const=DEFAULT_CREATOR)
 _cliparser.add_argument('--source', '-s', default='')
 _cliparser.add_argument('--xseed', '-x', action='store_true')
 _cliparser.add_argument('--max-piece-size', default=0, type=float)
 
 _cliparser.add_argument('--notracker', '-T', action='store_true')
 _cliparser.add_argument('--nowebseed', '-W', action='store_true')
 _cliparser.add_argument('--noprivate', '-P', action='store_true')
```

### Comparing `torf-cli-5.0.0/torfcli/_errors.py` & `torf-cli-5.1.0/torfcli/_errors.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/_main.py` & `torf-cli-5.1.0/torfcli/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             piece_size_max=cfg['max_piece_size'] if cfg['max_piece_size'] else None,
             trackers=() if cfg['notracker'] else trackers,
             webseeds=() if cfg['nowebseed'] else cfg['webseed'],
             private=False if cfg['noprivate'] else cfg['private'],
             source=None if cfg['nosource'] or not cfg['source'] else cfg['source'],
             randomize_infohash=False if cfg['noxseed'] else cfg['xseed'],
             comment=None if cfg['nocomment'] else cfg['comment'],
-            created_by=None if cfg['nocreator'] else _config.DEFAULT_CREATOR
+            created_by=None if cfg['nocreator'] else (cfg['creator'] or _config.DEFAULT_CREATOR),
         )
     except torf.TorfError as e:
         raise _errors.Error(e)
 
     if cfg['nodate']:
         torrent.creation_date = None
     elif cfg['date']:
@@ -134,14 +134,16 @@
             except torf.TorfError as e:
                 raise _errors.Error(e)
     list_set_or_remove('tracker', 'trackers', split_values_at=',')
     list_set_or_remove('webseed', 'webseeds')
 
     if cfg['nocreator']:
         torrent.created_by = None
+    elif cfg['creator']:
+        torrent.created_by = cfg['creator']
 
     if cfg['nodate']:
         torrent.creation_date = None
     elif cfg['date']:
         torrent.creation_date = cfg['date']
 
     if cfg['PATH']:
```

### Comparing `torf-cli-5.0.0/torfcli/_term.py` & `torf-cli-5.1.0/torfcli/_term.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/_ui.py` & `torf-cli-5.1.0/torfcli/_ui.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/_utils.py` & `torf-cli-5.1.0/torfcli/_utils.py`

 * *Files identical despite different names*

### Comparing `torf-cli-5.0.0/torfcli/_vars.py` & `torf-cli-5.1.0/torfcli/_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-__version__     = '5.0.0'
+__version__     = '5.1.0'
 __appname__     = 'torf'
 __url__         = 'https://github.com/rndusr/torf-cli'
 __description__ = 'CLI tool to create, read and edit torrent files'
```

