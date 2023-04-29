# Comparing `tmp/pymkpsxiso-0.1.2.tar.gz` & `tmp/pymkpsxiso-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymkpsxiso-0.1.2.tar", last modified: Wed Mar 29 07:04:32 2023, max compression
+gzip compressed data, was "pymkpsxiso-0.1.3.tar", last modified: Sat Apr 29 05:12:10 2023, max compression
```

## Comparing `pymkpsxiso-0.1.2.tar` & `pymkpsxiso-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.433084 pymkpsxiso-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-29 07:04:32.433084 pymkpsxiso-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.425084 pymkpsxiso-0.1.2/mkpsxiso/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.425084 pymkpsxiso-0.1.2/mkpsxiso/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-29 07:04:20.000000 pymkpsxiso-0.1.2/mkpsxiso/ThreadPool/ThreadPool.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.425084 pymkpsxiso-0.1.2/mkpsxiso/miniaudio/
--rw-r--r--   0 runner    (1001) docker     (123)  3083782 2023-03-29 07:04:22.000000 pymkpsxiso-0.1.2/mkpsxiso/miniaudio/miniaudio.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.425084 pymkpsxiso-0.1.2/mkpsxiso/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.429084 pymkpsxiso-0.1.2/mkpsxiso/src/dumpsxiso/
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/dumpsxiso/cdreader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/dumpsxiso/cdreader.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.429084 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/cdwriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/cdwriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/edcecc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/edcecc.h
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/global.h
--rw-r--r--   0 runner    (1001) docker     (123)    30305 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/iso.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/iso.h
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.429084 pymkpsxiso-0.1.2/mkpsxiso/src/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/cd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/listview.h
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/mmappedfile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/mmappedfile.h
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/platform.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/platform.h
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/xa.h
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/mkpsxiso/src/shared/xml.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.429084 pymkpsxiso-0.1.2/mkpsxiso/tinyxml2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    77745 2023-03-29 07:04:23.000000 pymkpsxiso-0.1.2/mkpsxiso/tinyxml2/tinyxml2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    73727 2023-03-29 07:04:23.000000 pymkpsxiso-0.1.2/mkpsxiso/tinyxml2/tinyxml2.h
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/pymkpsxiso.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:04:32.433084 pymkpsxiso-0.1.2/pymkpsxiso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-29 07:04:32.000000 pymkpsxiso-0.1.2/pymkpsxiso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-29 07:04:32.000000 pymkpsxiso-0.1.2/pymkpsxiso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 07:04:32.000000 pymkpsxiso-0.1.2/pymkpsxiso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 07:04:32.000000 pymkpsxiso-0.1.2/pymkpsxiso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 07:04:32.433084 pymkpsxiso-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-29 07:04:16.000000 pymkpsxiso-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.065299 pymkpsxiso-0.1.3/mkpsxiso/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.069299 pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-29 05:11:52.000000 pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/ThreadPool.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.069299 pymkpsxiso-0.1.3/mkpsxiso/miniaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)  3083782 2023-04-29 05:11:57.000000 pymkpsxiso-0.1.3/mkpsxiso/miniaudio/miniaudio.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.065299 pymkpsxiso-0.1.3/mkpsxiso/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.073299 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/global.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29623 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/src/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/cd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/listview.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.h
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/xa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/xml.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77745 2023-04-29 05:11:58.000000 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73727 2023-04-29 05:11:58.000000 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/pymkpsxiso.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/setup.py
```

### Comparing `pymkpsxiso-0.1.2/LICENSE` & `pymkpsxiso-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/PKG-INFO` & `pymkpsxiso-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkpsxiso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface for mkpsxiso.
 Home-page: https://github.com/Illidanz/pymkpsxiso
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/ThreadPool/ThreadPool.h` & `pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/ThreadPool.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/miniaudio/miniaudio.h` & `pymkpsxiso-0.1.3/mkpsxiso/miniaudio/miniaudio.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/dumpsxiso/cdreader.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {
     if (filePtr != NULL)
 		fclose(filePtr);
 
 }
 
 
-bool cd::IsoReader::Open(const std::filesystem::path& fileName)
+bool cd::IsoReader::Open(const fs::path& fileName)
 {
 	Close();
 
     filePtr = OpenFile(fileName, "rb");
 
     if (filePtr == NULL)
 		return(false);
@@ -265,17 +265,17 @@
 		pathTableList.emplace_back(std::move(pathTableEntry));
 	}
 
 	return pathTableList.size();
 
 }
 
-std::filesystem::path cd::IsoPathTable::GetFullDirPath(int dirEntry) const
+fs::path cd::IsoPathTable::GetFullDirPath(int dirEntry) const
 {
-	std::filesystem::path path;
+	fs::path path;
 
 	while (true)
 	{
 		if (pathTableList[dirEntry].name.empty())
 			break;
 
 		// Prepend!
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/dumpsxiso/cdreader.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #ifndef _CDREADER_H
 #define _CDREADER_H
 
 #include "cd.h"
 #include "xa.h"
 #include "listview.h"
-#include <filesystem>
+#include "fs.h"
 #include <memory>
 #include <optional>
 #include <vector>
 #include <string>
 
 namespace cd {
 
@@ -34,15 +34,15 @@
 
         // Initializer
         IsoReader();
         // De-initializer
         ~IsoReader();
 
         // Open ISO image
-        bool Open(const std::filesystem::path& fileName);
+        bool Open(const fs::path& fileName);
 
         // Read data sectors in bytes (supports sequential reading)
         size_t ReadBytes(void* ptr, size_t bytes, bool singleSector = false);
 
         size_t ReadBytesXA(void* ptr, size_t bytes, bool singleSector = false);
 
         size_t ReadBytesDA(void* ptr, size_t bytes, bool singleSector = false);
@@ -77,27 +77,27 @@
         };
 
         std::vector<Entry> pathTableList;
 
         void FreePathTable();
         size_t ReadPathTable(cd::IsoReader* reader, int lba);
 
-        std::filesystem::path GetFullDirPath(int dirEntry) const;
+        fs::path GetFullDirPath(int dirEntry) const;
     };
 
 
     class IsoDirEntries
     {
     public:
         struct Entry
         {
             ISO_DIR_ENTRY entry;
             cdxa::ISO_XA_ATTRIB extData;
             std::string identifier;
-            std::filesystem::path virtualPath;
+            fs::path virtualPath;
 
             std::unique_ptr<IsoDirEntries> subdir;
         };
         ListView<Entry> dirEntryList;
 
         IsoDirEntries(ListView<Entry> view);
         void ReadDirEntries(cd::IsoReader* reader, int lba, int sectors);
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/cdwriter.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return { val, SwapBytes16(val) };
 }
 
 ISO_UINT_PAIR cd::SetPair32(unsigned int val) {
 	return { val, SwapBytes32(val) };
 }
 
-bool IsoWriter::Create(const std::filesystem::path& fileName, unsigned int sizeLBA)
+bool IsoWriter::Create(const fs::path& fileName, unsigned int sizeLBA)
 {
 	const uint64_t sizeBytes = static_cast<uint64_t>(sizeLBA) * CD_SECTOR_SIZE;
 
 	m_threadPool = std::make_unique<ThreadPool>(std::thread::hardware_concurrency());
 	
 	m_mmap = std::make_unique<MMappedFile>();
 	return m_mmap->Create(fileName, sizeBytes);
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/cdwriter.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #ifndef _CDWRITER_H
 #define _CDWRITER_H
 
 #include "cd.h"
 #include "mmappedfile.h"
-
+#include "fs.h"
 #include <ThreadPool.h>
-#include <filesystem>
 #include <forward_list>
 #include <memory>
 
 namespace cd {
 
 class IsoWriter
 {
@@ -75,15 +74,15 @@
 	private:
 		MMappedFile::View m_view;
 		unsigned int m_endLBA;
 	};
 
 	IsoWriter() = default;
 
-	bool Create(const std::filesystem::path& fileName, unsigned int sizeLBA);
+	bool Create(const fs::path& fileName, unsigned int sizeLBA);
 	void Close();
 
 	std::unique_ptr<SectorView> GetSectorViewM2F1(unsigned int offsetLBA, unsigned int sizeLBA, EdcEccForm edcEccForm) const;
 	std::unique_ptr<SectorView> GetSectorViewM2F2(unsigned int offsetLBA, unsigned int sizeLBA, EdcEccForm edcEccForm) const;
 	std::unique_ptr<RawSectorView> GetRawSectorView(unsigned int offsetLBA, unsigned int sizeLBA) const;
 
 private:
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/edcecc.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/edcecc.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/iso.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 template<typename T>
 static T RoundToEven(T val)
 {
 	return (val + 1) & -2;
 }
 
-int iso::DirTreeClass::GetAudioSize(const std::filesystem::path& audioFile)
+int iso::DirTreeClass::GetAudioSize(const fs::path& audioFile)
 {
 	ma_decoder decoder;
 	VirtualWavEx vw;
 	bool isLossy;
 	if(ma_redbook_decoder_init_path_by_ext(audioFile, &decoder, &vw, isLossy) != MA_SUCCESS)
 	{
 		return 0;
@@ -109,15 +109,15 @@
 	entry.UID		= attributes.UID;
 
 	entries.emplace_back( std::move(entry) );
 
 	return entries.back();
 }
 
-bool iso::DirTreeClass::AddFileEntry(const char* id, EntryType type, const std::filesystem::path& srcfile, const EntryAttributes& attributes, const char *trackid)
+bool iso::DirTreeClass::AddFileEntry(const char* id, EntryType type, const fs::path& srcfile, const EntryAttributes& attributes, const char *trackid)
 {
     auto fileAttrib = Stat(srcfile);
     if ( !fileAttrib )
 	{
 		if ( !global::QuietMode )
 		{
 			printf("      ");
@@ -260,29 +260,28 @@
 	entry.type		= EntryType::EntryDummy;
 	entry.length	= 2048*sectors;
 
 	entries.emplace_back(std::move(entry));
 	entriesInDir.emplace_back(entries.back());
 }
 
-iso::DirTreeClass* iso::DirTreeClass::AddSubDirEntry(const char* id, const std::filesystem::path& srcDir, const EntryAttributes& attributes, bool& alreadyExists)
+iso::DirTreeClass* iso::DirTreeClass::AddSubDirEntry(const char* id, const fs::path& srcDir, const EntryAttributes& attributes, bool& alreadyExists)
 {
 	// Duplicate directory entries are allowed, but the subsequent occurences will not add
 	// a new directory to 'entries'.
 	// TODO: It's not possible now, but a warning should be issued if entry attributes are specified for the subsequent occurences
 	// of the directory. This check probably needs to be moved outside of the function.
-	auto currentSubdir = std::find_if(entries.begin(), entries.end(), [id](const auto& e)
-		{
-			return e.type == EntryType::EntryDir && e.id == id;
-		});
-
-	if (currentSubdir != entries.end())
+	for(auto& e : entriesInDir)
 	{
-		alreadyExists = true;
-		return currentSubdir->subdir.get();
+		const iso::DIRENTRY& entry = e.get();
+		if((entry.type == EntryType::EntryDir) && (entry.id == id))
+		{
+			alreadyExists = true;
+			return entry.subdir.get();
+		}
 	}
 
 	auto fileAttrib = Stat(srcDir);
 	time_t dirTime;
 	if ( fileAttrib )
 	{
 		dirTime = fileAttrib->st_mtime;
@@ -295,15 +294,14 @@
 		{
 			if ( !global::QuietMode )
 			{
 				printf( "\n    " );
 			}
 
 			printf( "WARNING: 'source' attribute for subdirectory '%s' is invalid or empty.\n", id );
-			fflush(stdout);
 		}
 	}
 
 	DIRENTRY entry {};
 
 	if (id != nullptr)
 	{
@@ -338,28 +336,14 @@
 
 	parent->PrintRecordPath();
 	printf( "/%s", name.c_str() );
 }
 
 int iso::DirTreeClass::CalculateTreeLBA(int lba)
 {
-	bool passedSector = false;
-	lba += GetSizeInSectors(CalculateDirEntryLen(&passedSector));
-
-	if ( ( global::NoLimit == false) && passedSector )
-	{
-		if (!global::QuietMode)
-			printf("      ");
-
-		printf("WARNING: Directory record ");
-		PrintRecordPath();
-		printf(" exceeds 2048 bytes.\n");
-		fflush(stdout);
-	}
-
 	bool firstDAWritten = false;
 	for ( DIRENTRY& entry : entries )
 	{
 		// Set current LBA to directory record entry
 		entry.lba = lba;
 
 		// If it is a subdir
@@ -390,15 +374,15 @@
 			}
 		}
 	}
 
 	return lba;
 }
 
-int iso::DirTreeClass::CalculateDirEntryLen(bool* passedSector) const
+int iso::DirTreeClass::CalculateDirEntryLen() const
 {
 	int dirEntryLen = 68;
 
 	if ( !global::noXA )
 	{
 		dirEntryLen += 28;
 	}
@@ -426,19 +410,14 @@
 			// Round dirEntryLen to the nearest multiple of 2048 as the rest of that sector is "unusable"
 			dirEntryLen = ((dirEntryLen + 2047) / 2048) * 2048;
 		}
 
 		dirEntryLen += dataLen;
 	}
 
-	if (dirEntryLen > 2048 && passedSector != nullptr)
-	{
-		*passedSector = true;
-	}
-
 	return 2048 * GetSizeInSectors(dirEntryLen);
 }
 
 void iso::DirTreeClass::SortDirectoryEntries()
 {
 	// Search for directories
 	for ( const auto& e : entriesInDir )
@@ -632,70 +611,65 @@
 		if ( entry.type == EntryType::EntryFile )
 		{
 			if ( !entry.srcfile.empty() )
 			{
 				if ( !global::QuietMode )
 				{
 					printf( "      Packing %" PRFILESYSTEM_PATH "... ", entry.srcfile.lexically_normal().c_str() );
-					fflush(stdout);
 				}
 
 				FILE *fp = OpenFile( entry.srcfile, "rb" );
 				if (fp != nullptr)
 				{
 					auto sectorView = writer->GetSectorViewM2F1(entry.lba, GetSizeInSectors(entry.length), cd::IsoWriter::EdcEccForm::Form1);
 					sectorView->WriteFile(fp);
 
 					fclose(fp);
 				}
 
 				if ( !global::QuietMode )
 				{
 					printf("Done.\n");
-					fflush(stdout);
 				}
 
 			}
 
 		// Write XA/STR video streams as Mode 2 Form 1 (video sectors) and Mode 2 Form 2 (XA audio sectors)
 		// Video sectors have EDC/ECC while XA does not
 		}
 		else if ( entry.type == EntryType::EntryXA )
 		{
 			if ( !global::QuietMode )
 			{
 				printf( "      Packing XA %" PRFILESYSTEM_PATH "... ", entry.srcfile.lexically_normal().c_str() );
-				fflush(stdout);
 			}
 
 			FILE *fp = OpenFile( entry.srcfile, "rb" );
 			if (fp != nullptr)
 			{
 				auto sectorView = writer->GetSectorViewM2F2(entry.lba, GetSizeInSectors(entry.length, 2336), cd::IsoWriter::EdcEccForm::Autodetect);
 				sectorView->WriteFile(fp);
 
 				fclose( fp );
 			}			
 
 			if (!global::QuietMode)
 			{
 				printf( "Done.\n" );
-				fflush(stdout);
 			}
 
 		// Write data only STR streams as Mode 2 Form 1
 		}
 		else if ( entry.type == EntryType::EntryXA_DO )
 		{
 			if ( !entry.srcfile.empty() )
 			{
 				if ( !global::QuietMode )
 				{
 					printf( "      Packing XA-DO %" PRFILESYSTEM_PATH "... ", entry.srcfile.lexically_normal().c_str() );
-					fflush(stdout);
 				}
 
 				FILE *fp = OpenFile( entry.srcfile, "rb" );
 				if (fp != nullptr)
 				{
 					auto sectorView = writer->GetSectorViewM2F1(entry.lba, GetSizeInSectors(entry.length), cd::IsoWriter::EdcEccForm::Form1);
 					sectorView->SetSubheader(cd::IsoWriter::SubSTR);
@@ -703,15 +677,14 @@
 
 					fclose(fp);
 				}
 
 				if ( !global::QuietMode )
 				{
 					printf("Done.\n");
-					fflush(stdout);
 				}
 
 			}
 		// Write DA files as audio tracks
 		}
 		else if ( entry.type == EntryType::EntryDA )
 		{
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/iso.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include <stdlib.h>
 #include <list>
 #include <memory>
 #include <optional>
 #include <string>
 #include <utility>
 #include <vector>
-#include <filesystem>
+#include "fs.h"
 #include "cdwriter.h"
 #include "common.h"
 
 namespace iso
 {
 	typedef struct
 	{
@@ -30,15 +30,15 @@
 
 	struct DIRENTRY
 	{
 		std::string	id;		/// Entry identifier (empty if invisible dummy)
 		int64_t length;		/// Length of file in bytes
 		int		lba;		/// File LBA (in sectors)
 
-		std::filesystem::path srcfile;	/// Filename with path to source file (empty if directory or dummy)
+		fs::path srcfile;	/// Filename with path to source file (empty if directory or dummy)
 		EntryType	  type;		/// File type (0 - file, 1 - directory)
 		unsigned char attribs;	/// XA attributes, 0xFF is not set
 		unsigned short perms;	/// XA permissions
 		unsigned short GID;		/// Owner group ID
 		unsigned short UID;		/// Owner user ID
 		std::unique_ptr<class DirTreeClass> subdir;
 
@@ -79,15 +79,15 @@
 		/// Internal function for generating and writing directory records
 		bool WriteDirEntries(cd::IsoWriter* writer, const DIRENTRY& dir, const DIRENTRY& parentDir) const;
 
 		/// Internal function for recursive path table generation
 		std::unique_ptr<PathTableClass> GenPathTableSub(unsigned short& index, unsigned short parentIndex) const;
 
 	public:
-        static int GetAudioSize(const std::filesystem::path& audioFile);
+        static int GetAudioSize(const fs::path& audioFile);
 		EntryList& entries; // List of all entries on the disc
 		std::vector<std::reference_wrapper<iso::DIRENTRY>> entriesInDir; // References to entries in this directory
 
 		DirTreeClass(EntryList& entries, DirTreeClass* parent = nullptr);
 		~DirTreeClass();
 
 		static DIRENTRY& CreateRootDirectory(EntryList& entries, const cd::ISO_DATESTAMP& volumeDate);
@@ -95,18 +95,16 @@
 		void PrintRecordPath();
 
 		void OutputHeaderListing(FILE* fp, int level) const;
 		
 		/** Calculates the length of the directory record to be produced by this class in bytes.
 		 *
 		 *  Returns: Length of directory record in bytes.
-		 * 
-		 * * *passedSector - Flag to indicate if the directory record has exceeded a sector
 		 */
-		int	CalculateDirEntryLen(bool* passedSector = nullptr) const;
+		int	CalculateDirEntryLen() const;
 
 		/** Calculates the LBA of all file and directory entries in the directory record and returns the next LBA
 		 *	address.
 		 *
 		 *	lba			- LBA address where the first directory record begins.
 		 */
 		int CalculateTreeLBA(int lba);
@@ -116,15 +114,15 @@
 		 *	*id			- The name of the file entry. It will be converted to uppercase and adds the file version
 		 *				identifier (;1) automatically.
 		 *	type		- The type of file to add, EntryFile is for standard files, EntryXA is for XA streams and
 		 *				EntryStr is for STR streams. To add directories, use AddDirEntry().
 		 *	*srcfile	- Path and filename to the source file.
 		 *  attributes  - GMT offset/XA permissions for the file, if applicable.
 		 */
-		bool AddFileEntry(const char* id, EntryType type, const std::filesystem::path& srcfile, const EntryAttributes& attributes, const char *trackid = nullptr);
+		bool AddFileEntry(const char* id, EntryType type, const fs::path& srcfile, const EntryAttributes& attributes, const char *trackid = nullptr);
 
 		/** Adds an invisible dummy file entry to the directory record. Its invisible because its file entry
 		 *	is not actually added to the directory record.
 		 *
 		 *	sectors	- The size of the dummy file in sector units (1 = 2048 bytes, 1024 = 2MB).
 		 *  type	- 0 for form1 (data) dummy, 1 for form2 (XA) dummy
 		 */
@@ -144,15 +142,15 @@
 		 *
 		 *	*id		- The name of the subdirectory to add. It will be converted to uppercase automatically.
 		 *  attributes  - GMT offset/XA permissions for the file, if applicable.
 		 *  alreadyExists - set to true if a returned DirTreeClass already existed
 		 *
 		 *	Returns: Pointer to another DirTreeClass for accessing the directory record of the subdirectory.
 		 */
-		DirTreeClass* AddSubDirEntry(const char* id, const std::filesystem::path& srcDir, const EntryAttributes& attributes, bool& alreadyExists);
+		DirTreeClass* AddSubDirEntry(const char* id, const fs::path& srcDir, const EntryAttributes& attributes, bool& alreadyExists);
 
 		/**	Writes the source files assigned to the directory entries to a CD image. Its recommended to execute
 		 *	this first before writing the actual file system.
 		 *
 		 *	*writer	- Pointer to a cd::IsoWriter class that is ready for writing.
 		 */
 		bool WriteFiles(cd::IsoWriter* writer) const;
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #pragma once
 
 #ifdef __cplusplus
 #include "miniaudio.h"
 #include "miniaudio_pcm.h"
 
-ma_result ma_decoder_init_path(const std::filesystem::path& pFilePath, const ma_decoder_config* pConfig, ma_decoder* pDecoder);
+ma_result ma_decoder_init_path(const fs::path& pFilePath, const ma_decoder_config* pConfig, ma_decoder* pDecoder);
 
-ma_result ma_redbook_decoder_init_path_by_ext(const std::filesystem::path& filePath, ma_decoder* pDecoder, VirtualWavEx *vw, bool& isLossy);
+ma_result ma_redbook_decoder_init_path_by_ext(const fs::path& filePath, ma_decoder* pDecoder, VirtualWavEx *vw, bool& isLossy);
 
 #if defined(MINIAUDIO_IMPLEMENTATION) || defined(MA_IMPLEMENTATION)
 
 // Helper wrapper to simplify dealing with paths on Windows
-ma_result ma_decoder_init_path(const std::filesystem::path& pFilePath, const ma_decoder_config* pConfig, ma_decoder* pDecoder)
+ma_result ma_decoder_init_path(const fs::path& pFilePath, const ma_decoder_config* pConfig, ma_decoder* pDecoder)
 {
 #ifdef _WIN32
 	return ma_decoder_init_file_w(pFilePath.c_str(), pConfig, pDecoder);
 #else
 	return ma_decoder_init_file(pFilePath.c_str(), pConfig, pDecoder);
 #endif
 }
@@ -24,15 +24,15 @@
 	DAF_WAV,
 	DAF_FLAC,
 	DAF_MP3,
 	DAF_PCM
 } DecoderAudioFormats;
 
 // Helper wrapper to open as redbook (44100kHz stereo s16le) audio and use the file extension to determine the order to try decoders
-ma_result ma_redbook_decoder_init_path_by_ext(const std::filesystem::path& filePath, ma_decoder* pDecoder, VirtualWavEx *vw, bool& isLossy)
+ma_result ma_redbook_decoder_init_path_by_ext(const fs::path& filePath, ma_decoder* pDecoder, VirtualWavEx *vw, bool& isLossy)
 {
 	ma_decoder_config decoderConfig = ma_decoder_config_init(ma_format_s16, 2, 44100);	
 	isLossy = false;
 
     DecoderAudioFormats tryorder[4] = {DAF_WAV, DAF_FLAC, DAF_MP3, DAF_PCM};
 	const auto& extension = filePath.extension().u8string();
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #include "common.h"
 
 class VirtualWavEx : public VirtualWav {
     public:
     unique_file pcmFp;
 };
 
-MA_API ma_result ma_decoder_init_path_pcm(const std::filesystem::path& pFilePath, ma_decoder_config* pConfig, ma_decoder* pDecoder, VirtualWavEx *pUserData);
+MA_API ma_result ma_decoder_init_path_pcm(const fs::path& pFilePath, ma_decoder_config* pConfig, ma_decoder* pDecoder, VirtualWavEx *pUserData);
 #endif
 
 #if defined(MINIAUDIO_IMPLEMENTATION) || defined(MA_IMPLEMENTATION)
 
 static size_t virtual_wav_read(ma_decoder *pDecoder, void *pBufferOut, size_t bytesToRead)
 {
     VirtualWav *vw = (VirtualWav *)pDecoder->pUserData;
@@ -202,15 +202,15 @@
         return !MA_SUCCESS;
     }
 
     return MA_SUCCESS;
 }
 #ifdef __cplusplus
 // feed to pcm file to miniaudio as a wav file
-MA_API ma_result ma_decoder_init_path_pcm(const std::filesystem::path& pFilePath, ma_decoder_config* pConfig, ma_decoder* pDecoder, VirtualWavEx *pUserData)
+MA_API ma_result ma_decoder_init_path_pcm(const fs::path& pFilePath, ma_decoder_config* pConfig, ma_decoder* pDecoder, VirtualWavEx *pUserData)
 {
     unique_file file(OpenFile(pFilePath, "rb"));
     if(!file)
     {
         return !MA_SUCCESS;
     }
     if(ma_decoder_init_FILE_pcm(file.get(), pConfig, pDecoder, pUserData) != MA_SUCCESS)
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/cd.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/cd.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/common.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 {
 	return  ((val & 0xFF) << 24) |
 			((val & 0xFF00) << 8) |
 			((val & 0xFF0000) >> 8) |
 			((val & 0xFF000000) >> 24);
 }
 
-unique_file OpenScopedFile(const std::filesystem::path& path, const char* mode)
+unique_file OpenScopedFile(const fs::path& path, const char* mode)
 {
 	return unique_file { OpenFile(path, mode) };
 }
 
 bool CompareICase(std::string_view strLeft, std::string_view strRight)
 {
 	return std::equal(strLeft.begin(), strLeft.end(), strRight.begin(), strRight.end(), [](char left, char right)
@@ -149,20 +149,20 @@
 	if (!command.empty() && arg.length() > 1 && arg[0] == '-' && arg.substr(1) == command)
 	{
 		return true;
 	}
 	return false;
 }
 
-std::optional<std::filesystem::path> ParsePathArgument(char**& argv, std::string_view command, std::string_view longCommand)
+std::optional<fs::path> ParsePathArgument(char**& argv, std::string_view command, std::string_view longCommand)
 {
 	if (ParseArgument(argv, command, longCommand) && *(argv+1) != nullptr)
 	{
 		argv++;
-		return std::filesystem::u8path(*argv);
+		return fs::u8path(*argv);
 	}
 	return std::nullopt;
 }
 
 std::optional<std::string> ParseStringArgument(char**& argv, std::string_view command, std::string_view longCommand)
 {
 	if (ParseArgument(argv, command, longCommand) && *(argv+1) != nullptr)
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/common.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pragma once
 
 #include "cd.h"
-#include <filesystem>
+#include "fs.h"
 #include <memory>
 #include <optional>
 #include <string>
 
 enum class EntryType
 {
 	EntryFile,
@@ -67,15 +67,15 @@
 		if (file != nullptr)
 		{
 			std::fclose(file);
 		}
 	}
 };
 using unique_file = std::unique_ptr<FILE, file_deleter>;
-unique_file OpenScopedFile(const std::filesystem::path& path, const char* mode);
+unique_file OpenScopedFile(const fs::path& path, const char* mode);
 
 bool CompareICase(std::string_view strLeft, std::string_view strRight);
 
 // Argument parsing
 bool ParseArgument(char** argv, std::string_view command, std::string_view longCommand = std::string_view{});
-std::optional<std::filesystem::path> ParsePathArgument(char**& argv, std::string_view command, std::string_view longCommand = std::string_view{});
+std::optional<fs::path> ParsePathArgument(char**& argv, std::string_view command, std::string_view longCommand = std::string_view{});
 std::optional<std::string> ParseStringArgument(char**& argv, std::string_view command, std::string_view longCommand = std::string_view{});
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/listview.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/listview.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/mmappedfile.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	if (m_handle != nullptr)
 	{
 		close(static_cast<int>(reinterpret_cast<intptr_t>(m_handle)));
 	}
 #endif
 }
 
-bool MMappedFile::Create(const std::filesystem::path& filePath, uint64_t size)
+bool MMappedFile::Create(const fs::path& filePath, uint64_t size)
 {
 	bool result = false;
 
 #ifdef _WIN32
 	HANDLE file = CreateFileW(filePath.c_str(), GENERIC_READ | GENERIC_WRITE, FILE_SHARE_DELETE, nullptr, CREATE_ALWAYS, FILE_ATTRIBUTE_NORMAL, nullptr);
 	if (file != INVALID_HANDLE_VALUE)
 	{
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/mmappedfile.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #pragma once
 
 // Cross-platform memory mapped file wrapper
 
 #include <cstdint>
-#include <filesystem>
+#include "fs.h"
 
 class MMappedFile
 {
 public:
 	class View
 	{
 	public:
@@ -21,13 +21,13 @@
 		void* m_data = nullptr;
 		size_t m_size = 0; // Real size, with adjustments to granularity
 	};
 
 	MMappedFile();
 	~MMappedFile();
 
-	bool Create(const std::filesystem::path& filePath, uint64_t size);
+	bool Create(const fs::path& filePath, uint64_t size);
 	View GetView(uint64_t offset, size_t size) const;
 
 private:
 	void* m_handle = nullptr; // Opaque, platform-specific
 };
```

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/xa.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/xa.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/src/shared/xml.h` & `pymkpsxiso-0.1.3/mkpsxiso/src/shared/xml.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/tinyxml2/tinyxml2.cpp` & `pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/mkpsxiso/tinyxml2/tinyxml2.h` & `pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.2/pymkpsxiso.cpp` & `pymkpsxiso-0.1.3/pymkpsxiso.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#define VERSION "2.02"
+#define VERSION "2.03"
 // This is kind of dirty, but the main.cpp file for both programs includes a lot of code
 // They both use a Main function so we need to change the name
 #define Main dumpsxiso_main
 #include "mkpsxiso/src/dumpsxiso/main.cpp"
 #define Main mkpsxiso_main
 #include "mkpsxiso/src/mkpsxiso/main.cpp"
 #undef Main
```

### Comparing `pymkpsxiso-0.1.2/pymkpsxiso.egg-info/PKG-INFO` & `pymkpsxiso-0.1.3/pymkpsxiso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkpsxiso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface for mkpsxiso.
 Home-page: https://github.com/Illidanz/pymkpsxiso
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymkpsxiso-0.1.2/pymkpsxiso.egg-info/SOURCES.txt` & `pymkpsxiso-0.1.3/pymkpsxiso.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 mkpsxiso/src/mkpsxiso/iso.cpp
 mkpsxiso/src/mkpsxiso/iso.h
 mkpsxiso/src/mkpsxiso/miniaudio_helpers.h
 mkpsxiso/src/mkpsxiso/miniaudio_pcm.h
 mkpsxiso/src/shared/cd.h
 mkpsxiso/src/shared/common.cpp
 mkpsxiso/src/shared/common.h
+mkpsxiso/src/shared/fs.cpp
+mkpsxiso/src/shared/fs.h
 mkpsxiso/src/shared/listview.h
 mkpsxiso/src/shared/mmappedfile.cpp
 mkpsxiso/src/shared/mmappedfile.h
 mkpsxiso/src/shared/platform.cpp
 mkpsxiso/src/shared/platform.h
 mkpsxiso/src/shared/xa.h
 mkpsxiso/src/shared/xml.h
```

### Comparing `pymkpsxiso-0.1.2/setup.py` & `pymkpsxiso-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import codecs
 import os
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 MACROS = [
@@ -21,15 +20,15 @@
 for dir in INCLUDES:
     for file in os.listdir(dir):
         if file.endswith(".cpp") and "xmltest" not in file and "example" not in file and "main.cpp" not in file:
             sources.append(dir + "/" + file)
 
 def main():
     setup(name="pymkpsxiso",
-          version="0.1.2",
+          version="0.1.3",
           author="Illidan",
           description="Python interface for mkpsxiso.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           url="https://github.com/Illidanz/pymkpsxiso",
           classifiers=[
               "Programming Language :: Python :: 3",
```

