# Comparing `tmp/gather-scrobble-0.0.6.tar.gz` & `tmp/gather-scrobble-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gather-scrobble-0.0.6.tar", last modified: Sat Apr 29 16:19:56 2023, max compression
+gzip compressed data, was "gather-scrobble-0.0.7.tar", last modified: Sat Apr 29 16:25:52 2023, max compression
```

## Comparing `gather-scrobble-0.0.6.tar` & `gather-scrobble-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:19:56.789923 gather-scrobble-0.0.6/
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1089 2023-03-25 18:58:51.000000 gather-scrobble-0.0.6/LICENSE
--rw-r--r--   0 pyand     (1000) pyand     (1000)    11856 2023-04-29 16:19:56.789923 gather-scrobble-0.0.6/PKG-INFO
--rw-r--r--   0 pyand     (1000) pyand     (1000)    10132 2023-04-29 16:19:41.000000 gather-scrobble-0.0.6/README.md
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:19:56.788923 gather-scrobble-0.0.6/gather_scrobble/
--rw-r--r--   0 pyand     (1000) pyand     (1000)      100 2023-04-29 16:19:41.000000 gather-scrobble-0.0.6/gather_scrobble/__init__.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1967 2023-04-29 16:19:41.000000 gather-scrobble-0.0.6/gather_scrobble/cli.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     5576 2023-04-29 15:31:55.000000 gather-scrobble-0.0.6/gather_scrobble/config.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)      455 2023-03-25 22:09:58.000000 gather-scrobble-0.0.6/gather_scrobble/info.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     5193 2023-04-29 16:16:38.000000 gather-scrobble-0.0.6/gather_scrobble/scrobble.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)     1591 2023-04-29 14:26:39.000000 gather-scrobble-0.0.6/gather_scrobble/test.py
--rw-r--r--   0 pyand     (1000) pyand     (1000)      344 2023-04-29 15:28:29.000000 gather-scrobble-0.0.6/gather_scrobble/utils.py
-drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:19:56.789923 gather-scrobble-0.0.6/gather_scrobble.egg-info/
--rw-r--r--   0 pyand     (1000) pyand     (1000)    11856 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/PKG-INFO
--rw-r--r--   0 pyand     (1000) pyand     (1000)      493 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/SOURCES.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/dependency_links.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       61 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/entry_points.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/not-zip-safe
--rw-r--r--   0 pyand     (1000) pyand     (1000)      143 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/requires.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       16 2023-04-29 16:19:56.000000 gather-scrobble-0.0.6/gather_scrobble.egg-info/top_level.txt
--rw-r--r--   0 pyand     (1000) pyand     (1000)       62 2023-03-25 18:58:51.000000 gather-scrobble-0.0.6/pyproject.toml
--rw-r--r--   0 pyand     (1000) pyand     (1000)       38 2023-04-29 16:19:56.789923 gather-scrobble-0.0.6/setup.cfg
--rwxr-xr-x   0 pyand     (1000) pyand     (1000)     3032 2023-04-29 03:56:29.000000 gather-scrobble-0.0.6/setup.py
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:25:52.966129 gather-scrobble-0.0.7/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1089 2023-03-25 18:58:51.000000 gather-scrobble-0.0.7/LICENSE
+-rw-r--r--   0 pyand     (1000) pyand     (1000)    11856 2023-04-29 16:25:52.966129 gather-scrobble-0.0.7/PKG-INFO
+-rw-r--r--   0 pyand     (1000) pyand     (1000)    10132 2023-04-29 16:25:43.000000 gather-scrobble-0.0.7/README.md
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:25:52.965129 gather-scrobble-0.0.7/gather_scrobble/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      100 2023-04-29 16:25:43.000000 gather-scrobble-0.0.7/gather_scrobble/__init__.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1967 2023-04-29 16:25:43.000000 gather-scrobble-0.0.7/gather_scrobble/cli.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     5576 2023-04-29 15:31:55.000000 gather-scrobble-0.0.7/gather_scrobble/config.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      455 2023-03-25 22:09:58.000000 gather-scrobble-0.0.7/gather_scrobble/info.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     5191 2023-04-29 16:24:53.000000 gather-scrobble-0.0.7/gather_scrobble/scrobble.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)     1591 2023-04-29 14:26:39.000000 gather-scrobble-0.0.7/gather_scrobble/test.py
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      344 2023-04-29 15:28:29.000000 gather-scrobble-0.0.7/gather_scrobble/utils.py
+drwxr-xr-x   0 pyand     (1000) pyand     (1000)        0 2023-04-29 16:25:52.966129 gather-scrobble-0.0.7/gather_scrobble.egg-info/
+-rw-r--r--   0 pyand     (1000) pyand     (1000)    11856 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/PKG-INFO
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      493 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/SOURCES.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/dependency_links.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       61 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/entry_points.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)        1 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/not-zip-safe
+-rw-r--r--   0 pyand     (1000) pyand     (1000)      143 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/requires.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       16 2023-04-29 16:25:52.000000 gather-scrobble-0.0.7/gather_scrobble.egg-info/top_level.txt
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       62 2023-03-25 18:58:51.000000 gather-scrobble-0.0.7/pyproject.toml
+-rw-r--r--   0 pyand     (1000) pyand     (1000)       38 2023-04-29 16:25:52.966129 gather-scrobble-0.0.7/setup.cfg
+-rwxr-xr-x   0 pyand     (1000) pyand     (1000)     3032 2023-04-29 03:56:29.000000 gather-scrobble-0.0.7/setup.py
```

### Comparing `gather-scrobble-0.0.6/LICENSE` & `gather-scrobble-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gather-scrobble-0.0.6/PKG-INFO` & `gather-scrobble-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gather-scrobble
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gather Scrobble - Scrobble your last.fm or Spotify activity to the Gather status.
 Home-page: https://github.com/pyanderson/gather-scrobble
 Author: Anderson de Sousa Lima
 Author-email: anderson.sl93@hotmail.com
 License: MIT
 Keywords: gather,gather-town,lastfm,spotify,scrobble
 Classifier: Development Status :: 5 - Production/Stable
@@ -240,15 +240,15 @@
 ------
 
 Pull
 ~~~~
 
 .. code:: bash
 
-   $ docker pull pyanderson/gather-scrobble:0.0.6
+   $ docker pull pyanderson/gather-scrobble:0.0.7
 
 Docker Configuration
 ~~~~~~~~~~~~~~~~~~~~
 
 Keyring
 ^^^^^^^
 
@@ -294,15 +294,15 @@
 
 The docker container works as an executable, so you can use the same CLI
 command interface, for example, to test your configuration you can do
 this:
 
 .. code:: bash
 
-   $ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
    Testing connection with Gather...
    Success
    Testing connection with last.fm...
    Success
    Testing connection with Spotify...
    Success
 
@@ -319,15 +319,15 @@
 Examples
 ^^^^^^^^
 
 Validate your credentials:
 
 .. code:: bash
 
-   $ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
    Testing connection with Gather...
    Success
    Testing connection with last.fm...
    Please authorize this script to access your account: https://www.last.fm/api/auth/?api_key=<api_key>
    Success
    Testing connection with Spotify...
    Go to the following URL: https://accounts.spotify.com/authorize?client_id=<client_id>&response_type=code&redirect_uri=http%3A%2F%2F127.0.0.1%3A9090&scope=user-read-currently-playing+user-read-playback-state
@@ -344,15 +344,15 @@
    ┃ Spotify   ┃ True       ┃
    ┗━━━━━━━━━━━┻━━━━━━━━━━━━┛
 
 Run gather-scrobble in background:
 
 .. code:: bash
 
-   $ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 start "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 start "aAa0aAaAaaA0Aaaa/Name"
    cbe4b6c916d8e7977788462a447b8a6c9e526f46f5c9b85d7be5f843e7fd80dc
 
 Check the logs:
 
 .. code:: bash
 
    $ docker logs -f gather-scrobble
```

### Comparing `gather-scrobble-0.0.6/README.md` & `gather-scrobble-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 🎸 - Evil Papagali - Massacration 𝄛𝄙𝄘𝄛𝄙
 ```
 
 ## Docker
 ### Pull
 
 ```bash
-$ docker pull pyanderson/gather-scrobble:0.0.6
+$ docker pull pyanderson/gather-scrobble:0.0.7
 ```
 
 ### Docker Configuration
 #### Keyring
 The most common way to manage credentials in docker containers is through environment variables, but in this case, you can still use [keyring](https://github.com/jaraco/keyring), through the third-party [keyrings.cryptfile](https://github.com/frispete/keyrings.cryptfile), you will need to create a file with your credentials, mount a volume with the file in the path `/root/.local/share/python_keyring/cryptfile_pass.cfg` and set the `KEYRING_CRYPTFILE_PASSWORD` environment variable with the password that you used to create the file:
 
 ```bash
@@ -200,15 +200,15 @@
 $ docker run -v /path/to/save/cache:/root/.config ...
 ```
 
 ### Docker Usage
 The docker container works as an executable, so you can use the same CLI command interface, for example, to test your configuration you can do this:
 
 ```bash
-$ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+$ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
 Testing connection with Gather...
 Success
 Testing connection with last.fm...
 Success
 Testing connection with Spotify...
 Success
 
@@ -223,15 +223,15 @@
 ┗━━━━━━━━━━━┻━━━━━━━━━━━━┛
 ```
 
 #### Examples
 Validate your credentials:
 
 ```bash
-$ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+$ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
 Testing connection with Gather...
 Success
 Testing connection with last.fm...
 Please authorize this script to access your account: https://www.last.fm/api/auth/?api_key=<api_key>
 Success
 Testing connection with Spotify...
 Go to the following URL: https://accounts.spotify.com/authorize?client_id=<client_id>&response_type=code&redirect_uri=http%3A%2F%2F127.0.0.1%3A9090&scope=user-read-currently-playing+user-read-playback-state
@@ -248,15 +248,15 @@
 ┃ Spotify   ┃ True       ┃
 ┗━━━━━━━━━━━┻━━━━━━━━━━━━┛
 ```
 
 Run gather-scrobble in background:
 
 ```bash
-$ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 start "aAa0aAaAaaA0Aaaa/Name"
+$ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 start "aAa0aAaAaaA0Aaaa/Name"
 cbe4b6c916d8e7977788462a447b8a6c9e526f46f5c9b85d7be5f843e7fd80dc
 ```
 
 Check the logs:
 
 ```bash
 $ docker logs -f gather-scrobble
```

### Comparing `gather-scrobble-0.0.6/gather_scrobble/cli.py` & `gather-scrobble-0.0.7/gather_scrobble/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from gather_scrobble.config import logger
 from gather_scrobble.info import show_info
 from gather_scrobble.scrobble import start
 from gather_scrobble.test import test_configuration
 
 
 def main():
-    """Gather Scrobble v0.0.6
+    """Gather Scrobble v0.0.7
     Usage:
         gather-scrobble start <space_id> [--source SOURCE] [--emojis EMOJIS]
         gather-scrobble info
         gather-scrobble test <space_id>
 
     Arguments:
         <space_id>          Gather space id.
@@ -28,15 +28,15 @@
                             the priority: lastfm -> spotify [default: any]
         -e --emojis EMOJIS  It is possible to customize the emojis, by setting
                             the list of emojis that will be chosen randomly,
                             and also you don't like emojis, you can set an
                             empty string here. [default: 🎼🎵🎶🎧📻🎷🎸🎹]
 
     """
-    arguments = docopt(main.__doc__ or "", version="Gather Scrobble 0.0.6")
+    arguments = docopt(main.__doc__ or "", version="Gather Scrobble 0.0.7")
     if arguments["start"]:
         if arguments["--source"] not in ["lastfm", "spotify", "any"]:
             raise Exception(f"Invalid source: {arguments['--source']}")
         with suppress(KeyboardInterrupt):
             asyncio.get_event_loop().run_until_complete(
                 start(
                     arguments["<space_id>"],
```

### Comparing `gather-scrobble-0.0.6/gather_scrobble/config.py` & `gather-scrobble-0.0.7/gather_scrobble/config.py`

 * *Files identical despite different names*

### Comparing `gather-scrobble-0.0.6/gather_scrobble/scrobble.py` & `gather-scrobble-0.0.7/gather_scrobble/scrobble.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,19 @@
         for bars in cycle(PLAYING_ANIMATION):
             if q.qsize() > 0:
                 msg = q.get()
             if msg.strip() == "":
                 to_write = default_msg
             else:
                 to_write = f"{msg} {''.join(BARS[index] for index in bars)}"
-            terminal.write(f"\033[2K\r{to_write}")
-            terminal.flush()
+            # No show the playing now when running in docker
+            # to avoid messing with the logs.
+            if logger.level > logging.DEBUG:
+                terminal.write(f"\033[2K\r{to_write}")
+                terminal.flush()
             sleep(0.1)
 
     current_now_playing = None
     threading.Thread(target=show_now_playing, daemon=True).start()
     retry = 0
     logger.debug("application started")
     while True:
@@ -129,20 +132,18 @@
                 if current_now_playing is not None:
                     await clear_status(client)
                 current_now_playing = None
             elif current_now_playing != now_playing:
                 emoji = random.choice(scrobble_client.emojis)
                 current_now_playing = now_playing
                 await set_status(client, emoji, now_playing)
-                # No show the playing now when running in docker to avoid messing with the logs.
-                if logger.level > logging.DEBUG:
-                    if emoji:
-                        q.put(f"{emoji} - {current_now_playing}")
-                    else:
-                        q.put(f"{current_now_playing}")
+                if emoji:
+                    q.put(f"{emoji} - {current_now_playing}")
+                else:
+                    q.put(f"{current_now_playing}")
             await asyncio.sleep(15)
             retry = 0
         except KeyboardInterrupt:
             break
         except Exception:
             # The retry will ensure the problem is not temporary
             retry += 1
```

### Comparing `gather-scrobble-0.0.6/gather_scrobble/test.py` & `gather-scrobble-0.0.7/gather_scrobble/test.py`

 * *Files identical despite different names*

### Comparing `gather-scrobble-0.0.6/gather_scrobble.egg-info/PKG-INFO` & `gather-scrobble-0.0.7/gather_scrobble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gather-scrobble
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gather Scrobble - Scrobble your last.fm or Spotify activity to the Gather status.
 Home-page: https://github.com/pyanderson/gather-scrobble
 Author: Anderson de Sousa Lima
 Author-email: anderson.sl93@hotmail.com
 License: MIT
 Keywords: gather,gather-town,lastfm,spotify,scrobble
 Classifier: Development Status :: 5 - Production/Stable
@@ -240,15 +240,15 @@
 ------
 
 Pull
 ~~~~
 
 .. code:: bash
 
-   $ docker pull pyanderson/gather-scrobble:0.0.6
+   $ docker pull pyanderson/gather-scrobble:0.0.7
 
 Docker Configuration
 ~~~~~~~~~~~~~~~~~~~~
 
 Keyring
 ^^^^^^^
 
@@ -294,15 +294,15 @@
 
 The docker container works as an executable, so you can use the same CLI
 command interface, for example, to test your configuration you can do
 this:
 
 .. code:: bash
 
-   $ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config -it pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
    Testing connection with Gather...
    Success
    Testing connection with last.fm...
    Success
    Testing connection with Spotify...
    Success
 
@@ -319,15 +319,15 @@
 Examples
 ^^^^^^^^
 
 Validate your credentials:
 
 .. code:: bash
 
-   $ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 test "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run -it --rm --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 test "aAa0aAaAaaA0Aaaa/Name"
    Testing connection with Gather...
    Success
    Testing connection with last.fm...
    Please authorize this script to access your account: https://www.last.fm/api/auth/?api_key=<api_key>
    Success
    Testing connection with Spotify...
    Go to the following URL: https://accounts.spotify.com/authorize?client_id=<client_id>&response_type=code&redirect_uri=http%3A%2F%2F127.0.0.1%3A9090&scope=user-read-currently-playing+user-read-playback-state
@@ -344,15 +344,15 @@
    ┃ Spotify   ┃ True       ┃
    ┗━━━━━━━━━━━┻━━━━━━━━━━━━┛
 
 Run gather-scrobble in background:
 
 .. code:: bash
 
-   $ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.6 start "aAa0aAaAaaA0Aaaa/Name"
+   $ docker run -d --restart=always --name gather-scrobble --env-file /path/to/myfile.env -v /path/to/save/cache:/root/.config pyanderson/gather-scrobble:0.0.7 start "aAa0aAaAaaA0Aaaa/Name"
    cbe4b6c916d8e7977788462a447b8a6c9e526f46f5c9b85d7be5f843e7fd80dc
 
 Check the logs:
 
 .. code:: bash
 
    $ docker logs -f gather-scrobble
```

### Comparing `gather-scrobble-0.0.6/setup.py` & `gather-scrobble-0.0.7/setup.py`

 * *Files identical despite different names*

