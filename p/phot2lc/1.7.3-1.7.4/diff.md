# Comparing `tmp/phot2lc-1.7.3.tar.gz` & `tmp/phot2lc-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phot2lc-1.7.3.tar", last modified: Fri Feb 10 00:41:54 2023, max compression
+gzip compressed data, was "phot2lc-1.7.4.tar", last modified: Sat Apr 29 00:23:29 2023, max compression
```

## Comparing `phot2lc-1.7.3.tar` & `phot2lc-1.7.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-02-10 00:41:54.318916 phot2lc-1.7.3/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.3/LICENSE
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-02-10 00:41:54.318916 phot2lc-1.7.3/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.3/README.md
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-02-10 00:41:54.318916 phot2lc-1.7.3/setup.cfg
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1063 2023-02-10 00:40:57.000000 phot2lc-1.7.3/setup.py
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-02-10 00:41:54.318916 phot2lc-1.7.3/src/
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-02-10 00:41:54.318916 phot2lc-1.7.3/src/phot2lc/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.3/src/phot2lc/__init__.py
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      256 2023-02-08 00:12:29.000000 phot2lc-1.7.3/src/phot2lc/config.dat
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83535 2023-02-10 00:13:34.000000 phot2lc-1.7.3/src/phot2lc/phot2lc
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2020-06-25 13:35:54.000000 phot2lc-1.7.3/src/phot2lc/photconfig
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    16827 2023-02-10 00:38:26.000000 phot2lc-1.7.3/src/phot2lc/photfunc.py
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.3/src/phot2lc/quicklook
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.3/src/phot2lc/teledat.py
--rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.3/src/phot2lc/ucm_utils.py
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    20478 2023-02-09 06:58:27.000000 phot2lc-1.7.3/src/phot2lc/version_history.txt
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.3/src/phot2lc/weldlc
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-02-10 00:41:54.318916 phot2lc-1.7.3/src/phot2lc.egg-info/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-02-10 00:41:54.000000 phot2lc-1.7.3/src/phot2lc.egg-info/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      401 2023-02-10 00:41:54.000000 phot2lc-1.7.3/src/phot2lc.egg-info/SOURCES.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-02-10 00:41:54.000000 phot2lc-1.7.3/src/phot2lc.egg-info/dependency_links.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-02-10 00:41:54.000000 phot2lc-1.7.3/src/phot2lc.egg-info/top_level.txt
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:23:29.054431 phot2lc-1.7.4/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.4/LICENSE
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-04-29 00:23:29.050431 phot2lc-1.7.4/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.4/README.md
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-04-29 00:23:29.054431 phot2lc-1.7.4/setup.cfg
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-04-29 00:19:30.000000 phot2lc-1.7.4/setup.py
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:23:29.050431 phot2lc-1.7.4/src/
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:23:29.050431 phot2lc-1.7.4/src/phot2lc/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.4/src/phot2lc/__init__.py
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2333 2023-04-29 00:14:55.000000 phot2lc-1.7.4/src/phot2lc/addstar
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.4/src/phot2lc/config.dat
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83856 2023-04-29 00:22:15.000000 phot2lc-1.7.4/src/phot2lc/phot2lc
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      346 2023-02-22 04:17:40.000000 phot2lc-1.7.4/src/phot2lc/photconfig
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.4/src/phot2lc/photfunc.py
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.4/src/phot2lc/quicklook
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.4/src/phot2lc/teledat.py
+-rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.4/src/phot2lc/ucm_utils.py
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21321 2023-04-29 00:18:23.000000 phot2lc-1.7.4/src/phot2lc/version_history.txt
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.4/src/phot2lc/weldlc
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:23:29.050431 phot2lc-1.7.4/src/phot2lc.egg-info/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-04-29 00:23:28.000000 phot2lc-1.7.4/src/phot2lc.egg-info/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-04-29 00:23:28.000000 phot2lc-1.7.4/src/phot2lc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-04-29 00:23:28.000000 phot2lc-1.7.4/src/phot2lc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-04-29 00:23:28.000000 phot2lc-1.7.4/src/phot2lc.egg-info/top_level.txt
```

### Comparing `phot2lc-1.7.3/LICENSE` & `phot2lc-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/PKG-INFO` & `phot2lc-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.3
+Version: 1.7.4
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `phot2lc-1.7.3/README.md` & `phot2lc-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/setup.py` & `phot2lc-1.7.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phot2lc",
-    version="1.7.3",
+    version="1.7.4",
     author="Zach Vanderbosch",
     author_email="zvanderbosch@gmail.com",
     description="Light curve extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zvanderbosch/phot2lc",
     packages=setuptools.find_packages('src'),
@@ -17,15 +17,16 @@
     package_data={
         'phot2lc': ['config.dat',
                     'version_history.txt'],},
     scripts=[
         'src/phot2lc/phot2lc',
         'src/phot2lc/weldlc',
         'src/phot2lc/photconfig',
-        'src/phot2lc/quicklook'],
+        'src/phot2lc/quicklook',
+        'src/phot2lc/addstar'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",],
```

### Comparing `phot2lc-1.7.3/src/phot2lc/phot2lc` & `phot2lc-1.7.4/src/phot2lc/phot2lc`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 from matplotlib.patches import Circle
 from matplotlib.gridspec import GridSpec
 from matplotlib.ticker import MultipleLocator
 from matplotlib.widgets import Cursor, MultiCursor
 from matplotlib.widgets import RectangleSelector
 
 # Import Custom Functions
+import phot2lc.teledat
 from phot2lc.teledat import get_telinfo
 from phot2lc.photfunc import progress_bar, print_commands
 from phot2lc.photfunc import get_time, pp_scat, roll_std
 from phot2lc.photfunc import div_lc, gen_compstr, calc_lsp
 from phot2lc.photfunc import get_loc, window_std
 from phot2lc.ucm_utils import read_ucm
 
@@ -108,43 +109,46 @@
 config_path = os.path.dirname(os.path.realpath(phot2lc.teledat.__file__))
 config_dat = []
 with open(config_path + "/config.dat") as f:
     for l in f.readlines():
         config_dat.append(l.strip("\n").split("=")[-1].strip())
 
 
-# Name for whoever is performing these reductions
+# Name for whoever is running phot2lc
 author = config_dat[0]
 # File containing the list of images being analyzed
 list_name = config_dat[1]
-# Optional File containing initial guesses at target + comp pixel
-# locations. This is the same file used for IRAF ccd_hsp aperture
-# photometry and is not needed if you don't have it.
+# Optional File containing initial guesses at source locations.
 tloc_name = config_dat[2]
+# Base filename for photometry output from pipelines
+phot_basename = config_dat[3]
 # Path to file containing object names + coordinates
-star_dat_filename = config_dat[3] 
+star_dat_filename = config_dat[4] 
+
 
 
 # Defualt arguments for argparse
-default_telescope = config_dat[4]
-default_source = config_dat[5]
-default_image = None if config_dat[6] == 'None' else config_dat[6]
-default_object = None if config_dat[7] == 'None' else config_dat[7]
+default_telescope = config_dat[5]
+default_source = config_dat[6]
+default_image = None if config_dat[7] == 'None' else config_dat[7]
+default_object = None if config_dat[8] == 'None' else config_dat[8]
 
 
 #############################################################
 ## Generate arguments for command line parsing
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-c', '--codes',action='store_true',
                     help="If invoked, print list of available telescope codes.")
 parser.add_argument('-t', '--telescope',type=str,default=default_telescope,
                     help="Code name for telescope used.")
 parser.add_argument('-s', '--source',type=str,default=default_source,
                     help="Source of photometry (ccd_hsp or maestro)")
+parser.add_argument('-p', '--photname',type=str,default=phot_basename,
+                    help="Base filename for photometry output files.")
 parser.add_argument('-i', '--image',type=str,default=default_image,
                     help="Whether to use a list of images, or just one.")
 parser.add_argument('-o', '--object',type=str,default=default_object,
                     help="Name of object. If None, get object from FITS header.")
 parser.add_argument('-b', '--barycorr',action='store_false',
                     help="If invoked, do NOT perform barycentric corrections.")
 args = parser.parse_args()
@@ -201,14 +205,23 @@
           '"{}" is not currently supported.'.format(psource))
     print('Supported source codes:')
     for code in valid_sources:
         print("   {} = {}".format(code,source_dict[code]))
     print("")
     sys.exit(1)
 
+# Check that base name for photometry output is valid
+photbase = args.photname.strip()
+if len(photbase) == 0:
+    print('\nERROR: Base name provided for photometry files is an empty string!\n')
+    sys.exit(1)
+if len(glob(f"{photbase}*")) == 0:
+    print(f'\nERROR: No photometry files with base name "{photbase}" found in current working directory!\n')
+    sys.exit(1)
+
 # Set the barycorr parameter
 barycorr = args.barycorr
 
 # Get Camera Noise Characteristics
 dark = teldict['dark'] # Dark Current in ADU/s/pixel
 read = teldict['read'] # Read Noise in e-/s/pixel
 gain = teldict['gain'] # Gain in e-/ADU
@@ -235,28 +248,23 @@
 qtc.pyqtRemoveInputHook() # Supresses QCORE message during input
 plt.style.use('dark_background') # Sets default plot style
 
 
 #############################################################
 ## Start loading in data
 
-# Grab all of the runbase Photometry files
-if psource == 'hsp': # hsp_nd output
-    phot_names_raw = glob('runbase*')
-elif psource == 'mae': # maestro output
-    phot_names_raw = glob('counts*')
-elif psource == 'hcm': # hipercam output
-    phot_names_raw = glob('output*log')
-    if len(phot_names_raw) == 0:
-        print('No HiPERCAM output *.log) file found with name ')
-elif psource == 'ucm': # ultracam output
-    phot_names_raw = glob('output*log')
-    if len(phot_names_raw) == 0:
-        print('No HiPERCAM output *.log) file found with name ')
+# Grab all of the photometry output files
+phot_names_raw = glob(f'{photbase}*')
 Nf = len(phot_names_raw)
+if (psource in ['ucm','hcm']) & (Nf > 1):
+    print(f'\nERROR: Multiple photometry files found with base name "{photbase}":')
+    for fs in phot_names_raw:
+        print(f"       > {fs}")
+    print('       For ULTRA/HiPERCAM pipelines, only one photometry file can be used with phot2lc.\n')
+    sys.exit(1)
 
 
 # Grab all or just one of the FITS files
 if args.image is None:
     fits_list = np.loadtxt(list_name, dtype=str)
     num_fits = len(fits_list)
 else:
```

### Comparing `phot2lc-1.7.3/src/phot2lc/photfunc.py` & `phot2lc-1.7.4/src/phot2lc/photfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from copy import deepcopy
 from scipy.signal import find_peaks
 from astropy.io import fits
 from astropy.time import Time
 from astropy.coordinates import EarthLocation
 from astropy.timeseries import LombScargle as ls
+import astropy.units as u
 import lmfit as lmf
 from lmfit import Model
 
 
 """
 Script containing many functions needed by the 
 main phot2lc.py program.
@@ -124,33 +125,44 @@
     if telcode == 'mcd2':
         loc = EarthLocation.of_site('mcdonald')
     elif telcode == 'coud':
         loc = EarthLocation.of_site('mcdonald')
     elif telcode == 'perk':
         loc = EarthLocation.of_site('lowell')
     elif telcode == 'pjmo':
-        loc = EarthLocation.from_geodetic(31.67991667,97.67352778,333.0)
+        loc = EarthLocation.from_geodetic(
+            lon=31.67991667*u.deg,
+            lat=97.67352778*u.deg,
+            height=333.0*u.m)
     elif telcode == 'lco1':
         site_info = hdr['SITE'].split(" ")
         if any([x=='Haleakala'] for x in site_info):
             loc = EarthLocation.of_site('haleakala')
         elif any([x=='Spring'] for x in site_info):
             loc = EarthLocation.of_site('sso')
         elif any([x=='SAAO'] for x in site_info):
             loc = EarthLocation.of_site('SAAO')
         elif any([x=='McDonald'] for x in site_info):
             loc = EarthLocation.of_site('mcdonald')
         elif any([x=='Tololo'] for x in site_info):
             loc = EarthLocation.of_site('ctio')
+        elif any([x=='Tenerife'] for x in site_info):
+            loc = EarthLocation.from_geodetic(
+                lon=20.301111*u.deg,
+                lat=-16.510556*u.deg,
+                height=2390.*u.m)
     elif telcode == 'kped':
         loc = EarthLocation.of_site('Kitt Peak')
     elif telcode == 'p200':
         loc = EarthLocation.of_site('palomar')
     elif telcode == 'opd':
-        loc = EarthLocation.from_geodetic(-45.5825,-22.71777778,1864.0)
+        loc = EarthLocation.from_geodetic(
+            lon=-45.5825*u.deg,
+            lat=-22.71777778*u.deg,
+            height=1864.0*u.m)
     return loc
 
 # LNA:  long= W 45 34 57  lat= -22 43 04, altitude = 1864m
 
 ###################################################
 # Some functions used for calculating a divided light curve
 
@@ -324,14 +336,15 @@
     print('')
 
 
     # Let's change it up
     queries = ['author            = ',
                'image_list_name   = ',
                'pixloc_name       = ',
+               'photbase_name     = ',
                'stardat_location  = ',
                'default_telescope = ',
                'default_source    = ',
                'default_image     = ',
                'default_object    = ']
     output = []
     for i,q in enumerate(queries):
```

### Comparing `phot2lc-1.7.3/src/phot2lc/quicklook` & `phot2lc-1.7.4/src/phot2lc/quicklook`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/src/phot2lc/teledat.py` & `phot2lc-1.7.4/src/phot2lc/teledat.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/src/phot2lc/ucm_utils.py` & `phot2lc-1.7.4/src/phot2lc/ucm_utils.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/src/phot2lc/version_history.txt` & `phot2lc-1.7.4/src/phot2lc/version_history.txt`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,15 @@
     - So far it has only been tested for data acquired
       from the McDonald 2.1m ProEM instrument or the 
       Palomar 200-in CHIMERA instrument. Data from
       from other instruments reduced using the
       HiPERCAM pipeline may not yet play nice with phot2lc.
       
       
- Version 1.7.2 - 2023-02-08 (not yet released)
+ Version 1.7.2 - 2023-02-08
 ---------------------------
 > Improved error messaging for missing object name
   from the stars.dat file.
 > Improved header descriptions for the .lc and .phot files.
     - Added new header row in .lc file listing the IDs of
       comparison stars used to generate divided light curve.
     - Added new header row in both .phot and .lc files 
@@ -506,17 +506,35 @@
   that a file with a name like output*log exists containing 
   the raw photometry. It will also assume that a .ucm file
   needs to be loaded in order to display the first image,
   and use an ULTRACAM aperture file (.ape) to display the
   initial source aperture positions.
 
 
+ Version 1.7.3 (2023-02-09)
+---------------------------
+> Minor bug fixes
 
 
-
+ Version 1.7.4 - not yet released
+---------------------------
+> Added new location info for the Tenerife site of the 
+  Las Cumbres Observatory 1.0-m telescopes.
+> Added new option for the config.dat file called
+  phot_basename, which allows users to specify the base
+  filename for the output from the photometry pipeline
+  being used (e.g. "runbase" for ccd_hsp or "output.log"
+  for ULTRA/HiPERCAM). There is also a new command line
+  option for phot2lc (-p, --photname), which allows users
+  to specify the basename at runtime or override whatever
+  the default value is in the config.dat file.
+> Added a new command line convenience program "addstar"
+  that allows users to add a new entry into the stars.dat
+  file. Example usage:
+      addstar SDSSJ0000+1111 00:00:00.0 +11:11:11.1
```

### Comparing `phot2lc-1.7.3/src/phot2lc/weldlc` & `phot2lc-1.7.4/src/phot2lc/weldlc`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.3/src/phot2lc.egg-info/PKG-INFO` & `phot2lc-1.7.4/src/phot2lc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.3
+Version: 1.7.4
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

