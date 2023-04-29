# Comparing `tmp/fancybbox-0.0.11.tar.gz` & `tmp/fancybbox-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancybbox-0.0.11.tar", last modified: Mon Apr 24 01:45:03 2023, max compression
+gzip compressed data, was "fancybbox-0.0.12.tar", last modified: Sat Apr 29 04:30:44 2023, max compression
```

## Comparing `fancybbox-0.0.11.tar` & `fancybbox-0.0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.565336 fancybbox-0.0.11/
--rw-rw-rw-   0        0        0     1067 2023-04-23 16:35:21.000000 fancybbox-0.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0     1850 2023-04-24 01:45:03.562329 fancybbox-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-04-23 16:33:02.000000 fancybbox-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.506851 fancybbox-0.0.11/fancybbox/
--rw-rw-rw-   0        0        0      252 2023-04-24 01:30:58.000000 fancybbox-0.0.11/fancybbox/__init__.py
--rw-rw-rw-   0        0        0     8283 2023-04-23 15:48:01.000000 fancybbox-0.0.11/fancybbox/fancy_bbox.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.559333 fancybbox-0.0.11/fancybbox.egg-info/
--rw-rw-rw-   0        0        0     1850 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 01:45:03.566333 fancybbox-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-24 01:43:55.000000 fancybbox-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 04:30:44.401462 fancybbox-0.0.12/
+-rw-rw-rw-   0        0        0     1067 2023-04-23 16:35:21.000000 fancybbox-0.0.12/LICENSE.txt
+-rw-rw-rw-   0        0        0     2252 2023-04-29 04:30:44.399456 fancybbox-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2023-04-29 03:13:44.000000 fancybbox-0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 04:30:44.357967 fancybbox-0.0.12/fancybbox/
+-rw-rw-rw-   0        0        0      202 2023-04-24 04:05:43.000000 fancybbox-0.0.12/fancybbox/__init__.py
+-rw-rw-rw-   0        0        0     9405 2023-04-29 04:27:08.000000 fancybbox-0.0.12/fancybbox/fancy_bbox.py
+drwxrwxrwx   0        0        0        0 2023-04-29 04:30:44.395455 fancybbox-0.0.12/fancybbox.egg-info/
+-rw-rw-rw-   0        0        0     2252 2023-04-29 04:30:43.000000 fancybbox-0.0.12/fancybbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-29 04:30:43.000000 fancybbox-0.0.12/fancybbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 04:30:43.000000 fancybbox-0.0.12/fancybbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-29 04:30:43.000000 fancybbox-0.0.12/fancybbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 04:30:43.000000 fancybbox-0.0.12/fancybbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 04:30:44.402470 fancybbox-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1055 2023-04-29 04:30:09.000000 fancybbox-0.0.12/setup.py
```

### Comparing `fancybbox-0.0.11/LICENSE.txt` & `fancybbox-0.0.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancybbox-0.0.11/PKG-INFO` & `fancybbox-0.0.12/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: fancybbox
-Version: 0.0.11
+Version: 0.0.12
 Summary: Fancy Bounding Box - Rectangle for Object Detection
-Author: Prashant27050 (Prashant Verma)
+Home-page: https://github.com/Vprashant/fancybbox
+Author: Prashant Verma
 Author-email: prashant27050@gmail.com
 Keywords: python,image processing,bbox,bbox regtangle,fancy rectangle,bounding box
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Fancybbox
+[![PyPi version](https://img.shields.io/pypi/v/fancybbox)](https://pypi.org/project/fancybbox/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A package that allows to build Lib is a package that enables users to create visually appealing bounding boxes for object detection in image processing deep learning projects.  
 With a current version of 0.0.10, the package is constantly being updated and improved. The package offers a variety of features, including the ability to customize the appearance of bounding boxes with different colors, line widths, and styles. 
 Additionally, it provides users with the flexibility to adjust the size and shape of the bounding boxes to meet their specific needs.'
 
 
 Developed by Prashant Verma (c) 2023
 
+This project still very much experimental and may change significantly. 
+
+## Install
+Install with all dependencies:
+
+```bash
+pip install fancybbox
+```
+
 ## Examples of How To Use (Alpha Version)
 
 Creating A Sample detection function
 
 ```python
 import cv2
 from fancy_bbox import FancyBox
```

### Comparing `fancybbox-0.0.11/fancybbox/fancy_bbox.py` & `fancybbox-0.0.12/fancybbox/fancy_bbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 """
 Filename: fancy_bbox.py
 Author: Prashant Verma
 Email: Prashant27050@gmail.com
-Version: 0.0.10
+Version: 0.0.12
 Release Date: 
 """
 
 import cv2
+import numpy as np
 
 class FancyBox:
     def __init__(self, x, y, w, h, border_thickness=2, line_type=cv2.LINE_AA, border_color=(255, 0, 0)):
         self.x = x
         self.y = y
         self.w = w
         self.h = h
         self.border_thickness = border_thickness
         self.line_type = line_type
         self.border_color = border_color
+
+
+    def adjust_opacity(self, image, opacity, opacity_color):
+        # Define the fill color with 50% opacity (alpha = 0.5)
+        
+        tuple_value = (opacity_color, opacity)
+        fill_color = tuple_value[0] + (tuple_value[1],)
+        # Create a numpy array with the same shape as the image
+        mask = np.zeros_like(image)
+        # Draw the bounding box on the mask
+        cv2.rectangle(mask, [self.x, self.y, self.w, self.h], fill_color, cv2.FILLED)
+        image = cv2.addWeighted(image, 1, mask, 0.2, 0)
+        return image
+
     
-    def draw(self, image):
+    def draw(self, image, opacity = None):
         """_summary_
 
         Args:
             image (_type_): _description_
 
         Returns:
             _type_: _description_
         """
+        if opacity:
+            image = self.adjust_opacity(image, opacity[0], opacity[1])
         # Define the corner points of the rectangle
         pt1 = (self.x, self.y)
         pt2 = (self.x + self.w, self.y)
         pt3 = (self.x + self.w, self.y + self.h)
         pt4 = (self.x, self.y + self.h)
 
         # Define the corner points of the border
@@ -45,24 +62,26 @@
         cv2.line(image, bpt4, pt4, self.border_color, self.border_thickness, self.line_type)
         cv2.line(image, bpt2, pt2, self.border_color, self.border_thickness, self.line_type)
         cv2.line(image, bpt2, bpt3, self.border_color, self.border_thickness, self.line_type)
         cv2.line(image, bpt3, pt3, self.border_color, self.border_thickness, self.line_type)
 
         return image
 
-    def draw_dashed_border(self, image, dash_length=10):
+    def draw_dashed_border(self, image, dash_length=10, opacity = None):
         """_summary_
 
         Args:
             image (_type_): _description_
             dash_length (int, optional): _description_. Defaults to 10.
 
         Returns:
             _type_: _description_
         """
+        if opacity:
+            image = self.adjust_opacity(image, opacity[0], opacity[1])
         # Define the corner points of the rectangle
         pt1 = (self.x, self.y)
         pt2 = (self.x + self.w, self.y)
         pt3 = (self.x + self.w, self.y + self.h)
         pt4 = (self.x, self.y + self.h)
 
         # Define the corner points of the border
@@ -77,26 +96,28 @@
             cv2.line(image, (self.x+i, self.y+self.h), (self.x+i+dash_length, self.y+self.h), self.border_color, self.border_thickness, self.line_type)
         for i in range(0, self.h, dash_length*2):
             cv2.line(image, (self.x, self.y+i), (self.x, self.y+i+dash_length), self.border_color, self.border_thickness, self.line_type)
             cv2.line(image, (self.x+self.w, self.y+i), (self.x+self.w, self.y+i+dash_length), self.border_color, self.border_thickness, self.line_type)
 
         return image
 
-    def draw_rounded_corners(self, image, radius=10):
+    def draw_rounded_corners(self, image, radius=10, opacity= None):
         """_summary_
 
         Args:
             image (_type_): _description_
             radius (int, optional): _description_. Defaults to 10.
 
         Returns:
             _type_: _description_
         """
         # Define the corner points of the rectangle
         # Define the corner points of the rectangle
+        if opacity:
+            image = self.adjust_opacity(image, opacity[0], opacity[1])
         pt1 = (self.x, self.y)
         pt2 = (self.x + self.w, self.y)
         pt3 = (self.x + self.w, self.y + self.h)
         pt4 = (self.x, self.y + self.h)
         
         # Define the corner points of the border
         bpt1 = (self.x - self.border_thickness, self.y - self.border_thickness)
@@ -113,27 +134,29 @@
         cv2.ellipse(image, (self.x+radius, self.y+radius), (radius, radius), 180, 0, 90, self.border_color, self.border_thickness, self.line_type)
         cv2.ellipse(image, (self.x+self.w-radius, self.y+radius), (radius, radius), 270, 0, 90, self.border_color, self.border_thickness, self.line_type)
         cv2.ellipse(image, (self.x+radius, self.y+self.h-radius), (radius, radius), 90, 0, 90, self.border_color, self.border_thickness, self.line_type)
         cv2.ellipse(image, (self.x+self.w-radius, self.y+self.h-radius), (radius, radius), 0, 0, 90, self.border_color, self.border_thickness, self.line_type)
 
         return image
 
-    def target_rect_bbox(self, image, l=30, t =5, rt =1):
+    def target_rect_bbox(self, image, l=30, t =5, rt =1, opacity = None):
         """_summary_
 
         Args:
             image (_type_): _description_
             l (int, optional): _description_. Defaults to 30.
             t (int, optional): _description_. Defaults to 5.
             rt (int, optional): _description_. Defaults to 1.
 
         Returns:
             image: returning output image
         """
         x1, y1  = self.x + self.w, self.y + self.w
+        if opacity:
+            image = self.adjust_opacity(image, opacity[0], opacity[1])
         cv2.rectangle(image, [self.x, self.y, self.w, self.h], self.border_color, rt)
         # Top Left
         cv2.line(image, (self.x, self.y), (self.x+ l, self.y), self.border_color, t)
         cv2.line(image, (self.x, self.y), (self.x, self.y + l), self.border_color, t)
         # Top Right
         cv2.line(image, (x1, self.y), (x1 - l, self.y), self.border_color, t)
         cv2.line(image, (x1, self.y), (x1, self.y + l), self.border_color, t)
@@ -142,25 +165,27 @@
         cv2.line(image, (self.x, y1), (self.x, y1 - l), self.border_color, t)
         # Bottom Right
         cv2.line(image, (x1, y1), (x1 - l, y1), self.border_color, t)
         cv2.line(image, (x1, y1), (x1, y1 - l), self.border_color, t)
 
         return image
 
-    def target_angle_bbox(self, image, l= 30, t = 5):
+    def target_angle_bbox(self, image, l= 30, t = 5, opacity=None):
         """target_angle_bbox: return's fancy angle shape corners bbox
         Args:
             image (_type_): _description_
             l (int, optional): length of line - Defaults to 30.
             t (int, optional): width of line - Defaults to 5.
 
         Returns:
             image: returning output image
         """
         x1, y1  = self.x + self.w, self.y + self.w
+        if opacity:
+            image = self.adjust_opacity(image, opacity[0], opacity[1])
 
         cv2.line(image, (self.x, self.y), (self.x+ l, self.y), self.border_color, t)
         cv2.line(image, (self.x, self.y), (self.x, self.y + l), self.border_color, t)
         # Top Right
         cv2.line(image, (x1, self.y), (x1 - l, self.y), self.border_color, t)
         cv2.line(image, (x1, self.y), (x1, self.y + l), self.border_color, t)
         # Bottom Left
```

### Comparing `fancybbox-0.0.11/fancybbox.egg-info/PKG-INFO` & `fancybbox-0.0.12/fancybbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: fancybbox
-Version: 0.0.11
+Version: 0.0.12
 Summary: Fancy Bounding Box - Rectangle for Object Detection
-Author: Prashant27050 (Prashant Verma)
+Home-page: https://github.com/Vprashant/fancybbox
+Author: Prashant Verma
 Author-email: prashant27050@gmail.com
 Keywords: python,image processing,bbox,bbox regtangle,fancy rectangle,bounding box
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Fancybbox
+[![PyPi version](https://img.shields.io/pypi/v/fancybbox)](https://pypi.org/project/fancybbox/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A package that allows to build Lib is a package that enables users to create visually appealing bounding boxes for object detection in image processing deep learning projects.  
 With a current version of 0.0.10, the package is constantly being updated and improved. The package offers a variety of features, including the ability to customize the appearance of bounding boxes with different colors, line widths, and styles. 
 Additionally, it provides users with the flexibility to adjust the size and shape of the bounding boxes to meet their specific needs.'
 
 
 Developed by Prashant Verma (c) 2023
 
+This project still very much experimental and may change significantly. 
+
+## Install
+Install with all dependencies:
+
+```bash
+pip install fancybbox
+```
+
 ## Examples of How To Use (Alpha Version)
 
 Creating A Sample detection function
 
 ```python
 import cv2
 from fancy_bbox import FancyBox
```

### Comparing `fancybbox-0.0.11/setup.py` & `fancybbox-0.0.12/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 
 def readme():
     with open('README.md') as f:
         README = f.read()
     return README
 
-VERSION = '0.0.11'
+VERSION = '0.0.12'
 DESCRIPTION = 'Fancy Bounding Box - Rectangle for Object Detection'
 
 # Setting up
 setup(
     name="fancybbox",
     version=VERSION,
-    author="Prashant27050 (Prashant Verma)",
+    author="Prashant Verma",
     author_email="prashant27050@gmail.com",
+    url="https://github.com/Vprashant/fancybbox",
     long_description_content_type='text/markdown',
     description=DESCRIPTION,
     long_description= readme(),
     packages=find_packages(),
     install_requires=['opencv-python'],
     keywords=['python', 'image processing', 'bbox', 'bbox regtangle', 'fancy rectangle', 'bounding box'],
     classifiers=[
```

