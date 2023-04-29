# Comparing `tmp/SpectroscopicBinarySystem-1.0.17.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.17.tar", last modified: Fri Apr 28 12:33:43 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.18.tar", last modified: Sat Apr 29 04:53:31 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.17.tar` & `SpectroscopicBinarySystem-1.0.18.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.513624 SpectroscopicBinarySystem-1.0.17/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.17/LICENSE
--rw-rw-rw-   0        0        0     2128 2023-04-28 12:33:43.513624 SpectroscopicBinarySystem-1.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     1736 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.509614 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     2128 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-28 12:33:43.000000 SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.17/pyproject.toml
--rw-rw-rw-   0        0        0      725 2023-04-28 12:33:43.516632 SpectroscopicBinarySystem-1.0.17/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 12:33:43.510616 SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    26258 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 04:53:31.951898 SpectroscopicBinarySystem-1.0.18/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.18/LICENSE
+-rw-rw-rw-   0        0        0     2128 2023-04-29 04:53:31.951898 SpectroscopicBinarySystem-1.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.18/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 04:53:31.933185 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     2128 2023-04-29 04:53:31.000000 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-04-29 04:53:31.000000 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 04:53:31.000000 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-29 04:53:31.000000 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-29 04:53:31.000000 SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.18/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-04-29 04:53:31.951898 SpectroscopicBinarySystem-1.0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 04:53:31.951898 SpectroscopicBinarySystem-1.0.18/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    26559 2023-04-29 04:51:40.000000 SpectroscopicBinarySystem-1.0.18/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.0.17/LICENSE` & `SpectroscopicBinarySystem-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.17/PKG-INFO` & `SpectroscopicBinarySystem-1.0.18/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.17
+Version: 1.0.18
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.0.17/README.md` & `SpectroscopicBinarySystem-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.17
+Version: 1.0.18
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.0.17/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.0.18/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.17/setup.cfg` & `SpectroscopicBinarySystem-1.0.18/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 3137 0d0a  rsion = 1.0.17..
+00000030: 7273 696f 6e20 3d20 312e 302e 3138 0d0a  rsion = 1.0.18..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.0.17/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.0.18/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         Compute the radial velocity from a line position and a radial velocity correction
         Reference line rest position in Angstroms can be customize in conf["LAMBDA_REF"]
         :return: None
         """
         c = const.c.to('km/s')
         self._rv = (c * ((self._center_of_line -
                     self._conf["LAMBDA_REF"]) / self._conf["LAMBDA_REF"])) + self._rv_corr
-        
+
     def getCenterOfLine(self):
         """
         Return the center of the line computed for the spectrum using a fit (non corrected from heliocentric/barycentric velocity)
         :return: Float
         """
         return self._center_of_line
 
@@ -291,29 +291,42 @@
                     if self._debug:
                         print(sbSpec1D)
         if self._debug:
             print(f'{len(self._sb_spectra)} processed spectra')
             plt.rcParams['font.size'] = '6'
             plt.rcParams['font.family'] = 'monospace'
             grid_size = math.ceil(len(self._sb_spectra)/6)
-            fig, axs = plt.subplots(6,grid_size, figsize=(13,7), sharex=True, sharey=True)
+            fig, axs = plt.subplots(6, grid_size, figsize=(
+                13, 7), sharex=True, sharey=True)
             for i, s in enumerate(self._sb_spectra):
                 ax = axs.flat[i]
                 extracted_profil, line_fitting = s.getDebugLineFitting()
-                ax.set_title(f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
+                ax.set_title(
+                    f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
                 ax.grid(True)
                 ax.tick_params(axis='both', which='major', labelsize=6)
                 ax.tick_params(axis='both', which='minor', labelsize=6)
-                ax.plot(extracted_profil.spectral_axis.to(u.AA), extracted_profil.flux, color="k")
-                ax.plot(extracted_profil.spectral_axis.to(u.AA), line_fitting, color="r")
-                ax.axvline(x=s.getCenterOfLine(), color='r', linestyle='-',lw=0.7)
+                ax.plot(extracted_profil.spectral_axis.to(
+                    u.AA), extracted_profil.flux, color="k")
+                ax.plot(extracted_profil.spectral_axis.to(
+                    u.AA), line_fitting, color="r")
+                ax.axvline(x=s.getCenterOfLine(),
+                           color='r', linestyle='-', lw=0.7)
             plt.tight_layout(pad=0.8, w_pad=2, h_pad=1)
             plt.savefig(f'{self._spectra_path}/sbs_debug_result.png', dpi=150)
             plt.show()
 
+    def getObservationCount(self):
+        """
+        Return the count of processed spectra
+        :return: count
+        :rtype: int
+        """
+        return len(self._sb_spectra)
+
     def __getPhase(self, jd0, period, jd):
         """
         Compute the phase of a given JD
         :param jd0: JD of the first observation
         :param period: period of the orbit
         :param jd: JD to compute the phase
         :return: phase
```

