# Comparing `tmp/pdfsyntax-0.0.5.tar.gz` & `tmp/pdfsyntax-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfsyntax-0.0.5.tar", last modified: Fri Nov 18 20:29:14 2022, max compression
+gzip compressed data, was "pdfsyntax-0.0.6.tar", last modified: Sat Apr 29 16:37:13 2023, max compression
```

## Comparing `pdfsyntax-0.0.5.tar` & `pdfsyntax-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2022-11-18 20:29:14.396740 pdfsyntax-0.0.5/
--rw-r--r--   0 dej       (1000) dej       (1000)     1087 2022-09-29 21:26:33.000000 pdfsyntax-0.0.5/LICENSE
--rw-r--r--   0 dej       (1000) dej       (1000)     7702 2022-11-18 20:29:14.396740 pdfsyntax-0.0.5/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)     5642 2022-11-17 22:10:27.000000 pdfsyntax-0.0.5/README.md
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2022-11-18 20:29:14.387740 pdfsyntax-0.0.5/pdfsyntax/
--rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.0.5/pdfsyntax/__init__.py
--rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.0.5/pdfsyntax/__main__.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4636 2022-11-17 20:36:17.000000 pdfsyntax-0.0.5/pdfsyntax/api.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2896 2022-09-25 20:31:23.000000 pdfsyntax-0.0.5/pdfsyntax/cli.py
--rw-r--r--   0 dej       (1000) dej       (1000)     8229 2022-10-24 20:57:48.000000 pdfsyntax-0.0.5/pdfsyntax/display.py
--rw-r--r--   0 dej       (1000) dej       (1000)    11087 2022-11-13 18:38:03.000000 pdfsyntax-0.0.5/pdfsyntax/docstruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)    14258 2022-11-17 22:12:40.000000 pdfsyntax-0.0.5/pdfsyntax/filestruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)     1389 2022-11-13 19:16:33.000000 pdfsyntax-0.0.5/pdfsyntax/filters.py
--rw-r--r--   0 dej       (1000) dej       (1000)     7555 2022-11-13 17:39:14.000000 pdfsyntax-0.0.5/pdfsyntax/objects.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2660 2022-11-13 18:21:05.000000 pdfsyntax-0.0.5/pdfsyntax/text.py
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2022-11-18 20:29:14.396740 pdfsyntax-0.0.5/pdfsyntax.egg-info/
--rw-r--r--   0 dej       (1000) dej       (1000)     7702 2022-11-18 20:29:14.000000 pdfsyntax-0.0.5/pdfsyntax.egg-info/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)      370 2022-11-18 20:29:14.000000 pdfsyntax-0.0.5/pdfsyntax.egg-info/SOURCES.txt
--rw-r--r--   0 dej       (1000) dej       (1000)        1 2022-11-18 20:29:14.000000 pdfsyntax-0.0.5/pdfsyntax.egg-info/dependency_links.txt
--rw-r--r--   0 dej       (1000) dej       (1000)       10 2022-11-18 20:29:14.000000 pdfsyntax-0.0.5/pdfsyntax.egg-info/top_level.txt
--rw-r--r--   0 dej       (1000) dej       (1000)      923 2022-11-18 20:25:52.000000 pdfsyntax-0.0.5/pyproject.toml
--rw-r--r--   0 dej       (1000) dej       (1000)       38 2022-11-18 20:29:14.396740 pdfsyntax-0.0.5/setup.cfg
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2023-04-29 16:37:13.375827 pdfsyntax-0.0.6/
+-rw-r--r--   0 dej       (1000) dej       (1000)     1087 2022-09-29 21:26:33.000000 pdfsyntax-0.0.6/LICENSE
+-rw-r--r--   0 dej       (1000) dej       (1000)     8594 2023-04-29 16:37:13.375827 pdfsyntax-0.0.6/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)     6534 2023-04-20 20:00:07.000000 pdfsyntax-0.0.6/README.md
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2023-04-29 16:37:13.370828 pdfsyntax-0.0.6/pdfsyntax/
+-rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.0.6/pdfsyntax/__init__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.0.6/pdfsyntax/__main__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     5620 2023-04-23 20:37:53.000000 pdfsyntax-0.0.6/pdfsyntax/api.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4459 2023-04-28 21:43:02.000000 pdfsyntax-0.0.6/pdfsyntax/cli.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     9195 2023-04-24 21:55:07.000000 pdfsyntax-0.0.6/pdfsyntax/display.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    16641 2023-04-28 20:43:58.000000 pdfsyntax-0.0.6/pdfsyntax/docstruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    18703 2023-04-29 16:21:12.000000 pdfsyntax-0.0.6/pdfsyntax/filestruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     1726 2023-04-26 19:48:07.000000 pdfsyntax-0.0.6/pdfsyntax/filters.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     8495 2023-04-26 20:07:10.000000 pdfsyntax-0.0.6/pdfsyntax/objects.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2829 2023-04-20 21:05:35.000000 pdfsyntax-0.0.6/pdfsyntax/text.py
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2023-04-29 16:37:13.371827 pdfsyntax-0.0.6/pdfsyntax.egg-info/
+-rw-r--r--   0 dej       (1000) dej       (1000)     8594 2023-04-29 16:37:13.000000 pdfsyntax-0.0.6/pdfsyntax.egg-info/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)      580 2023-04-29 16:37:13.000000 pdfsyntax-0.0.6/pdfsyntax.egg-info/SOURCES.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)        1 2023-04-29 16:37:13.000000 pdfsyntax-0.0.6/pdfsyntax.egg-info/dependency_links.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)       10 2023-04-29 16:37:13.000000 pdfsyntax-0.0.6/pdfsyntax.egg-info/top_level.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)      923 2023-04-29 16:28:15.000000 pdfsyntax-0.0.6/pyproject.toml
+-rw-r--r--   0 dej       (1000) dej       (1000)       38 2023-04-29 16:37:13.375827 pdfsyntax-0.0.6/setup.cfg
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2023-04-29 16:37:13.374827 pdfsyntax-0.0.6/tests/
+-rw-r--r--   0 dej       (1000) dej       (1000)      884 2023-03-19 22:00:22.000000 pdfsyntax-0.0.6/tests/test_bdata.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      701 2023-04-13 21:52:11.000000 pdfsyntax-0.0.6/tests/test_dependencies.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2037 2023-04-13 21:22:18.000000 pdfsyntax-0.0.6/tests/test_parsing.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      303 2022-09-13 20:49:14.000000 pdfsyntax-0.0.6/tests/test_serialization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      454 2023-04-16 15:12:06.000000 pdfsyntax-0.0.6/tests/test_simplefile.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     1044 2023-04-20 21:04:55.000000 pdfsyntax-0.0.6/tests/test_text.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2231 2022-09-12 20:00:26.000000 pdfsyntax-0.0.6/tests/test_tokenization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      355 2022-09-24 21:06:18.000000 pdfsyntax-0.0.6/tests/test_updating.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      542 2023-04-02 20:58:32.000000 pdfsyntax-0.0.6/tests/test_xref.py
```

### Comparing `pdfsyntax-0.0.5/LICENSE` & `pdfsyntax-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.5/PKG-INFO` & `pdfsyntax-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python PDF parsing library and tool built on top to browse the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin D. <desgeeko@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -105,17 +105,17 @@
 ### File information
 
 `structure` and `metadata` are functions showing general information about the document.
 
 ```Python
 >>> #File structure
 >>> structure(doc)
-{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
->>> #File structure
+>>> #File metadata
 >>> metadata(doc)
 {'Title': None, 'Author': None, 'Subject': None, 'Keywords': None, 'Creator': None, 'Producer': None, 'CreationDate': None, 'ModDate': None}
 ```
 
 ### Low-level access to object tree
 
 `trailer` and `catalog` give access to the starting point of the object tree. 
@@ -138,23 +138,47 @@
 ```Python
 >>> #Access to document catalog, given that the trailer redirects to 1j for root
 >>> #(equivalent to catalog fonction)
 >>> doc.get_object(1j)
 {'/Pages': 3j, '/Outlines': 2j, '/Type': '/Catalog'}
 ```
 
+### Pages
+
+Page index is a tree structure where attributes can be inherited from parent nodes. For convenience `flat_page_tree` returns an ordered list of document pages and specifies inherited attributes that should apply to each page.
+
+```Python
+>>> #Each item of the list is a tuple with the page object reference and its inherited attributes
+>>> doc = pdf.read("samples/simple_text_string.pdf")
+>>> pdf.flat_page_tree(doc)
+[(4j, {})]
+>>> #(In this example, nothing is inherited from upper nodes)
+```
+
+The `page` function goes further by merging inherited attributes with local attributes of each page and giving the result in a list.
+
+```Python
+>>> #Equivalent list with computed page attribues
+>>> pdf.pages(doc)
+[{'/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j},
+  '/Contents': 5j,
+  '/MediaBox': [0, 0, 612, 792],
+  '/Parent': 3j,
+  '/Type': '/Page'}]
+```
+
 ### Incremental updates
 
 PDFSyntax tracks document incremental updates made possible by appending new or updated objects at the end of an original PDF file (and the matching XREF section). The `Revisions` entry of the `structure` function result, if greater than 1, indicates that incremental updates have been appended. By default, a newly opened document by PDFSyntax is ready to write modifications in the next revision. The `rewind` function rolls back to the previous revision. 
 
 ```Python
 >>> import pdfsyntax as pdf
 >>> doc = pdf.read("samples/add_text_annotation.pdf")
 >>> doc.structure()
-{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
 >>> #This file contains 2 revisions and PDFSyntax has initialized the doc object for a future revision 3
 
 >>> doc.get_object(4j)
 {'/Annots': 8j, '/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j}, '/Contents': 5j, '/MediaBox': [0, 0, 612, 792], '/Parent': 3j, '/Type': '/Page'}
 
 >>> #In its current state, the page (object 4) contains an annotation
```

### Comparing `pdfsyntax-0.0.5/README.md` & `pdfsyntax-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 ### File information
 
 `structure` and `metadata` are functions showing general information about the document.
 
 ```Python
 >>> #File structure
 >>> structure(doc)
-{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
->>> #File structure
+>>> #File metadata
 >>> metadata(doc)
 {'Title': None, 'Author': None, 'Subject': None, 'Keywords': None, 'Creator': None, 'Producer': None, 'CreationDate': None, 'ModDate': None}
 ```
 
 ### Low-level access to object tree
 
 `trailer` and `catalog` give access to the starting point of the object tree. 
@@ -97,23 +97,47 @@
 ```Python
 >>> #Access to document catalog, given that the trailer redirects to 1j for root
 >>> #(equivalent to catalog fonction)
 >>> doc.get_object(1j)
 {'/Pages': 3j, '/Outlines': 2j, '/Type': '/Catalog'}
 ```
 
+### Pages
+
+Page index is a tree structure where attributes can be inherited from parent nodes. For convenience `flat_page_tree` returns an ordered list of document pages and specifies inherited attributes that should apply to each page.
+
+```Python
+>>> #Each item of the list is a tuple with the page object reference and its inherited attributes
+>>> doc = pdf.read("samples/simple_text_string.pdf")
+>>> pdf.flat_page_tree(doc)
+[(4j, {})]
+>>> #(In this example, nothing is inherited from upper nodes)
+```
+
+The `page` function goes further by merging inherited attributes with local attributes of each page and giving the result in a list.
+
+```Python
+>>> #Equivalent list with computed page attribues
+>>> pdf.pages(doc)
+[{'/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j},
+  '/Contents': 5j,
+  '/MediaBox': [0, 0, 612, 792],
+  '/Parent': 3j,
+  '/Type': '/Page'}]
+```
+
 ### Incremental updates
 
 PDFSyntax tracks document incremental updates made possible by appending new or updated objects at the end of an original PDF file (and the matching XREF section). The `Revisions` entry of the `structure` function result, if greater than 1, indicates that incremental updates have been appended. By default, a newly opened document by PDFSyntax is ready to write modifications in the next revision. The `rewind` function rolls back to the previous revision. 
 
 ```Python
 >>> import pdfsyntax as pdf
 >>> doc = pdf.read("samples/add_text_annotation.pdf")
 >>> doc.structure()
-{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
 >>> #This file contains 2 revisions and PDFSyntax has initialized the doc object for a future revision 3
 
 >>> doc.get_object(4j)
 {'/Annots': 8j, '/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j}, '/Contents': 5j, '/MediaBox': [0, 0, 612, 792], '/Parent': 3j, '/Type': '/Page'}
 
 >>> #In its current state, the page (object 4) contains an annotation
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/api.py` & `pdfsyntax-0.0.6/pdfsyntax/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,16 +35,19 @@
     }
 
 
 def init_doc(fdata: Callable) -> tuple:
     """Initialize doc object representing PDF file"""
     chrono = build_chrono_from_xref(fdata)
     index = build_index_from_chrono(chrono)
+    data = build_data_from_cache(index, fdata)
+    for i in index:
+        del i[-1]
     cache = build_cache(fdata, index)
-    doc = Doc(fdata, index, cache)
+    doc = Doc(index, cache, data)
     return doc, chrono
 
 
 #def load(fp) -> Doc:
 #    """ """
 #    bdata = fp.read()
 #    doc, _ = init_doc(bdata)
@@ -55,113 +58,139 @@
 #def loads(bdata) -> Doc:
 #    """ """
 #    doc, _ = init_doc(bdata)
 #    doc = add_version(doc)
 #    return doc
 
 
-def read(filename: str) -> Doc:
+def read(filename: str, mode: str = "SINGLE") -> Doc:
     """Read file and initialize doc"""
     #bfile = open(filename, 'rb')
     #bdata = bfile.read()
     #bfile.close()
-    fdata = bdata_provider(filename)
+    fdata = bdata_provider(filename, mode)
     doc, _ = init_doc(fdata)
     doc = add_revision(doc)
     return doc
 
 
 def write(doc: Doc, filename: str) -> Doc:
     """Write doc into file"""
     bdata = b''
     idx = 0
+    doc = add_revision(doc)
     nb_rev = len(doc.index)
     eof_rev = -1
     for i in range(nb_rev):
-        if doc.index[i][-1]:
+        if 'eof_cut' in doc.data[i]:
             eof_rev = i
         else:
             break
     if eof_rev >= 0:
-        eof_pos = doc.index[eof_rev][-1]['abs_pos']
-        prov = doc.bdata(0, eof_pos+4)
-        bdata += prov[0][prov[1]:eof_pos+5]
-        bdata += b'\n'
+        eof_cut = doc.data[eof_rev]['eof_cut']
+        prov = doc.data[0]['fdata'](0, eof_cut)
+        bdata += prov[0][prov[1]:eof_cut]
         idx += len(bdata)
     else:
         FILE_HEADER = b'%PDF-' + version(doc).encode('ascii') + b'\n'
         bdata += FILE_HEADER
         idx += len(FILE_HEADER)
-    for i in range(eof_rev+1, nb_rev):
-        prep = prepare_revision(doc, i, idx)
-        bdata += prep
-        idx += len(prep)
+    for i in range(eof_rev+1, nb_rev-1):
+        fragment = doc.data[i]['bdata']
+        bdata += fragment
+        idx += len(fragment)
     bfile = open(filename, 'wb')
     bfile.write(bdata)
     bfile.close()
     return doc
 
 
 def structure(doc: Doc) -> dict:
     """Return various doc attributes (other than metadata)"""
     ret = {}
     ret['Version'] = version(doc)
     ret['Pages'] = number_pages(doc)
     ret['Revisions'] = updates(doc)
     ret['Encrypted'] = encrypted(doc)
-    ret['Paper'] = paper(page_layouts(doc)[0][0]) #TODO handle hybrid docs
+    ret['Hybrid'] = hybrid(doc)
+    if linearized(doc.data[0]['fdata']):
+        ret['Linearized'] = True
+    else:
+        ret['Linearized'] = False
+    ret['Paper of 1st page'] = paper(page_layouts(doc, 1)[0][0])
     return ret
 
 
 def metadata(doc: Doc) -> dict:
     """Return doc metadata"""
     ret = {}
     i = info(doc) or {}
     for entry in METADATA_ATTRS:
-        ret[entry[1:]] = text_string(i.get(entry)) or None    
-    ret['CreationDate'] = text_string(i.get('/CreationDate')) or None
-    ret['ModDate'] = text_string(i.get('/ModDate')) or None
+        ret[entry[1:]] = text_string(get_object(doc, i.get(entry))) or None
+    ret['CreationDate'] = text_string(get_object(doc, i.get('/CreationDate'))) or None
+    ret['ModDate'] = text_string(get_object(doc, i.get('/ModDate'))) or None
     return ret 
 
 
 def paper(mediabox: list) -> str:
     """Detect paper size"""
     x, y = mediabox[2] - mediabox[0], mediabox[3] - mediabox[1]
     ptype = PAPER_SIZES.get((x, y)) or PAPER_SIZES.get((y, x)) or "unknown"
     pdim = f'{int(x*25.4/72)}x{int(y*25.4/72)}mm or {round(x/72, 2)}x{round(y/72, 2)}in'
     return pdim + f' ({ptype})'
 
 
-def page_layouts(doc: Doc) -> list:
+def page_layouts(doc: Doc, max_nb=None) -> list:
     """List page layouts"""
-    pl = pages(doc)
+    pl = pages(doc, max_nb)
     med = [(p['/MediaBox'], p.get('/Rotate')) for p in pl]
     return med
 
 
 def rotate(doc: Doc, degrees: int = 90, pages: list = []) -> Doc:
     """Rotate 1 or several pages"""
     pl = page_layouts(doc)
     if pages:
         work_pages = pages
     else:
         work_pages = list(range(len(pl)))
     a = [(i ,x[1]) for i, x in enumerate(pl) if i in work_pages]
-    c = collect_inherited_attr_pages(doc)
+    c = flat_page_tree(doc)
     for nb, old_degrees in a:
         old_degrees = old_degrees or 0
         iref = c[nb][0]
         obj = deepcopy(get_object(doc, iref))
         obj['/Rotate'] = (old_degrees + degrees) % 360
         doc = update_object(doc, int(iref.imag), obj)
     return doc
 
 
+def single_text_annotation(doc: Doc, page_num: int, text: str) -> Doc:
+    """Add simple text annotation"""
+    annot = {
+        '/Type': '/Annot',
+        '/Subtype': '/Text',
+        '/Rect': [50, 50, 150, 150],
+        '/Contents': f"({text})",
+        '/Open': False,
+    }
+    doc, a_iref = add_object(doc, annot)
+    annot_array = [a_iref]
+    doc, aa_iref = add_object(doc, annot_array)
+    page_ref, _ = flat_page_tree(doc)[page_num]
+    new_page = deepcopy(get_object(doc, page_ref))
+    new_page['/Annots'] = aa_iref
+    doc = update_object(doc, int(page_ref.imag), new_page)
+    return doc
+
+
 Doc.trailer = trailer
 Doc.catalog = catalog
 Doc.metadata = metadata
 Doc.structure = structure
 Doc.get_object = get_object
 Doc.rewind = rewind
 Doc.rotate = rotate
 Doc.page_layouts = page_layouts
+Doc.flat_page_tree = flat_page_tree
+Doc.pages = pages
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/display.py` & `pdfsyntax-0.0.6/pdfsyntax/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module pdfsyntax.display: pretty print the PDF file structure as HTML"""
 
 import html
 from .objects import Stream
 
 NAME_MAX_WIDTH = 20
-VALUE_MAX_WIDTH = 40
+VALUE_MAX_WIDTH = 30
 
 HEADER = '''
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
@@ -73,15 +73,14 @@
 '''
 
 TRUNCATED = '<em> ...(truncated) </em>'
 
 
 def build_html(articles: list, pos_index: dict, nb_ver: int, filename: str, version: bytes) -> str:
     """Compose the page layout"""
-    #print(articles)
     page = HEADER
     page += build_header(filename, nb_ver, version)
     for article in articles:
         obj_attr = (article['o_num'], article['o_gen'], article['o_ver'])
         obj = article['content']
         if obj_attr[0] == -2:
             page += add_startxref(article, pos_index)
@@ -90,15 +89,19 @@
             page += add_eof(article)
             continue
         page += build_obj_header(article)
         mini_index = article['mini_index']
         if 'xref_table' in article:
             page += build_xref_table(article['xref_table'], mini_index)
             page += "\ntrailer\n"
-        page += follow_obj(obj, mini_index, pos_index)
+        if 'xref_stream' in article:
+            page += follow_obj(obj['entries'], mini_index, pos_index)
+            page += build_xref_stream(article['xref_stream'], mini_index)
+        else:
+            page += follow_obj(obj, mini_index, pos_index)
         page += build_obj_trailer()
     page += TRAILER
     return page
 
 def build_header(filename: str, nb_ver: int, version: bytes) -> str:
     """Add a banner with the file name"""
     ret = ''
@@ -145,14 +148,28 @@
             ret += '    '
             ret += f'<a href="#obj{o_num}.{o_gen}.{o_ver}">'
             ret += f'<span class="obj-link">#{o_num} {o_gen}</span>'
             ret += '</a>'
         ret += '\n'
     return ret
 
+def build_xref_stream(table: list, mini_index: list) -> str:
+    """Display XREF stream with additional links to objects """
+    ret = '\nstream\n'
+    for line, o_num in table:
+        ret += line.decode('ascii')
+        if o_num != None:
+            o_gen, o_ver = mini_index[o_num]
+            ret += '    '
+            ret += f'<a href="#obj{o_num}.{o_gen}.{o_ver}">'
+            ret += f'<span class="obj-link">#{o_num} {o_gen}</span>'
+            ret += '</a>'
+        ret += '\n'
+    return ret
+
 def move_list_item(mod_list: list, item: int, new_pos: int) -> str:
     """Reposition an item in a list"""
     if item in mod_list:
         old_pos = mod_list.index(item)
         mod_list.pop(old_pos)
         mod_list.insert(new_pos, item)
     return mod_list
@@ -182,20 +199,20 @@
             ret += ' ' * (NAME_MAX_WIDTH + 2) * depth
             if name == '/Type' or name == '/Subtype':
                 ret += f'  {name:{NAME_MAX_WIDTH}}<span class="important">{value}</span>\n'
             elif name == '/Prev':
                 ret += f'  {name:{NAME_MAX_WIDTH}}<a class="obj-link" href="#obj{pos_index[int(value)]}">{value}</a>\n'                
             else:
                 ret += f'  {name:{NAME_MAX_WIDTH}}{value}\n'
+        ret += ' ' * (NAME_MAX_WIDTH + 2) * depth
+        ret += '>>'
         if content:
             content = f'{content}'[2:-1]
             content = content[:VALUE_MAX_WIDTH * 2] + TRUNCATED
-            ret += f'  {"stream":{NAME_MAX_WIDTH}}{content}\n'                
-        ret += ' ' * (NAME_MAX_WIDTH + 2) * depth
-        ret += '>>'
+            ret += f'  \n{"stream":{NAME_MAX_WIDTH}}\n{content}\n'
     elif type(obj) == list:
         ret += '[ '
         for i in obj:
             value = follow_obj(i, mini_index, pos_index)
             ret += f'{value} '
         if len(ret) > VALUE_MAX_WIDTH and 'href' not in ret:
             ret = ret[:VALUE_MAX_WIDTH] + TRUNCATED
@@ -225,19 +242,23 @@
     o_num, o_gen, o_ver = article['o_num'], article['o_gen'], article['o_ver']
     ret = ''
     ret += f'<div id="obj{o_num}.{o_gen}.{o_ver}">\n<pre>\n\n\n'
     if o_num == 0:
         ret += f'<span class="obj-header"><strong>XREF table & trailer</strong></span>'
         ret += f'<em class="obj-low">  at offset {article.get("abs_pos")}</em>'
     else:
-        ret += f'<span class="obj-header"><strong>{o_num}</strong> <span class="obj-low">{o_gen} obj</span></span>'
-        if 'a_' not in article:
-            ret += f'<em class="obj-low">  at offset {article.get("abs_pos")}</em>'
+        if 'xref_stream' in article:
+            ret += f'<span class="obj-header"><strong>{o_num}</strong> <span class="obj-low">{o_gen} obj</span></span>'
+            ret += f'<em class="obj-low">  as XREF stream object at offset {article.get("abs_pos")}</em>'
         else:
-            ret += f'<em class="obj-low">  from object stream {article.get("env_num")} above</em>'
+            ret += f'<span class="obj-header"><strong>{o_num}</strong> <span class="obj-low">{o_gen} obj</span></span>'
+            if 'a_' not in article:
+                ret += f'<em class="obj-low">  at offset {article.get("abs_pos")}</em>'
+            else:
+                ret += f'<em class="obj-low">  from object stream {article.get("env_num")} above</em>'
     ret += f'<div class="obj-body">\n'
     return ret
 
 def build_obj_trailer() -> str:
     """Add closing elements to object"""
     ret = ''
     ret += f'</div>\n'
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/docstruct.py` & `pdfsyntax-0.0.6/pdfsyntax/docstruct.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import namedtuple
 from copy import deepcopy
 
 
 INHERITABLE_ATTRS = '/Resources /MediaBox /CropBox /Rotate'.split()
 
 
-Doc = namedtuple('Doc', 'bdata index cache')
+Doc = namedtuple('Doc', 'index cache data')
 
 class Doc(Doc):
     def __repr__(self):
         res = "<PDF Doc"
         res += f" with "
         i = len(self.index)
         if not changes(self):
@@ -26,15 +26,15 @@
         else:
             res += f", current update/revision containing {len(changes(self))} modifications"
         if self.cache:
             present = 0
             for i in range(1, len(self.index[-1])-1):
                 if self.cache[i] is not None:
                     present += 1 
-            res += f", cache loaded with {present} / {len(self.cache)-2} objects>\n"
+            res += f", cache loaded with {present} / {len(self.cache)-1} objects>\n"
         else:
             res += f", cache=None>\n"
         return res
 
 EOL = b'\r\n'
 SPACE = EOL + b'\x00\x09\x0c\x20'
 
@@ -43,139 +43,152 @@
     """Parse indirect object whose number is [key] and return a cache filled at index [key]
     cache argument may be:
     - a list that is updated,
     - or None that is replaced with an empty list
     """
     if cache is None:
         cache = (key + 1) * [None]
+    if 'DELETED' in idx[rev][key]:
+        return cache
     if  cache[key] != None:
         return cache
     if key == 0:
         index = idx[rev][key]
         if type(index) != list:
             indexes = [index]
         else:
             indexes = index
         obj = {}
         for index in indexes:
-            bdata, a0, _ = fdata(index['abs_pos'], index['abs_next'] - index['abs_pos'])
+            bdata, a0, _, _ = fdata(index['abs_pos'], index['abs_next'] - index['abs_pos'])
             i, j, _ = next_token(bdata, a0)
             i, j, _ = next_token(bdata, j)
             if 'xref_stream' in index:
                 i, j, _ = next_token(bdata, j)
                 i, j, _ = next_token(bdata, j)
             text = bdata
             i_obj = parse_obj(text, i)
             if type(i_obj) == Stream:
                 i_obj = i_obj['entries']
             obj.update(i_obj)
         cache[key] = obj    
     elif 'env_num' not in idx[rev][key]:
-        bdata, a0, _ = fdata(idx[rev][key]['abs_pos'], idx[rev][key]['abs_next'] - idx[rev][key]['abs_pos'])
+        bdata, a0, _, _ = fdata(idx[rev][key]['abs_pos'], idx[rev][key]['abs_next'] - idx[rev][key]['abs_pos'])
         i, j, _ = next_token(bdata, a0)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         text = bdata
         obj = parse_obj(text, i)
         if key == 0 and type(obj) == Stream:
             obj = obj['entries']
         cache[key] = obj    
     else:
         container = idx[rev][key]['env_num']
-        bdata, a0, _ = fdata(idx[rev][container]['abs_pos'], idx[rev][container]['abs_next'] - idx[rev][container]['abs_pos'])
+        bdata, a0, _, _ = fdata(idx[rev][container]['abs_pos'], idx[rev][container]['abs_next'] - idx[rev][container]['abs_pos'])
         i, j, _ = next_token(bdata, a0)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         text = bdata
         c_obj = parse_obj(text, i)
+        if container > key:
+            cache += (container-key) * [None]
         cache[container] = c_obj
         offset = int(c_obj['entries']['/First'])
         nb_obj = int(c_obj['entries']['/N'])
         x_array = parse_obj(b'[' + c_obj['stream'][:offset] + b']')
         for x in range(nb_obj):
+            if int(x_array[2 * x]) >= len(cache):
+                cache += (int(x_array[2 * x])-len(cache)+1) * [None]
             cache[int(x_array[2 * x])] = parse_obj(c_obj['stream'], offset + int(x_array[2 * x + 1]))
         if key == 0 and type(cache[0]) == Stream:
             cache[0] = cache[0]['entries']
     return cache
 
 
 def get_object(doc: Doc, obj):
     """Return raw object or the target of an indirect reference"""
     if isinstance(obj, complex) == True:
         ref = int(obj.imag)
-        res = memoize_obj_in_cache(doc.index, doc.bdata, ref, doc.cache)
-        return res[ref]
+        res = memoize_obj_in_cache(doc.index, doc.data[-1]['fdata'], ref, doc.cache)
+        return deepcopy(res[ref])
     else: 
-        return obj
+        return deepcopy(obj)
 
 
-def follow_pages_rec(doc: Doc, num, inherited={}) -> list:
+def flat_page_tree(doc: Doc, num=None, inherited={}, max_nb=None) -> list:
     """Recursively list the pages of a node"""
     accu = []
-    node = get_object(doc, num)
+    if num:
+        node = get_object(doc, num)
+    else:
+        node = get_object(doc, catalog(doc)['/Pages'])
     if node['/Type'] == '/Pages':
         for kid in node['/Kids']:
             e = {k: node.get(k) for k in INHERITABLE_ATTRS if node.get(k) is not None}
             inherited.update(e)
-            accu = accu + follow_pages_rec(doc, kid, inherited.copy())
+            accu = accu + flat_page_tree(doc, kid, inherited.copy(), max_nb)
+            if max_nb is not None and len(accu) == max_nb:
+                return accu
         return accu
     elif node['/Type'] == '/Page':
         return[(num, inherited)]
 
 
-def build_cache(bdata: Callable, index: list) -> list:
-    """Initialize cache with trailer and Root"""
+def build_cache(fdata: Callable, index: list) -> list:
+    """Initialize cache with trailer"""
     size = len(index[-1])
     cache = size * [None]
-    memoize_obj_in_cache(index, bdata, 0, cache)
+    memoize_obj_in_cache(index, fdata, 0, cache)
     return cache
 
 
 def changes(doc: Doc, rev: int=-1):
     """List deleted/updated/added objects"""
     res = []
     current = doc.index[rev]
     if len(doc.index) == 1:
         previous = [None] * len(current)
     else:
         previous = doc.index[rev-1]
-    ver = len(doc.index)-1
-    for i in range(1, len(current)-1):
-        if i < len(previous) - 1 and previous[i] == current[i]:
-            continue
-        elif previous[i] != None and current[i] == None:
+    for i in range(1, len(current)):
+        if i > len(previous)-1:
+            res.append((i, 'a'))
+        elif i < len(previous) and previous[i] == current[i]:
+            pass
+        elif previous[i] != None and 'DELETED' not in previous[i] and 'DELETED' in current[i]:
             res.append((i, 'd'))
         elif previous[i] != None and current[i] != previous[i]:
             res.append((i, 'u'))
         else:
             res.append((i, 'a'))
     return res
 
 
 def group_obj_into_stream(doc: Doc):
     """Provision a ObjStm object and tag all changes to target this envelope"""
-    doc2 = add_object(doc, b'')
+    doc2, _ = add_object(doc, b'')
     current = doc2.index[-1]
     o_num = current[-2]['o_num']
     chgs = changes(doc)
     for i, _ in chgs:
         if i == o_num:
-            print("continue")
+            #print("continue")
             continue
         current[i]['env_num'] = o_num
     d = {'/Type': '/ObjStm', '/Length': 0, '/N': 0, '/First': 0, '/FirstLine': []}
     doc2.cache[o_num] = Stream(d, b'')
     return doc2
 
 
 def version(doc: Doc) -> str:
     """Return PDF version"""
-    bdata, a0, _ = doc.bdata(5, 3)
+    fdata = doc.data[0]['fdata']
+    bdata, a0, _, _ = fdata(5, 3)
     ver = bdata[a0:a0+3]
     cat = catalog(doc)
     if '/Version' in cat and cat['/Version'] > ver.decode('ascii'):
             return cat['/Version'].decode('ascii')
     return ver.decode('ascii')
 
 
@@ -196,14 +209,22 @@
     encrypt = trail.get('/Encrypt')
     if encrypt:
         return True
     else:
         return False
 
 
+def hybrid(doc: Doc) -> bool:
+    """Detect if doc is hybrid"""
+    if len(doc.index) >= 2 and doc.index[1][0].get('xref_stm'):
+        return True
+    else:
+        return False
+
+
 def catalog(doc: Doc):
     """Return doc Root/Catalog dictionary"""
     return get_object(doc, trailer(doc)['/Root'])
 
 
 def info(doc: Doc):
     """Return doc Info dictionary if present"""
@@ -215,109 +236,251 @@
 
 def number_pages(doc: Doc):
     """Return doc number of pages"""
     p = get_object(doc, catalog(doc)['/Pages'])
     return p['/Count']
 
 
-def collect_inherited_attr_pages(doc: Doc) -> list:
-    """List pages with applied inherited attributes"""
-    p = get_object(doc, catalog(doc)['/Pages'])
-    page_index = follow_pages_rec(doc, p)
-    return page_index
-
-
-def pages(doc: Doc) -> list:
+def pages(doc: Doc, max_nb=None) -> list:
     """ """
     pl = []
-    for num, in_attr in collect_inherited_attr_pages(doc):
+    for num, in_attr in flat_page_tree(doc, max_nb=max_nb):
         temp = deepcopy(get_object(doc, num))
         for a in in_attr:
             if a not in temp:
                 temp[a] = in_attr[a]
         pl.append(temp)
     return pl
 
 
+def revision_index(doc: Doc, rev=-1) -> int:
+    index = 0
+    if rev == -1:
+        rev = len(doc.data)-1
+    for i in range(rev):
+        data = doc.data[i]
+        if 'eof_cut' in data:
+            index = data['eof_cut']
+        else:
+            index += len(data['bdata'])
+    return index
+
+
+def gen_fdata(fdata: Callable, index: int, bdata: bytes):
+    def new_fdata(start_pos: int, length: int) -> tuple:
+        if start_pos > index:
+            start_pos = start_pos - index
+            if start_pos == -1 and length == 0:
+                return (None, None, None, len(bdata))
+            if length == -1:
+                length = len(bdata) - start_pos
+            if start_pos == -1:
+                i = len(bdata) - length
+            else:
+                i = start_pos
+            return (bdata, i, 0, min(len(bdata) - start_pos, length))
+        else:
+            return fdata(start_pos, length)
+    return new_fdata
+
+
 def add_revision(doc: Doc) -> Doc:
     """Add new index for incremental update"""
     if len(changes(doc)) == 0:
         return doc
     ver = len(doc.index)
     current_v = doc.index[-1]
     new_cache = len(current_v) * [None]
     new_trailer = doc.cache[0].copy()
-    new_trailer['/Prev'] = current_v[0].get('xref_table_pos') or current_v[0].get('xref_stream_pos')
+    if type(current_v[0]) == list: #Linearized
+        new_trailer['/Prev'] = current_v[0][1].get('xref_table_pos') or current_v[0][1].get('xref_stream_pos')
+    else:
+        new_trailer['/Prev'] = current_v[0].get('xref_table_pos') or current_v[0].get('xref_stream_pos')
     new_cache[0] = new_trailer
     new_index = doc.index.copy()
     new_trailer = {'o_num': 0, 'o_gen': 0, 'o_ver': ver, 'doc_ver': ver}
-    new_v = [new_trailer] + [current_v[i] for i in range(1,len(current_v)-1)] + [None] 
+    new_data = doc.data.copy()
+    if 'eof_cut' not in new_data[-1]:
+        idx = revision_index(doc)
+        new_bdata, new_i = prepare_revision(doc, idx=idx)
+        if new_bdata:
+            new_data[-1]['bdata'] = new_bdata
+            new_data[-1]['fdata'] = gen_fdata(new_data[-1]['fdata'], idx, new_bdata)
+        new_index[-1] = new_i
+    new_data.append({'fdata': new_data[-1]['fdata']})
+    new_v = [new_trailer] + [new_index[-1][i] for i in range(1,len(new_index[-1]))] 
     new_index.append(new_v)
-    return Doc(doc.bdata, new_index, new_cache)
+    return Doc(new_index, new_cache, new_data)
 
 
-def prepare_revision(doc: Doc, rev:int = -1, idx:int = 0) -> bytes:
+def prepare_revision(doc: Doc, rev:int = -1, idx:int = 0) -> tuple:
     """Build bytes representing incremental update"""
-    res = b''
     chg = changes(doc, rev)
-    if doc.index[rev][-1] or not chg:
-        return res
+    if not chg:
+        return b''
     for num, _ in chg:
-        memoize_obj_in_cache(doc.index, doc.bdata, num, doc.cache, rev=-1)
-    fragments = build_fragments_and_xref(chg, doc.index[rev], doc.cache, idx, version(doc))
-    for f in fragments:
-        res += f
-    return res
+        memoize_obj_in_cache(doc.index, doc.data[rev]['fdata'], num, doc.cache, rev=-1)
+    if version(doc) < '1.5':
+        use_xref_stream = False
+    else:
+        use_xref_stream = True
+    fragments, new_index = build_fragment_and_xref(chg, doc.index[rev], doc.cache, idx, use_xref_stream)
+    return fragments, new_index
 
 
 def rewind(doc: Doc) -> Doc:
     """Go back to previous revision"""
     if len(doc.index) == 1:
         return doc
     new_index = doc.index.copy()
     new_index.pop()
-    new_current = new_index[-1].copy()
-    #new_current[-1] = None
-    new_index[-1] = new_current
-    new_cache = build_cache(doc.bdata, new_index)
-    return Doc(doc.bdata, new_index, new_cache)
+    new_index[-1] = new_index[-1].copy()
+    new_cache = build_cache(doc.data[-2]['fdata'], new_index)
+    new_data = doc.data[0:-1]
+    return Doc(new_index, new_cache, new_data)
+
+
+def copy_doc(doc: Doc) -> Doc:
+    """ """
+    new_index = doc.index.copy()
+    new_index[-1] = doc.index[-1].copy()
+    new_cache = doc.cache.copy()
+    return Doc(new_index, new_cache, doc.data)
 
 
 def update_object(doc: Doc, num: int, new_o) -> Doc:
     """Update object in the current revision"""
-    #if doc.index[-1][-1]:
-    #    doc = add_version(doc)
     ver = len(doc.index)
     old_i = doc.index[-1][num]
-    new_i = {'o_num': num, 'o_gen': old_i['o_gen'], 'o_ver': old_i['o_ver']+1, 'doc_ver': ver-1}
-    new_index = doc.index.copy()
-    new_index[-1] = doc.index[-1].copy()
-    new_index[-1][-1] = None
-    new_index[-1][num] = new_i
-    new_cache = doc.cache.copy()
-    new_cache[num] = new_o
-    return Doc(doc.bdata, new_index, new_cache)
+    if new_o is None:
+        new_i = {'o_num': num, 'o_gen': old_i['o_gen'], 'o_ver': old_i['o_ver']+1, 'doc_ver': ver-1, 'DELETED': True}
+    else:
+        new_i = {'o_num': num, 'o_gen': old_i['o_gen'], 'o_ver': old_i['o_ver']+1, 'doc_ver': ver-1}
+    new_doc = copy_doc(doc)
+    new_doc.index[-1][num] = new_i
+    new_doc.cache[num] = new_o
+    return new_doc
 
 
-def add_object(doc: Doc, new_o) -> Doc:
+def add_object(doc: Doc, new_o) -> tuple:
     """Add new object at the end of current index"""
     if doc.index[-1][-1]:
         doc = add_revision(doc)
     ver = len(doc.index)
-    num = len(doc.index[-1])-1
+    num = len(doc.index[-1])
     new_i = {'o_num': num, 'o_gen': 0, 'o_ver': 0, 'doc_ver': ver-1}
-    new_index = doc.index.copy()
-    new_index[-1] = doc.index[-1].copy()
-    new_index[-1].append(None)
-    new_index[-1][-1] = None
-    new_index[-1][num] = new_i
-    new_cache = doc.cache.copy()
-    new_cache.append(None)
-    new_cache[num] = new_o
-    return Doc(doc.bdata, new_index, new_cache)
+    new_doc = copy_doc(doc)
+    new_doc.index[-1].append(None)
+    new_doc.index[-1][num] = new_i
+    new_doc.cache.append(None)
+    new_doc.cache[num] = new_o
+    return new_doc, complex(0, num)
+
+
+def dependencies(doc: Doc, obj: Any) -> set:
+    """Recursively list indirect references found inside object""" 
+    if type(obj) == dict:
+        res = set()
+        for k, v in obj.items():
+            if k == '/Parent' or k == '/P':
+                continue
+            res = res | dependencies(doc, v)
+        return res
+    elif type(obj) == list:
+        res = set()
+        for i in obj:
+            res = res | dependencies(doc, i)
+        return res
+    elif type(obj) == complex:
+        res = {obj}
+        res = res | dependencies(doc, get_object(doc, obj))
+        return res
+    else:   
+        return set()
+
+
+def delete_pages(doc: Doc, del_pages) -> Doc:
+    """Delete one (an int) or more (an array of int) pages"""
+    if type(del_pages) != list:
+        del_pages = [del_pages]
+    pages = flat_page_tree(doc)
+    del_ref = {pages[p][0] for p in del_pages}
+    keep_ref = {p[0] for p in pages} - del_ref
+    del_dep = set()
+    keep_dep = set()
+    for i in del_ref:
+        del_dep = del_dep | dependencies(doc, i)
+    for i in keep_ref:
+        keep_dep = keep_dep | dependencies(doc, i)
+    for ref in del_ref:
+        parent = get_object(doc, ref)['/Parent']
+        new_parent = get_object(doc, parent)
+        kids = new_parent['/Kids']
+        kids.remove(ref)
+        new_parent['/Count'] = new_parent['/Count'] - 1
+        doc = update_object(doc, int(parent.imag), new_parent)
+        while '/Parent' in new_parent:
+            p = new_parent['/Parent']
+            new_parent = get_object(doc, p)
+            new_parent['/Count'] = new_parent['/Count'] - 1
+            doc = update_object(doc, int(p.imag), new_parent)
+    for ref in del_dep - keep_dep:
+        doc = update_object(doc, int(ref.imag), None)
+    return doc
+
+
+def defragment_map(current_index: list) -> tuple:
+    """Build new index without empty slots (ie deleted objects)"""
+    new_index = [None]
+    mapping = {}
+    nb = 0
+    for i, o in enumerate(current_index):
+        if i == 0: #trailer
+            continue
+        if 'DELETED' in o:
+            continue
+        else:
+            nb += 1
+            old_ref = complex(o['o_gen'], o['o_num']) 
+            new_index.append({'o_num': nb, 'o_gen': 0, 'doc_ver': 0, 'OLD_REF': old_ref})
+            new_ref = complex(0, nb) 
+            if old_ref != new_ref:
+                mapping[old_ref] = new_ref
+    return new_index, mapping
+
+
+def flatten(doc: Doc) -> Doc:
+    """ """
+    new_index, mapping = defragment_map(doc.index[-1])
+    new_cache = len(new_index) * [None]
+    new_data = [doc.data[0]]
+    new_cache[0] = trailer(doc)
+    for i in range(1, len(new_index)):
+        old_ref = new_index[i]['OLD_REF']
+        obj = get_object(doc, old_ref)
+        obj = rename_ref(obj, mapping)
+        new_cache[i] = obj
+    new_doc = Doc([new_index], new_cache, new_data)
+    chg = changes(new_doc)
+    if not chg:
+        return b''
+    v = version(doc)
+    if v < '1.5':
+        use_xref_stream = False
+    else:
+        use_xref_stream = True
+    del new_doc.cache[0]['/Prev']
+    header = f"%PDF-{v}".encode('ascii')
+    new_bdata, new_i = build_fragment_and_xref(chg, new_doc.index[0], new_doc.cache, len(header), use_xref_stream)
+    #new_data[-1]['bdata'] = new_bdata
+    new_data[-1]['fdata'] = bdata_dummy(header + new_bdata)
+    new_data[-1]['eof_cut'] = len(header + new_bdata)
+    new_doc.index[0] = new_i
+    return new_doc
+
 
 
 #def get_fonts(doc: Doc, page_num: int) -> dict:
 #    """Return the dictionary of fonts used in page number page_num"""
 #    page_idx = build_page_list(doc)
 #    fonts = {}
 #    resources = get_object(doc, page_idx[page_num]['/Resources'])
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/filestruct.py` & `pdfsyntax-0.0.6/pdfsyntax/filestruct.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,238 @@
 """Module pdfsyntax.filestruct: how objects are stored in a PDF file"""
 
 from typing import Callable
 from .objects import *
 import os
+from copy import deepcopy
+from .filters import *
 
 MARGIN = b'\n'
 
 
 def bdata_provider(filename: str, mode: str = "SINGLE"):
-    """ """
+    """Higher order function that offer an interface to binary data, either:
+    - from a buffer loaded at init,
+    - or directly from disk. 
+    A starting position equal to -1 means access to the last <length> bytes.
+    Return a tuple containing:
+    - the buffer to read,
+    - the index into the buffer,
+    - the offset from the beginning of the file to the buffer,
+    - the number of readable bytes.
+    """
     if mode == "SINGLE":
         bfile = open(filename, 'rb')
         bdata = bfile.read()
         bfile.close()
-        def single_load(i: int, n: int) -> tuple:
-            if i == -1:
-                i = len(bdata) - n
-            return (bdata, i, 0)
+        def single_load(start_pos: int, length: int) -> tuple:
+            if start_pos == -1 and length == 0:
+                return (None, None, None, len(bdata))
+            if length == -1:
+                length = len(bdata) - start_pos
+            if start_pos == -1:
+                i = len(bdata) - length
+            else:
+                i = start_pos
+            return (bdata, i, 0, min(len(bdata) - start_pos, length))
         return single_load
     else:
-        def continuous_load(i: int, n: int) -> tuple:
-            if n == -1:
-                n = os.stat(filename).st_size - i
-            elif i == -1:
-                i = os.stat(filename).st_size - n
+        def continuous_load(start_pos: int, length: int) -> tuple:
+            if start_pos == -1 and length == 0:
+                return (None, None, None, os.stat(filename).st_size)
+            if length == -1:
+                length = os.stat(filename).st_size - start_pos
+            if start_pos == -1:
+                i = os.stat(filename).st_size - length
+            else:
+                i = start_pos
             bfile = open(filename, 'rb')
             bfile.seek(i, 0)
-            bdata = bfile.read(n)
+            bdata = bfile.read(length)
             bfile.close()
-            return (bdata, 0, i)
+            return (bdata, 0, i, min(os.stat(filename).st_size - start_pos, length))
         return continuous_load
 
 
-def parse_xref_table(bdata: bytes, start_pos: int) -> list:
+def bdata_dummy(bdata: bytes):
+    """ """
+    def dummy_load(start_pos: int, length: int) -> tuple:
+        if start_pos == -1 and length == 0:
+            return (None, None, None, len(bdata))
+        if length == -1:
+            length = len(bdata) - start_pos
+        if start_pos == -1:
+            i = len(bdata) - length
+        else:
+            i = start_pos
+        return (bdata, i, 0, min(len(bdata) - start_pos, length))
+    return dummy_load
+
+
+def bdata_length(bdata: Callable) -> int:
+    """Direct access to data length without reading it"""
+    _, _, _, i = bdata(-1, 0)
+    return i
+
+
+def bdata_all(bdata: Callable) -> bytes:
+    """Return full bdata content as bytes"""
+    bdata, _, _, _ = bdata(0, -1)
+    return bdata
+
+
+def parse_xref_table(bdata: bytes, start_pos: int, general_offset: int) -> list:
     """Return a list of dicts indexing indirect objects
 
-       abs_pos is the absolute position of the object
-       o_num is the object number
-       o_gen is the object generation number
+    abs_pos is the absolute position of the object
+    o_num is the object number
+    o_gen is the object generation number
     """
     xref = []
     table = []
     trailer_pos = bdata.find(b'trailer', start_pos)
     lines = bdata[start_pos:trailer_pos].splitlines()
     for line in lines:
         line_a = line.strip(b'\n\r ').split()
-        #line_a = []
-        #i, n, begin_i = 0, len(line), 0
-        #while i < n:
-        #    if line[i] in b' ':
-        #        line_a.append(line[begin_i:i])
-        #        begin_i = i + 1
-        #    i += 1
-        #line_a.append(line[begin_i:i])
         l = len(line_a)
         if  l == 2:
             o_num = int(line_a[0])
             table.append((line, None))
         elif l == 3:
             offset = int(line_a[0])
             o_ver = int(line_a[1])
-            #o_start = bdata.find(b'obj', offset) + len(b'obj') + 1
-            #if bdata[o_start] in b'\r\n ': o_start += 1
-            if o_num != 0:
+            keyword = line_a[2]
+            if keyword != b'f' and o_num != 0:
                 xref.append({'abs_pos': offset, 'o_num': o_num, 'o_gen': o_ver})
             table.append((line, o_num))
             o_num += 1
-    xref.insert(0, {'o_num': 0, 'o_gen': 0, 'abs_pos': trailer_pos, 'xref_table_pos':start_pos, 'xref_table':table })
+    xref.insert(0, {'o_num': 0, 'o_gen': 0, 'abs_pos': general_offset + trailer_pos, 'xref_table_pos':general_offset + start_pos, 'xref_table':table })
     return xref
 
 
-def parse_xref_stream(xref_stream: dict, trailer_pos: int) -> list:
+def parse_xref_stream(xref_stream: dict, trailer_pos: int, o_num: int) -> list:
     """Return a list of dicts indexing indirect objects
 
-       for regular objects:
-           abs_pos is the absolute position of the object
-           o_num is the object number
-           o_gen is the object generation number
-       for objects embedded in object streams:
-           env_num is the number of the envelope object
-           o_num is the object number
-           o_gen is the object generation number
-           o_pos is the position of the object within the stream
+    for regular objects:
+        abs_pos is the absolute position of the object
+        o_num is the object number
+        o_gen is the object generation number
+    for objects embedded in object streams:
+        env_num is the number of the envelope object
+        o_num is the object number
+        o_gen is the object generation number
+        o_pos is the position of the object within the stream
     """
     xref = []
+    table = []
     cols = xref_stream['entries']['/W']
     i = 0
-    obj_range = (0, 0)
     if '/Index' in xref_stream['entries']:
         obj_range = xref_stream['entries']['/Index']
+    else:
+        obj_range = [0, xref_stream['entries']['/Size']]
     start_obj, nb_obj = int(obj_range[0]), int(obj_range[1])
     obj_num = start_obj
     while i < len(xref_stream['stream']):
-        line = ''
         params = []
+        ppr = b''
         for col in cols:
-            params.append(int.from_bytes(xref_stream['stream'][i:i+int(col)], byteorder='big')) # struct.unpack cannot work with 3-byte words
+            x = xref_stream['stream'][i:i+int(col)]
+            params.append(int.from_bytes(x, byteorder='big')) # struct.unpack cannot work with 3-byte words
             i += int(col)
+            ppr += asciihex(x) + b' '
+        table.append((ppr, obj_num))
         if params[0] == 1:
             xref.append({'abs_pos': params[1], 'o_num': obj_num, 'o_gen': params[2]})
         elif params[0] == 2:
             xref.append({'env_num': params[1], 'o_num': obj_num, 'o_gen': 0, 'o_pos': params[2]})
         obj_num += 1
-    xref.insert(0, {'o_num': 0, 'o_gen': 0, 'abs_pos': trailer_pos, 'xref_stream_pos': trailer_pos ,'xref_stream': []})
+    xref.insert(0, {'o_num': 0, 'o_gen': 0, 'abs_pos': trailer_pos, 'xref_stream_pos': trailer_pos ,'xref_stream': table, 'xref_stream_num': o_num})
     return xref
     
 
 def build_chrono_from_xref(fdata: Callable) -> list:
     """Return a merged list of all entries found in xref tables or xref streams """
     EOF = b'%%EOF'
     STARTXREF = b'startxref'
     XREF = b'xref'
-    bdata, a0, o0 = fdata(-1, 100)
+    xref_stm = False
+    bdata, a0, o0, _ = fdata(-1, 100)
     eof_pos = o0 + bdata.rfind(EOF, a0)
     startxref_pos = o0 + bdata.rfind(STARTXREF, a0)
-    i, j, _ = next_token(bdata, startxref_pos + len(STARTXREF))
+    i, j, _ = next_token(bdata, startxref_pos + len(STARTXREF) - o0)
     xref_pos = int(bdata[i:j])
-    bdata, a0, o0 = fdata(xref_pos, startxref_pos - xref_pos)
+    bdata, a0, o0, _ = fdata(xref_pos, startxref_pos - xref_pos)
     if bdata[a0:a0+4] == XREF:
-        chrono = parse_xref_table(bdata, a0)
-        i, j, _ = next_token(bdata, chrono[0]['abs_pos'])  # b'trailer'
+        chrono = parse_xref_table(bdata, a0, o0)
+        i, j, _ = next_token(bdata, chrono[0]['abs_pos'] - o0)  # b'trailer'
         i, j, _ = next_token(bdata, j)
         trailer = parse_obj(bdata[i:j])
+        if '/XRefStm' in trailer:
+            xref_stm = True
+            xref_stm_trailer = trailer
+            new_xref_pos = trailer['/XRefStm']
+            xref_pos = int(new_xref_pos)
+            bdata, a0, o0, _ = fdata(xref_pos, startxref_pos - xref_pos)
+            i, j, _ = next_token(bdata, a0)
+            o_num = parse_obj(bdata, i)
+            i, j, _ = next_token(bdata, j)
+            i, j, _ = next_token(bdata, j)
+            i, j, _ = next_token(bdata, j)
+            xref = parse_obj(bdata, i)
+            chrono = parse_xref_stream(xref, xref_pos, o_num)
+            trailer = xref['entries']
     else: # must be a /XRef stream
-        bdata, a0, o0 = fdata(xref_pos, startxref_pos - xref_pos)
+        bdata, a0, o0, _ = fdata(xref_pos, startxref_pos - xref_pos)
         i, j, _ = next_token(bdata, a0)
+        o_num = parse_obj(bdata, i)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
         xref = parse_obj(bdata, i)
-        chrono = parse_xref_stream(xref, xref_pos)
+        chrono = parse_xref_stream(xref, xref_pos, o_num)
         trailer = xref['entries']
     chrono[0]['startxref_pos'] = startxref_pos
+    if xref_stm:
+        chrono[0]['xref_stm'] = True
+        trailer = xref_stm_trailer
+    else:
+        chrono[0]['xref_stm'] = False
     chrono.append({'o_num': -1, 'o_gen': -1, 'abs_pos': eof_pos})
     prev_eof = eof_pos
     while '/Prev' in trailer:
         new_xref_pos = trailer['/Prev']
-        xref_pos = int(new_xref_pos)
-        bdata, a0, o0 = fdata(xref_pos, prev_eof - xref_pos)
-        startxref_pos = o0 + bdata.find(STARTXREF, a0)
-        eof_pos = o0 + bdata.find(EOF, a0)
+        if new_xref_pos < xref_pos:
+            xref_pos = int(new_xref_pos)
+            bdata, a0, o0, _ = fdata(xref_pos, prev_eof - xref_pos)
+            startxref_pos = o0 + bdata.find(STARTXREF, a0)
+            eof_pos = o0 + bdata.find(EOF, a0)
+        else: # Linearized
+            startxref_pos = o0 + bdata.find(STARTXREF, 0)
+            eof_pos = o0 + bdata.find(EOF, 0)
+            xref_pos = int(new_xref_pos)
+            bdata, a0, o0, _ = fdata(xref_pos, prev_eof - xref_pos)
         prev_eof = eof_pos
         if bdata[a0:a0+4] == XREF:
-            tmp_index = parse_xref_table(bdata, a0)
+            tmp_index = parse_xref_table(bdata, a0, o0)
             tmp_index[0]['startxref_pos'] = startxref_pos
             tmp_index.append({'o_num': -1, 'o_gen': -1, 'abs_pos': eof_pos})
             chrono = tmp_index + chrono
-            i, j, _ = next_token(bdata, chrono[0]['abs_pos'])
+            i, j, _ = next_token(bdata, chrono[0]['abs_pos'] - o0)
             i, j, _ = next_token(bdata, j)                     # actual trailer dict
             trailer = parse_obj(bdata[i:j])
         else: # must be a /XRef stream
-            bdata, a0, o0 = fdata(xref_pos, startxref_pos - xref_pos)
-            i, j, _ = next_token(bdata, a0)
+            bdata, a0, o0, _ = fdata(xref_pos, startxref_pos - xref_pos)
+            i, j, _ = next_token(bdata, a0 - o0)
+            o_num = parse_obj(bdata, i)
             i, j, _ = next_token(bdata, j)
             i, j, _ = next_token(bdata, j)
             i, j, _ = next_token(bdata, j)
             xref = parse_obj(bdata, i)
-            tmp_index = parse_xref_stream(xref, xref_pos)
+            tmp_index = parse_xref_stream(xref, xref_pos, o_num)
             tmp_index[0]['startxref_pos'] = startxref_pos
             tmp_index.append({'o_num': -1, 'o_gen': -1, 'abs_pos': eof_pos})
             chrono =  tmp_index + chrono
             trailer = xref['entries']
     seq = [i.get('abs_pos') for i in chrono if i.get('abs_pos')]
     seq.sort()
     idx = {}
@@ -181,15 +253,15 @@
     nb = max(chrono, key = lambda i: i['o_num']).get('o_num') + 2
     m = nb * [None]
     abs_pos_array = nb * [0]
     index = []
     doc_ver = -1
     prev_pos = 0
     for obj in chrono:
-        if obj['o_num'] == 0 and obj['abs_pos'] > prev_pos:
+        if obj['o_num'] == 0 and (obj['abs_pos'] > prev_pos or obj.get('xref_stm')):
             m = m[:]
             m[0] = None
             index.append(m)
             doc_ver += 1
             prev_pos = obj['abs_pos']
         elif obj['o_num'] == -1:
             pass
@@ -211,14 +283,31 @@
         for obj in abs_list:
             abs_pos_array[obj['o_num']] = obj['abs_pos']
         for obj in env_list:
             obj['a_'] = abs_pos_array[obj['env_num']] + (obj['o_pos'] + 1) / 1000
     return index
 
 
+def eof_cut(eof_index: int, fdata: Callable) -> int:
+    """ """
+    bdata, start, _, n = fdata(eof_index, bdata_length(fdata) - eof_index)
+    i = start + len('%%EOF')
+    while i < start + n:
+        if bdata[i] not in EOL:
+            break
+        i += 1
+    return i
+
+
+def build_data_from_cache(index: list, fdata: Callable) -> list:
+    """ """
+    data = [{'eof_cut': eof_cut(i[-1]['abs_pos'], fdata), 'fdata': fdata} for i in index if i[-1]]
+    return data
+
+
 def circular_deleted(changes: list) -> dict:
     """Build lookup dict to ref of next deleted object"""
     res = {}
     deleted = [x for x in changes if x[1] == 'd']
     for i, d in enumerate([(0, 'd')] + deleted):
         if i == len(deleted):
             res[d[0]] = 0
@@ -266,25 +355,25 @@
 def format_xref_stream(elems: list, trailer: dict, next_free: dict) -> bytes:
     """Build XREF stream object"""
     xref_stream = []
     index = []
     o_num = trailer['/Size'] - 1
     trailer['/Type'] = '/XRef'
     trailer['/Filter'] = '/ASCIIHexDecode'
-    trailer['/W'] = [1, 2, 2]
+    trailer['/W'] = [1, 3, 3]
     for use, num, o_gen, counter, env_num in elems:
         if use == 'f':
-            ref = b'\x00' + (next_free[num]).to_bytes(2, "big") + (o_gen+1).to_bytes(2, "big")
+            ref = b'\x00' + (next_free[num]).to_bytes(3, "big") + (o_gen+1).to_bytes(3, "big")
             xref_stream.append((ref, num))
         else:
             if env_num:
-                ref = b'\x02' + (env_num).to_bytes(2, "big") + (counter).to_bytes(2, "big")
+                ref = b'\x02' + (env_num).to_bytes(3, "big") + (counter).to_bytes(3, "big")
                 xref_stream.append((ref, num))
             else:
-                ref = b'\x01' + (counter).to_bytes(2, "big") + (o_gen).to_bytes(2, "big")
+                ref = b'\x01' + (counter).to_bytes(3, "big") + (o_gen).to_bytes(3, "big")
                 xref_stream.append((ref, num))
     # Index 
     i = len(xref_stream) - 1
     num = xref_stream[i][1]
     nb = 1
     while i >= 1:
         i -= 1
@@ -350,18 +439,20 @@
     entries['/N'] = len(tokens) // 2
     del entries['/FirstLine']
     new_ser = header + envelope['stream']
     envelope = Stream(entries, new_ser)
     return envelope
 
 
-def build_fragments_and_xref(changes: list, current_index: list, cache: list, starting_pos: int, version: str) -> list:
+def build_fragment_and_xref(changes: list, current_index: list, cache: list, starting_pos: int, use_xref_stream: bool) -> tuple:
     """List the sequence of byte blocks that make the update"""
     fragments = []
     xref_table = []
+    res = b''
+    new_index = deepcopy(current_index)
     counter = starting_pos + len(MARGIN)
     fragments.append(MARGIN)
     next_free = circular_deleted(changes)
     for num, action in ([(0, 'd')] + changes):
         env_num = None
         if action == 'd':
             if num == 0:
@@ -380,17 +471,45 @@
             else:
                 obj = cache[num]
                 if type(obj) == Stream and obj['entries'].get('/Type') == '/ObjStm':
                     obj = finalize_stream(obj)
                 block = serialize_fragment(num, o_gen, obj)
                 fragments.append(block)
                 xref_table.append(('n', num, o_gen, counter, env_num))
+                new_index[num]['abs_pos'] = counter
+                new_index[num]['abs_next'] = counter + len(block)
             counter += len(block)
-    if version < '1.5':
+    cache[0]['/Size'] = len(current_index)
+    if not use_xref_stream:
         built_xref = format_xref_table(xref_table, cache[0], next_free)
+        new_index[0] = {}
+        new_index[0]['abs_pos'] = starting_pos + built_xref.rfind(b'trailer')
+        new_index[0]['abs_next'] = starting_pos + len(built_xref)
     else:
         built_xref = format_xref_stream(xref_table, cache[0], next_free)
+        new_index[0] = {}
+        new_index[0]['abs_pos'] = starting_pos
+        new_index[0]['abs_next'] = starting_pos + len(built_xref)
     fragments.append(built_xref)
     fragments.append(f'startxref\n{counter}\n'.encode('ascii'))
     fragments.append(b'%%EOF\n')
-    return fragments
+    for i in fragments:
+        res += i
+    return res, new_index
+
+
+def linearized(fdata: Callable) -> dict:
+    """ """
+    HEADER = b'%PDF-X.Y'
+    bdata, a0, o0, _ = fdata(len(HEADER), 1024 - len(HEADER))
+    i, j, _ = next_token(bdata, a0) #comment
+    i, j, _ = next_token(bdata, j)  #o_num
+    i, j, _ = next_token(bdata, j)  #gen_num
+    i, j, _ = next_token(bdata, j)  #obj keyword
+    i, _, t = next_token(bdata, j)  #dict ?
+    if t == 'DICT':
+        first_obj = parse_obj(bdata, i)
+        if type(first_obj) == dict and '/Linearized' in first_obj:
+            return first_obj
+    return None
+
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/filters.py` & `pdfsyntax-0.0.6/pdfsyntax/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,11 +40,24 @@
     if stream_def['/Filter'] == '/FlateDecode':
         return zlib.compress(stream)
     elif stream_def['/Filter'] == '/ASCIIHexDecode':
         return asciihex(stream)
     return stream
 
 
-def asciihex(stream):
+def asciihex(stream, columns = None):
     """ """
-    return (binascii.hexlify(stream)).upper()
+    if columns is None:
+        return (binascii.hexlify(stream)).upper()
+    else:
+        res = b''
+        i = 0
+        l = sum(columns)
+        while i+l <= len(stream):
+            for c in columns:
+                res += (binascii.hexlify(stream[i:i+c])).upper() 
+                res += b' '
+                i += c
+            res += b'\n'
+        return res
+
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/objects.py` & `pdfsyntax-0.0.6/pdfsyntax/objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,26 @@
 DELIMITERS = b'<>[]/(){}%'
 
 
 @dataclass
 class Stream:
     entries: dict
     stream: bytes
+
     def __getitem__(self, item):
         return getattr(self, item)
 
+    def __repr__(self):
+        res = "<PDF Stream," + f" entries: {self.entries},"
+        if len(self.stream) > 40:
+            res += f" decoded stream: {self.stream[:10]+b' (...truncated...)'}>\n"
+        else:
+            res += f" decoded stream: {self.stream}>\n"
+        return res
+
 
 def next_token(text: bytes, i=0) -> tuple:
     """Find next token in raw string starting at some index"""
     search = "TBD"
     nested = 1
     h = i
     while i < len(text):
@@ -36,15 +45,19 @@
                 search = "DICT"
             elif single == b'[':
                 search = "ARRAY"
             elif single == b"/":
                 search = "NAME"
             elif text[i:i+6] == b"stream":
                 search = "STREAM"
-                offset = 7 if text[i+6:i+7] == b'\n' else 8
+                #offset = 7 if text[i+6:i+7] == b'\n' else 8
+                if text[i+6:i+8] == b'\r\n':
+                    offset = 8
+                else:
+                    offset = 7
                 i += offset
             elif single in b"+-.0123456789":
                 search = "VALUE"
             elif single in b"abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ":
                 search = "KEYWORD"
             elif single in b"(<":
                 search = "STRING"
@@ -85,15 +98,15 @@
         elif search == "VALUE":
             if single in (SPACE + DELIMITERS): #or i == len(text) - 1:
                 if b'.' in text[h:i]:
                     return (h, i, 'REAL')
                 else:
                     return (h, i, 'INTEGER')
         elif search == "STREAM":
-            if text[i:i+11] == b'\r\nendstream' or text[i:i+10] == b'\nendstream':
+            if text[i:i+11] == b'\r\nendstream' or text[i:i+10] == b'\nendstream' or text[i:i+10] == b'\rendstream':
                 return (h, i, 'STREAM')
         elif search == "ARRAY":
             if single == b'[':
                 nested += 1
             elif single == b']':
                 nested -= 1
             if nested == 0:
@@ -219,15 +232,15 @@
     ret = b''
     content = None
     if type(obj) == dict or type(obj) == Stream:
         if type(obj) == Stream:
             content = obj['stream']
             obj = obj['entries']
             encoded_content = encode_stream(content, obj)
-            obj['/Length'] = len(encoded_content) + 1
+            obj['/Length'] = len(encoded_content) + 1 #TODO Handle case when Length is an indirect object
         ret += b'<< '
         keys = list(obj.keys())
         for i in keys:
             name = i
             value = serialize(obj[i], depth + 1)
             ret += b' '  * depth
             ret += to_str(name)
@@ -246,7 +259,22 @@
             value = serialize(i)
             ret += value
             ret += b' '
         ret += b']'        
     else:
         ret += to_str(obj)
     return ret
+
+
+def rename_ref(obj: Any, mapping: dict) -> Any:
+    """Recursively replace an indirect reference in object tree""" 
+    if type(obj) == complex:
+        if obj in mapping:
+            return mapping[obj]
+    elif type(obj) == dict:
+        for k in obj:
+            obj[k] = rename_ref(obj[k], mapping)
+    elif type(obj) == list:
+        for k in range(len(obj)):
+            obj[k] = rename_ref(obj[k], mapping)
+    return obj
+
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax/text.py` & `pdfsyntax-0.0.6/pdfsyntax/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,19 @@
     """Transform a fundamental string into a text string"""
     if string is None: return None
     res = ''
     if string[0:1] == b'(': # Literal string
         if string[1:3] == b'\xfe\xff': 
             res = string[3:-1].decode('utf-16be')
         else:
-            res = decode_pdfdoc(string[1:-1])
+            s = string[1:-1]
+            s = s.replace(b'\x5c\x5c', b'\x5c') # x5c is backslash
+            s = s.replace(b'\x5c(', b'(')
+            s = s.replace(b'\x5c)', b')')
+            res = decode_pdfdoc(s)
     elif string[0:1] == b'<': # Hexadecimal string
         if string[1:5] == b'FEFF':
             b = bytes.fromhex(string[5:-1].decode('ascii'))
             res = b.decode('utf-16be')
         else:
             b = bytes.fromhex(decode_pdfdoc(string[1:-1]))
             res = decode_pdfdoc(b)
```

### Comparing `pdfsyntax-0.0.5/pdfsyntax.egg-info/PKG-INFO` & `pdfsyntax-0.0.6/pdfsyntax.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python PDF parsing library and tool built on top to browse the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin D. <desgeeko@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -105,17 +105,17 @@
 ### File information
 
 `structure` and `metadata` are functions showing general information about the document.
 
 ```Python
 >>> #File structure
 >>> structure(doc)
-{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 1, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
->>> #File structure
+>>> #File metadata
 >>> metadata(doc)
 {'Title': None, 'Author': None, 'Subject': None, 'Keywords': None, 'Creator': None, 'Producer': None, 'CreationDate': None, 'ModDate': None}
 ```
 
 ### Low-level access to object tree
 
 `trailer` and `catalog` give access to the starting point of the object tree. 
@@ -138,23 +138,47 @@
 ```Python
 >>> #Access to document catalog, given that the trailer redirects to 1j for root
 >>> #(equivalent to catalog fonction)
 >>> doc.get_object(1j)
 {'/Pages': 3j, '/Outlines': 2j, '/Type': '/Catalog'}
 ```
 
+### Pages
+
+Page index is a tree structure where attributes can be inherited from parent nodes. For convenience `flat_page_tree` returns an ordered list of document pages and specifies inherited attributes that should apply to each page.
+
+```Python
+>>> #Each item of the list is a tuple with the page object reference and its inherited attributes
+>>> doc = pdf.read("samples/simple_text_string.pdf")
+>>> pdf.flat_page_tree(doc)
+[(4j, {})]
+>>> #(In this example, nothing is inherited from upper nodes)
+```
+
+The `page` function goes further by merging inherited attributes with local attributes of each page and giving the result in a list.
+
+```Python
+>>> #Equivalent list with computed page attribues
+>>> pdf.pages(doc)
+[{'/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j},
+  '/Contents': 5j,
+  '/MediaBox': [0, 0, 612, 792],
+  '/Parent': 3j,
+  '/Type': '/Page'}]
+```
+
 ### Incremental updates
 
 PDFSyntax tracks document incremental updates made possible by appending new or updated objects at the end of an original PDF file (and the matching XREF section). The `Revisions` entry of the `structure` function result, if greater than 1, indicates that incremental updates have been appended. By default, a newly opened document by PDFSyntax is ready to write modifications in the next revision. The `rewind` function rolls back to the previous revision. 
 
 ```Python
 >>> import pdfsyntax as pdf
 >>> doc = pdf.read("samples/add_text_annotation.pdf")
 >>> doc.structure()
-{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper': '215x279mm or 8.5x11.0in (US Letter)'}
+{'Version': '1.4', 'Pages': 1, 'Revisions': 2, 'Encrypted': False, 'Paper of 1st page': '215x279mm or 8.5x11.0in (US Letter)'}
 
 >>> #This file contains 2 revisions and PDFSyntax has initialized the doc object for a future revision 3
 
 >>> doc.get_object(4j)
 {'/Annots': 8j, '/Resources': {'/Font': {'/F1': 7j}, '/ProcSet': 6j}, '/Contents': 5j, '/MediaBox': [0, 0, 612, 792], '/Parent': 3j, '/Type': '/Page'}
 
 >>> #In its current state, the page (object 4) contains an annotation
```

### Comparing `pdfsyntax-0.0.5/pyproject.toml` & `pdfsyntax-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pdfsyntax"
-version = "0.0.5"
+version = "0.0.6"
 authors = [ 
     { name="Martin D.", email="desgeeko@gmail.com" } 
 ]
 description = "A Python PDF parsing library and tool built on top to browse the internal structure of a PDF file"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

