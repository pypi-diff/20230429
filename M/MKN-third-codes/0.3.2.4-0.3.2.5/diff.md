# Comparing `tmp/MKN_third_codes-0.3.2.4.tar.gz` & `tmp/MKN_third_codes-0.3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.3.2.4.tar", last modified: Sat Apr 29 16:06:38 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.3.2.5.tar", last modified: Sat Apr 29 16:07:35 2023, max compression
```

## Comparing `MKN_third_codes-0.3.2.4.tar` & `MKN_third_codes-0.3.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:06:38.287276 MKN_third_codes-0.3.2.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 16:06:38.278302 MKN_third_codes-0.3.2.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:06:38.286279 MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-04-29 16:06:38.000000 MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-29 16:06:38.000000 MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:06:38.000000 MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 16:06:38.000000 MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1935 2023-04-29 16:06:38.287276 MKN_third_codes-0.3.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2023-04-29 15:53:24.000000 MKN_third_codes-0.3.2.4/README.md
--rw-rw-rw-   0        0        0     1698 2023-04-29 16:06:25.000000 MKN_third_codes-0.3.2.4/README_PYPI.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 16:06:38.287276 MKN_third_codes-0.3.2.4/setup.cfg
--rw-rw-rw-   0        0        0      394 2023-04-29 16:06:33.000000 MKN_third_codes-0.3.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:35.657161 MKN_third_codes-0.3.2.5/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:35.644194 MKN_third_codes-0.3.2.5/MKN_third_codes/
+-rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2.5/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:35.655165 MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     1943 2023-04-29 16:07:35.000000 MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-29 16:07:35.000000 MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:07:35.000000 MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 16:07:35.000000 MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1943 2023-04-29 16:07:35.656163 MKN_third_codes-0.3.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-04-29 15:53:24.000000 MKN_third_codes-0.3.2.5/README.md
+-rw-rw-rw-   0        0        0     1706 2023-04-29 16:07:27.000000 MKN_third_codes-0.3.2.5/README_PYPI.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:07:35.657161 MKN_third_codes-0.3.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      394 2023-04-29 16:07:31.000000 MKN_third_codes-0.3.2.5/setup.py
```

### Comparing `MKN_third_codes-0.3.2.4/LICENSE.txt` & `MKN_third_codes-0.3.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.3.2.5/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.3.2.5/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.3.2.4
+Version: 0.3.2.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 License-File: LICENSE.txt
 
 Здарова! Библиотека немного помогает с тервером по МКН 3
 
 Версия: 0.3.2
-`
+``
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
-`
+``
 Использование
-`
+``
 Функции
 - любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Все взаимодействие происходит в терминале.
 - любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под нее, то ими возможно будет неудобно пользоваться.
-`
+``
 Установка
-`
+``
 Консоль: pip install --upgrade MKN_third_codes
-`
+``
 Контакты
-`
+``
 Я в ВК: https://vk.com/ivandolgun
 Я в Discord: ИVAN#2599
-`
+``
```

### Comparing `MKN_third_codes-0.3.2.4/PKG-INFO` & `MKN_third_codes-0.3.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.3.2.4
+Version: 0.3.2.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 License-File: LICENSE.txt
 
 Здарова! Библиотека немного помогает с тервером по МКН 3
 
 Версия: 0.3.2
-`
+``
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
-`
+``
 Использование
-`
+``
 Функции
 - любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Все взаимодействие происходит в терминале.
 - любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под нее, то ими возможно будет неудобно пользоваться.
-`
+``
 Установка
-`
+``
 Консоль: pip install --upgrade MKN_third_codes
-`
+``
 Контакты
-`
+``
 Я в ВК: https://vk.com/ivandolgun
 Я в Discord: ИVAN#2599
-`
+``
```

### Comparing `MKN_third_codes-0.3.2.4/README.md` & `MKN_third_codes-0.3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2.4/README_PYPI.txt` & `MKN_third_codes-0.3.2.5/README_PYPI.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Здарова! Библиотека немного помогает с тервером по МКН 3
 
 Версия: 0.3.2
-`
+``
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
-`
+``
 Использование
-`
+``
 Функции
 - любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Все взаимодействие происходит в терминале.
 - любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под нее, то ими возможно будет неудобно пользоваться.
-`
+``
 Установка
-`
+``
 Консоль: pip install --upgrade MKN_third_codes
-`
+``
 Контакты
-`
+``
 Я в ВК: https://vk.com/ivandolgun
 Я в Discord: ИVAN#2599
-`
+``
```

