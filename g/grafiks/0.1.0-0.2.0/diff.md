# Comparing `tmp/grafiks-0.1.0.tar.gz` & `tmp/grafiks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafiks-0.1.0.tar", max compression
+gzip compressed data, was "grafiks-0.2.0.tar", max compression
```

## Comparing `grafiks-0.1.0.tar` & `grafiks-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2246 2023-04-08 07:24:46.028748 grafiks-0.1.0/grafiks/__init__.py
--rw-r--r--   0        0        0       22 2023-04-08 07:23:47.000000 grafiks-0.1.0/grafiks/__init__.py~
--rw-r--r--   0        0        0      320 2023-04-08 07:32:42.891610 grafiks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      515 2023-04-08 07:32:47.354382 grafiks-0.1.0/setup.py
--rw-r--r--   0        0        0      264 2023-04-08 07:32:47.354598 grafiks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2244 2023-04-29 14:09:40.779705 grafiks-0.2.0/grafiks/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-08 07:23:47.000000 grafiks-0.2.0/grafiks/__init__.py~
+-rw-r--r--   0        0        0      293 2023-04-29 14:14:54.445444 grafiks-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-04-29 14:14:57.903959 grafiks-0.2.0/setup.py
+-rw-r--r--   0        0        0      237 2023-04-29 14:14:57.904423 grafiks-0.2.0/PKG-INFO
```

### Comparing `grafiks-0.1.0/grafiks/__init__.py` & `grafiks-0.2.0/grafiks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     def draw_line(self, start_x, start_y, end_x, end_y, color, thickness):
         # Draw a line with the given parameters
         start_pos = (start_x, start_y)
         end_pos = (end_x, end_y)
         pygame.draw.line(self.screen, color, start_pos, end_pos, thickness)
 
-    def draw_text(self, text, x, y, font_size, color):
+    def draw_text(self, text, x, y, font_file, font_size, color):
         # Draw text with the given parameters
-        font = pygame.font.Font("VictorMono-Medium.tff", font_size)
+        font = pygame.font.Font(font_file, font_size)
         text_surface = font.render(text, True, color)
         text_rect = text_surface.get_rect()
         text_rect.center = (x, y)
         self.screen.blit(text_surface, text_rect)
 
     def draw_image(self, image_path, x, y):
         # Load an image and blit it onto the screen at the given position
@@ -55,8 +55,8 @@
                 self.keys[pygame.key.name(event.key)]=True
                 print(self.keys)
     def key_pressed(self,key):
         try:
             if self.keys[key]==True:
                 return True
         except:
-            pass
+            pass
```

