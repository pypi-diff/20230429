# Comparing `tmp/SpectroscopicBinarySystem-1.1.1.tar.gz` & `tmp/SpectroscopicBinarySystem-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.1.tar", last modified: Sat Apr 29 19:57:01 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.1.2.tar", last modified: Sat Apr 29 20:30:09 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.1.tar` & `SpectroscopicBinarySystem-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 19:57:01.648666 SpectroscopicBinarySystem-1.1.1/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3138 2023-04-29 19:57:01.649812 SpectroscopicBinarySystem-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2747 2023-04-29 19:27:34.000000 SpectroscopicBinarySystem-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 19:57:01.646374 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     3138 2023-04-29 19:57:01.000000 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-04-29 19:57:01.000000 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 19:57:01.000000 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-29 19:57:01.000000 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-29 19:57:01.000000 SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-29 19:57:01.650869 SpectroscopicBinarySystem-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 19:57:01.647379 SpectroscopicBinarySystem-1.1.1/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    29963 2023-04-29 19:56:17.000000 SpectroscopicBinarySystem-1.1.1/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 20:30:09.886562 SpectroscopicBinarySystem-1.1.2/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3143 2023-04-29 20:30:09.886562 SpectroscopicBinarySystem-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2752 2023-04-29 20:05:04.000000 SpectroscopicBinarySystem-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 20:30:09.882449 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     3143 2023-04-29 20:30:09.000000 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-04-29 20:30:09.000000 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 20:30:09.000000 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-29 20:30:09.000000 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-29 20:30:09.000000 SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-04-29 20:30:09.887568 SpectroscopicBinarySystem-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 20:30:09.884560 SpectroscopicBinarySystem-1.1.2/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    29983 2023-04-29 20:27:15.000000 SpectroscopicBinarySystem-1.1.2/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.1/LICENSE` & `SpectroscopicBinarySystem-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.1/PKG-INFO` & `SpectroscopicBinarySystem-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -78,11 +78,11 @@
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
     savefig=False
 )
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_2d_spectrum_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.1/README.md` & `SpectroscopicBinarySystem-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,11 +66,11 @@
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
     savefig=False
 )
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_2d_spectrum_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -78,11 +78,11 @@
     subtitle=f"{sbs.getObservationCount()} observations collected from april 2022 to april 2023",
     savefig=False
 )
 ```
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_2d_spectrum_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/hd123299_2d_spectrum_result.png)
 
 ![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.1.1/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.1.2/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.1/setup.cfg` & `SpectroscopicBinarySystem-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 310d 0a61  rsion = 1.1.1..a
+00000030: 7273 696f 6e20 3d20 312e 312e 320d 0a61  rsion = 1.1.2..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.1.1/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.1.2/spectroscopicbinarysystem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,16 +726,16 @@
                           doppler_rest=6562.82 * u.AA)
         spec2d = np.zeros((len(wv_to_kms), len(y_phase)))
 
         # resample each spectrum
         for s in self._sb_spectra:
             ss = copy.copy(s)
             # apply heliocentric/barycentric correction
-            ss.shift_spectrum_to(
-                radial_velocity=s.getRV()*u.km/u.s)
+            # ss.shift_spectrum_to(
+            #     radial_velocity=s.getRV()*u.km/u.s)
             fluxc_resample = LinearInterpolatedResampler()
             output_spectrum1D = fluxc_resample(ss, sc)
             phase = s.getPhase()
             indice = int(round(phase, 2) * len(y_phase))
             spec2d[:, indice] = output_spectrum1D.flux
 
         # prepare imshow
@@ -756,9 +756,9 @@
         ax.set_title("%s\n%s" % (t, subtitle), fontsize=9,
                      fontweight="0", color='black')
 
         plt.tight_layout(pad=3, w_pad=0, h_pad=1)
         plt.yticks(np.arange(0, 1.01, 0.1))
         if savefig:
             plt.savefig(
-                f'{self._spectra_path}/sbs_2d_spectrum_result.png', dpi=dpi)
+                f'{self._spectra_path}/{self._object_name}_2d_spectrum_result.png', dpi=dpi)
         plt.show()
```

