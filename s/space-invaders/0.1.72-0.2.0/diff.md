# Comparing `tmp/space-invaders-0.1.72.tar.gz` & `tmp/space-invaders-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.72.tar", last modified: Sat Apr 29 01:33:36 2023, max compression
+gzip compressed data, was "space-invaders-0.2.0.tar", last modified: Sat Apr 29 19:55:48 2023, max compression
```

## Comparing `space-invaders-0.1.72.tar` & `space-invaders-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:36.049977 space-invaders-0.1.72/
--rw-rw-rw-   0        0        0      295 2023-04-29 00:00:41.000000 space-invaders-0.1.72/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-04-29 01:33:36.049977 space-invaders-0.1.72/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 01:33:36.050976 space-invaders-0.1.72/setup.cfg
--rw-rw-rw-   0        0        0      619 2023-04-29 01:33:23.000000 space-invaders-0.1.72/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:35.919891 space-invaders-0.1.72/space_invaders/
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:35.942910 space-invaders-0.1.72/space_invaders/Fonts/
--rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.1.72/space_invaders/Fonts/AGENCYB.TTF
--rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.1.72/space_invaders/Fonts/AGENCYR.TTF
--rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.1.72/space_invaders/Fonts/Alien Invader Italic.ttf
--rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.1.72/space_invaders/Fonts/Alien Invader.ttf
--rw-rw-rw-   0        0        0     2116 2023-04-29 01:33:08.000000 space-invaders-0.1.72/space_invaders/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:36.004948 space-invaders-0.1.72/space_invaders/Sounds/
--rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.1.72/space_invaders/Sounds/122255__jivatma07__level_complete.wav
--rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.1.72/space_invaders/Sounds/156895__halgrimm__a-shot.wav
--rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.1.72/space_invaders/Sounds/18380__inferno__hvrl.wav
--rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.1.72/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
--rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.1.72/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
--rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.1.72/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
--rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.1.72/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
--rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.1.72/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
--rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.1.72/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
--rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.1.72/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
--rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.1.72/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:36.045976 space-invaders-0.1.72/space_invaders/Sprites/
--rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.1.72/space_invaders/Sprites/background.png
--rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.1.72/space_invaders/Sprites/default_enemy_gun.png
--rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.1.72/space_invaders/Sprites/default_enemy_projectile.png
--rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.1.72/space_invaders/Sprites/default_enemy_ship.png
--rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.1.72/space_invaders/Sprites/default_gun.png
--rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.1.72/space_invaders/Sprites/default_gun_pickup.png
--rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.1.72/space_invaders/Sprites/default_projectile.png
--rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.1.72/space_invaders/Sprites/default_ship.png
--rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.1.72/space_invaders/Sprites/explosion.png
--rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.1.72/space_invaders/Sprites/fire_rate_booster.png
--rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.1.72/space_invaders/Sprites/life.png
--rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.1.72/space_invaders/Sprites/medium_heal.png
--rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.1.72/space_invaders/Sprites/minigun.png
--rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.1.72/space_invaders/Sprites/minigun_pickup.png
--rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.1.72/space_invaders/Sprites/minigun_projectile.png
--rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.1.72/space_invaders/Sprites/repair.png
--rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.1.72/space_invaders/Sprites/rocket_gun.png
--rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.1.72/space_invaders/Sprites/rocket_gun_pickup.png
--rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.1.72/space_invaders/Sprites/rocket_projectile.png
--rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.1.72/space_invaders/Sprites/ship_explosion.png
--rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.1.72/space_invaders/Sprites/small_heal.png
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:36.048977 space-invaders-0.1.72/space_invaders/TestResults/
--rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.1.72/space_invaders/TestResults/flake8.txt
--rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.1.72/space_invaders/TestResults/pycodestyle.txt
--rw-rw-rw-   0        0        0      154 2023-04-29 01:06:13.000000 space-invaders-0.1.72/space_invaders/__entrypoint__.py
--rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.1.72/space_invaders/__init__.py
--rw-rw-rw-   0        0        0     3983 2023-04-29 00:42:23.000000 space-invaders-0.1.72/space_invaders/config.py
--rw-rw-rw-   0        0        0     3465 2023-04-28 23:45:55.000000 space-invaders-0.1.72/space_invaders/entity.py
--rw-rw-rw-   0        0        0    17426 2023-04-29 01:32:22.000000 space-invaders-0.1.72/space_invaders/level.py
--rw-rw-rw-   0        0        0    15737 2023-04-29 01:33:03.000000 space-invaders-0.1.72/space_invaders/main.py
--rw-rw-rw-   0        0        0     3126 2023-04-29 00:40:26.000000 space-invaders-0.1.72/space_invaders/pickup.py
--rw-rw-rw-   0        0        0    11271 2023-04-29 00:44:42.000000 space-invaders-0.1.72/space_invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-29 01:33:35.927641 space-invaders-0.1.72/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2268 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 01:33:35.000000 space-invaders-0.1.72/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.883988 space-invaders-0.2.0/
+-rw-rw-rw-   0        0        0      295 2023-04-29 00:00:41.000000 space-invaders-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2339 2023-04-29 19:55:48.882988 space-invaders-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 19:55:48.883988 space-invaders-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-04-29 19:55:41.000000 space-invaders-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.840769 space-invaders-0.2.0/space_invaders/
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.851783 space-invaders-0.2.0/space_invaders/Fonts/
+-rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.2.0/space_invaders/Fonts/AGENCYB.TTF
+-rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.2.0/space_invaders/Fonts/AGENCYR.TTF
+-rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.2.0/space_invaders/Fonts/Alien Invader Italic.ttf
+-rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.2.0/space_invaders/Fonts/Alien Invader.ttf
+-rw-rw-rw-   0        0        0     2116 2023-04-29 01:33:08.000000 space-invaders-0.2.0/space_invaders/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.864823 space-invaders-0.2.0/space_invaders/Sounds/
+-rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.2.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav
+-rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.2.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav
+-rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.2.0/space_invaders/Sounds/18380__inferno__hvrl.wav
+-rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.2.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
+-rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.2.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
+-rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.2.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
+-rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.2.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
+-rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.2.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
+-rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.2.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
+-rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.2.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
+-rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.2.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.878988 space-invaders-0.2.0/space_invaders/Sprites/
+-rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.2.0/space_invaders/Sprites/background.png
+-rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_gun.png
+-rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_projectile.png
+-rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_ship.png
+-rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.2.0/space_invaders/Sprites/default_gun.png
+-rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.2.0/space_invaders/Sprites/default_gun_pickup.png
+-rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.2.0/space_invaders/Sprites/default_projectile.png
+-rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.2.0/space_invaders/Sprites/default_ship.png
+-rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.2.0/space_invaders/Sprites/explosion.png
+-rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.2.0/space_invaders/Sprites/fire_rate_booster.png
+-rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.2.0/space_invaders/Sprites/life.png
+-rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.2.0/space_invaders/Sprites/medium_heal.png
+-rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun.png
+-rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun_pickup.png
+-rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun_projectile.png
+-rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.2.0/space_invaders/Sprites/repair.png
+-rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_gun.png
+-rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_gun_pickup.png
+-rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_projectile.png
+-rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.2.0/space_invaders/Sprites/ship_explosion.png
+-rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.2.0/space_invaders/Sprites/small_heal.png
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.879988 space-invaders-0.2.0/space_invaders/TestResults/
+-rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.2.0/space_invaders/TestResults/flake8.txt
+-rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.2.0/space_invaders/TestResults/pycodestyle.txt
+-rw-rw-rw-   0        0        0      225 2023-04-29 19:24:05.000000 space-invaders-0.2.0/space_invaders/__entrypoint__.py
+-rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.2.0/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     4006 2023-04-29 19:22:53.000000 space-invaders-0.2.0/space_invaders/config.py
+-rw-rw-rw-   0        0        0     3516 2023-04-29 19:47:34.000000 space-invaders-0.2.0/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    17495 2023-04-29 17:30:28.000000 space-invaders-0.2.0/space_invaders/level.py
+-rw-rw-rw-   0        0        0    16049 2023-04-29 19:33:35.000000 space-invaders-0.2.0/space_invaders/main.py
+-rw-rw-rw-   0        0        0     3296 2023-04-29 19:33:02.000000 space-invaders-0.2.0/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0    11389 2023-04-29 14:27:17.000000 space-invaders-0.2.0/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.882988 space-invaders-0.2.0/space_invaders/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:49:16.000000 space-invaders-0.2.0/space_invaders/tests/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-04-29 14:27:17.000000 space-invaders-0.2.0/space_invaders/tests/test_entity.py
+-rw-rw-rw-   0        0        0     2704 2023-04-29 17:32:02.000000 space-invaders-0.2.0/space_invaders/tests/test_level.py
+-rw-rw-rw-   0        0        0     2031 2023-04-29 19:47:22.000000 space-invaders-0.2.0/space_invaders/tests/test_main.py
+-rw-rw-rw-   0        0        0     1494 2023-04-29 15:11:06.000000 space-invaders-0.2.0/space_invaders/tests/test_pickup.py
+-rw-rw-rw-   0        0        0     3512 2023-04-29 14:40:40.000000 space-invaders-0.2.0/space_invaders/tests/test_spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.849784 space-invaders-0.2.0/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2339 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2481 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.72/PKG-INFO` & `space-invaders-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.72
+Version: 0.2.0
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.72/setup.py` & `space-invaders-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.72',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'pygame',
         'shapely'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `space-invaders-0.1.72/space_invaders/Fonts/AGENCYB.TTF` & `space-invaders-0.2.0/space_invaders/Fonts/AGENCYB.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Fonts/AGENCYR.TTF` & `space-invaders-0.2.0/space_invaders/Fonts/AGENCYR.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Fonts/Alien Invader Italic.ttf` & `space-invaders-0.2.0/space_invaders/Fonts/Alien Invader Italic.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Fonts/Alien Invader.ttf` & `space-invaders-0.2.0/space_invaders/Fonts/Alien Invader.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/README.md` & `space-invaders-0.2.0/space_invaders/README.md`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/122255__jivatma07__level_complete.wav` & `space-invaders-0.2.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/156895__halgrimm__a-shot.wav` & `space-invaders-0.2.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/18380__inferno__hvrl.wav` & `space-invaders-0.2.0/space_invaders/Sounds/18380__inferno__hvrl.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav` & `space-invaders-0.2.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav` & `space-invaders-0.2.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/353775__samueloak89__next-scene.mp3` & `space-invaders-0.2.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg` & `space-invaders-0.2.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav` & `space-invaders-0.2.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav` & `space-invaders-0.2.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav` & `space-invaders-0.2.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav` & `space-invaders-0.2.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/background.png` & `space-invaders-0.2.0/space_invaders/Sprites/background.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_enemy_gun.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_enemy_projectile.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_enemy_ship.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_gun.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_gun_pickup.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_projectile.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/default_ship.png` & `space-invaders-0.2.0/space_invaders/Sprites/default_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/explosion.png` & `space-invaders-0.2.0/space_invaders/Sprites/explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/fire_rate_booster.png` & `space-invaders-0.2.0/space_invaders/Sprites/fire_rate_booster.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/life.png` & `space-invaders-0.2.0/space_invaders/Sprites/life.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/medium_heal.png` & `space-invaders-0.2.0/space_invaders/Sprites/medium_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/minigun.png` & `space-invaders-0.2.0/space_invaders/Sprites/minigun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/minigun_pickup.png` & `space-invaders-0.2.0/space_invaders/Sprites/minigun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/minigun_projectile.png` & `space-invaders-0.2.0/space_invaders/Sprites/minigun_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/repair.png` & `space-invaders-0.2.0/space_invaders/Sprites/repair.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/rocket_gun.png` & `space-invaders-0.2.0/space_invaders/Sprites/rocket_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/rocket_gun_pickup.png` & `space-invaders-0.2.0/space_invaders/Sprites/rocket_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/rocket_projectile.png` & `space-invaders-0.2.0/space_invaders/Sprites/rocket_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/ship_explosion.png` & `space-invaders-0.2.0/space_invaders/Sprites/ship_explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/Sprites/small_heal.png` & `space-invaders-0.2.0/space_invaders/Sprites/small_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.72/space_invaders/config.py` & `space-invaders-0.2.0/space_invaders/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
 EXPLOSION_DURATION = 4
 RESET_SWITCH_DELAY = 200
 PICKUP_SPEED = 5
 PICKUP_SPAWN_INTERVAL = (4, 8)
 score = 0
 
+LAUNCH_GAME = False
+
 SHOW_HIT_BOXES = False
 WINDOW_WIDTH = 1400
 WINDOW_HEIGHT = 950
 CAPTION = "Space Invaders"
 BACKGROUND_IMAGE = get_path("Sprites", "background.png")
```

### Comparing `space-invaders-0.1.72/space_invaders/entity.py` & `space-invaders-0.2.0/space_invaders/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 
     @property
     def lives(self):
         return self._lives
 
     def add_life(self, amount=1):
         if self.alive():
-            self._lives += amount
+            self._lives = max(self._lives, self._lives + amount)
 
     def heal(self, amount):
-        if self.alive():
-            self._hp = min(self._hp + abs(amount), self._max_hp)
+        if self.alive() and amount > 0:
+            self._hp = min(self._hp + amount, self._max_hp)
 
     def take_damage(self, amount):
-        if not self.alive() or not self.in_bounds():
+        if not self.alive() or not self.in_bounds() or amount <= 0:
             return
 
-        self._hp = max(0, self._hp - abs(amount))
+        self._hp = max(0, self._hp - amount)
 
         if self._hp == 0:
             self._lives -= 1
             if self._lives == 0:
                 self.die()
             else:
                 self._hp = self._max_hp
```

### Comparing `space-invaders-0.1.72/space_invaders/level.py` & `space-invaders-0.2.0/space_invaders/level.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,18 @@
                 self._phases.remove(self._phases[0])
             else:
                 self._phases[0].execute_all_actions()
 
     def is_complete(self):
         return len(self._phases) == 0
 
+    @property
+    def phases(self):
+        return self._phases
+
 
 def shoot_actions(duration_in_seconds=1/60):
     return [("shoot", [])] * int(60 * duration_in_seconds)
 
 
 def go_towards_actions(position, target, speed, fire=False):
     actions = []
```

### Comparing `space-invaders-0.1.72/space_invaders/main.py` & `space-invaders-0.2.0/space_invaders/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import random
 import pygame.display
 from pygame.locals import K_w, K_a, K_s, K_d, K_SPACE, K_LSHIFT, USEREVENT
 from shapely.geometry import Polygon
 from space_invaders.entity import Entity
 from space_invaders.pickup import PICKUP_LIFE, PICKUP_MINIGUN, PICKUP_REPAIR, PICKUP_ROCKET_GUN, PICKUP_SMALL_HEAL, \
-    PICKUP_MEDIUM_HEAL, PICKUP_FIRE_RATE_BOOSTER, Pickup, RESET_FIRE_RATE
+    PICKUP_MEDIUM_HEAL, PICKUP_FIRE_RATE_BOOSTER, Pickup, RESET_FIRE_RATE, PICKUP_DEFAULT_GUN
 from space_invaders.spaceship import ROCKET_GUN, MINIGUN
 from space_invaders.config import WINDOW_WIDTH, WINDOW_HEIGHT, play_sound, PICKUP_SPEED, PICKUP_SPAWN_INTERVAL, \
     SOUND_CREDITS_DATA, SOUND_EXPLOSION_DATA, SOUND_MAIN_THEME_DATA, SOUND_DEFEAT_DATA, SOUND_VICTORY_DATA, \
     SOUND_ENEMY_HIT_DATA, SOUND_PLAYER_HIT_DATA, SHOW_HIT_BOXES, get_credits_text, EXPLOSION_DURATION, \
     RESET_SWITCH_DELAY, FONT_CREDITS_TEXT_DATA, FONT_CREDITS_TITLE_DATA, FONT86_DATA, FONT15_DATA, FONT152_DATA, \
-    FONT25_DATA, FONT36_DATA, CHANNEL_COUNT, CAPTION, BACKGROUND_IMAGE, SOUND_PICKUP_DATA
+    FONT25_DATA, FONT36_DATA, CHANNEL_COUNT, CAPTION, BACKGROUND_IMAGE, SOUND_PICKUP_DATA, LAUNCH_GAME
 import space_invaders.config as config
 import space_invaders.level as level
 
 
 def update_pickups():
     global pickups, window, player
     player_poly = Polygon(player.hit_box)
@@ -69,15 +69,15 @@
 def get_pickup_image_by_gun(gun):
     match gun.type:
         case "rocket":
             return PICKUP_ROCKET_GUN.image
         case "minigun":
             return PICKUP_MINIGUN.image
         case _:
-            return pygame.image.load(config.get_path("Sprites", "default_gun_pickup.png"))
+            return PICKUP_DEFAULT_GUN.image
 
 
 def display_hud():
     global player, enemies, window
 
     # Enemy healths
     for enemy_ in enemies:
@@ -298,106 +298,106 @@
 
     pygame.display.update()
     pygame.time.wait(2000)
 
     return player, current_level
 
 
-# MAIN CODE
-pygame.init()
-pygame.mixer.init()
-pygame.mixer.set_num_channels(CHANNEL_COUNT)
-LEVEL_OVER = False
-CAN_SWITCH_GUN = True
-RESET_CAN_SWITCH = USEREVENT + 2
-SPAWN_PICKUP = USEREVENT + 3
-LEVELS = [level.LEVEL_ONE, level.LEVEL_TWO, level.LEVEL_THREE, level.LEVEL_FOUR, level.LEVEL_FIVE, level.LEVEL_SIX]
-level_index = 0
-
-pygame.display.set_caption(CAPTION)
-window = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
-
-FONT_CREDITS_TEXT = pygame.font.Font(*FONT_CREDITS_TEXT_DATA)
-FONT_CREDITS_TITLE = pygame.font.Font(*FONT_CREDITS_TITLE_DATA)
-FONT152 = pygame.font.Font(*FONT152_DATA)
-FONT86 = pygame.font.Font(*FONT86_DATA)
-FONT36 = pygame.font.Font(*FONT36_DATA)
-FONT25 = pygame.font.Font(*FONT25_DATA)
-FONT15 = pygame.font.Font(*FONT15_DATA)
-background_img = pygame.image.load(BACKGROUND_IMAGE).convert()
-background_img = pygame.transform.scale(background_img, (WINDOW_WIDTH, WINDOW_HEIGHT))
-
-clock = pygame.time.Clock()
-play_sound(SOUND_MAIN_THEME_DATA, -1)
-
-# Declaration of global arrays
-entities = enemies = pickups = explosions = []
-
-current_level = player = None
-player, current_level = load_level(LEVELS[0])
-if player is not None and current_level is not None:
-    spawn_at_random_interval()
-
-    while True:
-        if LEVEL_OVER:
-            level_over()
-
-        for event in pygame.event.get():
-            if event.type == pygame.QUIT:
-                pygame.quit()
-                exit()
-            elif event.type == SPAWN_PICKUP:
-                spawn_pickup()
-                spawn_at_random_interval()
-            elif event.type == RESET_FIRE_RATE:
-                Pickup.action_reset_fire_rate(player)
-            elif event.type == RESET_CAN_SWITCH:
-                CAN_SWITCH_GUN = True
-
-        handle_player_input(player, WINDOW_WIDTH, WINDOW_HEIGHT)
-        current_level.execute_phase()
-        check_entity_collision(player, enemies)
-
-        if player.alive():
-            explosions.extend(player.check_projectile_hit(enemies))
-
-            for enemy in enemies:
-                explosions.extend(enemy.check_projectile_hit([player]))
-
-                if not enemy.alive():
-                    play_sound(SOUND_EXPLOSION_DATA, 0)
-                    config.score += 500
+if LAUNCH_GAME:
+    pygame.init()
+    pygame.mixer.init()
+    pygame.mixer.set_num_channels(CHANNEL_COUNT)
+    LEVEL_OVER = False
+    CAN_SWITCH_GUN = True
+    RESET_CAN_SWITCH = USEREVENT + 2
+    SPAWN_PICKUP = USEREVENT + 3
+    LEVELS = [level.LEVEL_ONE, level.LEVEL_TWO, level.LEVEL_THREE, level.LEVEL_FOUR, level.LEVEL_FIVE, level.LEVEL_SIX]
+    level_index = 0
+
+    pygame.display.set_caption(CAPTION)
+    window = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
+
+    FONT_CREDITS_TEXT = pygame.font.Font(*FONT_CREDITS_TEXT_DATA)
+    FONT_CREDITS_TITLE = pygame.font.Font(*FONT_CREDITS_TITLE_DATA)
+    FONT152 = pygame.font.Font(*FONT152_DATA)
+    FONT86 = pygame.font.Font(*FONT86_DATA)
+    FONT36 = pygame.font.Font(*FONT36_DATA)
+    FONT25 = pygame.font.Font(*FONT25_DATA)
+    FONT15 = pygame.font.Font(*FONT15_DATA)
+    background_img = pygame.image.load(BACKGROUND_IMAGE).convert()
+    background_img = pygame.transform.scale(background_img, (WINDOW_WIDTH, WINDOW_HEIGHT))
+
+    clock = pygame.time.Clock()
+    play_sound(SOUND_MAIN_THEME_DATA, -1)
+
+    # Declaration of global arrays
+    entities = enemies = pickups = explosions = []
+
+    current_level = player = None
+    player, current_level = load_level(LEVELS[0])
+    if player is not None and current_level is not None:
+        spawn_at_random_interval()
+
+        while True:
+            if LEVEL_OVER:
+                level_over()
+
+            for event in pygame.event.get():
+                if event.type == pygame.QUIT:
+                    pygame.quit()
+                    exit()
+                elif event.type == SPAWN_PICKUP:
+                    spawn_pickup()
+                    spawn_at_random_interval()
+                elif event.type == RESET_FIRE_RATE:
+                    Pickup.action_reset_fire_rate(player)
+                elif event.type == RESET_CAN_SWITCH:
+                    CAN_SWITCH_GUN = True
+
+            handle_player_input(player, WINDOW_WIDTH, WINDOW_HEIGHT)
+            current_level.execute_phase()
+            check_entity_collision(player, enemies)
+
+            if player.alive():
+                explosions.extend(player.check_projectile_hit(enemies))
+
+                for enemy in enemies:
+                    explosions.extend(enemy.check_projectile_hit([player]))
+
+                    if not enemy.alive():
+                        play_sound(SOUND_EXPLOSION_DATA, 0)
+                        config.score += 500
+
+                        explosions.append([pygame.image.load(config.get_path("Sprites", "ship_explosion.png")),
+                                           enemy.image_rect.center, EXPLOSION_DURATION])
+
+                        enemies.remove(enemy)
+                        entities.remove(enemy)
+
+            # render everything
+            window.blit(background_img, (0, 0))
+            for entity in entities:
+                entity.render(window, SHOW_HIT_BOXES)
+            update_pickups()
+            for explosion in explosions:
+                if explosion[2] == 0:
+                    explosions.remove(explosion)
+                else:
+                    explosion_image = explosion[0]
+                    explosion_image = pygame.transform.scale(explosion_image, (explosion_image.get_size()[0] * 1.15,
+                                                                               explosion_image.get_size()[1] * 1.15))
+                    explosion[0] = explosion_image
+
+                    window.blit(explosion_image, (explosion[1][0] - explosion_image.get_rect().width // 2,
+                                                  explosion[1][1] - explosion_image.get_rect().height // 2))
+                    explosion[2] -= 1
+            display_hud()
 
+            if not player.alive() or current_level.is_complete():
+                if not player.alive():
                     explosions.append([pygame.image.load(config.get_path("Sprites", "ship_explosion.png")),
-                                       enemy.image_rect.center, EXPLOSION_DURATION])
+                                       player.image_rect.center, EXPLOSION_DURATION])
 
-                    enemies.remove(enemy)
-                    entities.remove(enemy)
+                LEVEL_OVER = True
 
-        # render everything
-        window.blit(background_img, (0, 0))
-        for entity in entities:
-            entity.render(window, SHOW_HIT_BOXES)
-        update_pickups()
-        for explosion in explosions:
-            if explosion[2] == 0:
-                explosions.remove(explosion)
-            else:
-                explosion_image = explosion[0]
-                explosion_image = pygame.transform.scale(explosion_image, (explosion_image.get_size()[0] * 1.15,
-                                                                           explosion_image.get_size()[1] * 1.15))
-                explosion[0] = explosion_image
-
-                window.blit(explosion_image, (explosion[1][0] - explosion_image.get_rect().width // 2,
-                                              explosion[1][1] - explosion_image.get_rect().height // 2))
-                explosion[2] -= 1
-        display_hud()
-
-        if not player.alive() or current_level.is_complete():
-            if not player.alive():
-                explosions.append([pygame.image.load(config.get_path("Sprites", "ship_explosion.png")),
-                                   player.image_rect.center, EXPLOSION_DURATION])
-
-            LEVEL_OVER = True
-
-        pygame.display.update()
-        clock.tick(60)
+            pygame.display.update()
+            clock.tick(60)
```

### Comparing `space-invaders-0.1.72/space_invaders/pickup.py` & `space-invaders-0.2.0/space_invaders/pickup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import pygame
 from pygame.locals import USEREVENT
 import space_invaders.spaceship as spaceship
 import space_invaders.config as config
 
 
 class Pickup(pygame.sprite.Sprite):
-    def __init__(self, action, **kwargs):   # image=None, image_file="", *args
+    def __init__(self, action, args, image=None, image_file=""):
         super().__init__()
 
-        if kwargs.get('image', None) is not None:
-            self._image = kwargs['image']
+        if image is not None:
+            self._image = image
         else:
-            self._image = pygame.image.load(kwargs['image_file'])
+            self._image = pygame.image.load(image_file)
 
         self._rect = self._image.get_rect()
         self._action = action
-        self._args = kwargs['args']
+        self._args = args
 
     def new_pickup(self):
         return Pickup(action=self._action, args=self._args, image=copy.copy(self._image))
 
     def move(self, vec):
         self._rect.center = (self._rect.center[0] + vec[0], self._rect.center[1] + vec[1])
 
@@ -87,14 +87,20 @@
     args=[5]
 )
 PICKUP_MEDIUM_HEAL = Pickup(
     action=Pickup.action_heal,
     image_file=config.get_path("Sprites", "medium_heal.png"),
     args=[10]
 )
+# Only for technical purposes, it is not spawned at all tho
+PICKUP_DEFAULT_GUN = Pickup(
+    action=Pickup.action_give_gun,
+    image_file=config.get_path("Sprites", "default_gun_pickup.png"),
+    args=[spaceship.DEFAULT_GUN]
+)
 PICKUP_MINIGUN = Pickup(
     action=Pickup.action_give_gun,
     image_file=config.get_path("Sprites", "minigun_pickup.png"),
     args=[spaceship.MINIGUN]
 )
 PICKUP_ROCKET_GUN = Pickup(
     action=Pickup.action_give_gun,
```

### Comparing `space-invaders-0.1.72/space_invaders/spaceship.py` & `space-invaders-0.2.0/space_invaders/spaceship.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,18 @@
         return self._image
 
     @property
     def type(self):
         return self._type
 
     @property
+    def rect(self):
+        return self._rect
+
+    @property
     def ammo(self):
         return self._ammo
 
     def add_ammo(self, amount):
         self._ammo += amount
 
     def shoot(self, fire_rate_multiplier):
@@ -242,15 +246,15 @@
 
     def move_forward(self, enemy):
         diff = self._speed if enemy else -self._speed
         self._hit_box.center = (self._hit_box.center[0], self._hit_box.center[1] + diff)
         self._image_rect.center = (self._image_rect.center[0], self._image_rect.center[1] + diff)
 
     def check_if_out(self):
-        return self._hit_box.top < -100
+        return self._hit_box.bottom < -100 or self._hit_box.top > config.WINDOW_HEIGHT + 100
 
 
 def get_sound_by_projectile(projectile):
     global DEFAULT_PROJECTILE, DEFAULT_ENEMY_PROJECTILE, MINIGUN_PROJECTILE, ROCKET_PROJECTILE
     if projectile in (DEFAULT_PROJECTILE, DEFAULT_ENEMY_PROJECTILE):
         return config.SOUND_DEFAULT_GUN_DATA
     if projectile == MINIGUN_PROJECTILE:
```

### Comparing `space-invaders-0.1.72/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.2.0/space_invaders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.72
+Version: 0.2.0
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.72/space_invaders.egg-info/SOURCES.txt` & `space-invaders-0.2.0/space_invaders.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -48,8 +48,14 @@
 space_invaders/Sprites/repair.png
 space_invaders/Sprites/rocket_gun.png
 space_invaders/Sprites/rocket_gun_pickup.png
 space_invaders/Sprites/rocket_projectile.png
 space_invaders/Sprites/ship_explosion.png
 space_invaders/Sprites/small_heal.png
 space_invaders/TestResults/flake8.txt
-space_invaders/TestResults/pycodestyle.txt
+space_invaders/TestResults/pycodestyle.txt
+space_invaders/tests/__init__.py
+space_invaders/tests/test_entity.py
+space_invaders/tests/test_level.py
+space_invaders/tests/test_main.py
+space_invaders/tests/test_pickup.py
+space_invaders/tests/test_spaceship.py
```

