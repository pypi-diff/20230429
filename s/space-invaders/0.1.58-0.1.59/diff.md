# Comparing `tmp/space-invaders-0.1.58.tar.gz` & `tmp/space-invaders-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.58.tar", last modified: Fri Apr 28 16:55:27 2023, max compression
+gzip compressed data, was "space-invaders-0.1.59.tar", last modified: Fri Apr 28 23:05:32 2023, max compression
```

## Comparing `space-invaders-0.1.58.tar` & `space-invaders-0.1.59.tar`

### file list

```diff
@@ -1,63 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.414465 space-invaders-0.1.58/
--rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.58/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-04-28 16:55:27.414465 space-invaders-0.1.58/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 16:55:27.414465 space-invaders-0.1.58/setup.cfg
--rw-rw-rw-   0        0        0      597 2023-04-28 16:55:19.000000 space-invaders-0.1.58/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.379438 space-invaders-0.1.58/space-invaders/
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.381943 space-invaders-0.1.58/space-invaders/Fonts/
--rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.1.58/space-invaders/Fonts/AGENCYB.TTF
--rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.1.58/space-invaders/Fonts/AGENCYR.TTF
--rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.1.58/space-invaders/Fonts/Alien Invader Italic.ttf
--rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.1.58/space-invaders/Fonts/Alien Invader.ttf
--rw-rw-rw-   0        0        0     2116 2023-04-28 12:58:34.000000 space-invaders-0.1.58/space-invaders/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.393450 space-invaders-0.1.58/space-invaders/Sounds/
--rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.1.58/space-invaders/Sounds/122255__jivatma07__level_complete.wav
--rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.1.58/space-invaders/Sounds/156895__halgrimm__a-shot.wav
--rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.1.58/space-invaders/Sounds/18380__inferno__hvrl.wav
--rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.1.58/space-invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
--rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.1.58/space-invaders/Sounds/340452__zagi2__dondolan2-loop.wav
--rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.1.58/space-invaders/Sounds/353775__samueloak89__next-scene.mp3
--rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.1.58/space-invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
--rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.1.58/space-invaders/Sounds/565481__jakegwizdak__small-explosion.wav
--rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.1.58/space-invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
--rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.1.58/space-invaders/Sounds/648200__strangehorizon__glitch_blip.wav
--rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.1.58/space-invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.404956 space-invaders-0.1.58/space-invaders/Sprites/
--rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.1.58/space-invaders/Sprites/background.png
--rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.1.58/space-invaders/Sprites/default_enemy_gun.png
--rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.1.58/space-invaders/Sprites/default_enemy_projectile.png
--rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.1.58/space-invaders/Sprites/default_enemy_ship.png
--rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.1.58/space-invaders/Sprites/default_gun.png
--rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.1.58/space-invaders/Sprites/default_gun_pickup.png
--rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.1.58/space-invaders/Sprites/default_projectile.png
--rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.1.58/space-invaders/Sprites/default_ship.png
--rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.1.58/space-invaders/Sprites/explosion.png
--rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.1.58/space-invaders/Sprites/fire_rate_booster.png
--rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.1.58/space-invaders/Sprites/life.png
--rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.1.58/space-invaders/Sprites/medium_heal.png
--rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.1.58/space-invaders/Sprites/minigun.png
--rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.1.58/space-invaders/Sprites/minigun_pickup.png
--rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.1.58/space-invaders/Sprites/minigun_projectile.png
--rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.1.58/space-invaders/Sprites/repair.png
--rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.1.58/space-invaders/Sprites/rocket_gun.png
--rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.1.58/space-invaders/Sprites/rocket_gun_pickup.png
--rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.1.58/space-invaders/Sprites/rocket_projectile.png
--rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.1.58/space-invaders/Sprites/ship_explosion.png
--rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.1.58/space-invaders/Sprites/small_heal.png
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.405956 space-invaders-0.1.58/space-invaders/TestResults/
--rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.1.58/space-invaders/TestResults/flake8.txt
--rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.1.58/space-invaders/TestResults/pycodestyle.txt
--rw-rw-rw-   0        0        0        0 2023-04-28 16:51:05.000000 space-invaders-0.1.58/space-invaders/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.58/space-invaders/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.58/space-invaders/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.58/space-invaders/level.py
--rw-rw-rw-   0        0        0    16011 2023-04-28 16:50:54.000000 space-invaders-0.1.58/space-invaders/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.58/space-invaders/pickup.py
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.58/space-invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:55:27.413465 space-invaders-0.1.58/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 16:55:27.000000 space-invaders-0.1.58/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.902772 space-invaders-0.1.59/
+-rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.59/MANIFEST.in
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:05:32.902772 space-invaders-0.1.59/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:05:32.902772 space-invaders-0.1.59/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-28 23:05:29.000000 space-invaders-0.1.59/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.891235 space-invaders-0.1.59/space_invaders/
+-rw-rw-rw-   0        0        0        0 2023-04-28 16:51:05.000000 space-invaders-0.1.59/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.59/space_invaders/config.py
+-rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.59/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.59/space_invaders/level.py
+-rw-rw-rw-   0        0        0    15997 2023-04-28 22:47:17.000000 space-invaders-0.1.59/space_invaders/main.py
+-rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.59/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.59/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.901266 space-invaders-0.1.59/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       57 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.58/PKG-INFO` & `space-invaders-0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.58
+Version: 0.1.59
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.58/setup.py` & `space-invaders-0.1.59/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.58',
-    py_modules=['main'],
+    version='0.1.59',
+    py_modules=['entity', 'config', 'main', 'spaceship', 'level', 'pickup'],
     packages=find_packages(),
     install_requires=[
         'pygame',
         'shapely'
     ],
-    entry_points="""
-    [console_scripts]
-    space-invaders=main:start
-    """,
+    entry_points={
+        'console_scripts': [
+            'space-invaders=space_invaders.main:main'
+        ]
+    },
     author='Bódi Martin',
     author_email='bodimartin22@gmail.com',
     description='A cool space shooter rouge like game',
-    long_description=open('space-invaders/README.md').read(),
+    long_description=open('space_invaders/README.md').read(),
     long_description_content_type='text/markdown',
     include_package_data=True
 )
```

### Comparing `space-invaders-0.1.58/space-invaders/README.md` & `space-invaders-0.1.59/space_invaders.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: space-invaders
+Version: 0.1.59
+Summary: A cool space shooter rouge like game
+Author: Bódi Martin
+Author-email: bodimartin22@gmail.com
+Description-Content-Type: text/markdown
+
 # Space Invaders
 ## HOW TO INSTALL?  
 *use this command in the terminal to install the game*
 
     pip install space-invaders 
 
  
@@ -47,8 +55,8 @@
 
 ### FONTS
 - alien-invader-font:   https://www.dafont.com/alien-invader.font
 - agency-fb-font:  Builtin Windows Font
 <br>_(2023.04.28)_
 
 ### COPYRIGHT
-#### All other assets, code, everything else basically belongs to me™ based on the  © §42069 ¶1337 2023-infinity ®
+#### All other assets, code, everything else basically belongs to meâ„˘ based on the  Â© Â§42069 Â¶1337 2023-infinity Â®
```

### Comparing `space-invaders-0.1.58/space-invaders/config.py` & `space-invaders-0.1.59/space_invaders/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.58/space-invaders/entity.py` & `space-invaders-0.1.59/space_invaders/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.58/space-invaders/level.py` & `space-invaders-0.1.59/space_invaders/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.58/space-invaders/main.py` & `space-invaders-0.1.59/space_invaders/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,20 +302,19 @@
 
     pygame.display.update()
     pygame.time.wait(2000)
 
     return player, current_level
 
 
-def start():
+def main():
     print('STARTING GAME!')
 
 
 if __name__ == '__main__':
-    start()
     pygame.init()
     pygame.mixer.init()
     pygame.mixer.set_num_channels(CHANNEL_COUNT)
     LEVEL_OVER = False
     CAN_SWITCH_GUN = True
     RESET_CAN_SWITCH = USEREVENT + 2
     SPAWN_PICKUP = USEREVENT + 3
```

### Comparing `space-invaders-0.1.58/space-invaders/pickup.py` & `space-invaders-0.1.59/space_invaders/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.58/space-invaders/spaceship.py` & `space-invaders-0.1.59/space_invaders/spaceship.py`

 * *Files identical despite different names*

