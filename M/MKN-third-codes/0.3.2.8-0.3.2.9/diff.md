# Comparing `tmp/MKN_third_codes-0.3.2.8.tar.gz` & `tmp/MKN_third_codes-0.3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.3.2.8.tar", last modified: Sat Apr 29 16:12:47 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.3.2.9.tar", last modified: Sat Apr 29 16:13:53 2023, max compression
```

## Comparing `MKN_third_codes-0.3.2.8.tar` & `MKN_third_codes-0.3.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:12:47.806397 MKN_third_codes-0.3.2.8/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 16:12:47.798420 MKN_third_codes-0.3.2.8/MKN_third_codes/
--rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2.8/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:12:47.805400 MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     1931 2023-04-29 16:12:47.000000 MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-29 16:12:47.000000 MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:12:47.000000 MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 16:12:47.000000 MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1931 2023-04-29 16:12:47.805400 MKN_third_codes-0.3.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2023-04-29 15:53:24.000000 MKN_third_codes-0.3.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 16:12:47.806397 MKN_third_codes-0.3.2.8/setup.cfg
--rw-rw-rw-   0        0        0      393 2023-04-29 16:12:07.000000 MKN_third_codes-0.3.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:13:53.765948 MKN_third_codes-0.3.2.9/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2.9/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 16:13:53.756971 MKN_third_codes-0.3.2.9/MKN_third_codes/
+-rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2.9/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:13:53.764949 MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     1955 2023-04-29 16:13:53.000000 MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-29 16:13:53.000000 MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:13:53.000000 MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 16:13:53.000000 MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1955 2023-04-29 16:13:53.765948 MKN_third_codes-0.3.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-04-29 15:53:24.000000 MKN_third_codes-0.3.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:13:53.765948 MKN_third_codes-0.3.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      393 2023-04-29 16:13:47.000000 MKN_third_codes-0.3.2.9/setup.py
```

### Comparing `MKN_third_codes-0.3.2.8/LICENSE.txt` & `MKN_third_codes-0.3.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2.8/MKN_third_codes/solutions.py` & `MKN_third_codes-0.3.2.9/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2.8/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.3.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.3.2.8
+Name: MKN_third_codes
+Version: 0.3.2.9
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 License-File: LICENSE.txt
 
-Здарова! Библиотека немного помогает с тервером по МКН 3
+### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-Версия: 0.3.2
+## Версия: 0.3.2
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
 
-Использование
+# Использование
 
-Функции
+## Функции
 - любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Все взаимодействие происходит в терминале.
 - любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 
-Классы
+## Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под нее, то ими возможно будет неудобно пользоваться.
 
-Установка
+# Установка
 
-Консоль: pip install --upgrade MKN_third_codes
+### Консоль: pip install --upgrade MKN_third_codes
 
-Контакты
+## Контакты
 
 - Я в ВК: https://vk.com/ivandolgun
 - Я в Discord: ИVAN#2599
```

### Comparing `MKN_third_codes-0.3.2.8/PKG-INFO` & `MKN_third_codes-0.3.2.9/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.3.2.8
+Name: MKN-third-codes
+Version: 0.3.2.9
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 License-File: LICENSE.txt
 
-Здарова! Библиотека немного помогает с тервером по МКН 3
+### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-Версия: 0.3.2
+## Версия: 0.3.2
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
 
-Использование
+# Использование
 
-Функции
+## Функции
 - любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Все взаимодействие происходит в терминале.
 - любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 
-Классы
+## Классы
 - Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под нее, то ими возможно будет неудобно пользоваться.
 
-Установка
+# Установка
 
-Консоль: pip install --upgrade MKN_third_codes
+### Консоль: pip install --upgrade MKN_third_codes
 
-Контакты
+## Контакты
 
 - Я в ВК: https://vk.com/ivandolgun
 - Я в Discord: ИVAN#2599
```

### Comparing `MKN_third_codes-0.3.2.8/README.md` & `MKN_third_codes-0.3.2.9/README.md`

 * *Files identical despite different names*

