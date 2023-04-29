# Comparing `tmp/pyarmor-8.1.dev9.zip` & `tmp/pyarmor-8.2.dev1.zip`

## zipinfo {}

```diff
@@ -1,139 +1,139 @@
-Zip file size: 2305851 bytes, number of entries: 137
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/
--rw-r--r--  2.0 unx     3004 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/PKG-INFO
--rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.1.dev9/MANIFEST.in
--rw-r--r--  2.0 unx     6531 b- defN 23-Apr-01 19:34 pyarmor-8.1.dev9/README.md
--rw-r--r--  2.0 unx     4296 b- defN 23-Apr-09 07:41 pyarmor-8.1.dev9/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/setup.cfg
--rw-r--r--  2.0 unx     3004 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     2911 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      135 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 07:42 pyarmor-8.1.dev9/pyarmor.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/plugins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/polyfills/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/helper/
--rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/pyshield.lic
--rwxr-xr-x  2.0 unx     2038 b- defN 23-Apr-09 07:41 pyarmor-8.1.dev9/src/config.py
--rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/benchmark.py
--rw-r--r--  2.0 unx     7265 b- defN 22-Feb-25 10:48 pyarmor-8.1.dev9/src/register.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/product.key
--rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.1.dev9/src/pyarmor.py
--rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.1.dev9/src/protect_code.pt
--rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.1.dev9/src/pytransform.py
--rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.1.dev9/src/sppmode.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/public.key
--rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.1.dev9/src/__init__.py
--rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.1.dev9/src/reform.py
--rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.1.dev9/src/packer.py
--rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.1.dev9/src/cobuilder.py
--rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.1.dev9/src/utils.py
--rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/pyarmor-webui.py
--rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.1.dev9/src/build_meta.py
--rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/license.tri
--rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.1.dev9/src/README.rst
--rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.1.dev9/src/protect_code2.pt
--rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/public_capsule.zip
--rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.1.dev9/src/project.py
--rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.1.dev9/src/pyshield.key
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/linux/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/darwin/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/windows/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/linux/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/linux/x86_64/
--rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.1.dev9/src/platforms/linux/x86/_pytransform.so
--rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.1.dev9/src/platforms/linux/x86_64/_pytransform.so
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/darwin/x86_64/
--rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.1.dev9/src/platforms/darwin/x86_64/_pytransform.dylib
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/windows/x86/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/platforms/windows/x86_64/
--rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.1.dev9/src/platforms/windows/x86/_pytransform.dll
--rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.1.dev9/src/platforms/windows/x86_64/_pytransform.dll
--rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.1.dev9/src/plugins/README.md
--rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/plugins/check_ntp_time.py
--rw-r--r--  2.0 unx     8608 b- defN 23-Apr-02 22:49 pyarmor-8.1.dev9/src/cli/config.py
--rw-r--r--  2.0 unx    10980 b- defN 23-Apr-07 06:19 pyarmor-8.1.dev9/src/cli/register.py
--rw-r--r--  2.0 unx     5603 b- defN 23-Apr-05 09:07 pyarmor-8.1.dev9/src/cli/generate.py
--rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.1.dev9/src/cli/shell.py
--rw-r--r--  2.0 unx     6366 b- defN 23-Apr-06 19:59 pyarmor-8.1.dev9/src/cli/resource.py
--rw-r--r--  2.0 unx     1292 b- defN 23-Apr-06 00:02 pyarmor-8.1.dev9/src/cli/__init__.py
--rw-r--r--  2.0 unx    15562 b- defN 23-Apr-08 08:25 pyarmor-8.1.dev9/src/cli/context.py
--rw-r--r--  2.0 unx      880 b- defN 23-Jan-12 17:29 pyarmor-8.1.dev9/src/cli/errors.py
--rw-r--r--  2.0 unx     4008 b- defN 23-Feb-11 09:53 pyarmor-8.1.dev9/src/cli/mixer.py
--rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.1.dev9/src/cli/public_capsule.zip
--rw-r--r--  2.0 unx     7736 b- defN 23-Apr-08 12:34 pyarmor-8.1.dev9/src/cli/default.cfg
--rw-r--r--  2.0 unx    20090 b- defN 23-Apr-09 07:41 pyarmor-8.1.dev9/src/cli/__main__.py
--rw-r--r--  2.0 unx    11386 b- defN 23-Mar-29 21:18 pyarmor-8.1.dev9/src/cli/repack.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/helloworld/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/cx_Freeze/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/simple/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/pybench/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/testpkg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/testmod/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/py2exe/
--rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.1.dev9/src/examples/obfuscate-pkg.bat
--rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.1.dev9/src/examples/obfuscate-app.bat
--rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/obfuscate-app.sh
--rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/obfuscate-pkg.sh
--rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/build-with-project.bat
--rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/README.md
--rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.sh
--rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.bat
--rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/build-with-project.sh
--rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/build-for-freeze.bat
--rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/examples/README-ZH.md
--rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/build-for-exe.bat
--rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/helloworld/foo.py
--rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/cx_Freeze/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/cx_Freeze/queens.py
--rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/cx_Freeze/setup.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/simple/queens.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/pybench/package/
--rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Arithmetic.py
--rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/With.py
--rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Lists.py
--rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Tuples.py
--rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Instances.py
--rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/systimes.py
--rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/clockres.py
--rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Lookups.py
--rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/CommandLine.py
--rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Numbers.py
--rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Imports.py
--rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Setup.py
--rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Exceptions.py
--rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Dict.py
--rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/pybench.py
--rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/NewInstances.py
--rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Calls.py
--rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Strings.py
--rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/Constructs.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/package/__init__.py
--rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/pybench/package/submodule.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-09 07:42 pyarmor-8.1.dev9/src/examples/testpkg/mypkg/
--rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/testpkg/main.py
--rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/testpkg/mypkg/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/testpkg/mypkg/foo.py
--rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/testmod/hello.py
--rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/testmod/queens.py
--rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/py2exe/hello.py
--rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/py2exe/queens.py
--rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/examples/py2exe/setup.py
--rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/polyfills/__init__.py
--rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.1.dev9/src/polyfills/argparse.py
--rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/superuntime.py
--rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.1.dev9/src/helper/merge.py
--rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/buildext.py
--rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/get_platform_name.py
--rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/get_license_info.py
--rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/get_bind_key.py
--rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/__init__.py
--rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.1.dev9/src/helper/build_data_module.py
--rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.1.dev9/src/helper/repack.py
-137 files, 7358944 bytes uncompressed, 2284127 bytes compressed:  69.0%
+Zip file size: 2309199 bytes, number of entries: 137
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/
+-rw-r--r--  2.0 unx     3004 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/PKG-INFO
+-rwxr-xr-x  2.0 unx      191 b- defN 23-Mar-04 11:58 pyarmor-8.2.dev1/MANIFEST.in
+-rw-r--r--  2.0 unx     6692 b- defN 23-Apr-20 10:36 pyarmor-8.2.dev1/README.md
+-rw-r--r--  2.0 unx     4296 b- defN 23-Apr-28 08:42 pyarmor-8.2.dev1/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/setup.cfg
+-rw-r--r--  2.0 unx     3004 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     2911 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      135 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-29 09:12 pyarmor-8.2.dev1/pyarmor.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/plugins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/polyfills/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/helper/
+-rw-r--r--  2.0 unx      234 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/pyshield.lic
+-rwxr-xr-x  2.0 unx     2038 b- defN 23-Apr-28 08:40 pyarmor-8.2.dev1/src/config.py
+-rwxr-xr-x  2.0 unx    10197 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/benchmark.py
+-rw-r--r--  2.0 unx     7265 b- defN 22-Feb-25 10:48 pyarmor-8.2.dev1/src/register.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/product.key
+-rwxr-xr-x  2.0 unx    65827 b- defN 23-Mar-26 00:20 pyarmor-8.2.dev1/src/pyarmor.py
+-rw-r--r--  2.0 unx     2664 b- defN 22-Jan-29 09:20 pyarmor-8.2.dev1/src/protect_code.pt
+-rw-r--r--  2.0 unx    13587 b- defN 21-Nov-02 17:34 pyarmor-8.2.dev1/src/pytransform.py
+-rw-r--r--  2.0 unx     3363 b- defN 22-Jun-27 00:08 pyarmor-8.2.dev1/src/sppmode.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/public.key
+-rwxr-xr-x  2.0 unx      113 b- defN 20-Jan-02 11:09 pyarmor-8.2.dev1/src/__init__.py
+-rw-r--r--  2.0 unx     2191 b- defN 22-Dec-04 19:13 pyarmor-8.2.dev1/src/reform.py
+-rwxr-xr-x  2.0 unx    25832 b- defN 22-Nov-20 13:42 pyarmor-8.2.dev1/src/packer.py
+-rw-r--r--  2.0 unx     5200 b- defN 23-Jan-06 00:02 pyarmor-8.2.dev1/src/cobuilder.py
+-rwxr-xr-x  2.0 unx    67431 b- defN 22-Dec-23 17:42 pyarmor-8.2.dev1/src/utils.py
+-rw-r--r--  2.0 unx       37 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/pyarmor-webui.py
+-rw-r--r--  2.0 unx     4028 b- defN 21-Dec-16 08:28 pyarmor-8.2.dev1/src/build_meta.py
+-rw-r--r--  2.0 unx      256 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/license.tri
+-rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor-8.2.dev1/src/README.rst
+-rw-r--r--  2.0 unx     1596 b- defN 22-Jan-30 11:51 pyarmor-8.2.dev1/src/protect_code2.pt
+-rw-r--r--  2.0 unx     2487 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/public_capsule.zip
+-rwxr-xr-x  2.0 unx     8023 b- defN 22-Jun-28 09:01 pyarmor-8.2.dev1/src/project.py
+-rw-r--r--  2.0 unx      140 b- defN 19-Dec-07 07:11 pyarmor-8.2.dev1/src/pyshield.key
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/darwin/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/linux/x86_64/
+-rwxr-xr-x  2.0 unx  1421600 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so
+-rwxr-xr-x  2.0 unx  1198080 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/darwin/x86_64/
+-rwxr-xr-x  2.0 unx  1469620 b- defN 22-Sep-28 18:28 pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/x86/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/platforms/windows/x86_64/
+-rw-r--r--  2.0 unx  1373710 b- defN 22-Sep-28 21:00 pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll
+-rwxr-xr-x  2.0 unx  1165824 b- defN 22-Sep-28 20:59 pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll
+-rw-r--r--  2.0 unx     6360 b- defN 22-Jul-14 19:38 pyarmor-8.2.dev1/src/plugins/README.md
+-rw-r--r--  2.0 unx    13688 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/plugins/check_ntp_time.py
+-rw-r--r--  2.0 unx    10694 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev1/src/cli/config.py
+-rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 08:43 pyarmor-8.2.dev1/src/cli/register.py
+-rw-r--r--  2.0 unx     5553 b- defN 23-Apr-22 08:21 pyarmor-8.2.dev1/src/cli/generate.py
+-rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor-8.2.dev1/src/cli/shell.py
+-rw-r--r--  2.0 unx     6398 b- defN 23-Apr-13 14:46 pyarmor-8.2.dev1/src/cli/resource.py
+-rw-r--r--  2.0 unx     1479 b- defN 23-Apr-25 09:18 pyarmor-8.2.dev1/src/cli/__init__.py
+-rw-r--r--  2.0 unx    17255 b- defN 23-Apr-29 06:34 pyarmor-8.2.dev1/src/cli/context.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Apr-22 22:15 pyarmor-8.2.dev1/src/cli/plugin.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor-8.2.dev1/src/cli/mixer.py
+-rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor-8.2.dev1/src/cli/public_capsule.zip
+-rw-r--r--  2.0 unx     7475 b- defN 23-Apr-27 08:20 pyarmor-8.2.dev1/src/cli/default.cfg
+-rw-r--r--  2.0 unx    22591 b- defN 23-Apr-29 07:46 pyarmor-8.2.dev1/src/cli/__main__.py
+-rw-r--r--  2.0 unx    11386 b- defN 23-Apr-20 15:01 pyarmor-8.2.dev1/src/cli/repack.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/helloworld/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/cx_Freeze/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/simple/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/pybench/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testpkg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testmod/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/py2exe/
+-rwxr-xr-x  2.0 unx     2048 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat
+-rwxr-xr-x  2.0 unx     1645 b- defN 22-Mar-10 20:03 pyarmor-8.2.dev1/src/examples/obfuscate-app.bat
+-rwxr-xr-x  2.0 unx     1103 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/obfuscate-app.sh
+-rwxr-xr-x  2.0 unx     1685 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh
+-rwxr-xr-x  2.0 unx     4102 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/build-with-project.bat
+-rw-r--r--  2.0 unx     6876 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/README.md
+-rwxr-xr-x  2.0 unx      773 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh
+-rwxr-xr-x  2.0 unx      928 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat
+-rwxr-xr-x  2.0 unx     3146 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/build-with-project.sh
+-rwxr-xr-x  2.0 unx     4395 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/build-for-freeze.bat
+-rw-r--r--  2.0 unx     7078 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/examples/README-ZH.md
+-rwxr-xr-x  2.0 unx     4231 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/build-for-exe.bat
+-rw-r--r--  2.0 unx     1747 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/helloworld/foo.py
+-rwxr-xr-x  2.0 unx       49 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py
+-rwxr-xr-x  2.0 unx      641 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/simple/queens.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/pybench/package/
+-rwxr-xr-x  2.0 unx    13565 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py
+-rwxr-xr-x  2.0 unx     4134 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/With.py
+-rwxr-xr-x  2.0 unx     6460 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Lists.py
+-rwxr-xr-x  2.0 unx     8034 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Tuples.py
+-rwxr-xr-x  2.0 unx     1388 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Instances.py
+-rwxr-xr-x  2.0 unx     6672 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/systimes.py
+-rwxr-xr-x  2.0 unx     1193 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/clockres.py
+-rwxr-xr-x  2.0 unx    15254 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Lookups.py
+-rwxr-xr-x  2.0 unx    16870 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py
+-rwxr-xr-x  2.0 unx    16198 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Numbers.py
+-rwxr-xr-x  2.0 unx     2941 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Imports.py
+-rwxr-xr-x  2.0 unx      961 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Setup.py
+-rwxr-xr-x  2.0 unx    13400 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py
+-rwxr-xr-x  2.0 unx     9261 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Dict.py
+-rwxr-xr-x  2.0 unx    31828 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/pybench.py
+-rwxr-xr-x  2.0 unx     1561 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py
+-rwxr-xr-x  2.0 unx     9252 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Calls.py
+-rwxr-xr-x  2.0 unx    10946 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Strings.py
+-rwxr-xr-x  2.0 unx    13207 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/Constructs.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/package/__init__.py
+-rwxr-xr-x  2.0 unx        0 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/pybench/package/submodule.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-29 09:12 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/
+-rw-r--r--  2.0 unx       66 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/main.py
+-rw-r--r--  2.0 unx      202 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testpkg/mypkg/foo.py
+-rwxr-xr-x  2.0 unx     1734 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testmod/hello.py
+-rwxr-xr-x  2.0 unx     3694 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/testmod/queens.py
+-rwxr-xr-x  2.0 unx       44 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/hello.py
+-rwxr-xr-x  2.0 unx     2309 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/queens.py
+-rwxr-xr-x  2.0 unx     1081 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/examples/py2exe/setup.py
+-rw-r--r--  2.0 unx       28 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/polyfills/__init__.py
+-rwxr-xr-x  2.0 unx    88440 b- defN 19-Dec-05 18:38 pyarmor-8.2.dev1/src/polyfills/argparse.py
+-rw-r--r--  2.0 unx     1505 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/superuntime.py
+-rw-r--r--  2.0 unx     9191 b- defN 22-Jan-06 22:40 pyarmor-8.2.dev1/src/helper/merge.py
+-rw-r--r--  2.0 unx    11618 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/buildext.py
+-rw-r--r--  2.0 unx     2144 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_platform_name.py
+-rw-r--r--  2.0 unx      778 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_license_info.py
+-rw-r--r--  2.0 unx      728 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/get_bind_key.py
+-rw-r--r--  2.0 unx        1 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/__init__.py
+-rw-r--r--  2.0 unx     3821 b- defN 21-Oct-13 13:01 pyarmor-8.2.dev1/src/helper/build_data_module.py
+-rw-r--r--  2.0 unx    12719 b- defN 23-Mar-21 13:48 pyarmor-8.2.dev1/src/helper/repack.py
+137 files, 7373641 bytes uncompressed, 2287475 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,412 +1,412 @@
-Filename: pyarmor-8.1.dev9/
+Filename: pyarmor-8.2.dev1/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/
+Filename: pyarmor-8.2.dev1/src/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/PKG-INFO
+Filename: pyarmor-8.2.dev1/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.1.dev9/MANIFEST.in
+Filename: pyarmor-8.2.dev1/MANIFEST.in
 Comment: 
 
-Filename: pyarmor-8.1.dev9/README.md
+Filename: pyarmor-8.2.dev1/README.md
 Comment: 
 
-Filename: pyarmor-8.1.dev9/setup.py
+Filename: pyarmor-8.2.dev1/setup.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/setup.cfg
+Filename: pyarmor-8.2.dev1/setup.cfg
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/PKG-INFO
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/SOURCES.txt
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/entry_points.txt
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/requires.txt
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/requires.txt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/top_level.txt
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/pyarmor.egg-info/dependency_links.txt
+Filename: pyarmor-8.2.dev1/pyarmor.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/
+Filename: pyarmor-8.2.dev1/src/platforms/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/plugins/
+Filename: pyarmor-8.2.dev1/src/plugins/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/
+Filename: pyarmor-8.2.dev1/src/cli/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/
+Filename: pyarmor-8.2.dev1/src/examples/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/polyfills/
+Filename: pyarmor-8.2.dev1/src/polyfills/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/
+Filename: pyarmor-8.2.dev1/src/helper/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/pyshield.lic
+Filename: pyarmor-8.2.dev1/src/pyshield.lic
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/config.py
+Filename: pyarmor-8.2.dev1/src/config.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/benchmark.py
+Filename: pyarmor-8.2.dev1/src/benchmark.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/register.py
+Filename: pyarmor-8.2.dev1/src/register.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/product.key
+Filename: pyarmor-8.2.dev1/src/product.key
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/pyarmor.py
+Filename: pyarmor-8.2.dev1/src/pyarmor.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/protect_code.pt
+Filename: pyarmor-8.2.dev1/src/protect_code.pt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/pytransform.py
+Filename: pyarmor-8.2.dev1/src/pytransform.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/sppmode.py
+Filename: pyarmor-8.2.dev1/src/sppmode.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/public.key
+Filename: pyarmor-8.2.dev1/src/public.key
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/__init__.py
+Filename: pyarmor-8.2.dev1/src/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/reform.py
+Filename: pyarmor-8.2.dev1/src/reform.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/packer.py
+Filename: pyarmor-8.2.dev1/src/packer.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cobuilder.py
+Filename: pyarmor-8.2.dev1/src/cobuilder.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/utils.py
+Filename: pyarmor-8.2.dev1/src/utils.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/pyarmor-webui.py
+Filename: pyarmor-8.2.dev1/src/pyarmor-webui.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/build_meta.py
+Filename: pyarmor-8.2.dev1/src/build_meta.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/license.tri
+Filename: pyarmor-8.2.dev1/src/license.tri
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/README.rst
+Filename: pyarmor-8.2.dev1/src/README.rst
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/protect_code2.pt
+Filename: pyarmor-8.2.dev1/src/protect_code2.pt
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/public_capsule.zip
+Filename: pyarmor-8.2.dev1/src/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/project.py
+Filename: pyarmor-8.2.dev1/src/project.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/pyshield.key
+Filename: pyarmor-8.2.dev1/src/pyshield.key
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/linux/
+Filename: pyarmor-8.2.dev1/src/platforms/linux/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/darwin/
+Filename: pyarmor-8.2.dev1/src/platforms/darwin/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/windows/
+Filename: pyarmor-8.2.dev1/src/platforms/windows/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/linux/x86/
+Filename: pyarmor-8.2.dev1/src/platforms/linux/x86/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/linux/x86_64/
+Filename: pyarmor-8.2.dev1/src/platforms/linux/x86_64/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/linux/x86/_pytransform.so
+Filename: pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/linux/x86_64/_pytransform.so
+Filename: pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/darwin/x86_64/
+Filename: pyarmor-8.2.dev1/src/platforms/darwin/x86_64/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/darwin/x86_64/_pytransform.dylib
+Filename: pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/windows/x86/
+Filename: pyarmor-8.2.dev1/src/platforms/windows/x86/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/windows/x86_64/
+Filename: pyarmor-8.2.dev1/src/platforms/windows/x86_64/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/windows/x86/_pytransform.dll
+Filename: pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/platforms/windows/x86_64/_pytransform.dll
+Filename: pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/plugins/README.md
+Filename: pyarmor-8.2.dev1/src/plugins/README.md
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/plugins/check_ntp_time.py
+Filename: pyarmor-8.2.dev1/src/plugins/check_ntp_time.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/config.py
+Filename: pyarmor-8.2.dev1/src/cli/config.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/register.py
+Filename: pyarmor-8.2.dev1/src/cli/register.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/generate.py
+Filename: pyarmor-8.2.dev1/src/cli/generate.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/shell.py
+Filename: pyarmor-8.2.dev1/src/cli/shell.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/resource.py
+Filename: pyarmor-8.2.dev1/src/cli/resource.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/__init__.py
+Filename: pyarmor-8.2.dev1/src/cli/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/context.py
+Filename: pyarmor-8.2.dev1/src/cli/context.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/errors.py
+Filename: pyarmor-8.2.dev1/src/cli/plugin.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/mixer.py
+Filename: pyarmor-8.2.dev1/src/cli/mixer.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/public_capsule.zip
+Filename: pyarmor-8.2.dev1/src/cli/public_capsule.zip
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/default.cfg
+Filename: pyarmor-8.2.dev1/src/cli/default.cfg
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/__main__.py
+Filename: pyarmor-8.2.dev1/src/cli/__main__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/cli/repack.py
+Filename: pyarmor-8.2.dev1/src/cli/repack.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/helloworld/
+Filename: pyarmor-8.2.dev1/src/examples/helloworld/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/cx_Freeze/
+Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/simple/
+Filename: pyarmor-8.2.dev1/src/examples/simple/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/
+Filename: pyarmor-8.2.dev1/src/examples/pybench/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testpkg/
+Filename: pyarmor-8.2.dev1/src/examples/testpkg/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testmod/
+Filename: pyarmor-8.2.dev1/src/examples/testmod/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/py2exe/
+Filename: pyarmor-8.2.dev1/src/examples/py2exe/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/obfuscate-pkg.bat
+Filename: pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/obfuscate-app.bat
+Filename: pyarmor-8.2.dev1/src/examples/obfuscate-app.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/obfuscate-app.sh
+Filename: pyarmor-8.2.dev1/src/examples/obfuscate-app.sh
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/obfuscate-pkg.sh
+Filename: pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/build-with-project.bat
+Filename: pyarmor-8.2.dev1/src/examples/build-with-project.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/README.md
+Filename: pyarmor-8.2.dev1/src/examples/README.md
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.sh
+Filename: pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.bat
+Filename: pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/build-with-project.sh
+Filename: pyarmor-8.2.dev1/src/examples/build-with-project.sh
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/build-for-freeze.bat
+Filename: pyarmor-8.2.dev1/src/examples/build-for-freeze.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/README-ZH.md
+Filename: pyarmor-8.2.dev1/src/examples/README-ZH.md
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/build-for-exe.bat
+Filename: pyarmor-8.2.dev1/src/examples/build-for-exe.bat
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/helloworld/foo.py
+Filename: pyarmor-8.2.dev1/src/examples/helloworld/foo.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/cx_Freeze/hello.py
+Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/hello.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/cx_Freeze/queens.py
+Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/cx_Freeze/setup.py
+Filename: pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/simple/queens.py
+Filename: pyarmor-8.2.dev1/src/examples/simple/queens.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/package/
+Filename: pyarmor-8.2.dev1/src/examples/pybench/package/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Arithmetic.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/With.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/With.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Lists.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Lists.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Tuples.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Tuples.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Instances.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Instances.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/systimes.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/systimes.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/clockres.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/clockres.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Lookups.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Lookups.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/CommandLine.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Numbers.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Numbers.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Imports.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Imports.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Setup.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Setup.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Exceptions.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Dict.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Dict.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/pybench.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/pybench.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/NewInstances.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Calls.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Calls.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Strings.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Strings.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/Constructs.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/Constructs.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/package/__init__.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/package/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/pybench/package/submodule.py
+Filename: pyarmor-8.2.dev1/src/examples/pybench/package/submodule.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testpkg/mypkg/
+Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testpkg/main.py
+Filename: pyarmor-8.2.dev1/src/examples/testpkg/main.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testpkg/mypkg/__init__.py
+Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testpkg/mypkg/foo.py
+Filename: pyarmor-8.2.dev1/src/examples/testpkg/mypkg/foo.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testmod/hello.py
+Filename: pyarmor-8.2.dev1/src/examples/testmod/hello.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/testmod/queens.py
+Filename: pyarmor-8.2.dev1/src/examples/testmod/queens.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/py2exe/hello.py
+Filename: pyarmor-8.2.dev1/src/examples/py2exe/hello.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/py2exe/queens.py
+Filename: pyarmor-8.2.dev1/src/examples/py2exe/queens.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/examples/py2exe/setup.py
+Filename: pyarmor-8.2.dev1/src/examples/py2exe/setup.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/polyfills/__init__.py
+Filename: pyarmor-8.2.dev1/src/polyfills/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/polyfills/argparse.py
+Filename: pyarmor-8.2.dev1/src/polyfills/argparse.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/superuntime.py
+Filename: pyarmor-8.2.dev1/src/helper/superuntime.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/merge.py
+Filename: pyarmor-8.2.dev1/src/helper/merge.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/buildext.py
+Filename: pyarmor-8.2.dev1/src/helper/buildext.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/get_platform_name.py
+Filename: pyarmor-8.2.dev1/src/helper/get_platform_name.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/get_license_info.py
+Filename: pyarmor-8.2.dev1/src/helper/get_license_info.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/get_bind_key.py
+Filename: pyarmor-8.2.dev1/src/helper/get_bind_key.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/__init__.py
+Filename: pyarmor-8.2.dev1/src/helper/__init__.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/build_data_module.py
+Filename: pyarmor-8.2.dev1/src/helper/build_data_module.py
 Comment: 
 
-Filename: pyarmor-8.1.dev9/src/helper/repack.py
+Filename: pyarmor-8.2.dev1/src/helper/repack.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-8.1.dev9/PKG-INFO` & `pyarmor-8.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.1.dev9
+Version: 8.2.dev1
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.1.dev9/README.md` & `pyarmor-8.2.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 
 - Python 2 and Python 3[^1]
 - Windows
 - Various Linux distributions, including embedded systems and Raspberry Pi
 - Apple Intel and Apple Silicon
 - Supported architectures: x86_64, aarch64, armv7, etc.[^2]
 
+For more information, check out the [Pyarmor Environments][encironments].
+
 [^1]: Some features may be exclusive to Python 3.
 [^2]: Some features may be exclusive to specific architectures.
 
+[encironments]: https://pyarmor.readthedocs.io/en/stable/reference/environments.html
+
 ## Quick start
 
 1. **Install Pyarmor**:
 ```shell
 pip install pyarmor
 ```
```

## Comparing `pyarmor-8.1.dev9/setup.py` & `pyarmor-8.2.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     package_dir={'pyarmor': 'src'},
     package_data={
         'pyarmor': pyarmor_data_files + platform_data_files,
         'pyarmor.cli': ['default.cfg', 'public_capsule.zip'],
     },
 
     install_requires=[
-        'pyarmor.cli.core~=2.1.dev9'
+        'pyarmor.cli.core~=3.2.dev1'
     ],
 
     entry_points={
         'console_scripts': [
             'pyarmor=pyarmor.pyarmor:main_entry_8',
             'pyarmor-7=pyarmor.pyarmor:main_entry',
             'pyarmor-8=pyarmor.cli.__main__:main',
```

## Comparing `pyarmor-8.1.dev9/pyarmor.egg-info/PKG-INFO` & `pyarmor-8.2.dev1/pyarmor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor
-Version: 8.1.dev9
+Version: 8.2.dev1
 Summary: A tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor-8.1.dev9/pyarmor.egg-info/SOURCES.txt` & `pyarmor-8.2.dev1/pyarmor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 src/sppmode.py
 src/utils.py
 src/cli/__init__.py
 src/cli/__main__.py
 src/cli/config.py
 src/cli/context.py
 src/cli/default.cfg
-src/cli/errors.py
 src/cli/generate.py
 src/cli/mixer.py
+src/cli/plugin.py
 src/cli/public_capsule.zip
 src/cli/register.py
 src/cli/repack.py
 src/cli/resource.py
 src/cli/shell.py
 src/examples/README-ZH.md
 src/examples/README.md
```

## Comparing `pyarmor-8.1.dev9/src/config.py` & `pyarmor-8.2.dev1/src/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sys import platform
 
-version = '8.1.dev9'
+version = '8.2.dev1'
 
 # The corresponding version of pytransform.so
 core_version = 'r52.6'
 
 version_info = '''
 PyArmor is a command line tool used to obfuscate python scripts, bind
 obfuscated scripts to fixed machine or expire obfuscated scripts.
```

## Comparing `pyarmor-8.1.dev9/src/benchmark.py` & `pyarmor-8.2.dev1/src/benchmark.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/register.py` & `pyarmor-8.2.dev1/src/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/pyarmor.py` & `pyarmor-8.2.dev1/src/pyarmor.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/protect_code.pt` & `pyarmor-8.2.dev1/src/protect_code.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/pytransform.py` & `pyarmor-8.2.dev1/src/pytransform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/sppmode.py` & `pyarmor-8.2.dev1/src/sppmode.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/reform.py` & `pyarmor-8.2.dev1/src/reform.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/packer.py` & `pyarmor-8.2.dev1/src/packer.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/cobuilder.py` & `pyarmor-8.2.dev1/src/cobuilder.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/utils.py` & `pyarmor-8.2.dev1/src/utils.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/build_meta.py` & `pyarmor-8.2.dev1/src/build_meta.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/README.rst` & `pyarmor-8.2.dev1/src/README.rst`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/protect_code2.pt` & `pyarmor-8.2.dev1/src/protect_code2.pt`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/public_capsule.zip` & `pyarmor-8.2.dev1/src/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/project.py` & `pyarmor-8.2.dev1/src/project.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/platforms/linux/x86/_pytransform.so` & `pyarmor-8.2.dev1/src/platforms/linux/x86/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/platforms/linux/x86_64/_pytransform.so` & `pyarmor-8.2.dev1/src/platforms/linux/x86_64/_pytransform.so`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/platforms/darwin/x86_64/_pytransform.dylib` & `pyarmor-8.2.dev1/src/platforms/darwin/x86_64/_pytransform.dylib`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/platforms/windows/x86/_pytransform.dll` & `pyarmor-8.2.dev1/src/platforms/windows/x86/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/platforms/windows/x86_64/_pytransform.dll` & `pyarmor-8.2.dev1/src/platforms/windows/x86_64/_pytransform.dll`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/plugins/README.md` & `pyarmor-8.2.dev1/src/plugins/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/plugins/check_ntp_time.py` & `pyarmor-8.2.dev1/src/plugins/check_ntp_time.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/cli/config.py` & `pyarmor-8.2.dev1/src/cli/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Thu Jan 12 10:27:05 CST 2023
 #
 import configparser
 import fnmatch
-import logging
 import os
 
-logger = logging.getLogger('Pyarmor')
+from . import logger, CliError
 
 
 def indent(lines, n=2):
     fmt = ' ' * 2 + '%s'
     return [fmt % x for x in lines]
 
 
 def str_opt(k, v, n=30):
+    v = '\n\t'.join(v.splitlines())
     return '  %s = %s%s' % (k, v[:n], '...' if len(v) > n else '')
 
 
 class Configer(object):
 
-    SECTIONS = 'pyarmor', 'logging', 'finder', 'builder', \
-        'pack', 'bcc', 'rft', 'mix.str', 'assert.call', 'assert.import'
+    SECTIONS = 'pyarmor', 'logging', 'finder', 'builder', 'runtime', \
+        'pack', 'bcc', 'mix.str', 'assert.call', 'assert.import'
 
     def __init__(self, ctx, encoding=None):
         self.ctx = ctx
         self._encoding = encoding
 
     def _read_config(self, filename):
         cfg = configparser.ConfigParser(empty_lines_in_values=False)
@@ -122,29 +122,47 @@
         if name:
             cfg = self._read_config(self.ctx.get_filename(local, name))
             if cfg.has_section(sect) and cfg.has_option(sect, opt):
                 plines.append(format_value(opt))
 
         return clines, glines, lines, plines
 
-    def _set_option(self, sect, opt, local=True, name=None):
+    def _set_option(self, sect, opt, value, local=True, name=None):
         ctx = self.ctx
         filename = ctx.get_filename(local=local, name=name)
 
         cfg = self._read_config(filename)
         if not cfg.has_section(sect):
             cfg.add_section(sect)
 
         # TBD: input multiple lines
-        optname, optvalue = opt.split('=', 2)
-        if optvalue and optvalue[0] in ("'", '"'):
+        optname, optvalue = opt, value
+        if optvalue and optvalue[:1] in ('+', '-', '=', '^'):
+            op = optvalue[:1]
+            optvalue = optvalue.strip(op)
+            if op == '=':
+                op = None
+        else:
+            op = None
+        if optvalue and optvalue[:1] in ("'", '"'):
             optvalue = optvalue.strip(optvalue[0])
 
         if not optvalue:
-            return self.clear(sect, optname, local, name)
+            if op is None:
+                self._clear(sect, optname, local, name)
+            return
+
+        old = cfg[sect].get(optname, '') if cfg.has_section(sect) else ''
+        if op == '+':
+            if (optvalue + ' ').find(old + ' ') == -1:
+                optvalue = ('%s %s' % (old, optvalue)).strip()
+        elif op == '-':
+            optvalue = (old + ' ').replace(optvalue + ' ', '').strip()
+        elif op == '^':
+            optvalue = '\n'.join((old.splitlines() + [optvalue]))
 
         logger.info('change option "%s" to new value "%s"', optname, optvalue)
         cfg.set(sect, optname, optvalue)
 
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, 'w') as f:
             cfg.write(f)
@@ -214,26 +232,62 @@
         for pat in options:
             for sect, opts in self._parse_opt(pat):
                 self._remove(sect, opts, local, name)
 
     def run(self, options=None, local=True, name=None):
         lines = []
 
-        if options:
-            for pat in options:
-                for sect, opts in self._parse_opt(pat):
+        if options and len(options) == 1 and options[0].find('=') == -1:
+            for sect, opts in self._parse_opt(options[0]):
+                title = 'Section: %s' % sect
+                lines.extend(['', '-' * 60, title])
+                self.infos = [], [], [], []
+
+                for opt in opts:
+                    self._list_value(sect, opt, local, name)
+
+                lines.extend(['', 'Current settings'])
+                lines.extend(self.infos[0])
+                lines.extend(['', 'Global settings'])
+                lines.extend(self.infos[1])
+                lines.extend(['', 'Local settings'])
+                lines.extend(self.infos[2])
+                if name:
+                    lines.extend(['', 'Private "%s" settings' % name])
+                    lines.extend(self.infos[3])
+
+        elif options:
+            pairs = []
+            prev, op = None, ''
+            for opt in options:
+                i = opt.find('=')
+                if i > 0:
+                    pairs.append([opt[:i], opt[i+1:]])
+                elif opt in ('+', '=', '-', '^'):
+                    op = opt
+                elif prev:
+                    pairs.append((prev, op + opt))
+                    prev, op = None, ''
+                else:
+                    prev = opt
+            if prev:
+                raise CliError('no value for option "%s"' % prev)
+
+            for pat, value in pairs:
+                sect_opts = self._parse_opt(pat)
+                if not sect_opts:
+                    logger.debug('new builder option "%s"', pat)
+                    sect_opts = [('builder', [pat])]
+                for sect, opts in sect_opts:
                     title = 'Section: %s' % sect
                     lines.extend(['', '-' * 60, title])
                     self.infos = [], [], [], []
 
                     for opt in opts:
-                        if opt.find('=') == -1:
-                            self._list_value(sect, opt, local, name)
-                        else:
-                            self._set_option(sect, opt, local, name)
+                        self._set_option(sect, opt, value, local, name)
 
                     lines.extend(['', 'Current settings'])
                     lines.extend(self.infos[0])
                     lines.extend(['', 'Global settings'])
                     lines.extend(self.infos[1])
                     lines.extend(['', 'Local settings'])
                     lines.extend(self.infos[2])
```

## Comparing `pyarmor-8.1.dev9/src/cli/generate.py` & `pyarmor-8.2.dev1/src/cli/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,24 +15,21 @@
 #
 #  @File: cli/generate.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: 2022-12-06
 #
-import logging
 import os
 import shutil
 
-from .errors import CliError
+from . import logger, CliError
 from .core import Pytransform3
 from .resource import FileResource, PathResource
 
-logger = logging.getLogger('Builder')
-
 
 class Finder(object):
 
     def __init__(self, ctx):
         self.ctx = ctx
 
     def prepare(self, input_paths):
@@ -85,20 +82,20 @@
     def generate_runtime_package(self, output):
         if self.ctx.runtime_key is None:
             self.ctx.runtime_key = self.generate_runtime_key()
         Pytransform3.generate_runtime_package(self.ctx, output)
 
     def _pack_script(self, bundle, output, entry=None, codesign=None):
         from .repack import repacker
-        build = os.path.join('.pyarmor', 'build')
-        repacker(bundle, output, build, entry=entry, codesign=codesign)
-        shutil.rmtree(build)
+        buildpath = os.path.join('.pyarmor', 'pack')
+        repacker(bundle, output, buildpath, entry=entry, codesign=codesign)
+        shutil.rmtree(buildpath)
 
     def _obfuscate_scripts(self):
-        rev = self.ctx.version_info(verbose=2)
+        rev = self.ctx.version_info()
         template = self.ctx.bootstrap_template
         relative = self.ctx.import_prefix
         pkgname = self.ctx.runtime_package + self.ctx.runtime_suffix
         bootpath = self.ctx.cfg.get('builder', 'bootstrap_file')
 
         namelist = []
         for res in self.ctx.resources:
```

## Comparing `pyarmor-8.1.dev9/src/cli/shell.py` & `pyarmor-8.2.dev1/src/cli/shell.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/cli/resource.py` & `pyarmor-8.2.dev1/src/cli/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,30 +171,31 @@
         recursive = options.get('recursive', False)
         includes = options.get('includes', '').split()
         excludes = options.get('excludes', '').split()
         patterns = options.get('data_files', '').split()
 
         def in_filter(path, name):
             fullpath = os.path.join(path, name)
+            ext = os.path.splitext(name)[1]
             return not ex_filter(path, name) and (
-                os.path.splitext(name)[1] in pyexts
+                (ext and ext in pyexts)
                 or any([fnmatch(fullpath, x) for x in includes]))
 
         def ex_filter(path, name):
             fullpath = os.path.join(path, name)
             return excludes and any([fnmatch(fullpath, x) for x in excludes])
 
         def is_res(path, name):
             s = os.path.join(path, name)
             return any([fnmatch(s, x) for x in patterns])
 
         for path, dirnames, filenames in os.walk(self.fullpath):
             self.resfiles = [x for x in [
-                Resource(name, parent=self) if is_res(path, name)
-                else FileResource(name, parent=self) if in_filter(path, name)
+                FileResource(name, parent=self) if in_filter(path, name)
+                else Resource(name, parent=self) if is_res(path, name)
                 else None for name in filenames
             ] if x]
             self.respaths = [PathResource(name, parent=self)
                              for name in dirnames
                              if not ex_filter(path, name)]
             break
```

## Comparing `pyarmor-8.1.dev9/src/cli/__init__.py` & `pyarmor-8.2.dev1/src/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import logging
 
 __VERSION__ = '8.1'
 
+logger = logging.getLogger('cli')
+
+
+class CliError(Exception):
+    pass
+
 
 def resoptions(meth):
 
     def process(self, res, *args, **kwargs):
         self._options = self.ctx.get_res_options(res.fullname, self._Catalog)
         return meth(self, res, *args, **kwargs)
 
@@ -14,33 +20,37 @@
 
 class Component(object):
 
     trace_loggers = {
         'StrProtector': 'trace.mix.str',
         'CallProtector': 'trace.assert.call',
         'ImportProtector': 'trace.assert.import',
+        'CodeProtector': 'trace.co',
         'CoPatcher': 'trace.co',
         'BccPatcher': 'trace.bcc',
     }
 
     def __init__(self, ctx):
         self.ctx = ctx
         self._options = {}
 
         clsname = self.__class__.__name__
         self.logger = logging.getLogger(self.trace_loggers[clsname])
 
     def __getattr__(self, opt):
         if opt.startswith('o_'):
-            return self._options.get(opt[2:])
+            return self._options.get(opt[2:], '')
         elif opt.startswith('oi_'):
             return int(self._options.get(opt[3:]))
         elif opt.startswith('ob_'):
             v = self._options.get(opt[3:], '')
             if isinstance(v, str):
+                if v.isdigit():
+                    return bool(int(v))
                 return v.lower() in ('1', 'true', 'on', 'yes')
+
             return v
         return AttributeError(opt)
 
     def trace(self, res, node, value):
         lineno = getattr(node, 'lineno', -1)
         self.logger.info('%s:%s:%s', res.fullname, lineno, value)
```

## Comparing `pyarmor-8.1.dev9/src/cli/context.py` & `pyarmor-8.2.dev1/src/cli/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 runtime_package_template2 = '''# Pyarmor $rev, $timestamp
 for suffix in '', '_a1', '_a2', '_a3':
     try:
         __pyarmor__ = __import__('pyarmor_runtime' + suffix,
                                  globals(), locals(),
                                  ('__pyarmor__',),
-                                 0)
+                                 0).__pyarmor__
         break
     except ModuleNotFoundError:
         pass
 else:
     raise ModuleNotFoundError('no pyarmor_runtime extension found')
 '''
 
@@ -126,18 +126,20 @@
         self.module_builtins = set()
 
         self.obfuscated_modules = set()
         self.extra_libs = {}
 
         self.rft_auto_excludes = set(['super'])
         self.rft_export_names = set()
+        self.rft_transform_op = '?'
 
         self.runtime_key = None
 
         self.cmd_options = {}
+        self.plugins = []
 
     def _read_config(self, filelist, encoding=None):
         cfg = configparser.ConfigParser(
             empty_lines_in_values=False,
             interpolation=configparser.ExtendedInterpolation(),
         )
         cfg.read(filelist, encoding=encoding)
@@ -158,14 +160,18 @@
             f.write(data)
 
     def clear_token(self):
         if os.path.exists(self.license_token):
             with open(self.license_token, 'wb') as f:
                 f.close()
 
+    def group_device_file(self, devid):
+        filename = 'pyarmor-group-device.%s' % devid
+        return os.path.join(self.local_path, 'group', filename)
+
     def read_license(self):
         if os.path.exists(self.license_file):
             with open(self.license_file, 'rb') as f:
                 return f.read()
 
     def push(self, options):
         finder = {}
@@ -220,15 +226,15 @@
         verinfo = ['%s (%s)' % (rev, lictype)]
 
         if verbose > 1:
             verinfo.append(licinfo['licno'][-6:])
 
         if verbose > 2:
             pname = licinfo['product']
-            verinfo.append('non-profits' if pname in ('', 'TBD') else pname)
+            verinfo.append(pname)
 
         if verbose > 3:
             regname = licinfo['regname']
             if regname:
                 verinfo.append(regname)
 
         return ', '.join(verinfo)
@@ -312,17 +318,14 @@
             self.cfg['logging'].get('debug_logfile', 'pyarmor.debug.log'))
 
     @property
     def trace_logfile(self):
         return self._check_logpath(
             self.cfg['logging'].get('trace_logfile', 'pyarmor.trace.log'))
 
-    def trace_rftfile(self, name):
-        return self._check_logpath(os.path.join(self.local_path, 'rft', name))
-
     def _optb(self, section, name):
         return self.cfg.getboolean(section, name, vars=self.cmd_options)
 
     def _opts(self, section, name):
         return self.cfg.get(section, name, vars=self.cmd_options)
 
     def _opti(self, section, name):
@@ -500,26 +503,79 @@
         return self._opti('runtime', 'timer')
 
     @property
     def runtime_simple_extension_name(self):
         return self._optb('runtime', 'simple_extension_name')
 
     @property
-    def runtime_hooks(self):
-        value = self._rt_opt('hooks')
-        if value:
-            from ast import literal_eval
-            name, encoding = (value + ':utf-8').split(':')[:2]
-            for x in self.local_path, self.global_path:
-                filename = os.path.join(x, name)
-                if os.path.exists(filename):
-                    with open(filename, encoding=encoding) as f:
-                        return literal_eval(f.read())
+    def runtime_user_data(self):
+        data = b''
+        filename = self.cmd_options.get('user_data')
+        if filename:
+            if filename[0] == '@':
+                with open(filename[1:], 'rb') as f:
+                    data = f.read()
+            else:
+                data = filename.encode()
+
+        hook = b''
+        filename = os.path.join(self.local_path, 'hooks', 'pyarmor_runtime.py')
+        if os.path.exists(filename):
+            with open(filename, 'rb') as f:
+                hook = f.read()
+
+        return hook, data
 
     @property
     def runtime_messages(self):
         value = self.cfg['runtime'].get('messages', '')
         if value:
             name, encoding = (value + ':utf-8').split(':')[:2]
             cfg = self._named_config(name, encoding=encoding)
             if cfg.has_section('runtime.message'):
                 return cfg
+
+    #
+    # RFT settings
+    #
+
+    def rft_output_script(self, name):
+        return self._check_logpath(os.path.join(self.local_path, 'rft', name))
+
+    def rft_set_exclude_table(self, encoding=None):
+        filename = os.path.join(self.local_path, 'rft_exclude_table')
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+        with open(filename, 'w', encoding=encoding) as f:
+            f.write(' '.join(self.rft_auto_excludes))
+
+    def rft_get_exclude_table(self, encoding=None):
+        filename = os.path.join(self.local_path, 'rft_exclude_table')
+        if os.path.exists(filename):
+            with open(filename, encoding=encoding) as f:
+                return f.read().split()
+        return []
+
+    #
+    # BCC settings
+    #
+
+    @property
+    def bcc_build_path(self):
+        path = os.path.join(self.local_path, 'bcc')
+        os.makedirs(path, exist_ok=True)
+        return path
+
+    #
+    # Plugin and hook
+    #
+    def runtime_hook(self, modname):
+        for path in self.local_path, self.global_path:
+            filename = os.path.join(path, 'hooks', modname + '.py')
+            if os.path.exists(filename):
+                encoding = self.cfg['builder'].get('encoding', 'utf-8')
+                with open(filename, encoding=encoding) as f:
+                    return f.read()
+
+    def runtime_plugin(self, source, target, platforms):
+        for plugin in self.plugins:
+            if hasattr(plugin, 'post_runtime'):
+                plugin.post_runtime(self, source, target, platforms)
```

## Comparing `pyarmor-8.1.dev9/src/cli/mixer.py` & `pyarmor-8.2.dev1/src/cli/mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 #  @File: cli/mixer.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: 2022-12-06
 #
 import ast
-import logging
 
 from random import randint
 
-logger = logging.getLogger('Mixer')
-
 
 class StrNodeTransformer(ast.NodeTransformer):
 
     def _reform_str(self, s):
         encoding = getattr(self, 'encoding')
         value = bytearray(s.encode(encoding) if encoding else s.encode())
         key = [randint(0, 255)] * len(value)
```

## Comparing `pyarmor-8.1.dev9/src/cli/public_capsule.zip` & `pyarmor-8.2.dev1/src/cli/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/cli/default.cfg` & `pyarmor-8.2.dev1/src/cli/default.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [pyarmor]
 
 ;; Pyarmor version
 major = 8
-minor = 1
+minor = 2
 patch = 0
 
 ;; Core version
-core = 2.1
-runtime = 2.1
+cli.core = 3.2
+cli.runtime = 3.2
 
 ;; Default timeout when send request to remote server for
 ;;     check Pyarmor license
 ;;     register Pyarmor license
 timeout = 6
 
 regurl = https://api.dashingsoft.com/product/key/enter/%s/?
@@ -35,20 +35,14 @@
 data_files = 0
 
 ;;
 ;; How to find dependent packages
 ;;
 findall = 0
 
-;; Extra paths to find dependent package
-; pypaths =
-
-;; List module names couldn't be found automically
-; hidden_imports =
-
 [builder]
 ;;
 ;; Part 1: only global/local settings, not in module level
 ;;
 
 ;; File encoding to read scripts
 encoding = utf-8
@@ -83,19 +77,38 @@
 ;; How many loops for jit iv
 jit_iv_threshold = 100
 
 ;; Now "argument" is not available
 rft_enables = builtin import function class method global local
 
 ;; Exclude unknown attrs automically
+;    0     disable auto exclude, use auto include
+;    1     auto exclude and load .pyarmor/rft/exclude_table
+;    2     auto exclude but not load exclude_table
 rft_auto_exclude = 1
 
+;; Export all the names in module attribute __all__
+rft_auto_export = 1
+
+;; Enable dev mode for rft
+rft_dev_mode = 0
+
 ;; Export module and classes
 ; rft_export_names = pkg.mod pkg.mod.cls pkg.mod.attr
 
+;; Extra paths to find dependent package
+; pypaths =
+
+;; List module names couldn't be found automically
+; hidden_imports =
+
+;; If it's enabled, disable some features to make scripts work with nuitka
+;; convenient settings for nuitka, but now it's TBD
+; support_nuitka = 0
+
 ;;
 ;; Part 2: global/local/module level options
 ;;
 
 ;; The argument optimize specifies the optimization level of the
 ;; compiler; the default value of -1 selects the optimization level of
 ;; the interpreter as given by -O options. Explicit levels are 0 (no
@@ -118,14 +131,15 @@
 assert_import = 0
 
 ;; mix string constant
 mix_str = 0
 
 mix_coname = 0
 mix_localnames = 1
+;; Enable it may result in annotations error
 mix_argnames = 0
 
 obf_module = 1
 obf_code = 1
 wrap_mode = 1
 
 restrict_module = 1
@@ -157,15 +171,15 @@
 
 ;; Whether encrypt name in statement import
 rft_mix_import_name = 0
 
 [runtime]
 
 ;; Generate extension for all Python3.7+
-universal = false
+universal = 0
 
 ;; The file ext only keep .so/.pyd, for example
 ;;     pyarmor_runtime.cpython-37m-darwin.so
 ;;     if simple_extension_name == 1 then
 ;;     pyarmor_runtime.so
 simple_extension_name = 1
 
@@ -223,30 +237,32 @@
 ;; Target platforms
 ; platforms =
 
 ;; If there are customized runtime messages
 messages = messages.cfg:utf-8
 
 [assert.call]
-enables = all
+;; and: function is in obfuscated script and match ruler
+;;  or: function is in obfuscated script or match ruler
+auto_mode = and
 
 ; includes =
 ; excludes =
 
 [assert.import]
-enables = all
+;; and: module is obfuscated and match ruler
+;;  or: module is obfuscated or match ruler
+auto_mode = and
 
 ; includes =
 ; excludes =
 
 [mix.str]
-enables = all
-
 ;; do not mix short string len(s) < this value
-threshold = 4
+threshold = 8
 
 ; includes =
 ; excludes =
 
 [pack]
 ;; Strip output path to match archive info
 strip = 0
@@ -261,34 +277,16 @@
 ;; How to do when the obfuscated module has no matched .pyc in bundle
 ;;    error, issue a error and exit
 ;;    warning, issue a warning and continue
 ;;    ignore, do nothing
 ;;    append, append it to archive
 no_matched_pyc = error
 
-[windows.x86_64.bcc]
-cc = clang.exe
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
-
-[linux.x86_64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
-
-[linux.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib
-linker_script = ${bcc:linker_script}
-
-[darwin.x86_64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
-
-[darwin.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem -T${bcc:tempdir}/darwin.aarch64.ldscript
-linker_script = ${bcc:linker_script}
-
 [bcc]
-unsupported_functions = exec eval super locals
+unsupported_functions = exec eval super locals __assert_armored__
 unsupported_nodes = AsyncFunctionDef AsyncFor AsyncWith Await Yield YieldFrom GeneratorExp NamedExpr MatchValue MatchSingleton MatchSequence MatchMapping MatchClass MatchStar MatchAs MatchOr
 
 ;; Exclude co_names
 ; excludes =
 
 ;; Use opcode CALL_FUNCTION_EX to patch call
 ;; Global option, all scripts must be same
@@ -305,29 +303,22 @@
 
 ;; Use op_mkfunc2 to build unsupported functions
 enable_pure_function = 1
 
 ;; Convert comprehensions to bcc code
 enable_comprehension = 1
 
-tempdir = .pyarmor/bcc
-linker_script = /* pyarmor bcc mode link script */
-    SECTIONS {
-       . = 0x1000;
-       PROVIDE (_scode = .);
-       .text           : { *(.text) }
-       .data           : { *(.data) }
-       .rodata         : { *(.rodata) }
-       .got            : { *(.got) }
-       .got.plt        : { *(.got.plt) }
-       .imptbl         : { *(.imptbl) }
-       .explt          : { *(.explt) }
-       PROVIDE (_ecode = .);
-       .note.gnu.build-id      : { *(.note.gnu.build-id) }
-       .note.gnu.property      : { *(.note.gnu.property) }
-       .gnu.hash               : { *(.gnu.hash) }
-       .dynsym                 : { *(.dynsym) }
-       .dynstr                 : { *(.dynstr) }
-       .rela.dyn               : { *(.rela.dyn) }
-       .dynamic                : { *(.dynamic) }
-       .comment                : { *(.comment) }
-    }
+[windows.x86_64.bcc]
+cc = clang.exe
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
+
+[linux.x86_64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
+
+[linux.aarch64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+
+[darwin.x86_64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
+
+[darwin.aarch64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
```

## Comparing `pyarmor-8.1.dev9/src/cli/__main__.py` & `pyarmor-8.2.dev1/src/cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,44 +20,49 @@
 #  @Create Date: Thu Jan 12 10:27:05 CST 2023
 #
 import argparse
 import logging
 import os
 import sys
 
-from .errors import CliError
+from . import logger, CliError
 from .context import Context
 from .register import Register, WebRegister
 from .config import Configer
 from .shell import PyarmorShell
-
-logger = logging.getLogger('Pyarmor')
+from .plugin import Plugin
 
 
 def _cmd_gen_key(builder, options):
     n = len(options['inputs'])
     if n > 1:
-        raise CliError('too many args %s' % options['inputs'][1:])
+        logger.error('please check online documentation to learn')
+        logger.error('how to use command "pyarmor gen key"')
+        raise CliError('invalid arguments: %s' % options['inputs'][1:])
     keyname = builder.ctx.outer_keyname
 
     logger.info('start to generate outer runtime key "%s"', keyname)
     data = builder.generate_runtime_key(outer=True)
     output = options.get('output', 'dist')
     os.makedirs(output, exist_ok=True)
 
     target = os.path.join(output, keyname)
     logger.info('write %s', target)
     with open(target, 'wb') as f:
         f.write(data)
+
+    Plugin.post_key(builder.ctx, target)
     logger.info('generate outer runtime key OK')
 
 
 def _cmd_gen_runtime(builder, options):
     if len(options['inputs']) > 1:
-        raise CliError('too many args %s' % options['inputs'][1:])
+        logger.error('please check online documentation to learn')
+        logger.error('how to use command "pyarmor gen runtime"')
+        raise CliError('invalid arguments: %s' % options['inputs'][1:])
 
     output = options.get('output', 'dist')
 
     logger.info('start to generate runtime package')
     builder.generate_runtime(output)
 
     keyname = os.path.join(output, builder.ctx.runtime_keyfile)
@@ -74,14 +79,25 @@
               'obf_module', 'obf_code', 'assert_import', 'assert_call',
               'mix_str', 'import_prefix', 'restrict_module',
               'platforms', 'outer', 'period', 'expired', 'devices'):
         v = getattr(args, x)
         if v is not None:
             options[x] = v
 
+    if options.get('platforms'):
+        platforms = []
+        for item in options['platforms']:
+            platforms.extend([x.strip() for x in item.split(',')])
+        options['platforms'] = platforms
+    elif ctx.runtime_platforms:
+        options['platforms'] = ctx.runtime_platforms.split()
+        logger.info('get runtime platforms from configuration file')
+    if options.get('platforms'):
+        logger.info('use runtime platforms: %s', options['platforms'])
+
     if args.inputs:
         options['inputs'] = [os.path.normpath(x) for x in args.inputs]
 
     if args.use_runtime:
         options['no_runtime'] = True
         options['use_runtime'] = args.use_runtime
 
@@ -92,44 +108,58 @@
 
     if options.get('restrict_module', 0) > 1:
         options['mix_coname'] = 1
 
     if args.enables:
         for x in args.enables:
             options['enable_' + x] = True
+    if options.get('enable_themida'):
+        raise NotImplementedError('--enable_themida is still not implemented')
 
     if args.prefix:
         options['import_prefix'] = args.prefix
 
     if args.no_wrap:
         options['wrap_mode'] = 0
 
     if args.includes:
         options['includes'] = ' '.join(args.includes)
     if args.excludes:
         options['excludes'] = ' '.join(args.excludes)
 
+    if args.bind_data:
+        options['user_data'] = args.bind_data
+
     return options
 
 
 def check_cross_platform(ctx, platforms):
+    rtver = ctx.cfg.get('pyarmor', 'cli.runtime')
+    cmd = 'pip install pyarmor.cli.runtime~=%s.0' % rtver
     try:
         from pyarmor.cli import runtime
-    except ModuleNotFoundError:
-        raise CliError('cross platform need pyarmor.cli.runtime, please '
-                       'run "pip install pyarmor.cli.runtime==2.1.dev9" first')
+    except (ImportError, ModuleNotFoundError):
+        logger.error('cross platform need package "pyarmor.cli.runtime"')
+        logger.error('please run "%s" to fix it', cmd)
+        raise CliError('no package "pyarmor.cli.runtime" found')
+
+    if runtime.__VERSION__ != rtver:
+        logger.error('please run "%s" to fix it', cmd)
+        raise CliError('unexpected "pyarmor.cli.runtime" version')
 
     platnames = []
     for path in runtime.__path__:
+        logger.debug('search runtime platforms at: %s', path)
         platnames.extend(os.listdir(os.path.join(path, 'libs')))
 
     map_platform = runtime.map_platform
     unknown = set([map_platform(x) for x in platforms]) - set(platnames)
 
     if unknown:
+        logger.error('please check documentation "References/Environments"')
         raise CliError('unsupported platforms "%s"' % ', '.join(unknown))
 
 
 def check_gen_context(ctx, args):
     enable_bcc = args.enable_bcc or (args.enables and 'bcc' in args.enables)
     if ctx.runtime_platforms:
         if ctx.enable_themida and not ctx.pyarmor_platform.startswith('win'):
@@ -140,47 +170,53 @@
 
     if enable_bcc:
         plat, arch = ctx.pyarmor_platform.split('.')
         if arch not in ('x86_64', 'aarch64'):
             raise CliError('bcc mode still not support arch "%s"' % arch)
 
     if ctx.cmd_options['no_runtime'] and not ctx.runtime_outer:
-        raise CliError('--no_runtime need pass outer key by --outer')
+        raise CliError('--no_runtime must be used with --outer')
 
     if ctx.use_runtime and not ctx.runtime_outer:
         if os.path.exists(ctx.use_runtime):
             keyname = os.path.join(ctx.use_runtime, ctx.runtime_keyfile)
             if not os.path.exists(keyname):
                 raise CliError('no runtime key in "%s"', ctx.use_runtime)
 
     if ctx.runtime_outer and any(
             [ctx.runtime_devices, ctx.runtime_period, ctx.runtime_expired]):
         raise CliError('--outer conflicts with any -e, --period, -b')
 
-    if args.pack and (args.no_runtime or ctx.import_prefix):
-        raise CliError('--pack conficts with --no-runtime, --use-runtime, '
-                       '-i, --prefix')
+    if args.pack:
+        if not os.path.isfile(args.pack):
+            raise CliError('--pack must be an executable file')
+        if args.no_runtime:
+            raise CliError('--pack conficts with --no-runtime, --use-runtime')
+        if ctx.import_prefix:
+            raise CliError('--pack conficts with -i, --prefix')
 
 
 def cmd_gen(ctx, args):
     from .generate import Builder
 
     options = format_gen_args(ctx, args)
     logger.debug('command options: %s', options)
     ctx.push(options)
     check_gen_context(ctx, args)
 
     builder = Builder(ctx)
 
+    Plugin.install(ctx)
     if args.inputs[0].lower() in ('key', 'k'):
         _cmd_gen_key(builder, options)
     elif args.inputs[0].lower() in ('runtime', 'run', 'r'):
         _cmd_gen_runtime(builder, options)
     else:
         builder.process(options, pack=args.pack)
+        Plugin.post_build(ctx, pack=args.pack)
 
 
 def cmd_cfg(ctx, args):
     scope = 'global' if args.scope else 'local'
     cfg = Configer(ctx, encoding=args.encoding)
     name = 'reset' if args.reset else 'run'
     getattr(cfg, name)(args.options, scope == 'local', args.name)
@@ -188,68 +224,84 @@
 
 def cmd_reg(ctx, args):
     if args.buy:
         from webbrowser import open_new_tab
         open_new_tab(ctx.cfg['pyarmor']['buyurl'])
         return
 
+    if args.device and not args.regfile:
+        reg = Register(ctx)
+        reg.generate_group_device(args.device)
+        logger.info('device file has been generated successfully')
+        return
+
     regfile = args.regfile
     if not regfile:
         reg = Register(ctx)
         logger.info('Current license information:\n\n%s', reg)
         return
 
+    if regfile.endswith('.txt') and not args.product:
+        logger.error('please use -p to specify product name for this license')
+        raise CliError('missing product name')
+
+    if regfile.endswith('.zip') and args.product:
+        logger.error('please do not use -p for non initial registration')
+        raise CliError('unwanted product name')
+
     upgrade = args.upgrade
     if upgrade:
         if not regfile.endswith('.txt'):
             raise CliError('upgrade need text file "pyarmor-keycode-xxxx.txt"')
         url = 'https://github.com/dashingsoft/pyarmor/issues/980'
         msg = ("",
-               "Pyarmor 8.0 changes EULA and uses new commands",
+               "Pyarmor 8 changes EULA and uses new commands",
                "It's different from previous Pyarmor totally",
                "Please read this import notes first:",
                url,
-               "Do not upgrade to Pyarmor 8 if you don't known what's changed",
+               "Do not upgrade to Pyarmor 8 if don't know what are changed",
                "", "")
         prompt = 'I have known the changes of Pyarmor 8? (yes/no/help) '
         choice = input('\n'.join(msg) + prompt).lower()[:1]
         if choice == 'h':
             import webbrowser
             webbrowser.open(url)
         if not choice == 'y':
             return
 
-    if regfile.endswith('.zip'):
+    if args.device:
+        if not regfile.endswith('.zip'):
+            logger.error('invalid registeration file "%s"', regfile)
+            raise CliError('please use ".zip" file to register group device')
+        regsvr = WebRegister(ctx)
+        regsvr.register_group_device(regfile, args.device)
+        logger.info('The device regfile has been generated successfully')
+
+    elif regfile.endswith('.zip'):
         reg = Register(ctx)
         logger.info('register "%s"', regfile)
         reg.register_regfile(regfile)
         logger.info('This license registration information:\n\n%s', str(reg))
 
     else:
         regsvr = WebRegister(ctx)
-        if (not args.confirm) or upgrade:
-            info, msg = regsvr.prepare(regfile, args.product, upgrade=upgrade)
-            prompt = 'Are you sure to continue? (yes/no) '
-            if input(msg + prompt) != 'yes':
-                return
-            if info['upgrade'] and info['product'] in ('TBD', 'non-profits'):
-                msg = '\n'.join([
-                    '',
-                    'The product name is set to "%s", once upgrade, '
-                    'it can not be changed.' % info['product'],
-                    ''
-                ])
-                if input(msg + prompt) != 'yes':
-                    return
-            # Free upgrade to Pyarmor Basic
-            if upgrade and not info['upgrade']:
-                return regsvr.register(regfile, args.product, upgrade=True)
-
-        meth = 'upgrade_to_pro' if upgrade else 'register'
-        getattr(regsvr, meth)(regfile, args.product)
+        info, msg = regsvr.prepare(regfile, args.product, upgrade=upgrade)
+        prompt = 'Are you sure to continue? (yes/no) '
+        if input(msg + prompt) not in ('y', 'yes'):
+            logger.info('abort registration')
+            return
+        # Free upgrade to Pyarmor Basic
+        if upgrade and not info['upgrade']:
+            return regsvr.register(regfile, args.product, upgrade=True)
+
+        if upgrade:
+            regsvr.upgrade_to_pro(regfile, args.product)
+        else:
+            group = info['lictype'] == 'GROUP'
+            regsvr.register(regfile, args.product, group=group)
 
 
 def main_parser():
     parser = argparse.ArgumentParser(
         prog='pyarmor',
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
@@ -287,15 +339,19 @@
     '''generate obfuscated scripts and all required runtime files
     pyarmor gen <options> <scripts>
 
 generate runtime key only
     pyarmor gen key <options>
 
 generate runtime package only
-    pyarmor gen runtime <options>'''
+    pyarmor gen runtime <options>
+
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-gen
+'''
     cparser = subparsers.add_parser(
         'gen',
         aliases=['generate', 'g'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=gen_parser.__doc__,
         help='generate obfuscated scripts and required runtime files'
     )
@@ -422,14 +478,18 @@
         help='check runtime key periodically'
     )
     group.add_argument(
         '-b', '--bind-device', dest='devices', metavar='DEV', action='append',
         help='bind obfuscated scripts to device'
     )
     group.add_argument(
+        '--bind-data', metavar='FILE',
+        help=argparse.SUPPRESS
+    )
+    group.add_argument(
         '--bind-interp', metavar='INTERP',
         help=argparse.SUPPRESS
     )
     group.add_argument(
         '--hook', metavar='HOOK',
         help=argparse.SUPPRESS
     )
@@ -447,14 +507,17 @@
     pyarmor cfg
 
 show option `OPT` value:
     pyarmor cfg OPT
 
 change option value:
     pyarmor cfg OPT=VALUE
+
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-cfg
     '''
 
     cparser = subparsers.add_parser(
         'cfg',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=cfg_parser.__doc__,
         help='show and config Pyarmor environments',
@@ -488,22 +551,19 @@
     cparser.set_defaults(func=cmd_cfg)
 
 
 def reg_parser(subparsers):
     '''register Pyarmor or upgrade Pyarmor license
 
 At the first time to register Pyarmor, `-p` (product name) should be
-set. If not set, this Pyarmor license is bind to "non-profits", and
-could not be used for commercial product.
-
-Once register successfully, product name can't be changed.
-
-There is only one exception, if product name is set to "TBD" at the
-first time, it can be changed once later.
+set. For non-commercial use, set it to "non-profits". The product name
+can't be changed after initial registration.
 
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-reg
     '''
     cparser = subparsers.add_parser(
         'reg',
         aliases=['register', 'r'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=reg_parser.__doc__,
         help='register Pyarmor or upgrade Pyarmor license'
@@ -511,27 +571,31 @@
 
     cparser.add_argument(
         '-r', '--regname', metavar='NAME',
         help=argparse.SUPPRESS
     )
     cparser.add_argument(
         '-p', '--product', metavar='NAME',
-        help='license to this product'
+        help='bind license to this product'
     )
     cparser.add_argument(
         '-u', '--upgrade', action='store_true',
-        help='upgrade Pyarmor license'
+        help='upgrade old Pyarmor license'
+    )
+    cparser.add_argument(
+        '-g', '--device', metavar='ID', type=int, choices=range(1, 101),
+        help='device id (1-100) in group license'
     )
     cparser.add_argument(
         '--buy', action='store_true',
         help='open buy link in default web browser'
     )
     cparser.add_argument(
         '-y', '--confirm', action='store_true',
-        help='register Pyarmor without asking for confirmation'
+        help=argparse.SUPPRESS
     )
 
     cparser.add_argument(
         'regfile', nargs='?', metavar='FILE',
         help='pyarmor-regcode-xxx.txt or pyarmor-regfile-xxxx.zip'
     )
     cparser.set_defaults(func=cmd_reg)
@@ -556,19 +620,19 @@
         tracelog.addHandler(handler)
 
     if args.silent:
         logging.getLogger().setLevel(100)
 
 
 def log_exception(e):
-    logger.critical('unknown error, please check pyarmor.error.log')
+    logger.debug('unknown error, please check pyarmor.error.log')
     handler = logging.FileHandler('pyarmor.error.log', mode='w')
     fmt = '%(process)d %(processName)s %(asctime)s'
     handler.setFormatter(logging.Formatter(fmt))
-    log = logging.getLogger('Pyarmor.Error')
+    log = logging.getLogger('error')
     log.propagate = False
     log.addHandler(logging.NullHandler())
     log.addHandler(handler)
     log.exception(e)
 
 
 def print_version(ctx):
@@ -602,15 +666,15 @@
         parser.exit()
 
     if args.interactive:
         return PyarmorShell(ctx).cmdloop()
 
     logger.info('Python %d.%d.%d', *sys.version_info[:3])
     logger.info('Pyarmor %s', ctx.version_info())
-    logger.debug('Platform %s', ctx.pyarmor_platform)
+    logger.info('Platform %s', ctx.pyarmor_platform)
 
     logger.debug('native platform %s', ctx.native_platform)
     logger.debug('home path: %s', ctx.home_path)
 
     if hasattr(args, 'func'):
         args.func(ctx, args)
     else:
@@ -621,18 +685,17 @@
     logging.basicConfig(
         level=logging.INFO,
         format='%(levelname)-8s %(message)s',
     )
 
     try:
         main_entry(sys.argv[1:])
-    # # TBD: comment for debug
-    # except (CliError, RuntimeError) as e:
-    #     logger.error(e)
-    #     sys.exit(1)
+    except CliError as e:
+        logger.error(e)
+        sys.exit(1)
     except Exception as e:
         log_exception(e)
         logger.error(e)
         sys.exit(2)
 
 
 if __name__ == '__main__':
```

## Comparing `pyarmor-8.1.dev9/src/cli/repack.py` & `pyarmor-8.2.dev1/src/cli/repack.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from PyInstaller.loader.pyimod02_archive import PYZ_TYPE_PKG
 except ModuleNotFoundError:
     from PyInstaller.loader.pyimod01_archive import ZlibArchiveReader
     from PyInstaller.loader.pyimod01_archive import PYZ_TYPE_PKG
 from PyInstaller.compat import is_darwin, is_linux, is_win
 
 
-logger = logging.getLogger('Packer')
+logger = logging.getLogger('repack')
 
 
 class ZlibArchive(ZlibArchiveReader):
 
     def checkmagic(self):
         """ Overridable.
             Check to see if the file object self.lib actually has a file
```

## Comparing `pyarmor-8.1.dev9/src/examples/obfuscate-pkg.bat` & `pyarmor-8.2.dev1/src/examples/obfuscate-pkg.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/obfuscate-app.bat` & `pyarmor-8.2.dev1/src/examples/obfuscate-app.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/obfuscate-app.sh` & `pyarmor-8.2.dev1/src/examples/obfuscate-app.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/obfuscate-pkg.sh` & `pyarmor-8.2.dev1/src/examples/obfuscate-pkg.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/build-with-project.bat` & `pyarmor-8.2.dev1/src/examples/build-with-project.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/README.md` & `pyarmor-8.2.dev1/src/examples/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.sh` & `pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pack-obfuscated-scripts.bat` & `pyarmor-8.2.dev1/src/examples/pack-obfuscated-scripts.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/build-with-project.sh` & `pyarmor-8.2.dev1/src/examples/build-with-project.sh`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/build-for-freeze.bat` & `pyarmor-8.2.dev1/src/examples/build-for-freeze.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/README-ZH.md` & `pyarmor-8.2.dev1/src/examples/README-ZH.md`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/build-for-exe.bat` & `pyarmor-8.2.dev1/src/examples/build-for-exe.bat`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/helloworld/foo.py` & `pyarmor-8.2.dev1/src/examples/helloworld/foo.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/cx_Freeze/queens.py` & `pyarmor-8.2.dev1/src/examples/cx_Freeze/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/cx_Freeze/setup.py` & `pyarmor-8.2.dev1/src/examples/cx_Freeze/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/simple/queens.py` & `pyarmor-8.2.dev1/src/examples/simple/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Arithmetic.py` & `pyarmor-8.2.dev1/src/examples/pybench/Arithmetic.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/With.py` & `pyarmor-8.2.dev1/src/examples/pybench/With.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Lists.py` & `pyarmor-8.2.dev1/src/examples/pybench/Lists.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Tuples.py` & `pyarmor-8.2.dev1/src/examples/pybench/Tuples.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Instances.py` & `pyarmor-8.2.dev1/src/examples/pybench/Instances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/systimes.py` & `pyarmor-8.2.dev1/src/examples/pybench/systimes.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/clockres.py` & `pyarmor-8.2.dev1/src/examples/pybench/clockres.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Lookups.py` & `pyarmor-8.2.dev1/src/examples/pybench/Lookups.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/CommandLine.py` & `pyarmor-8.2.dev1/src/examples/pybench/CommandLine.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Numbers.py` & `pyarmor-8.2.dev1/src/examples/pybench/Numbers.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Imports.py` & `pyarmor-8.2.dev1/src/examples/pybench/Imports.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Setup.py` & `pyarmor-8.2.dev1/src/examples/pybench/Setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Exceptions.py` & `pyarmor-8.2.dev1/src/examples/pybench/Exceptions.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Dict.py` & `pyarmor-8.2.dev1/src/examples/pybench/Dict.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/pybench.py` & `pyarmor-8.2.dev1/src/examples/pybench/pybench.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/NewInstances.py` & `pyarmor-8.2.dev1/src/examples/pybench/NewInstances.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Calls.py` & `pyarmor-8.2.dev1/src/examples/pybench/Calls.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Strings.py` & `pyarmor-8.2.dev1/src/examples/pybench/Strings.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/pybench/Constructs.py` & `pyarmor-8.2.dev1/src/examples/pybench/Constructs.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/testmod/hello.py` & `pyarmor-8.2.dev1/src/examples/testmod/hello.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/testmod/queens.py` & `pyarmor-8.2.dev1/src/examples/testmod/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/py2exe/queens.py` & `pyarmor-8.2.dev1/src/examples/py2exe/queens.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/examples/py2exe/setup.py` & `pyarmor-8.2.dev1/src/examples/py2exe/setup.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/polyfills/argparse.py` & `pyarmor-8.2.dev1/src/polyfills/argparse.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/superuntime.py` & `pyarmor-8.2.dev1/src/helper/superuntime.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/merge.py` & `pyarmor-8.2.dev1/src/helper/merge.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/buildext.py` & `pyarmor-8.2.dev1/src/helper/buildext.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/get_platform_name.py` & `pyarmor-8.2.dev1/src/helper/get_platform_name.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/get_license_info.py` & `pyarmor-8.2.dev1/src/helper/get_license_info.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/get_bind_key.py` & `pyarmor-8.2.dev1/src/helper/get_bind_key.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/build_data_module.py` & `pyarmor-8.2.dev1/src/helper/build_data_module.py`

 * *Files identical despite different names*

## Comparing `pyarmor-8.1.dev9/src/helper/repack.py` & `pyarmor-8.2.dev1/src/helper/repack.py`

 * *Files identical despite different names*

