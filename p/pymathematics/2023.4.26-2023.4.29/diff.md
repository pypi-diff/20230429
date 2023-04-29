# Comparing `tmp/pymathematics-2023.4.26.tar.gz` & `tmp/pymathematics-2023.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.26.tar", last modified: Wed Apr 26 15:51:58 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.29.tar", last modified: Sat Apr 29 08:37:21 2023, max compression
```

## Comparing `pymathematics-2023.4.26.tar` & `pymathematics-2023.4.29.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:58.108329 pymathematics-2023.4.26/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.26/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-26 15:51:58.096332 pymathematics-2023.4.26/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      166 2023-04-26 15:45:31.000000 pymathematics-2023.4.26/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:57.575325 pymathematics-2023.4.26/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    22129 2023-04-26 15:51:10.000000 pymathematics-2023.4.26/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-26 15:45:02.000000 pymathematics-2023.4.26/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-26 15:51:57.931333 pymathematics-2023.4.26/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/requires.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-26 15:51:50.000000 pymathematics-2023.4.26/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-26 15:51:58.113329 pymathematics-2023.4.26/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-26 15:45:24.000000 pymathematics-2023.4.26/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.414260 pymathematics-2023.4.29/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.29/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-29 08:37:21.406159 pymathematics-2023.4.29/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      166 2023-04-29 08:30:20.000000 pymathematics-2023.4.29/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.112787 pymathematics-2023.4.29/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    26470 2023-04-29 08:31:31.000000 pymathematics-2023.4.29/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-29 08:30:00.000000 pymathematics-2023.4.29/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.352156 pymathematics-2023.4.29/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-29 08:37:18.000000 pymathematics-2023.4.29/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-29 08:37:21.416282 pymathematics-2023.4.29/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-29 08:33:18.000000 pymathematics-2023.4.29/setup.py
```

### Comparing `pymathematics-2023.4.26/LICENSE` & `pymathematics-2023.4.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.26/pymathematics/__init__.py` & `pymathematics-2023.4.29/pymathematics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+"""
+pymathematics
+=============
+
+Provides
+  1. fast and accurate calculations
+  2. work with vectors, matrices and sets
+  3. statistics, basic mathematics calculation
+
+  >>> from pymathematics import *
+  >>> about.version
+  ... 2023.4.28
+  >>> about.homepage
+  ... "https://github.com/Sahil-Rajwar-2004/pymathematics"
+  >>> sqrt(4)
+  ... 2.0
+  >>> constants.inf
+  ... inf
+  >>> constants.pi
+  ... 3.1415926535897932384626433832795
+  >>> constants.e
+  ... 2.7182818284590452353602874713527
+  >>> mean([1,2,3,4,5])
+  ... 5.5
+"""
+
 import sympy
 
 from .info import (
     author,version,homepage
 )
 
 class about:
@@ -212,14 +238,103 @@
         B = sets.toset(B)
         res = []
         for i in A:
             for j in B:
                 res.append([i,j])
         return res
     
+class area:
+    def rectangle(length,breadth) -> int|float:
+        return length*breadth
+    
+    def square(side) -> int|float:
+        return side**2
+    
+    def trapezoid(a,b,height) -> int|float:
+        return (a+b)*height/2
+    
+    def parallelogram(breadth,height) -> int|float:
+        return breadth*height
+    
+    def triangle(base,height) -> int|float:
+        return 0.5*base*height
+    
+    def circle(radius) -> int|float:
+        return constants.pi*radius**2
+    
+    def semi_circle(radius) -> int|float:
+        return 0.5*constants.pi*radius**2
+    
+    def ellipse(minor_axis,major_axis) -> int|float:
+        return constants.pi*minor_axis*major_axis
+
+    def equilateral_triangle(side) -> int|float:
+        return sqrt(3)/4*side**2
+    
+    def sector(angle,radius) -> int|float:
+        return angle/360*constants.pi*radius**2
+    
+    def segment(angle,radius) -> int|float:
+        return area.sector(angle,radius) - area.triangle(radius,radius)
+    
+    def annulus(Radius,radius) -> int|float:
+        if radius > Radius:
+            return constants.pi*(radius-Radius)
+        return constants.pi*(Radius-radius)
+    
+    def regular_hexagon(side) -> int|float:
+        return 3*sqrt(3)/2*side**2
+    
+    def regular_octagon(side) -> int|float:
+        return 2*(1+sqrt(2))*side**2
+    
+    def sector(angle,radius) -> int|float:
+        return angle/360*constants.pi*radius**2
+    
+    def segment(angle,radius) -> int|float:
+        return 0.5*radius**2*(angle-sin(angle))
+    
+class volume:
+    def cuboid(length,breadth,height) -> int|float:
+        return length*breadth*height
+    
+    def cube(side) -> int|float:
+        return side**3
+    
+    def sphere(radius) -> int|float:
+        return (4/3)*constants.pi*radius**3
+    
+    def hemisphere(radius) -> int|float:
+        return (2/3)*constants.pi*radius**3
+    
+    def right_circular_cone(radius,height) -> int|float:
+        return (1/3)*constants.pi*radius**2*height
+    
+    def right_circular_cylinder(radius,height) -> int|float:
+        return constants.pi*radius**2*height
+    
+    def rhombus(d1,d2) -> int|float:
+        return 0.5*d1*d2
+    
+class perimeter:
+    def rectangle(length,breadth) -> int|float:
+        return 2*(length+breadth)
+    
+    def square(side) -> int|float:
+        return 4*side
+    
+    def circumference(radius) -> int|float:
+        return 2*constants.pi*radius
+    
+    def semi_circle(radius) -> int|float:
+        return constants.pi*radius
+    
+    def rhombus(side) -> int|float:
+        return 4*side
+    
 class calculus:
     def integral(eqn:str,wrt:str = "x",limits:list = [None,None]):
         if len(limits) != 2:
             raise ValueError(f"size of the limits should be 2, not {len(limits)}")
         expr = sympy.sympify(eqn)
         return sympy.integrate(expr,(wrt,limits[0],limits[1]))
     
@@ -267,14 +382,24 @@
     return summation([(number**n)/factorial(n) for n in range(0,100)])
 
 def absolute(number:int|float) -> int|float:
     if number < 0:
         return -1*number
     return number
 
+def floor(number:int|float) -> int:
+    if number < 0:
+        return int(number)-1
+    return int(number)
+
+def ceil(number:int|float) -> int:
+    if number < 0:
+        return int(number)
+    return int(number)+1
+
 def sqrt(number:int|float) -> float:
     if number < 0:
         return "undefined"
     elif number == 0:
         return 0
     flag = number/2
     while absolute(flag*flag - number) > 0.00001:
@@ -396,14 +521,27 @@
     return 1/sin(theta)
 
 def sec(theta:int|float) -> float:
     if cos(theta) == 0:
         raise ValueError(f"sec({theta}) isn't defined at rad({theta})")
     return 1/cos(theta)
 
+def arcsin(value:int|float) -> float:
+    if value < -1 or value > 1:
+        raise ValueError("domain error")
+    term = 0
+    for n in range(0,100):
+        term += factorial(2*n)/(factorial(n)**2*4**n*(2*n+1))*value**(2*n+1)
+    return term
+
+def arccos(value:int|float) -> float:
+    if value < -1 or value > 1:
+        raise ValueError("domain error")
+    return constants.pi/2-arcsin(value)
+
 def mean(array:list) -> int|float:
     return sum(array)/len(array)
 
 def median(array:list) -> list:
     sorted_array = quick_sort(array)
     if len(sorted_array)%2 == 0:
         mid1 = int(len(sorted_array)/2)
@@ -416,15 +554,15 @@
 def standard_deviation(array:list,kind:str = "population") -> list:
     if kind == "sample":
         d = len(array)-1
     elif kind == "population":
         d = len(array)
     else:
         raise ValueError(f"invalid input {kind}! input should be whether 'population' or 'sample'")
-    return sqrt(summation((i - mean(array))**2 for i in array)/(d))
+    return sqrt(summation((x - mean(array))**2 for x in array)/(d))
 
 def variance(array:list,kind:str = "population") -> int|float:
     if kind == "sample":
         d = len(array)-1
     elif kind == "population":
         d = len(array)
     else:
@@ -637,7 +775,22 @@
     return sqrt(mean_sqrd_error(actual,predicted))
 
 def cost_function(actual:list, predicted:list) -> int|float:
     if len(actual) != len(predicted):
         raise ValueError("length of actual and predicted data aren't equal!")
     errors = [(actual[i]-predicted[i])**2 for i in range(len(actual))]
     return summation(errors)/(2*len(actual))
+
+def scaling(array:list,feature_range:tuple = (0,1)):
+    min_val = min(array)
+    max_val = max(array)
+    scaled_data = [(val - min_val)/(max_val - min_val)*(feature_range[1]-feature_range[0])+feature_range[0] for val in array]
+    return scaled_data
+
+def gaussian(array):
+    result = []
+    std_dev = standard_deviation(array)
+    m = mean(array)
+    for x in array:
+        each = (1/(std_dev*sqrt(2*constants.pi)))*exp(-((x-m)**2)/(2*(std_dev**2)))
+        result.append(each)
+    return result
```

### Comparing `pymathematics-2023.4.26/setup.py` & `pymathematics-2023.4.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.26",
+    version = "2023.4.29",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

