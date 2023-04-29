# Comparing `tmp/MKN_third_codes-0.3.2.tar.gz` & `tmp/MKN_third_codes-0.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.3.2.tar", last modified: Sat Apr 29 15:45:23 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.3.3.1.tar", last modified: Sat Apr 29 16:21:29 2023, max compression
```

## Comparing `MKN_third_codes-0.3.2.tar` & `MKN_third_codes-0.3.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.413063 MKN_third_codes-0.3.2/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.399100 MKN_third_codes-0.3.2/MKN_third_codes/
--rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.412065 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     2156 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2156 2023-04-29 15:45:23.412065 MKN_third_codes-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2023-04-29 15:40:40.000000 MKN_third_codes-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 15:45:23.413063 MKN_third_codes-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      387 2023-04-29 15:45:14.000000 MKN_third_codes-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.3.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.733668 MKN_third_codes-0.3.3.1/MKN_third_codes/
+-rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.3.1/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:21:29.741646 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     2174 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 16:21:29.000000 MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2174 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-04-29 16:21:01.000000 MKN_third_codes-0.3.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:21:29.742643 MKN_third_codes-0.3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      440 2023-04-29 16:21:27.000000 MKN_third_codes-0.3.3.1/setup.py
```

### Comparing `MKN_third_codes-0.3.2/LICENSE.txt` & `MKN_third_codes-0.3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2/MKN_third_codes/solutions.py` & `MKN_third_codes-0.3.3.1/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.2/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.3.3.1/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.3.2
+Version: 0.3.3.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-### Здарова! Библиотека немного помогает с тервером по МКН 3
-
-## Версия: 0.3.2
-
-- Функции buckets_n_balls => задачи про урны
-- Функции things_complexity => задачи про путаницу вещей
-- Функции geometric_meeting => задачи про встречи
-- Функция combinations => число сочетаний
-
-# Использование
-## 🕹 Функции
-- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-## 🧱 Классы
-- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
-
-# Установка
-### Консоль: pip install --upgrade MKN_third_codes
-### Страница библиотеки: [MKN_lib][libaPage]
-
-## Контакты
-### Я в ВК: [Долгун Иван][vkCom]
-### Я в Discord: ИVAN#2599
-
-[vkCom]: https://vk.com/ivandolgun
+### Здарова! Библиотека немного помогает с тервером по МКН 3
+
+## Версия: 0.3.3
+
+- Функции buckets_n_balls => задачи про урны
+- Функции things_complexity => задачи про путаницу вещей
+- Функции geometric_meeting => задачи про встречи
+- Функция combinations => число сочетаний
+
+# Использование
+## 🕹 Функции
+- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+## 🧱 Классы
+- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
+
+# Установка
+### Консоль: pip install --upgrade MKN_third_codes
+### Страница библиотеки: [MKN_lib][libaPage]
+
+## Контакты
+### Я в ВК: [Долгун Иван][vkCom]
+### Я в Discord: ИVAN#2599
+
+[vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
```

### Comparing `MKN_third_codes-0.3.2/PKG-INFO` & `MKN_third_codes-0.3.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.3.2
+Version: 0.3.3.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-### Здарова! Библиотека немного помогает с тервером по МКН 3
-
-## Версия: 0.3.2
-
-- Функции buckets_n_balls => задачи про урны
-- Функции things_complexity => задачи про путаницу вещей
-- Функции geometric_meeting => задачи про встречи
-- Функция combinations => число сочетаний
-
-# Использование
-## 🕹 Функции
-- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-## 🧱 Классы
-- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
-
-# Установка
-### Консоль: pip install --upgrade MKN_third_codes
-### Страница библиотеки: [MKN_lib][libaPage]
-
-## Контакты
-### Я в ВК: [Долгун Иван][vkCom]
-### Я в Discord: ИVAN#2599
-
-[vkCom]: https://vk.com/ivandolgun
+### Здарова! Библиотека немного помогает с тервером по МКН 3
+
+## Версия: 0.3.3
+
+- Функции buckets_n_balls => задачи про урны
+- Функции things_complexity => задачи про путаницу вещей
+- Функции geometric_meeting => задачи про встречи
+- Функция combinations => число сочетаний
+
+# Использование
+## 🕹 Функции
+- 📱 любая функция имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+## 🧱 Классы
+- Классы данной библиотеки можно использовать вне функций, предавстовляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
+
+# Установка
+### Консоль: pip install --upgrade MKN_third_codes
+### Страница библиотеки: [MKN_lib][libaPage]
+
+## Контакты
+### Я в ВК: [Долгун Иван][vkCom]
+### Я в Discord: ИVAN#2599
+
+[vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
```

### Comparing `MKN_third_codes-0.3.2/README.md` & `MKN_third_codes-0.3.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-## Версия: 0.3.2
+## Версия: 0.3.3
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функция combinations => число сочетаний
 
 # Использование
```

