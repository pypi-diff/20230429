# Comparing `tmp/frascii-3.2.tar.gz` & `tmp/frascii-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-3.2.tar", last modified: Wed Apr 26 12:54:33 2023, max compression
+gzip compressed data, was "frascii-3.3.tar", last modified: Sat Apr 29 14:18:52 2023, max compression
```

## Comparing `frascii-3.2.tar` & `frascii-3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 12:54:33.170385 frascii-3.2/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-3.2/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-26 12:54:11.000000 frascii-3.2/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-3.2/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.2/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.2/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.2/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.2/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.2/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.2/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.2/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-26 10:11:08.000000 frascii-3.2/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3743 2023-04-26 12:53:19.000000 frascii-3.2/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.2/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.2/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.2/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.2/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-26 12:54:33.170385 frascii-3.2/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.2/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.219963 frascii-3.3/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-29 14:18:52.219963 frascii-3.3/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-3.3/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.215963 frascii-3.3/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2053 2023-04-29 14:18:25.000000 frascii-3.3/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7915 2023-04-29 14:05:16.000000 frascii-3.3/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.219963 frascii-3.3/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.3/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.3/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.3/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.3/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.3/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.3/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.3/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.3/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3707 2023-04-29 13:56:22.000000 frascii-3.3/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.3/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.3/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.3/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.3/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:18:52.215963 frascii-3.3/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-29 14:18:52.000000 frascii-3.3/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-29 14:18:52.219963 frascii-3.3/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.3/setup.py
```

### Comparing `frascii-3.2/PKG-INFO` & `frascii-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.2
+Version: 3.3
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.2/README.md` & `frascii-3.3/README.md`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/__init__.py` & `frascii-3.3/frascii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from frascii.fractals.cantor import cantor_string
 from frascii.fractals.koch import koch_string
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
-from frascii.fractals.l_system import l_system_string
+from frascii.fractals.l_system import l_system_string, l_system_animate
 
-__version__ = '3.2'
+__version__ = '3.3'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
@@ -46,9 +46,11 @@
 
 def dragon_curve(n):
 	return dragon_curve_string(n)
 
 def fibonacci(n):
 	return fibonacci_string(n)
 
-def l_system(start, rules, n, direction):
-	return l_system_string(start, rules, n, direction)
+def l_system(start, rules, n, direction, animate):
+	if animate is None:
+		return l_system_string(start, rules, n, direction)
+	return l_system_animate(start, rules, n, direction, animate)
```

### Comparing `frascii-3.2/frascii/commands.py` & `frascii-3.3/frascii/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
 	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
 	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
 	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
 	l_system_parser.add_argument("-direction", type=str, help="pixels added on top and bottom of center", choices=["U", "R", "D", "L"], nargs="?", default="U")
+	l_system_parser.add_argument("-animate", type=float, help="if set scene is animated with chosen delay between frames.", nargs="?", default=None)
 	l_system_parser.set_defaults(func=frascii.l_system)
 
 
 	args = parser.parse_args()
 	if args.subcommand == None:
 		parser.print_help()
 		parser.exit()
```

### Comparing `frascii-3.2/frascii/fractals/dragon_curve.py` & `frascii-3.3/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/fibonacci.py` & `frascii-3.3/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/hilbert_curve.py` & `frascii-3.3/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/julia.py` & `frascii-3.3/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/koch.py` & `frascii-3.3/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/mandelbrot.py` & `frascii-3.3/frascii/fractals/mandelbrot.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,19 @@
 		nonlocal style
 		nonlocal grid
 		nonlocal i
 		styles = ["non-repeating", "repeating"]
 		si = 0 if style == "non-repeating" else 1
  	
 		while True:
-			stdscr.clear()
 			rows, cols = stdscr.getmaxyx()
 			y_rad = min(y_radius, rows//2-1)
 			x_rad = min(x_radius, cols//(2 if grid == "rect" else 4)-1)
 			stdscr.addstr(0, 0, mandelbrot_string(x, y, x_rad, y_rad, s, i, styles[si], grid))
-			stdscr.refresh()
+			#stdscr.refresh()
 			key = stdscr.getch()
 			curses.flushinp()
 			if key == curses.KEY_RIGHT:
 				x += 5*s
 			elif key == curses.KEY_LEFT:
 				x -= 5*s
 			elif key == curses.KEY_UP:
@@ -91,15 +90,14 @@
 			elif key == curses.KEY_MOUSE:
 				_, mx, my, _, _ = curses.getmouse()
 				x += ((mx if grid == "rect" else mx/2) - x_rad)*s
 				y += (-my + y_rad)*(2*s if grid == "rect" else s)
 			elif key == 27 or key == ord('x'):
 				break
 			elif key == ord('h'):
-				stdscr.clear()
 				stdscr.addstr(0, 0, ("CONTROLS:\n\nARROWS       : navigate complex plane\nPAGE-UP/DOWN : zoom in/out\n',' and '.'  :")+
 									(" change max-iterations\n'-'          : change style\nESC and 'x'  : leave explore mode and print to screen.\n\n")+
 									(f"CURRENT COMMAND:\nfrascii mandelbrot -x {x} -y {y} -x_radius {x_rad} -y_radius {y_rad} -stepsize {s}")+
 									(f" -max_iter {i} -style {styles[si]} -grid {grid}"))
 				curses.flushinp()
 				while stdscr.getch() not in (ord('h'), ord('x'), 27):
 					pass
```

### Comparing `frascii-3.2/frascii/fractals/peano_curve.py` & `frascii-3.3/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii/fractals/sierpinski_carpet.py` & `frascii-3.3/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-3.2/frascii.egg-info/PKG-INFO` & `frascii-3.3/frascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.2
+Version: 3.3
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.2/frascii.egg-info/SOURCES.txt` & `frascii-3.3/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frascii-3.2/setup.py` & `frascii-3.3/setup.py`

 * *Files identical despite different names*

