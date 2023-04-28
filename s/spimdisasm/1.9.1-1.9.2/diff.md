# Comparing `tmp/spimdisasm-1.9.1.tar.gz` & `tmp/spimdisasm-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spimdisasm-1.9.1.tar", last modified: Thu Dec 29 21:07:19 2022, max compression
+gzip compressed data, was "spimdisasm-1.9.2.tar", last modified: Mon Jan  2 19:38:18 2023, max compression
```

## Comparing `spimdisasm-1.9.1.tar` & `spimdisasm-1.9.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.412568 spimdisasm-1.9.1/spimdisasm/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/common/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/Context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/ContextSymbols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/ElementBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/FileSectionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/FileSplitFormat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/GlobalConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/GlobalOffsetTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/OrderedEnum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/Relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/SortedDict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/SymbolsSegment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/disasmdis/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/disasmdis/DisasmdisInternals.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/disasmdis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/disasmdis/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/elf32/
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32Dyns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32GlobalOffsetTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32Header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32RegInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32Rels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32SectionHeaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32StringTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/Elf32Syms.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elf32/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/elfObjDisasm/
--rw-r--r--   0 runner    (1001) docker     (123)    16151 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elfObjDisasm/ElfObjDisasmInternals.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elfObjDisasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/elfObjDisasm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/frontendCommon/
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/frontendCommon/FrontendUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/frontendCommon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.416569 spimdisasm-1.9.1/spimdisasm/mips/
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/FilesHandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/InstructionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/MipsFileBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/MipsFileSplits.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/spimdisasm/mips/sections/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionBss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionData.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionRelocZ64.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionRodata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionText.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/spimdisasm/mips/symbols/
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolBss.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolData.py
--rw-r--r--   0 runner    (1001) docker     (123)    28778 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolRodata.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolText.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/spimdisasm/mips/symbols/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    21056 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/analysis/InstrAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/mips/symbols/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/spimdisasm/rspDisasm/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/rspDisasm/RspDisasmInternals.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/rspDisasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/rspDisasm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.420569 spimdisasm-1.9.1/spimdisasm/singleFileDisasm/
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/singleFileDisasm/SingleFileDisasmInternals.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/singleFileDisasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-29 21:07:11.000000 spimdisasm-1.9.1/spimdisasm/singleFileDisasm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:07:19.412568 spimdisasm-1.9.1/spimdisasm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2022-12-29 21:07:19.000000 spimdisasm-1.9.1/spimdisasm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2022-12-29 21:07:19.000000 spimdisasm-1.9.1/spimdisasm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 21:07:19.000000 spimdisasm-1.9.1/spimdisasm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-29 21:07:19.000000 spimdisasm-1.9.1/spimdisasm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-29 21:07:19.000000 spimdisasm-1.9.1/spimdisasm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.721070 spimdisasm-1.9.2/spimdisasm/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.725070 spimdisasm-1.9.2/spimdisasm/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/Context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/ContextSymbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/ElementBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/FileSectionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/FileSplitFormat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/GlobalConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/GlobalOffsetTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/OrderedEnum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/Relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/SortedDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/SymbolsSegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.725070 spimdisasm-1.9.2/spimdisasm/disasmdis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/disasmdis/DisasmdisInternals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/disasmdis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/disasmdis/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.725070 spimdisasm-1.9.2/spimdisasm/elf32/
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32Dyns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32GlobalOffsetTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32Header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32RegInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32Rels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32SectionHeaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32StringTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/Elf32Syms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elf32/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.729070 spimdisasm-1.9.2/spimdisasm/elfObjDisasm/
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elfObjDisasm/ElfObjDisasmInternals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elfObjDisasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/elfObjDisasm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.729070 spimdisasm-1.9.2/spimdisasm/frontendCommon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/frontendCommon/FrontendUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/frontendCommon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.729070 spimdisasm-1.9.2/spimdisasm/mips/
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/FilesHandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/InstructionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/MipsFileBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/MipsFileSplits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.729070 spimdisasm-1.9.2/spimdisasm/mips/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionBss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionRelocZ64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionRodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionText.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/spimdisasm/mips/symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolBss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28727 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolRodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolText.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/spimdisasm/mips/symbols/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/analysis/InstrAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/mips/symbols/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/spimdisasm/rspDisasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/rspDisasm/RspDisasmInternals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/rspDisasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/rspDisasm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.733070 spimdisasm-1.9.2/spimdisasm/singleFileDisasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/singleFileDisasm/SingleFileDisasmInternals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/singleFileDisasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-02 19:38:00.000000 spimdisasm-1.9.2/spimdisasm/singleFileDisasm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 19:38:18.721070 spimdisasm-1.9.2/spimdisasm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-01-02 19:38:18.000000 spimdisasm-1.9.2/spimdisasm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-01-02 19:38:18.000000 spimdisasm-1.9.2/spimdisasm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 19:38:18.000000 spimdisasm-1.9.2/spimdisasm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-02 19:38:18.000000 spimdisasm-1.9.2/spimdisasm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-02 19:38:18.000000 spimdisasm-1.9.2/spimdisasm.egg-info/top_level.txt
```

### Comparing `spimdisasm-1.9.1/LICENSE` & `spimdisasm-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/PKG-INFO` & `spimdisasm-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spimdisasm
-Version: 1.9.1
+Version: 1.9.2
 Summary: MIPS disassembler
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/spimdisasm
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/spimdisasm/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spimdisasm-1.9.1/README.md` & `spimdisasm-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/pyproject.toml` & `spimdisasm-1.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "spimdisasm"
 # Version should be synced with spimdisasm/__init__.py
-version = "1.9.1"
+version = "1.9.2"
 description = "MIPS disassembler"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `spimdisasm-1.9.1/spimdisasm/__main__.py` & `spimdisasm-1.9.2/spimdisasm/__main__.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/Context.py` & `spimdisasm-1.9.2/spimdisasm/common/Context.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/ContextSymbols.py` & `spimdisasm-1.9.2/spimdisasm/common/ContextSymbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
 from typing import Callable
 import rabbitizer
 
-from .GlobalConfig import GlobalConfig
+from .GlobalConfig import GlobalConfig, Compiler
 from .FileSectionType import FileSectionType
 
 
 class SymbolSpecialType(enum.Enum):
     function        = enum.auto()
     branchlabel     = enum.auto()
     jumptable       = enum.auto()
@@ -70,14 +70,15 @@
 }
 
 
 @dataclasses.dataclass
 class ContextSymbol:
     address: int
     name: str|None = None
+    nameEnd: str|None = None
     size: int|None = None
     autodetectedSize: int|None = None
     type: SymbolSpecialType|str|None = None
 
     accessType: rabbitizer.Enum|None = None
     unsignedAccessType: bool|None = None
 
@@ -238,14 +239,17 @@
         if self._isStatic:
             return True
         if self.name is None:
             return False
         return self.name.startswith(".")
 
     def isLateRodata(self) -> bool:
+        if GlobalConfig.COMPILER != Compiler.IDO:
+            # late rodata only exists in IDO world
+            return False
         # if self.referenceCounter > 1: return False # ?
         return self.isJumpTable() or self.isFloat() or self.isDouble()
 
 
     def getDefaultName(self) -> str:
         suffix = ""
         if self.overlayCategory is not None:
@@ -285,14 +289,17 @@
     def setNameGetCallback(self, callback: Callable[[ContextSymbol], str]) -> None:
         self.nameGetCallback = callback
 
     def setNameGetCallbackIfUnset(self, callback: Callable[[ContextSymbol], str]) -> None:
         if self.nameGetCallback is None:
             self.nameGetCallback = callback
 
+    def getNameEnd(self) -> str|None:
+        return self.nameEnd
+
     def getSize(self) -> int:
         # User-declared size first
         if self.size is not None:
             return self.size
 
         if self.autodetectedSize is not None:
             return self.autodetectedSize
@@ -359,50 +366,49 @@
     def getSymbolPlusOffset(self, address: int) -> str:
         if self.address == address:
             return self.getName()
         if self.address > address:
             return f"{self.getName()} - 0x{self.address - address:X}"
         return f"{self.getName()} + 0x{address - self.address:X}"
 
-    def getSymbolLabel(self) -> str:
+    def getLabelMacro(self) -> str|None:
         if not GlobalConfig.ASM_USE_SYMBOL_LABEL:
-            return ""
+            return None
         label = ""
         if GlobalConfig.ASM_COMMENT:
             if self.isStatic():
                 label += f"# static variable{GlobalConfig.LINE_ENDS}"
             if self.isAutogeneratedPad():
                 label += f"# Automatically generated pad{GlobalConfig.LINE_ENDS}"
         if self.type == SymbolSpecialType.jumptablelabel:
             label += GlobalConfig.ASM_JTBL_LABEL
         elif self.sectionType == FileSectionType.Text:
             label += GlobalConfig.ASM_TEXT_LABEL
         else:
             label += GlobalConfig.ASM_DATA_LABEL
-        label += " " + self.getName()
         return label
 
     def isAutogeneratedPad(self) -> bool:
         return self.isAutoCreatedPad and self.referenceCounter == 0 and self.isAutogenerated
 
 
     @staticmethod
     def getCsvHeader() -> str:
-        output = "address,name,getName,getType,accessType,"
+        output = "address,name,getName,getNameEnd,getType,accessType,"
         output += "size,"
         output += "autodetectedSize,"
         output += "getSize,getVrom,sectionType,"
         output += "isDefined,isUserDeclared,isAutogenerated,isMaybeString,"
         output += "referenceCounter,overlayCategory,unknownSegment,"
         output += "isGot,isGotGlobal,isGotLocal,gotIndex,"
         output += "firstLoAccess,isAutogeneratedPad,isElfNotype"
         return output
 
     def toCsv(self) -> str:
-        output = f"0x{self.address:06X},{self.name},{self.getName()},{self.getType()},"
+        output = f"0x{self.address:06X},{self.name},{self.getName()},{self.getNameEnd()},{self.getType()},"
         if self.accessType is None:
             output += "None,"
         else:
             output += f"{self.accessType.name},"
         if self.size is None:
             output += "None,"
         else:
```

### Comparing `spimdisasm-1.9.1/spimdisasm/common/ElementBase.py` & `spimdisasm-1.9.2/spimdisasm/common/ElementBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,34 +69,38 @@
 
     def setVram(self, vram: int):
         self.vram = vram
 
     def setCommentOffset(self, commentOffset: int):
         self.commentOffset = commentOffset
 
+    def getName(self) -> str:
+        return self.name
+
     def getVromOffset(self, localOffset: int) -> int:
         return self.vromStart + localOffset
 
     def getVramOffset(self, localOffset: int) -> int:
         return self.vram + localOffset
 
     def containsVram(self, vram: int) -> bool:
         if vram < self.vram:
             return False
         if vram >= self.vramEnd:
             return False
         return True
 
 
-    def getLabelFromSymbol(self, sym: ContextSymbol|None) -> str:
+    def getLabelFromSymbol(self, sym: ContextSymbol|None, symName: str|None) -> str:
         "Generates a glabel for the passed symbol, including an optional index value if it was set and it is enabled in the GlobalConfig"
         if sym is not None:
-            label = sym.getSymbolLabel()
-            if not label:
+            label = sym.getLabelMacro()
+            if label is None:
                 return ""
+            label += f" {symName or sym.getName()}"
             if GlobalConfig.GLABEL_ASM_COUNT:
                 if self.index is not None:
                     label += f" # {self.index}"
             label +=  GlobalConfig.LINE_ENDS
             return label
         return ""
```

### Comparing `spimdisasm-1.9.1/spimdisasm/common/FileSectionType.py` & `spimdisasm-1.9.2/spimdisasm/common/FileSectionType.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/FileSplitFormat.py` & `spimdisasm-1.9.2/spimdisasm/common/FileSplitFormat.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/GlobalConfig.py` & `spimdisasm-1.9.2/spimdisasm/common/GlobalConfig.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/GlobalOffsetTable.py` & `spimdisasm-1.9.2/spimdisasm/common/GlobalOffsetTable.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/OrderedEnum.py` & `spimdisasm-1.9.2/spimdisasm/common/OrderedEnum.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/Relocation.py` & `spimdisasm-1.9.2/spimdisasm/common/Relocation.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/SortedDict.py` & `spimdisasm-1.9.2/spimdisasm/common/SortedDict.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/SymbolsSegment.py` & `spimdisasm-1.9.2/spimdisasm/common/SymbolsSegment.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/Utils.py` & `spimdisasm-1.9.2/spimdisasm/common/Utils.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/common/__init__.py` & `spimdisasm-1.9.2/spimdisasm/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/disasmdis/DisasmdisInternals.py` & `spimdisasm-1.9.2/spimdisasm/disasmdis/DisasmdisInternals.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32Constants.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32Constants.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32Dyns.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32Dyns.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32File.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32File.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32GlobalOffsetTable.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32GlobalOffsetTable.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32Header.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32Header.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32RegInfo.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32RegInfo.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32Rels.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32Rels.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32SectionHeaders.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32SectionHeaders.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32StringTable.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32StringTable.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/Elf32Syms.py` & `spimdisasm-1.9.2/spimdisasm/elf32/Elf32Syms.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elf32/__init__.py` & `spimdisasm-1.9.2/spimdisasm/elf32/__init__.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/elfObjDisasm/ElfObjDisasmInternals.py` & `spimdisasm-1.9.2/spimdisasm/elfObjDisasm/ElfObjDisasmInternals.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/frontendCommon/FrontendUtilities.py` & `spimdisasm-1.9.2/spimdisasm/frontendCommon/FrontendUtilities.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/FilesHandlers.py` & `spimdisasm-1.9.2/spimdisasm/mips/FilesHandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     for rodataSym in rodataSection.symbolList:
         if rodataSym.vram not in intersection:
             continue
 
         if not rodataSym.shouldMigrate():
             continue
 
-        if rodataSym.contextSym.isLateRodata() and common.GlobalConfig.COMPILER == common.Compiler.IDO:
+        if rodataSym.contextSym.isLateRodata():
             lateRodataList.append(rodataSym)
             lateRodataSize += rodataSym.sizew
         else:
             rdataList.append(rodataSym)
 
     return rdataList, lateRodataList, lateRodataSize
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/InstructionConfig.py` & `spimdisasm-1.9.2/spimdisasm/mips/InstructionConfig.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/MipsFileBase.py` & `spimdisasm-1.9.2/spimdisasm/mips/MipsFileBase.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/MipsFileSplits.py` & `spimdisasm-1.9.2/spimdisasm/mips/MipsFileSplits.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionBase.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionBase.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionBss.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionBss.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionData.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionData.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionRelocZ64.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionRelocZ64.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionRodata.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionRodata.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,26 @@
             sym.analyze()
             self.symbolList.append(sym)
 
             # File boundaries detection
             if sym.inFileOffset % 16 == 0:
                 # Files are always 0x10 aligned
 
-                if previousSymbolWasLateRodata and not sym.contextSym.isLateRodata() and common.GlobalConfig.COMPILER == common.Compiler.IDO:
+                if previousSymbolWasLateRodata and not sym.contextSym.isLateRodata():
                     # late rodata followed by normal rodata implies a file split
                     self.fileBoundaries.append(sym.inFileOffset)
                 elif previousSymbolExtraPadding > 0:
-                    if sym.contextSym.isDouble():
+                    if sym.isDouble(0):
                         # doubles require a bit extra of alignment
                         if previousSymbolExtraPadding >= 2:
                             self.fileBoundaries.append(sym.inFileOffset)
+                    elif sym.isJumpTable() and common.GlobalConfig.COMPILER != common.Compiler.IDO:
+                        # non-IDO compilers emit a directive to align jumptables to 0x8 boundary
+                        if previousSymbolExtraPadding >= 2:
+                            self.fileBoundaries.append(sym.inFileOffset)
                     else:
                         self.fileBoundaries.append(sym.inFileOffset)
 
             previousSymbolWasLateRodata = sym.contextSym.isLateRodata()
             previousSymbolExtraPadding = sym.countExtraPadding()
 
         self.processStaticRelocs()
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/sections/MipsSectionText.py` & `spimdisasm-1.9.2/spimdisasm/mips/sections/MipsSectionText.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolBase.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
         self.relocs: dict[int, common.RelocationInfo] = dict()
         "key: word offset"
 
 
     def getName(self) -> str:
         return self.contextSym.getName()
 
+    def getNameEnd(self) -> str|None:
+        return self.contextSym.getNameEnd()
+
     def setNameIfUnset(self, name: str) -> None:
         self.contextSym.setNameIfUnset(name)
 
     def setNameGetCallback(self, callback: Callable[[common.ContextSymbol], str]) -> None:
         self.contextSym.setNameGetCallback(callback)
 
     def setNameGetCallbackIfUnset(self, callback: Callable[[common.ContextSymbol], str]) -> None:
@@ -53,21 +56,38 @@
         wordValueHex = ""
         if wordValue is not None:
             wordValueHex = f"{common.Utils.wordToCurrenEndian(wordValue):08X} "
 
         return f"/* {offsetHex} {vramHex} {wordValueHex}*/"
 
 
+    def getSymbolAsmDeclaration(self, symName: str, useGlobalLabel: bool=True) -> str:
+        if not useGlobalLabel:
+            return f"{symName}:" + common.GlobalConfig.LINE_ENDS
+
+        output = ""
+        output += self.getLabelFromSymbol(self.contextSym, symName)
+        if self.sectionType == common.FileSectionType.Text:
+            if common.GlobalConfig.ASM_TEXT_ENT_LABEL:
+                output += f"{common.GlobalConfig.ASM_TEXT_ENT_LABEL} {symName}{common.GlobalConfig.LINE_ENDS}"
+
+            if common.GlobalConfig.ASM_TEXT_FUNC_AS_LABEL:
+                output += f"{symName}:{common.GlobalConfig.LINE_ENDS}"
+        else:
+            if common.GlobalConfig.ASM_DATA_SYM_AS_LABEL:
+                output += f"{symName}:{common.GlobalConfig.LINE_ENDS}"
+        return output
+
     def getExtraLabelFromSymbol(self, contextSym: common.ContextSymbol|None) -> str:
         label = ""
         if contextSym is not None:
             label = common.GlobalConfig.LINE_ENDS
-            symLabel = contextSym.getSymbolLabel()
-            if symLabel:
-                label += symLabel + common.GlobalConfig.LINE_ENDS
+            symLabel = contextSym.getLabelMacro()
+            if symLabel is not None:
+                label += f"{symLabel} {contextSym.getName()}{common.GlobalConfig.LINE_ENDS}"
                 if common.GlobalConfig.ASM_DATA_SYM_AS_LABEL:
                     label += f"{contextSym.getName()}:" + common.GlobalConfig.LINE_ENDS
         return label
 
 
     def isByte(self, index: int) -> bool:
         return self.contextSym.isByte() and not self.isString()
@@ -347,29 +367,30 @@
 
 
     def countExtraPadding(self) -> int:
         "Returns how many extra word paddings this symbol has"
         return 0
 
     def getPrevAlignDirective(self, i: int=0) -> str:
-        commentPaddingNum = 22
-        if not common.GlobalConfig.ASM_COMMENT:
-            commentPaddingNum = 1
-
-        alignDirective = ""
+        if self.parent is not None and self.parent.vram % 0x8 != 0:
+            # Can't emit alignment directives if the parent file isn't properly aligned
+            return ""
 
         if self.isDouble(i):
             if common.GlobalConfig.COMPILER in {common.Compiler.SN64, common.Compiler.PSYQ}:
                 # This should be harmless in other compilers
                 # TODO: investigate if it is fine to use it unconditionally
-                alignDirective += commentPaddingNum * " "
-                alignDirective += ".align 3"
-                alignDirective += common.GlobalConfig.LINE_ENDS
+                return f".align 3{common.GlobalConfig.LINE_ENDS}"
+        elif self.isJumpTable():
+            if i == 0 and common.GlobalConfig.COMPILER not in {common.Compiler.IDO, common.Compiler.PSYQ}:
 
-        return alignDirective
+                if self.vram % 0x8 == 0:
+                    return f".align 3{common.GlobalConfig.LINE_ENDS}"
+
+        return ""
 
     def getPostAlignDirective(self, i: int=0) -> str:
         commentPaddingNum = 22
         if not common.GlobalConfig.ASM_COMMENT:
             commentPaddingNum = 1
 
         alignDirective = ""
@@ -399,22 +420,17 @@
             for sym in self.contextSym.referenceSymbols:
                 output += f" {sym.getName()}"
             return f"{output}{common.GlobalConfig.LINE_ENDS}"
         return ""
 
     def disassembleAsData(self, useGlobalLabel: bool=True) -> str:
         output = self.getReferenceeSymbols()
+        output += self.getPrevAlignDirective(0)
 
-        if useGlobalLabel:
-            output += self.getPrevAlignDirective(0)
-            output += self.getLabelFromSymbol(self.contextSym)
-            if common.GlobalConfig.ASM_DATA_SYM_AS_LABEL:
-                output += f"{self.getName()}:" + common.GlobalConfig.LINE_ENDS
-        else:
-            output += f"{self.getName()}:" + common.GlobalConfig.LINE_ENDS
+        output += self.getSymbolAsmDeclaration(self.getName(), useGlobalLabel)
 
         canReferenceSymbolsWithAddends = self.canUseAddendsOnData()
         canReferenceConstants = self.canUseConstantsOnData()
 
         i = 0
         while i < self.sizew:
             vram = self.getVramOffset(i*4)
@@ -443,14 +459,19 @@
             if i != 0:
                 output += self.getPrevAlignDirective(i)
             output += data
             output += self.getPostAlignDirective(i)
 
             i += skip
             i += 1
+
+        nameEnd = self.getNameEnd()
+        if nameEnd is not None:
+            output += self.getSymbolAsmDeclaration(nameEnd, useGlobalLabel)
+
         return output
 
     def disassemble(self, migrate: bool=False, useGlobalLabel: bool=True) -> str:
         output = ""
 
         if migrate:
             output += self.getSpimdisasmVersionString()
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolBss.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolBss.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,26 @@
         self.spaceSize: int = spaceSize
 
 
     @property
     def sizew(self) -> int:
         return self.spaceSize // 4
 
-    def disassembleAsBss(self) -> str:
+    def disassembleAsBss(self, useGlobalLabel: bool=True) -> str:
         output = self.getReferenceeSymbols()
+        output += self.getPrevAlignDirective(0)
 
-        output += self.getLabelFromSymbol(self.contextSym)
-        if common.GlobalConfig.ASM_DATA_SYM_AS_LABEL:
-            output += f"{self.getName()}:" + common.GlobalConfig.LINE_ENDS
+        output += self.getSymbolAsmDeclaration(self.getName(), useGlobalLabel)
         output += self.generateAsmLineComment(0)
-        output += f" .space 0x{self.spaceSize:02X}" + common.GlobalConfig.LINE_ENDS
+        output += f" .space 0x{self.spaceSize:02X}{common.GlobalConfig.LINE_ENDS}"
+
+        nameEnd = self.getNameEnd()
+        if nameEnd is not None:
+            output += self.getSymbolAsmDeclaration(nameEnd, useGlobalLabel)
+
         return output
 
     def disassemble(self, migrate: bool=False, useGlobalLabel: bool=True) -> str:
         output = ""
 
         if migrate:
             output += self.getSpimdisasmVersionString()
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolData.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolData.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolFunction.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolFunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,17 +557,18 @@
 
         if labelSym is None or labelSym.overlayCategory != self.overlayCategory:
             return ""
 
         labelSym.isDefined = True
         labelSym.sectionType = self.sectionType
         if labelSym.type == common.SymbolSpecialType.function or (labelSym.type == common.SymbolSpecialType.jumptablelabel and not migrate):
-            label = labelSym.getSymbolLabel()
-            if label:
-                label += common.GlobalConfig.LINE_ENDS
+            label = ""
+            labelMacro = labelSym.getLabelMacro()
+            if labelMacro is not None:
+                label += f"{labelMacro} {labelSym.getName()}{common.GlobalConfig.LINE_ENDS}"
             if common.GlobalConfig.ASM_TEXT_FUNC_AS_LABEL:
                 label += f"{labelSym.getName()}:{common.GlobalConfig.LINE_ENDS}"
             return label
         return labelSym.getName() + ":" + common.GlobalConfig.LINE_ENDS
 
     def _emitInstruction(self, instr: rabbitizer.Instruction, instructionOffset: int, wasLastInstABranch: bool) -> str:
         immOverride = self.getImmOverrideForInstruction(instr, instructionOffset)
@@ -617,21 +618,15 @@
         output += self.getReferenceeSymbols()
 
         if self.isLikelyHandwritten:
             if not self.isRsp:
                 # RSP functions are always handwritten, so this is redundant
                 output += "# Handwritten function" + common.GlobalConfig.LINE_ENDS
 
-        output += self.getLabelFromSymbol(self.contextSym)
-
-        if common.GlobalConfig.ASM_TEXT_ENT_LABEL:
-            output += f"{common.GlobalConfig.ASM_TEXT_ENT_LABEL} {self.getName()}" + common.GlobalConfig.LINE_ENDS
-
-        if common.GlobalConfig.ASM_TEXT_FUNC_AS_LABEL:
-            output += f"{self.getName()}:" + common.GlobalConfig.LINE_ENDS
+        output += self.getSymbolAsmDeclaration(self.getName(), useGlobalLabel)
 
         wasLastInstABranch = False
         instructionOffset = 0
         for instr in self.instructions:
             label = self.getLabelForOffset(instructionOffset, migrate=migrate)
             output += label
 
@@ -643,12 +638,16 @@
 
             wasLastInstABranch = instr.hasDelaySlot()
             instructionOffset += 4
 
         if common.GlobalConfig.ASM_TEXT_END_LABEL:
             output += f"{common.GlobalConfig.ASM_TEXT_END_LABEL} {self.getName()}" + common.GlobalConfig.LINE_ENDS
 
+        nameEnd = self.getNameEnd()
+        if nameEnd is not None:
+            output += self.getSymbolAsmDeclaration(nameEnd, useGlobalLabel)
+
         return output
 
     def disassembleAsData(self, useGlobalLabel: bool=True) -> str:
         self.words = [instr.getRaw() for instr in self.instructions]
         return super().disassembleAsData(useGlobalLabel=useGlobalLabel)
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolRodata.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolRodata.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,24 +102,17 @@
         else:
             for i in range(len(self.words)-1, 0, -1):
                 if self.words[i] != 0:
                     break
                 count += 1
         return count
 
-    def getPrevAlignDirective(self, i: int=0) -> str:
-        if self.isJumpTable():
-            if i == 0 and common.GlobalConfig.COMPILER != common.Compiler.IDO:
-                return f".align 3{common.GlobalConfig.LINE_ENDS}"
-        return super().getPrevAlignDirective(i)
-
     def getNthWord(self, i: int, canReferenceSymbolsWithAddends: bool=False, canReferenceConstants: bool=False) -> tuple[str, int]:
         localOffset = 4*i
         w = self.words[i]
-        vram = self.getVramOffset(localOffset)
         vrom = self.getVromOffset(localOffset)
 
         label = ""
         rodataWord: int|None = w
         value: str = f"0x{w:08X}"
 
         dotType = ".word"
```

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/MipsSymbolText.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/MipsSymbolText.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/mips/symbols/analysis/InstrAnalyzer.py` & `spimdisasm-1.9.2/spimdisasm/mips/symbols/analysis/InstrAnalyzer.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/rspDisasm/RspDisasmInternals.py` & `spimdisasm-1.9.2/spimdisasm/rspDisasm/RspDisasmInternals.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm/singleFileDisasm/SingleFileDisasmInternals.py` & `spimdisasm-1.9.2/spimdisasm/singleFileDisasm/SingleFileDisasmInternals.py`

 * *Files identical despite different names*

### Comparing `spimdisasm-1.9.1/spimdisasm.egg-info/PKG-INFO` & `spimdisasm-1.9.2/spimdisasm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spimdisasm
-Version: 1.9.1
+Version: 1.9.2
 Summary: MIPS disassembler
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/spimdisasm
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/spimdisasm/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spimdisasm-1.9.1/spimdisasm.egg-info/SOURCES.txt` & `spimdisasm-1.9.2/spimdisasm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

