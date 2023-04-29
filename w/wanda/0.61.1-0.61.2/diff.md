# Comparing `tmp/wanda-0.61.1.tar.gz` & `tmp/wanda-0.61.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wanda-0.61.1.tar", max compression
+gzip compressed data, was "wanda-0.61.2.tar", max compression
```

## Comparing `wanda-0.61.1.tar` & `wanda-0.61.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-01-07 08:58:17.544267 wanda-0.61.1/LICENSE
--rw-r--r--   0        0        0     2012 2023-02-11 11:57:52.161176 wanda-0.61.1/README.md
--rw-r--r--   0        0        0      920 2023-02-11 12:21:01.282899 wanda-0.61.1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-01-07 08:58:17.544267 wanda-0.61.1/wanda/__init__.py
--rw-r--r--   0        0        0    11975 2023-02-11 12:19:41.389505 wanda-0.61.1/wanda/sources.py
--rw-r--r--   0        0        0        0 2023-02-11 11:57:52.161176 wanda-0.61.1/wanda/utils/__init__.py
--rw-r--r--   0        0        0      150 2023-02-11 11:59:28.909000 wanda-0.61.1/wanda/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2499 2023-02-11 11:59:28.909000 wanda-0.61.1/wanda/utils/__pycache__/common_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2997 2023-02-11 11:59:28.965669 wanda-0.61.1/wanda/utils/__pycache__/image_utils.cpython-310.pyc
--rw-r--r--   0        0        0     3245 2023-02-11 11:59:28.965669 wanda-0.61.1/wanda/utils/__pycache__/os_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1708 2023-02-11 11:57:52.161176 wanda-0.61.1/wanda/utils/common_utils.py
--rw-r--r--   0        0        0     4189 2023-02-11 11:58:04.285072 wanda-0.61.1/wanda/utils/image_utils.py
--rw-r--r--   0        0        0     3201 2023-02-11 11:57:52.161176 wanda-0.61.1/wanda/utils/os_utils.py
--rwxr-xr-x   0        0        0     4803 2023-02-11 12:17:13.133322 wanda-0.61.1/wanda/wanda.py
--rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 wanda-0.61.1/setup.py
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 wanda-0.61.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-29 06:18:58.249614 wanda-0.61.2/LICENSE
+-rw-r--r--   0        0        0     2012 2023-04-29 06:18:58.249614 wanda-0.61.2/README.md
+-rw-r--r--   0        0        0      920 2023-04-29 07:47:10.638626 wanda-0.61.2/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/__init__.py
+-rw-r--r--   0        0        0    12124 2023-04-29 07:33:50.334412 wanda-0.61.2/wanda/sources.py
+-rw-r--r--   0        0        0        0 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/__init__.py
+-rw-r--r--   0        0        0      150 2023-04-29 06:25:38.899989 wanda-0.61.2/wanda/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2499 2023-04-29 06:25:38.899989 wanda-0.61.2/wanda/utils/__pycache__/common_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2997 2023-04-29 06:25:38.956658 wanda-0.61.2/wanda/utils/__pycache__/image_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3245 2023-04-29 06:25:38.956658 wanda-0.61.2/wanda/utils/__pycache__/os_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1708 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/common_utils.py
+-rw-r--r--   0        0        0     4189 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/image_utils.py
+-rw-r--r--   0        0        0     3201 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/os_utils.py
+-rwxr-xr-x   0        0        0     5741 2023-04-29 06:54:06.187103 wanda-0.61.2/wanda/wanda.py
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 wanda-0.61.2/setup.py
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 wanda-0.61.2/PKG-INFO
```

### Comparing `wanda-0.61.1/LICENSE` & `wanda-0.61.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wanda-0.61.1/README.md` & `wanda-0.61.2/README.md`

 * *Files identical despite different names*

### Comparing `wanda-0.61.1/pyproject.toml` & `wanda-0.61.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wanda"
-version = "0.61.1"
+version = "0.61.2"
 description = "Set wallpapers with keywords or randomly"
 authors = ["kshib <ksyko@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/kshib/wanda"
 repository = "https://gitlab.com/kshib/wanda"
 keywords=["wallpaper", "reddit", "wallhaven","unsplash","termux"]
@@ -20,15 +20,15 @@
 screeninfo = "^0.8"
 colorthief = "^0.2.1"
 filetype = "^1.0.13"
 musicbrainzngs = "^0.7.1"
 appdirs = "^1.4.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.3.1"
 black = "^22.3.0"
 mypy = "^0.991"
 pytest-xdist = "^3.1.0"
 pytest-cov = "^4.0.0"
 pytest-rerunfailures = "^11"
 
 [build-system]
```

### Comparing `wanda-0.61.1/wanda/sources.py` & `wanda-0.61.2/wanda/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,31 @@
     elif "@" not in search:
         search = f"{search.lower()}" if search else ""
         board = "wg"
     else:
         board = search.split("@")[1]
         search = search.split("@")[0].lower()
 
-    api = f"https://s1.alice.al/_/api/chan/search/?boards={board}&subject={search.lower()}"
+    api = f"https://archive.palanq.win/_/api/chan/search/?boards={board}&subject={search.lower()}"
     response = get(api).json()
     no_results() if "error" in response else ok()
     posts = list(
         filter(lambda p: "media" in p and "nimages" in p, response["0"]["posts"])
     )
     ok() if posts else no_results()
     post = random.choice(posts)
     thread = post["thread_num"]
     board = post["board"]["shortname"]
-    api = f"https://s1.alice.al/_/api/chan/thread/?board={board}&num={thread}"
+    api = f"https://archive.palanq.win/_/api/chan/thread/?board={board}&num={thread}"
     posts = get(api).json()[thread]["posts"]
     ok() if posts else no_results()
     post = random.choice(list(filter(lambda p: "media" in posts[p], posts)))
-    return posts[post]["media"]["media_link"]
+    if posts[post]:
+        return posts[post]["media"]["media_link"]
+    return no_results()
 
 
 def suggested_subreddits():
     if screen_orientation() == "portrait":
         return "mobilewallpaper+amoledbackgrounds+verticalwallpapers"
     return "wallpaper+wallpapers+minimalwallpaper"
 
@@ -292,19 +294,21 @@
 def musicbrainz(search=None):
     print("[!] This source is experimental")
     import musicbrainzngs as mb  # type: ignore
 
     if blank(search):
         print("Please enter [artist]-[album]")
         exit(1)
-    mb.set_useragent("wanda", "", user_agent["User-Agent"])
+    mb.set_useragent("wanda", "*", user_agent["User-Agent"])
     [artist, album] = search.split("-")
     try:
         albums = mb.search_releases(album, artist=artist)
         ok() if albums else no_results()
+        if not albums["release-list"]:
+            raise mb.MusicBrainzError
         album_id = albums["release-list"][0]["release-group"]["id"]
         cover = mb.get_release_group_image_front(album_id)
         path = get_dl_path()
         with open(path, "wb") as f:
             f.write(cover)
         ext = filetype.guess(path).EXTENSION
         os.rename(path, f"{path}.{ext}")
@@ -317,15 +321,15 @@
     api = "https://wallhaven.cc/api/v1/search?sorting=random"
     ratios = "portrait" if screen_orientation() == "portrait" else "landscape"
     response = get(f"{api}&ratios={ratios}&q={search or ''}").json()["data"]
     return response[0]["path"] if response else no_results()
 
 
 def unsplash(search=None):
-    api = f"https://source.unsplash.com/random/{size()[0]}x{size()[1]}/?{search or ''}"
+    api = f"https://source.unsplash.com/random/{size()[0]}x{size()[1]}/?{search or 'wallpaper'}"
     response = get(api).url
     return response if "source-404" not in response else no_results()
 
 
 def earthview(_):  # NOSONAR
     from lxml import html  # type: ignore
     folder = appdirs.user_cache_dir("wanda")
```

### Comparing `wanda-0.61.1/wanda/utils/__pycache__/common_utils.cpython-310.pyc` & `wanda-0.61.2/wanda/utils/__pycache__/common_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Feb 11 11:57:52 2023 UTC, .py size: 1708 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c082 e763 ac06 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 d2b6 4c64 ac06 0000  o.........Ld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6503  d.l.Z.d.d.l.Z.e.
 00000060: a006 6402 a101 5a07 6403 6508 6404 6508  ..d...Z.d.e.d.e.
 00000070: 6604 6405 6406 8404 5a09 6407 6408 8400  f.d.d...Z.d.d...
```

### Comparing `wanda-0.61.1/wanda/utils/__pycache__/image_utils.cpython-310.pyc` & `wanda-0.61.2/wanda/utils/__pycache__/image_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Feb 11 11:58:04 2023 UTC, .py size: 4189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cc82 e763 5d10 0000  o..........c]...
+00000000: 6f0d 0d0a 0000 0000 d2b6 4c64 5d10 0000  o.........Ld]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6405 8400 5a0a 6406 6407 8400  ..d.d...Z.d.d...
 00000070: 5a0b 6408 6409 8400 5a0c 640a 640b 8400  Z.d.d...Z.d.d...
@@ -170,17 +170,17 @@
 00000a90: 0000 da04 686f 6d65 da04 6c6f 636b da05  ....home..lock..
 00000aa0: 6669 7477 7072 2c00 0000 722e 0000 0072  fitwpr,...r....r
 00000ab0: 0c00 0000 720c 0000 0072 0d00 0000 da06  ....r....r......
 00000ac0: 7365 745f 7770 6100 0000 7326 0000 0008  set_wpa...s&....
 00000ad0: 0212 0306 010c 010c 0106 0108 0204 0104  ................
 00000ae0: 0308 0108 0306 0210 010c 010c 010c 010c  ................
 00000af0: 0108 020c 0172 3400 0000 2903 5454 4629  .....r4...).TTF)
-00000b00: 1172 2b00 0000 da18 7761 6e64 612e 7574  .r+.....wanda.ut
+00000b00: 1172 2b00 0000 5a18 7761 6e64 612e 7574  .r+...Z.wanda.ut
 00000b10: 696c 732e 636f 6d6d 6f6e 5f75 7469 6c73  ils.common_utils
-00000b20: 7202 0000 0072 0300 0000 da14 7761 6e64  r....r......wand
+00000b20: 7202 0000 0072 0300 0000 5a14 7761 6e64  r....r....Z.wand
 00000b30: 612e 7574 696c 732e 6f73 5f75 7469 6c73  a.utils.os_utils
 00000b40: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
 00000b50: 0700 0000 7208 0000 0072 0e00 0000 7212  ....r....r....r.
 00000b60: 0000 0072 1500 0000 7218 0000 0072 2500  ...r....r....r%.
 00000b70: 0000 da03 7374 7272 3400 0000 720c 0000  ....strr4...r...
 00000b80: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
 00000b90: da08 3c6d 6f64 756c 653e 0100 0000 7312  ..<module>....s.
```

### Comparing `wanda-0.61.1/wanda/utils/__pycache__/os_utils.cpython-310.pyc` & `wanda-0.61.2/wanda/utils/__pycache__/os_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Feb 11 11:57:52 2023 UTC, .py size: 3201 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c082 e763 810c 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 d2b6 4c64 810c 0000  o.........Ld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 8400 5a06 6405 6406 8400  ..d.d...Z.d.d...
 00000060: 5a07 6407 6408 8400 5a08 6409 640a 8400  Z.d.d...Z.d.d...
 00000070: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
```

### Comparing `wanda-0.61.1/wanda/utils/common_utils.py` & `wanda-0.61.2/wanda/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.1/wanda/utils/image_utils.py` & `wanda-0.61.2/wanda/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.1/wanda/utils/os_utils.py` & `wanda-0.61.2/wanda/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.1/wanda/wanda.py` & `wanda-0.61.2/wanda/wanda.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import wanda.utils.common_utils as common
 import wanda.utils.image_utils as image
 import wanda.utils.os_utils as osu
 import wanda.sources as sources
 
 folder = appdirs.user_cache_dir("wanda")
-version = "0.61.1"
+version = "0.61.2"
 
 
 def usage(level=0):
     cyan = "\033[36m"
     pink = "\033[35m"
     print("Sources:")
     print(f"{cyan}4chan {pink}[keyword]|[keyword@board]")
@@ -133,23 +133,49 @@
     fitwp = False
     if "-l" in sys.argv and args.l:
         home = False
     if "-h" in sys.argv and args.h:
         lock = False
     if "-f" in sys.argv and source not in ('e', 'earthview'):
         fitwp = True
-    try:
-        if source != "local" and not common.is_connected():
-            print("Please check your internet connection and try again")
-            exit(1)
-        image.set_wp(eval(f"sources.{source_map(source)}")(term), home, lock, fitwp)
-    except NameError:
-        print(f"Unknown source: '{source}'")
-        usage()
-
+    if source != "local" and not common.is_connected():
+        print("Please check your internet connection and try again")
+        exit(1)
+    if source == "fourchan":
+        wp = sources.fourchan(term)
+    elif source == "reddit":
+        wp = sources.reddit(term)
+    elif source == "picsum":
+        wp = sources.picsum(term)
+    elif source == "imgur":
+        wp = sources.imgur(term)
+    elif source == "fivehundredpx":
+        wp = sources.fivehundredpx(term)
+    elif source == "artstation_prints":
+        wp = sources.artstation_prints(term)
+    elif source == "artstation_artist":
+        wp = sources.artstation_artist(term)
+    elif source == "artstation_any":
+        wp = sources.artstation_any(term)
+    elif source == "local":
+        wp = sources.local(term)
+    elif source == "waifuim":
+        wp = sources.waifuim(term)
+    elif source == "musicbrainz":
+        wp = sources.musicbrainz(term)
+    elif source == "wallhaven":
+        wp = sources.wallhaven(term)
+    elif source == "unsplash":
+        wp = sources.unsplash(term)
+    elif source == "earthview":
+        wp = sources.earthview(term)
+    else:
+        print(f"Unknown Source: {source}. Using unsplash.")
+        wp = sources.unsplash(term)
+    image.set_wp(wp, home, lock, fitwp)
     return 0
 
 
 def shortcodes():
     return {
         "4": "fourchan",
         "5": "fivehundredpx",
```

### Comparing `wanda-0.61.1/setup.py` & `wanda-0.61.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'screeninfo>=0.8,<0.9']
 
 entry_points = \
 {'console_scripts': ['wanda = wanda.wanda:run']}
 
 setup_kwargs = {
     'name': 'wanda',
-    'version': '0.61.1',
+    'version': '0.61.2',
     'description': 'Set wallpapers with keywords or randomly',
     'long_description': '# wanda\nScript to set wallpaper using keyword or randomly\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e5aacd529ce04f3fb8c0f9ce6a3bdd9e)](https://www.codacy.com/gh/ksyko/wanda/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ksyko/wanda&amp;utm_campaign=Badge_Grade)[![PyPI](https://img.shields.io/pypi/v/wanda)](https://pypi.org/project/wanda/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/wanda)](https://pypistats.org/packages/wanda)\n[![PyPI - License](https://img.shields.io/pypi/l/wanda)](https://tldrlegal.com/license/mit-license)\n[![codecov](https://codecov.io/gl/kshib/wanda/branch/main/graph/badge.svg?token=L88CXOYRTW)](https://codecov.io/gl/kshib/wanda)\n\n## Installation / Update\n```\npip install wanda -U\n```\n\nOn android (with termux):\n```\npkg in libxml2 libxslt libjpeg-turbo\npip install wanda -U\n```\n\nFor issues installing pillow refer this [document](https://pillow.readthedocs.io/en/stable/installation.html)\n\n\n## Usage\n```\n# Set randomly\nwanda\n\n# Set from a keyword \nwanda -t mountain\n\n# Set from a source\nwanda -s wallhaven\n\n# Set from a source \nwanda -s wallhaven -t japan\n```\n`wanda -h` for more details\n\n## Notes\n- By default, the source is [unsplash](https://unsplash.com).\n- Some sources may have inapt images. Use them at your own risk.\n\n## Supported sources\n\n- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive.alice.al)\n- [500px](https://500px.com)\n- [artstation](https://artstation.com)\n- [imgur](https://imgur.com) via [rimgo](https://rimgo.pussthecat.org)\n- [earthview](https://earthview.withgoogle.com)\n- local\n- [picsum](https://picsum.photos)\n- [reddit](https://reddit.com)\n- [unsplash](https://unsplash.com)\n- [wallhaven](https://wallhaven.cc)\n\n## Build\n[python](https://www.python.org/downloads/) and [poetry](https://python-poetry.org/) are needed\n```\ngit clone https://github.com/ksh-b/wanda.git\ncd wanda\npoetry install\npoetry build\npoetry run wanda\n```\n\n## Uninstall\n```\npip uninstall wanda\n```\n\n## License\nMIT\n',
     'author': 'kshib',
     'author_email': 'ksyko@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/kshib/wanda',
```

### Comparing `wanda-0.61.1/PKG-INFO` & `wanda-0.61.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wanda
-Version: 0.61.1
+Version: 0.61.2
 Summary: Set wallpapers with keywords or randomly
 Home-page: https://gitlab.com/kshib/wanda
 License: MIT
 Keywords: wallpaper,reddit,wallhaven,unsplash,termux
 Author: kshib
 Author-email: ksyko@pm.me
 Requires-Python: >=3.7,<4.0
```

