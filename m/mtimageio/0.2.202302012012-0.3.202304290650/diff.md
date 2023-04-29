# Comparing `tmp/mtimageio-0.2.202302012012-py3-none-any.whl.zip` & `tmp/mtimageio-0.3.202304290650-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8651 bytes, number of entries: 12
--rw-r--r--  2.0 unx      162 b- defN 23-Feb-01 17:38 mt/iio/__init__.py
--rw-r--r--  2.0 unx      194 b- defN 23-Jan-22 22:24 mt/imageio/__init__.py
--rw-r--r--  2.0 unx     3600 b- defN 23-Feb-01 20:12 mt/imageio/immview.py
--rw-r--r--  2.0 unx     9821 b- defN 23-Jan-22 22:24 mt/imageio/imread.py
--rw-r--r--  2.0 unx     6664 b- defN 23-Jan-22 22:24 mt/imageio/imwrite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Feb-01 20:12 mt/imageio/version.py
--rwxr-xr-x  2.0 unx     1003 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.data/scripts/immview
--rw-r--r--  2.0 unx     1500 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.dist-info/LICENSE
--rw-r--r--  2.0 unx      290 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1015 b- defN 23-Feb-01 20:12 mtimageio-0.2.202302012012.dist-info/RECORD
-12 files, 24740 bytes uncompressed, 6929 bytes compressed:  72.0%
+Zip file size: 8979 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      162 b- defN 23-Feb-21 07:08 mt/iio/__init__.py
+-rw-r--r--  2.0 unx      194 b- defN 22-Dec-30 06:14 mt/imageio/__init__.py
+-rw-r--r--  2.0 unx     3600 b- defN 23-Feb-21 07:08 mt/imageio/immview.py
+-rw-r--r--  2.0 unx    10139 b- defN 23-Apr-29 06:50 mt/imageio/imread.py
+-rw-r--r--  2.0 unx     7561 b- defN 23-Apr-29 06:40 mt/imageio/imwrite.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-29 06:50 mt/imageio/version.py
+-rwxr-xr-x  2.0 unx     1003 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.data/scripts/immview
+-rw-r--r--  2.0 unx     1500 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/LICENSE
+-rw-r--r--  2.0 unx      290 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1016 b- defN 23-Apr-29 06:51 mtimageio-0.3.202304290650.dist-info/RECORD
+12 files, 25956 bytes uncompressed, 7257 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: mt/imageio/imwrite.py
 Comment: 
 
 Filename: mt/imageio/version.py
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.data/scripts/immview
+Filename: mtimageio-0.3.202304290650.data/scripts/immview
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.dist-info/LICENSE
+Filename: mtimageio-0.3.202304290650.dist-info/LICENSE
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.dist-info/METADATA
+Filename: mtimageio-0.3.202304290650.dist-info/METADATA
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.dist-info/WHEEL
+Filename: mtimageio-0.3.202304290650.dist-info/WHEEL
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.dist-info/top_level.txt
+Filename: mtimageio-0.3.202304290650.dist-info/top_level.txt
 Comment: 
 
-Filename: mtimageio-0.2.202302012012.dist-info/RECORD
+Filename: mtimageio-0.3.202304290650.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/imageio/imread.py

```diff
@@ -1,10 +1,11 @@
 """Extra imread functions."""
 
 import typing as tp
+import json
 
 from imageio import v3 as iio
 
 from mt import np, cv, path, aio
 
 
 __all__ = [
@@ -132,14 +133,23 @@
     imageio.v3.imread
         the underlying imread function
     imageio.v3.immeta
         the underlying immeta function
     """
 
     meta = iio.immeta(data, plugin=plugin, extension=extension, **plugin_kwargs)
+    if "xmp" in meta and isinstance(meta["xmp"], bytes):
+        meta2 = json.loads(meta["xmp"])
+        del meta["xmp"]
+        for x in ["mode", "shape"]:
+            meta2[x] = meta[x]
+            del meta[x]
+        # meta2["image_meta"] = meta # MT-TODO: expose later in future.
+        meta = meta2
+
     image = iio.imread(
         data,
         plugin=plugin,
         extension=extension,
         format_hint=format_hint,
         **plugin_kwargs
     )
```

## mt/imageio/imwrite.py

```diff
@@ -21,15 +21,15 @@
     fname: str,
     image: np.ndarray,
     plugin: tp.Optional[str] = None,
     extension: tp.Optional[str] = None,
     format_hint: tp.Optional[str] = None,
     plugin_kwargs: dict = {},
     context_vars: dict = {},
-    **kwargs
+    **kwargs,
 ):
     """An asyn function that saves an image file using :func:`imageio.v3.imwrite`.
 
     Parameters
     ----------
     fname : str
         local filepath where the image will be saved. If "<bytes>" is provided, the function
@@ -64,55 +64,33 @@
     if fname == "<bytes>":
         return iio.imwrite(
             fname,
             image,
             plugin=plugin,
             extension=extension,
             format_hint=format_hint,
-            **plugin_kwargs
+            **plugin_kwargs,
         )
 
     if extension is None:
         extension = path.splitext(fname.lower())[1]
 
     data = iio.imwrite(
         "<bytes>",
         image,
         plugin=plugin,
         extension=extension,
         format_hint=format_hint,
-        **plugin_kwargs
+        **plugin_kwargs,
     )
 
     return await aio.write_binary(fname, data, context_vars=context_vars)
 
 
-def immencode(imm: cv.Image) -> bytes:
-    """Encodes a :class:`mt.cv.opencv.Image` instance as a PNG image with metadata.
-
-    Parameters
-    ----------
-    imm : cv.Image
-        an image with metadata
-
-    Returns
-    -------
-    data : bytes
-        the image encoded into PNG content, ready for writing to file
-
-    Notes
-    -----
-    All metadata values are converted to json strings if they are not strings.
-
-    See Also
-    --------
-    imageio.v3.imwrite
-        the underlying imwrite function
-    """
-
+def immencode_png(imm: cv.Image) -> bytes:
     pnginfo = PngImagePlugin.PngInfo()
     pnginfo.add_text("pixel_format", imm.pixel_format)
     for k, v in imm.meta.items():
         if not isinstance(v, str):
             v = json.dumps(v)
         pnginfo.add_text(k, v)
 
@@ -130,33 +108,76 @@
         extension=".png",
         mode=mode,
         pnginfo=pnginfo,
     )
     return data
 
 
+def immencode_webp(imm: cv.Image) -> bytes:
+    xmp = json.dumps(imm.meta)
+    data = iio.imwrite(
+        "<bytes>", imm.image, plugin="pillow", extension=".webp", lossless=True, xmp=xmp
+    )
+    return data
+
+
+def immencode(imm: cv.Image, encoding_format: str = "png") -> bytes:
+    """Encodes a :class:`mt.cv.opencv.Image` instance as a PNG or WEBP image with metadata.
+
+    Parameters
+    ----------
+    imm : cv.Image
+        an image with metadata
+    encoding_format : {'png', 'webp'}
+        the encoding format
+
+    Returns
+    -------
+    data : bytes
+        the encoded image, ready for writing to file
+
+    Notes
+    -----
+    All metadata values are converted to json strings if they are not strings.
+
+    See Also
+    --------
+    imageio.v3.imwrite
+        the underlying imwrite function
+    """
+
+    if encoding_format == "png":
+        return immencode_png(imm)
+
+    if encoding_format == "webp":
+        return immencode_webp(imm)
+
+    raise NotImplementedError(f"Unknown encoding format '{encoding_format}'.")
+
+
 async def immwrite_asyn(
     filepath: str,
     imm: cv.Image,
-    file_format: str = "hdf5",
+    file_format: tp.Optional[str] = None,
     file_mode: int = 0o664,
     file_write_delayed: bool = False,
     context_vars: dict = {},
     logger=None,
 ):
     """An asyn function that saves an image with metadata to file.
 
     Parameters
     ----------
     filepath : str
         local filepath to save the content to.
     imm : Image
         an image with metadata
-    file_format : {'hdf5', 'png'}
-        format to be used for saving the content.
+    file_format : {'hdf5', 'png', 'webp'}, optional
+        format to be used for saving the content. If not provided, it will be figured out from the
+        file extension.
     file_mode : int
         file mode to be set to using :func:`os.chmod`. If None is given, no setting of file mode
         will happen.
     file_write_delayed : bool
         Only valid in asynchronous mode and the format is 'json'. If True, wraps the file write
         task into a future and returns the future. In all other cases, proceeds as usual.
     context_vars : dict
@@ -167,55 +188,60 @@
 
     Returns
     -------
     int
         the number of bytes written to file
     """
 
+    if file_format is None:
+        ext = path.splitext(filepath)[1]
+        file_format = ext[1:]
+
     if file_format == "hdf5":
         return await cv.immsave_asyn(
             imm,
             filepath,
             file_format=file_format,
             file_mode=file_mode,
             file_write_delayed=file_write_delayed,
             image_codec="png",
             context_vars=context_vars,
             logger=logger,
         )
 
-    data = immencode(imm)
+    data = immencode(imm, encoding_format=file_format)
     return await aio.write_binary(
         filepath,
         data,
         file_mode=file_mode,
         file_write_delayed=file_write_delayed,
         context_vars=context_vars,
     )
 
 
 def immwrite(
     filepath: str,
     imm: cv.Image,
-    file_format: str = "hdf5",
+    file_format: tp.Optional[str] = None,
     file_mode: int = 0o664,
     file_write_delayed: bool = False,
     context_vars: dict = {},
     logger=None,
 ):
     """Saves an image with metadata to file.
 
     Parameters
     ----------
     filepath : str
         local filepath to save the content to.
     imm : Image
         an image with metadata
-    file_format : {'hdf5', 'png'}
-        format to be used for saving the content.
+    file_format : {'hdf5', 'png', 'webp'}, optional
+        format to be used for saving the content. If not provided, it will be figured out from the
+        file extension.
     file_mode : int
         file mode to be set to using :func:`os.chmod`. If None is given, no setting of file mode
         will happen.
     file_write_delayed : bool
         Only valid in asynchronous mode and the format is 'json'. If True, wraps the file write
         task into a future and returns the future. In all other cases, proceeds as usual.
     context_vars : dict
```

## mt/imageio/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('02')
-VERSION_DAY = int('01')
-VERSION_HOUR = int('20')
-VERSION_MINUTE = int('12')
+VERSION_MONTH = int('04')
+VERSION_DAY = int('29')
+VERSION_HOUR = int('06')
+VERSION_MINUTE = int('50')
 MAJOR_VERSION = 0
-MINOR_VERSION = 2
-PATCH_VERSION = 202302012012
-version_date = '2023/02/01 20:12'
+MINOR_VERSION = 3
+PATCH_VERSION = 202304290650
+version_date = '2023/04/29 06:50'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtimageio-0.2.202302012012.data/scripts/immview` & `mtimageio-0.3.202304290650.data/scripts/immview`

 * *Files identical despite different names*

## Comparing `mtimageio-0.2.202302012012.dist-info/LICENSE` & `mtimageio-0.3.202304290650.dist-info/LICENSE`

 * *Files identical despite different names*

