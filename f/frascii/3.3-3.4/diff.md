# Comparing `tmp/frascii-3.3.tar.gz` & `tmp/frascii-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-3.3.tar", last modified: Sat Apr 29 14:18:52 2023, max compression
+gzip compressed data, was "frascii-3.4.tar", last modified: Sat Apr 29 14:54:00 2023, max compression
```

## Comparing `frascii-3.3.tar` & `frascii-3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.219963 frascii-3.3/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-29 14:18:52.219963 frascii-3.3/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-3.3/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.215963 frascii-3.3/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2053 2023-04-29 14:18:25.000000 frascii-3.3/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7915 2023-04-29 14:05:16.000000 frascii-3.3/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.219963 frascii-3.3/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.3/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.3/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.3/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.3/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.3/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.3/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.3/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.3/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3707 2023-04-29 13:56:22.000000 frascii-3.3/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.3/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.3/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.3/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.3/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.215963 frascii-3.3/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-29 14:18:52.219963 frascii-3.3/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.3/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14887 2023-04-29 14:54:00.014015 frascii-3.4/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12821 2023-04-29 14:53:52.000000 frascii-3.4/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2134 2023-04-29 14:53:28.000000 frascii-3.4/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7913 2023-04-29 14:51:12.000000 frascii-3.4/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.4/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.4/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.4/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.4/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.4/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.4/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.4/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.4/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3707 2023-04-29 13:56:22.000000 frascii-3.4/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.4/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.4/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.4/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.4/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14887 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-29 14:54:00.000000 frascii-3.4/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-29 14:54:00.014015 frascii-3.4/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.4/setup.py
```

### Comparing `frascii-3.3/PKG-INFO` & `frascii-3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.3
+Version: 3.4
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
@@ -31,15 +31,15 @@
         
         `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
         
         `frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
         
         `frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
         
-        `frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
+        `frascii l_system <start, rules, n, animate>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
         
         
         more to come ...
         
         # Examples
         
         ## Mandelbrot set
```

### Comparing `frascii-3.3/README.md` & `frascii-3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
 
 `frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
 
 `frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
 
-`frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
+`frascii l_system <start, rules, n, animate>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
 
 
 more to come ...
 
 # Examples
 
 ## Mandelbrot set
```

### Comparing `frascii-3.3/frascii/__init__.py` & `frascii-3.4/frascii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string, l_system_animate
 
-__version__ = '3.3'
+__version__ = '3.4'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
@@ -47,10 +47,12 @@
 def dragon_curve(n):
 	return dragon_curve_string(n)
 
 def fibonacci(n):
 	return fibonacci_string(n)
 
 def l_system(start, rules, n, direction, animate):
-	if animate is None:
+	if animate is -1:
 		return l_system_string(start, rules, n, direction)
+	elif animate is None:
+		return l_system_animate(start, rules, n, direction, 0.01)
 	return l_system_animate(start, rules, n, direction, animate)
```

### Comparing `frascii-3.3/frascii/commands.py` & `frascii-3.4/frascii/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
 	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
 	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
 	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
 	l_system_parser.add_argument("-direction", type=str, help="pixels added on top and bottom of center", choices=["U", "R", "D", "L"], nargs="?", default="U")
-	l_system_parser.add_argument("-animate", type=float, help="if set scene is animated with chosen delay between frames.", nargs="?", default=None)
+	l_system_parser.add_argument("-animate", type=float, help="if set scene is animated with chosen delay between frames.", nargs="?", default=-1)
 	l_system_parser.set_defaults(func=frascii.l_system)
 
 
 	args = parser.parse_args()
 	if args.subcommand == None:
 		parser.print_help()
 		parser.exit()
```

### Comparing `frascii-3.3/frascii/fractals/dragon_curve.py` & `frascii-3.4/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/fibonacci.py` & `frascii-3.4/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/hilbert_curve.py` & `frascii-3.4/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/julia.py` & `frascii-3.4/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/koch.py` & `frascii-3.4/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/l_system.py` & `frascii-3.4/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/mandelbrot.py` & `frascii-3.4/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/peano_curve.py` & `frascii-3.4/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii/fractals/sierpinski_carpet.py` & `frascii-3.4/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-3.3/frascii.egg-info/PKG-INFO` & `frascii-3.4/frascii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.3
+Version: 3.4
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
@@ -31,15 +31,15 @@
         
         `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
         
         `frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
         
         `frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter, grid, style, explore>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
         
-        `frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
+        `frascii l_system <start, rules, n, animate>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
         
         
         more to come ...
         
         # Examples
         
         ## Mandelbrot set
```

### Comparing `frascii-3.3/frascii.egg-info/SOURCES.txt` & `frascii-3.4/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frascii-3.3/setup.py` & `frascii-3.4/setup.py`

 * *Files identical despite different names*

