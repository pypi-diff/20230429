# Comparing `tmp/gather-scrobble-0.0.3.tar.gz` & `tmp/gather-scrobble-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gather-scrobble-0.0.3.tar", last modified: Sat Apr 29 02:01:00 2023, max compression
+gzip compressed data, was "gather-scrobble-0.0.5.tar", last modified: Sat Apr 29 15:48:19 2023, max compression
```

## Comparing `gather-scrobble-0.0.3.tar` & `gather-scrobble-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 02:01:00.751914 gather-scrobble-0.0.3/
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1089 2023-03-25 18:58:51.000000 gather-scrobble-0.0.3/LICENSE
--rw-r--r--   0 pyand     (1000) pyand     (1000)     7419 2023-04-29 02:01:00.751914 gather-scrobble-0.0.3/PKG-INFO
--rw-r--r--   0 pyand     (1000) pyand     (1000)     6003 2023-03-26 20:28:46.000000 gather-scrobble-0.0.3/README.md
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 02:01:00.750914 gather-scrobble-0.0.3/gather_scrobble/
--rw-r--r--   0 pyand     (1000) pyand     (1000)      100 2023-04-29 02:00:26.000000 gather-scrobble-0.0.3/gather_scrobble/__init__.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1897 2023-04-29 02:00:26.000000 gather-scrobble-0.0.3/gather_scrobble/cli.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     5001 2023-04-29 01:55:05.000000 gather-scrobble-0.0.3/gather_scrobble/config.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)      455 2023-03-25 22:09:58.000000 gather-scrobble-0.0.3/gather_scrobble/info.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     4857 2023-03-26 19:49:44.000000 gather-scrobble-0.0.3/gather_scrobble/scrobble.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1591 2023-03-26 20:24:35.000000 gather-scrobble-0.0.3/gather_scrobble/test.py
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 02:01:00.751914 gather-scrobble-0.0.3/gather_scrobble.egg-info/
--rw-r--r--   0 pyand     (1000) pyand     (1000)     7419 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/PKG-INFO
--rw-r--r--   0 pyand     (1000) pyand     (1000)      468 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/SOURCES.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/dependency_links.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       61 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/entry_points.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/not-zip-safe
--rw-r--r--   0 pyand     (1000) pyand     (1000)      117 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/requires.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       16 2023-04-29 02:01:00.000000 gather-scrobble-0.0.3/gather_scrobble.egg-info/top_level.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       62 2023-03-25 18:58:51.000000 gather-scrobble-0.0.3/pyproject.toml
--rw-r--r--   0 pyand     (1000) pyand     (1000)       38 2023-04-29 02:01:00.751914 gather-scrobble-0.0.3/setup.cfg
--rwxr-xr-x   0 pyand     (1000) pyand     (1000)     2949 2023-03-26 20:54:05.000000 gather-scrobble-0.0.3/setup.py
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 15:48:19.226252 gather-scrobble-0.0.5/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1089 2023-03-25 18:58:51.000000 gather-scrobble-0.0.5/LICENSE
+-rw-r--r--   0 pyand     (1000) pyand     (1000)    10541 2023-04-29 15:48:19.226252 gather-scrobble-0.0.5/PKG-INFO
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     8878 2023-04-29 15:48:05.000000 gather-scrobble-0.0.5/README.md
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 15:48:19.225252 gather-scrobble-0.0.5/gather_scrobble/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      100 2023-04-29 15:48:05.000000 gather-scrobble-0.0.5/gather_scrobble/__init__.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1967 2023-04-29 15:48:05.000000 gather-scrobble-0.0.5/gather_scrobble/cli.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     5576 2023-04-29 15:31:55.000000 gather-scrobble-0.0.5/gather_scrobble/config.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      455 2023-03-25 22:09:58.000000 gather-scrobble-0.0.5/gather_scrobble/info.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     5031 2023-04-29 15:35:56.000000 gather-scrobble-0.0.5/gather_scrobble/scrobble.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1591 2023-04-29 14:26:39.000000 gather-scrobble-0.0.5/gather_scrobble/test.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      344 2023-04-29 15:28:29.000000 gather-scrobble-0.0.5/gather_scrobble/utils.py
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 15:48:19.226252 gather-scrobble-0.0.5/gather_scrobble.egg-info/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)    10541 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/PKG-INFO
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      493 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/SOURCES.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/dependency_links.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       61 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/entry_points.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/not-zip-safe
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      143 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/requires.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       16 2023-04-29 15:48:19.000000 gather-scrobble-0.0.5/gather_scrobble.egg-info/top_level.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       62 2023-03-25 18:58:51.000000 gather-scrobble-0.0.5/pyproject.toml
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       38 2023-04-29 15:48:19.226252 gather-scrobble-0.0.5/setup.cfg
+-rwxr-xr-x   0 pyand     (1000) pyand     (1000)     3032 2023-04-29 03:56:29.000000 gather-scrobble-0.0.5/setup.py
```

### Comparing `gather-scrobble-0.0.3/LICENSE` & `gather-scrobble-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gather-scrobble-0.0.3/gather_scrobble/cli.py` & `gather-scrobble-0.0.5/gather_scrobble/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 from contextlib import suppress
 
 from docopt import docopt
 
+from gather_scrobble.config import logger
 from gather_scrobble.info import show_info
 from gather_scrobble.scrobble import start
 from gather_scrobble.test import test_configuration
 
 
 def main():
-    """Gather Scrobble v0.0.3
+    """Gather Scrobble v0.0.5
     Usage:
         gather-scrobble start <space_id> [--source SOURCE] [--emojis EMOJIS]
         gather-scrobble info
         gather-scrobble test <space_id>
 
     Arguments:
         <space_id>          Gather space id.
@@ -27,24 +28,25 @@
                             the priority: lastfm -> spotify [default: any]
         -e --emojis EMOJIS  It is possible to customize the emojis, by setting
                             the list of emojis that will be chosen randomly,
                             and also you don't like emojis, you can set an
                             empty string here. [default: 🎼🎵🎶🎧📻🎷🎸🎹]
 
     """
-    arguments = docopt(main.__doc__ or "", version="Gather Scrobble 0.0.3")
+    arguments = docopt(main.__doc__ or "", version="Gather Scrobble 0.0.5")
     if arguments["start"]:
         if arguments["--source"] not in ["lastfm", "spotify", "any"]:
             raise Exception(f"Invalid source: {arguments['--source']}")
         with suppress(KeyboardInterrupt):
             asyncio.get_event_loop().run_until_complete(
                 start(
                     arguments["<space_id>"],
                     arguments["--source"],
                     arguments["--emojis"],
                 )
             )
+        logger.debug("bye")
         print("bye")
     if arguments["info"]:
         show_info()
     if arguments["test"]:
         test_configuration(arguments["<space_id>"])
```

### Comparing `gather-scrobble-0.0.3/gather_scrobble/config.py` & `gather-scrobble-0.0.5/gather_scrobble/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+import logging
 import os
 import platform
 from pathlib import Path
 from typing import Optional, cast
 
 import keyring
 import pylast
 import spotipy
-from decouple import config
+from decouple import AutoConfig
 from spotipy.cache_handler import CacheFileHandler
 from spotipy.oauth2 import SpotifyOAuth
 
+from gather_scrobble.utils import get_logger
+
+config = AutoConfig(os.getcwd())  # search for settings in the current dir
+USE_CRYPTFILE = config("USE_CRYPTFILE", cast=bool, default=False)
 CONFIG_FOLDER = "gather-scrobble"
 
+logger = get_logger(
+    "gather-scrobble", logging.DEBUG if USE_CRYPTFILE else logging.INFO
+)
+
 
 class Credentials:
     def __init__(
         self,
         gather_api_key: str,
         lastfm_api_key: Optional[str],
         lastfm_api_secret: Optional[str],
@@ -56,14 +65,20 @@
 def _get_config_value(var_name: str) -> Optional[str]:
     keyring_value = keyring.get_password("gather-scrobble", var_name)
     env_var = config(var_name, default=None)
     return keyring_value or cast(Optional[str], env_var)
 
 
 def get_credentials():
+    if USE_CRYPTFILE:
+        from keyrings.cryptfile.cryptfile import CryptFileKeyring
+
+        kr = CryptFileKeyring()
+        kr.keyring_key = config("KEYRING_CRYPTFILE_PASSWORD", default="secret")
+        keyring.set_keyring(kr)
     gather_api_key = _get_config_value("GATHER_API_KEY")
     if gather_api_key is None or str(gather_api_key).strip() == "":
         raise Exception("Missing 'GATHER_API_KEY' value")
     lastfm_api_key = _get_config_value("LASTFM_API_KEY")
     lastfm_api_secret = _get_config_value("LASTFM_API_SECRET")
     lastfm_username = _get_config_value("LASTFM_USERNAME")
     spotify_client_id = _get_config_value("SPOTIFY_CLIENT_ID")
@@ -144,9 +159,10 @@
 
     auth_manager = SpotifyOAuth(
         credentials.spotify_client_id,
         credentials.spotify_client_secret,
         credentials.spotify_client_redirect_uri,
         scope=["user-read-currently-playing", "user-read-playback-state"],
         cache_handler=CustomCacheHandler(),
+        open_browser=not USE_CRYPTFILE,
     )
     return spotipy.Spotify(auth_manager=auth_manager)
```

### Comparing `gather-scrobble-0.0.3/gather_scrobble/scrobble.py` & `gather-scrobble-0.0.5/gather_scrobble/scrobble.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from gather_client_ws import GatherClient
 
 from gather_scrobble.config import (
     Credentials,
     get_credentials,
     get_lastfm_client,
     get_spotify_client,
+    logger,
 )
 
 BARS = "𝄖𝄗𝄘𝄙𝄚𝄛"
 
 PLAYING_ANIMATION = [
     [1, 2, 0, 1, 4],
     [2, 2, 0, 2, 4],
@@ -93,14 +94,15 @@
     await client.set_emoji_status("")
     await client.set_text_status("")
 
 
 async def set_status(client, emoji: str, text: str):
     await client.set_emoji_status(emoji)
     await client.set_text_status(text)
+    logger.debug("%s - %s", emoji, text)
 
 
 async def scrobble(client, scrobble_client):
     q = queue.Queue()
 
     def show_now_playing():
         default_msg = "Nothing is playing now 😕"
@@ -115,14 +117,15 @@
             terminal.write(f"\033[2K\r{to_write}")
             terminal.flush()
             sleep(0.1)
 
     current_now_playing = None
     threading.Thread(target=show_now_playing, daemon=True).start()
     retry = 0
+    logger.debug("application started")
     while True:
         try:
             now_playing = scrobble_client.get_now_playing()
             if now_playing is None:
                 if current_now_playing is not None:
                     await clear_status(client)
                 current_now_playing = None
@@ -143,15 +146,17 @@
             retry += 1
             if retry >= 3:
                 break
             await asyncio.sleep(2)
 
 
 async def start(space_id, source, emojis):
+    logger.debug("loading credentials")
     credentials = get_credentials()
     if not credentials.is_valid:
         raise Exception("At least one source needs to be configured.")
     scrobble_client = ScrobbleClient(credentials, source, emojis)
     client = GatherClient(
         credentials.gather_api_key, space_id, log_level=logging.ERROR
     )
+    logger.debug("starting application")
     await client.run(scrobble, scrobble_client)
```

### Comparing `gather-scrobble-0.0.3/gather_scrobble/test.py` & `gather-scrobble-0.0.5/gather_scrobble/test.py`

 * *Files identical despite different names*

### Comparing `gather-scrobble-0.0.3/setup.py` & `gather-scrobble-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     readme = ""
 
 
 package = "gather_scrobble"
 requirements = [
     "gather-client-ws<1",
     "keyring==23.13.1",
+    "keyrings.cryptfile==1.3.9",
     "python-decouple==3.8",
     "tabulate==0.9.0",
     "pylast==5.1.0",
     "spotipy==2.22.1",
     "docopt==0.6.2",
 ]
 test_requirements = []
@@ -68,15 +69,15 @@
     print("  git push --tags")
     sys.exit()
 
 
 setup(
     name="gather-scrobble",
     version=get_version(package),
-    description="Gather WebSocket service client",
+    description="Gather Scrobble - Scrobble your last.fm or Spotify activity to the Gather status.",
     long_description=readme,
     author=get_author(package),
     author_email=get_email(package),
     url="https://github.com/pyanderson/gather-scrobble",
     packages=[
         "gather_scrobble",
     ],
```

