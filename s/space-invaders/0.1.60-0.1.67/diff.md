# Comparing `tmp/space-invaders-0.1.60.tar.gz` & `tmp/space-invaders-0.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.60.tar", last modified: Fri Apr 28 23:14:19 2023, max compression
+gzip compressed data, was "space-invaders-0.1.67.tar", last modified: Fri Apr 28 23:58:02 2023, max compression
```

## Comparing `space-invaders-0.1.60.tar` & `space-invaders-0.1.67.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.938530 space-invaders-0.1.60/
--rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.60/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-04-28 23:14:19.938530 space-invaders-0.1.60/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 23:14:19.938530 space-invaders-0.1.60/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-28 23:13:57.000000 space-invaders-0.1.60/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.933025 space-invaders-0.1.60/space_invaders/
--rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.1.60/space_invaders/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.60/space_invaders/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.60/space_invaders/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.60/space_invaders/level.py
--rw-rw-rw-   0        0        0    15997 2023-04-28 22:47:17.000000 space-invaders-0.1.60/space_invaders/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.60/space_invaders/pickup.py
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.60/space_invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.937530 space-invaders-0.1.60/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       57 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:58:02.882224 space-invaders-0.1.67/
+-rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.67/MANIFEST.in
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:58:02.882224 space-invaders-0.1.67/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:58:02.882224 space-invaders-0.1.67/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-04-28 23:52:36.000000 space-invaders-0.1.67/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:58:02.872635 space-invaders-0.1.67/space_invaders/
+-rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.1.67/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.67/space_invaders/config.py
+-rw-rw-rw-   0        0        0     3465 2023-04-28 23:45:55.000000 space-invaders-0.1.67/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    16824 2023-04-28 23:46:14.000000 space-invaders-0.1.67/space_invaders/level.py
+-rw-rw-rw-   0        0        0    16106 2023-04-28 23:53:21.000000 space-invaders-0.1.67/space_invaders/main.py
+-rw-rw-rw-   0        0        0     2946 2023-04-28 23:46:27.000000 space-invaders-0.1.67/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0    11046 2023-04-28 23:46:40.000000 space-invaders-0.1.67/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:58:02.881224 space-invaders-0.1.67/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 23:58:02.000000 space-invaders-0.1.67/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.60/PKG-INFO` & `space-invaders-0.1.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.60
+Version: 0.1.67
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.60/setup.py` & `space-invaders-0.1.67/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='space-invaders',
-    version='0.1.60',
-    py_modules=['entity', 'config', 'main', 'spaceship', 'level', 'pickup'],
-    packages=find_packages(),
+    version='0.1.67',
+    packages=['space_invaders'],
     install_requires=[
         'pygame',
         'shapely'
     ],
     entry_points={
         'console_scripts': [
-            'space-invaders=space_invaders.main:main'
+            'test-invaders=space_invaders.main:main'
         ]
     },
     author='Bódi Martin',
     author_email='bodimartin22@gmail.com',
     description='A cool space shooter rouge like game',
     long_description=open('space_invaders/README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `space-invaders-0.1.60/space_invaders/config.py` & `space-invaders-0.1.67/space_invaders/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.60/space_invaders/entity.py` & `space-invaders-0.1.67/space_invaders/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pygame
 
-from config import WINDOW_WIDTH, WINDOW_HEIGHT
+from space_invaders.config import WINDOW_WIDTH, WINDOW_HEIGHT
 
 
 class Entity(pygame.sprite.Sprite):
     def __init__(self, ship, spawn_position, speed, lives=1, looks_down=True):
         super().__init__()
         self._ship = ship.new_ship()
         self._hp = ship.hp
```

### Comparing `space-invaders-0.1.60/space_invaders/level.py` & `space-invaders-0.1.67/space_invaders/level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 from math import log2
-from entity import Entity, Enemy
-import spaceship
-from spaceship import DEFAULT_ENEMY_SHIP, DEFAULT_SHIP
-from config import WINDOW_WIDTH, WINDOW_HEIGHT
+from space_invaders.entity import Entity, Enemy
+import space_invaders.spaceship as spaceship
+from space_invaders.spaceship import DEFAULT_ENEMY_SHIP, DEFAULT_SHIP
+from space_invaders.config import WINDOW_WIDTH, WINDOW_HEIGHT
 
 
 class Phase:
     """This class represents a phase of a level, which is basically a set of enemies and their actions"""
     def __init__(self, phase_enemies, positions, speeds, actions):
         self._enemy_ships = phase_enemies
         self._positions = positions
```

### Comparing `space-invaders-0.1.60/space_invaders/main.py` & `space-invaders-0.1.67/space_invaders/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import random
 import pygame.display
 from pygame.locals import K_w, K_a, K_s, K_d, K_SPACE, K_LSHIFT, USEREVENT
 from shapely.geometry import Polygon
-from entity import Entity
-from pickup import PICKUP_LIFE, PICKUP_MINIGUN, PICKUP_REPAIR, PICKUP_ROCKET_GUN, PICKUP_SMALL_HEAL, \
+from space_invaders.entity import Entity
+from space_invaders.pickup import PICKUP_LIFE, PICKUP_MINIGUN, PICKUP_REPAIR, PICKUP_ROCKET_GUN, PICKUP_SMALL_HEAL, \
     PICKUP_MEDIUM_HEAL, PICKUP_FIRE_RATE_BOOSTER, Pickup, RESET_FIRE_RATE
-from spaceship import ROCKET_GUN, MINIGUN
-from config import WINDOW_WIDTH, WINDOW_HEIGHT, play_sound, PICKUP_SPEED, PICKUP_SPAWN_INTERVAL, SOUND_PICKUP_DATA, \
+from space_invaders.spaceship import ROCKET_GUN, MINIGUN
+from space_invaders.config import WINDOW_WIDTH, WINDOW_HEIGHT, play_sound, PICKUP_SPEED, PICKUP_SPAWN_INTERVAL, \
     SOUND_CREDITS_DATA, SOUND_EXPLOSION_DATA, SOUND_MAIN_THEME_DATA, SOUND_DEFEAT_DATA, SOUND_VICTORY_DATA, \
     SOUND_ENEMY_HIT_DATA, SOUND_PLAYER_HIT_DATA, SHOW_HIT_BOXES, get_credits_text, EXPLOSION_DURATION, \
     RESET_SWITCH_DELAY, FONT_CREDITS_TEXT_DATA, FONT_CREDITS_TITLE_DATA, FONT86_DATA, FONT15_DATA, FONT152_DATA, \
-    FONT25_DATA, FONT36_DATA, CHANNEL_COUNT, CAPTION, BACKGROUND_IMAGE
-import config
-import level
+    FONT25_DATA, FONT36_DATA, CHANNEL_COUNT, CAPTION, BACKGROUND_IMAGE, SOUND_PICKUP_DATA
+import space_invaders.config as config
+import space_invaders.level as level
 
 
 def update_pickups():
     global pickups, window, player
     player_poly = Polygon(player.hit_box)
 
     for pickup in pickups:
```

### Comparing `space-invaders-0.1.60/space_invaders/pickup.py` & `space-invaders-0.1.67/space_invaders/pickup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import pygame
 from pygame.locals import USEREVENT
-import spaceship
+import space_invaders.spaceship as spaceship
 
 
 class Pickup(pygame.sprite.Sprite):
     def __init__(self, action, **kwargs):   # image=None, image_file="", *args
         super().__init__()
 
         if kwargs.get('image', None) is not None:
```

### Comparing `space-invaders-0.1.60/space_invaders/spaceship.py` & `space-invaders-0.1.67/space_invaders/spaceship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import pygame
 from shapely.geometry import Polygon
-import config
+import space_invaders.config as config
 
 
 class Spaceship:
     def __init__(self, gun, hp, hit_box, enemy, image_file="", image=None):
         self._image = image if image is not None else pygame.image.load(image_file)
         self._guns = gun if isinstance(gun, list) else [gun]
         self._active_gun = 0
```

### Comparing `space-invaders-0.1.60/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.1.67/space_invaders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.60
+Version: 0.1.67
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

