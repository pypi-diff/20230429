# Comparing `tmp/pystacker-1.2.4.tar.gz` & `tmp/pystacker-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystacker-1.2.4.tar", last modified: Mon Apr 24 15:17:49 2023, max compression
+gzip compressed data, was "pystacker-1.2.5.tar", last modified: Sat Apr 29 15:32:31 2023, max compression
```

## Comparing `pystacker-1.2.4.tar` & `pystacker-1.2.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-24 15:17:49.291621 pystacker-1.2.4/
--rw-rw-r--   0 tw        (1000) tw        (1000)     1065 2023-04-18 14:24:35.000000 pystacker-1.2.4/LICENSE
--rw-rw-r--   0 tw        (1000) tw        (1000)    29582 2023-04-24 15:17:49.291621 pystacker-1.2.4/PKG-INFO
--rw-rw-r--   0 tw        (1000) tw        (1000)    28063 2023-04-24 10:49:50.000000 pystacker-1.2.4/README.md
-drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-24 15:17:49.291621 pystacker-1.2.4/pystacker.egg-info/
--rw-rw-r--   0 tw        (1000) tw        (1000)    29582 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/PKG-INFO
--rw-rw-r--   0 tw        (1000) tw        (1000)      421 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/SOURCES.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)        1 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/dependency_links.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)       49 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/entry_points.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)       15 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/requires.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)        8 2023-04-24 15:17:49.000000 pystacker-1.2.4/pystacker.egg-info/top_level.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)       38 2023-04-24 15:17:49.291621 pystacker-1.2.4/setup.cfg
--rw-rw-r--   0 tw        (1000) tw        (1000)      968 2023-04-24 10:49:50.000000 pystacker-1.2.4/setup.py
-drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-24 15:17:49.291621 pystacker-1.2.4/stacker/
--rw-rw-r--   0 tw        (1000) tw        (1000)      299 2023-04-23 02:23:05.000000 pystacker-1.2.4/stacker/__init__.py
--rw-rw-r--   0 tw        (1000) tw        (1000)       72 2023-04-23 02:23:05.000000 pystacker-1.2.4/stacker/__main__.py
-drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-24 15:17:49.291621 pystacker-1.2.4/stacker/data/
--rw-rw-r--   0 tw        (1000) tw        (1000)      652 2023-04-20 14:02:07.000000 pystacker-1.2.4/stacker/data/about.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)     2835 2023-04-21 11:53:37.000000 pystacker-1.2.4/stacker/data/help-jp.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)     2589 2023-04-21 11:45:01.000000 pystacker-1.2.4/stacker/data/help.txt
--rw-rw-r--   0 tw        (1000) tw        (1000)      232 2023-04-19 14:25:26.000000 pystacker-1.2.4/stacker/data/top.txt
-drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-24 15:17:49.291621 pystacker-1.2.4/stacker/plugins/
--rw-rw-r--   0 tw        (1000) tw        (1000)     2442 2023-04-24 10:49:50.000000 pystacker-1.2.4/stacker/plugins/set_color.py
--rw-rw-r--   0 tw        (1000) tw        (1000)    24117 2023-04-24 10:49:50.000000 pystacker-1.2.4/stacker/stacker.py
--rw-rw-r--   0 tw        (1000) tw        (1000)     5096 2023-04-23 16:16:48.000000 pystacker-1.2.4/stacker/test.py
+drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-29 15:32:31.065811 pystacker-1.2.5/
+-rw-rw-r--   0 tw        (1000) tw        (1000)     1065 2023-04-18 14:24:35.000000 pystacker-1.2.5/LICENSE
+-rw-rw-r--   0 tw        (1000) tw        (1000)    29542 2023-04-29 15:32:31.065811 pystacker-1.2.5/PKG-INFO
+-rw-rw-r--   0 tw        (1000) tw        (1000)    28023 2023-04-29 15:29:09.000000 pystacker-1.2.5/README.md
+drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-29 15:32:31.061811 pystacker-1.2.5/pystacker.egg-info/
+-rw-rw-r--   0 tw        (1000) tw        (1000)    29542 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/PKG-INFO
+-rw-rw-r--   0 tw        (1000) tw        (1000)      469 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/SOURCES.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)        1 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/dependency_links.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)       49 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/entry_points.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)       15 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/requires.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)        8 2023-04-29 15:32:31.000000 pystacker-1.2.5/pystacker.egg-info/top_level.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)       38 2023-04-29 15:32:31.065811 pystacker-1.2.5/setup.cfg
+-rw-rw-r--   0 tw        (1000) tw        (1000)      968 2023-04-29 15:29:09.000000 pystacker-1.2.5/setup.py
+drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-29 15:32:31.065811 pystacker-1.2.5/stacker/
+-rw-rw-r--   0 tw        (1000) tw        (1000)      299 2023-04-23 02:23:05.000000 pystacker-1.2.5/stacker/__init__.py
+-rw-rw-r--   0 tw        (1000) tw        (1000)       72 2023-04-23 02:23:05.000000 pystacker-1.2.5/stacker/__main__.py
+drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-29 15:32:31.065811 pystacker-1.2.5/stacker/data/
+-rw-rw-r--   0 tw        (1000) tw        (1000)      652 2023-04-20 14:02:07.000000 pystacker-1.2.5/stacker/data/about.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)     2835 2023-04-21 11:53:37.000000 pystacker-1.2.5/stacker/data/help-jp.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)     2589 2023-04-21 11:45:01.000000 pystacker-1.2.5/stacker/data/help.txt
+-rw-rw-r--   0 tw        (1000) tw        (1000)      232 2023-04-19 14:25:26.000000 pystacker-1.2.5/stacker/data/top.txt
+drwxrwxr-x   0 tw        (1000) tw        (1000)        0 2023-04-29 15:32:31.065811 pystacker-1.2.5/stacker/plugins/
+-rw-rw-r--   0 tw        (1000) tw        (1000)     1253 2023-04-27 13:00:21.000000 pystacker-1.2.5/stacker/plugins/matrix.py
+-rw-rw-r--   0 tw        (1000) tw        (1000)     2442 2023-04-24 10:49:50.000000 pystacker-1.2.5/stacker/plugins/set_color.py
+-rw-rw-r--   0 tw        (1000) tw        (1000)     3038 2023-04-29 12:31:28.000000 pystacker-1.2.5/stacker/plugins/sh.py
+-rw-rw-r--   0 tw        (1000) tw        (1000)    24424 2023-04-29 15:29:09.000000 pystacker-1.2.5/stacker/stacker.py
+-rw-rw-r--   0 tw        (1000) tw        (1000)     5096 2023-04-23 16:16:48.000000 pystacker-1.2.5/stacker/test.py
```

### Comparing `pystacker-1.2.4/LICENSE` & `pystacker-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystacker-1.2.4/PKG-INFO` & `pystacker-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystacker
-Version: 1.2.4
+Version: 1.2.5
 Summary: Stacker: RPN Calculator in Python
 Home-page: https://github.com/remokasu/stacker
 Author: remokasu
 License: MIT License
         
         Copyright (c) 2023 Remokasu
         
@@ -99,14 +99,15 @@
 | asinh    | Inverse hyperbolic sine                               | `1 asinh`                  | math.asinh(1)            |
 | acosh    | Inverse hyperbolic cosine                             | `2 acosh`                  | math.acosh(2)            |
 | atanh    | Inverse hyperbolic tangent                            | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt     | Square root                                           | `9 sqrt`                   | math.sqrt(9)             |
 | ceil     | Ceiling                                               | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor    | Floor                                                 | `3.8 floor`                | math.floor(3.8)          |
 | round    | Round                                                 | `3.5 round`                | round(3.5)               |
+| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | float    | Convert to floating-point number                      | `5 float`                  | 5.0                      |
 | int      | Convert to integer                                    | `3.14 int`                 | 3                        |
 | ==       | Equal                                                 | `1 1 ==`                   | True                     |
 | !=       | Not equal                                             | `1 0 !=`                   | True                     |
 | <        | Less than                                             | `1 2 <`                    | True                     |
 | <=       | Less than or equal to                                 | `3 3 <=`                   | True                     |
 | >        | Greater than                                          | `2 1 >`                    | True                     |
@@ -120,15 +121,14 @@
 | bin      | Binary representation (result is a string)            | `5 bin`                    | '0b101'                  |
 | oct      | Octal representation (result is a string)             | `10 oct`                   | '0o12'                   |
 | dec      | Decimal representation (result is an integer)         | `0b101010 dec`             | 42                       |
 | hex      | Hexadecimal representation (result is a string)       | `255 hex`                  | '0xff'                   |
 | gcd      | Greatest common divisor                               | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !        | Factorial                                             | `4 !`                      | math.factorial(4)        |
 | radians  | Convert degrees to radians                            | `180 radians`              | math.radians(180)        |
-| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | random   | Generate a random floating-point number between 0 and 1| `random`                   | random.random()          |
 | randint  | Generate a random integer within a specified range    | `1 6 randint`              | random.randint(1, 6)     |
 | uniform  | Generate a random floating-point number within a specified range | `1 2 uniform` | random.uniform(1, 2) |
 | dice     | Roll dice (e.g., 3d6)                                 | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | Remove the element at the specified index             | `2 delete`                 | Remove the element at index 2 from the stack  |
 | pluck    | Remove the element at the specified index and move it to the top of the stack | `2 pluck`              | Remove the element at index 2 and move it to the top of the stack  |
 | pick     | Copy the element at the specified index to the top of the stack | `2 pick`                   | Copy the element at index 2 to the top of the stack  |
@@ -173,20 +173,20 @@
 <br>
 <hr>
 
 
 ## Custom Functions::
 
 ### Example 1: Function to calculate the average of two numbers (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
 
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (Note that the function definition syntax is a custom RPN-like syntax）
 
 <br>
 <hr>
 
 
@@ -415,14 +415,15 @@
 | asinh  | 逆双曲線正弦                                          | `1 asinh`                  | math.asinh(1)            |
 | acosh  | 逆双曲線余弦                                          | `2 acosh`                  | math.acosh(2)            |
 | atanh  | 逆双曲線正接                                          | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt   | 平方根                                                | `9 sqrt`                   | math.sqrt(9)             |
 | ceil   | 切り上げ                                              | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor  | 切り捨て                                              | `3.8 floor`                | math.floor(3.8)          |
 | round  | 四捨五入                                              | `3.5 round`                | round(3.5)               |
+| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | float  | 浮動小数点数に変換                                    | `5 float`                  | 5.0                      |
 | int    | 整数に変換                                            | `3.14 int`                 | 3                        |
 | ==     | 等しい                                                | `1 1 ==`                   | True                     |
 | !=     | 等しくない                                            | `1 0 !=`                   | True                     |
 | <      | より小さい                                            | `1 2 <`                    | True                     |
 | <=     | 以下                                                  | `3 3 <=`                   | True                     |
 | >      | より大きい                                            | `2 1 >`                    | True                     |
@@ -436,15 +437,14 @@
 | bin    | ２進数表示 (結果はstring)                             | `5 bin`                    | '0b101'                  |
 | oct    | 8進数表示 (結果はstring)                              | `10 oct`                   | '0o12'                   |
 | dec    | 10進数表示 (結果はinteger)                            | `0b101010 dec`             | 42                       |
 | hex    | 16進数表示 (結果はstring)                             | `255 hex`                  | '0xff'                   |
 | gcd    | 最大公約数                                            | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !      | 階乗                                                  | `4 !`                      | math.factorial(4)        |
 | radians| 度数法から弧度法へ変換                                | `180 radians`              | math.radians(180)        |
-| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | random | 0と1の間の乱数を生成                                  | `random`                   | random.random()          |
 | randint| 指定した範囲内の整数乱数を生成                        | `1 6 randint`              | random.randint(1, 6)     |
 | uniform| 指定した範囲内の浮動小数点数乱数を生成                | `1 2 uniform`              | random.uniform(1, 2)     |
 | dice   | サイコロを振る (例：3d6)                              | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | 指定のindexを削除                                     | `2 delete`               | スタックからindex 2の要素を削除  |
 | pluck    | 指定のindexを削除し、スタックのトップに移動           | `2 pluck`                | index 2の要素を削除し、スタックのトップに移動  |
 | pick     | 指定されたインデックスの要素をスタックのトップにコピー | `2 pick`                | index 2の要素をスタックのトップにコピー  |
@@ -486,19 +486,19 @@
 
 <br>
 <hr>
 
 ## 自作関数:
 
 ### 例 1: 二つの数の平均を計算する関数 (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (関数定義の構文はRPN構文っぽい独自定義の構文)
 
 <br>
 <hr>
 
 ## プラグインの使い方
```

### Comparing `pystacker-1.2.4/README.md` & `pystacker-1.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 | asinh    | Inverse hyperbolic sine                               | `1 asinh`                  | math.asinh(1)            |
 | acosh    | Inverse hyperbolic cosine                             | `2 acosh`                  | math.acosh(2)            |
 | atanh    | Inverse hyperbolic tangent                            | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt     | Square root                                           | `9 sqrt`                   | math.sqrt(9)             |
 | ceil     | Ceiling                                               | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor    | Floor                                                 | `3.8 floor`                | math.floor(3.8)          |
 | round    | Round                                                 | `3.5 round`                | round(3.5)               |
+| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | float    | Convert to floating-point number                      | `5 float`                  | 5.0                      |
 | int      | Convert to integer                                    | `3.14 int`                 | 3                        |
 | ==       | Equal                                                 | `1 1 ==`                   | True                     |
 | !=       | Not equal                                             | `1 0 !=`                   | True                     |
 | <        | Less than                                             | `1 2 <`                    | True                     |
 | <=       | Less than or equal to                                 | `3 3 <=`                   | True                     |
 | >        | Greater than                                          | `2 1 >`                    | True                     |
@@ -88,15 +89,14 @@
 | bin      | Binary representation (result is a string)            | `5 bin`                    | '0b101'                  |
 | oct      | Octal representation (result is a string)             | `10 oct`                   | '0o12'                   |
 | dec      | Decimal representation (result is an integer)         | `0b101010 dec`             | 42                       |
 | hex      | Hexadecimal representation (result is a string)       | `255 hex`                  | '0xff'                   |
 | gcd      | Greatest common divisor                               | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !        | Factorial                                             | `4 !`                      | math.factorial(4)        |
 | radians  | Convert degrees to radians                            | `180 radians`              | math.radians(180)        |
-| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | random   | Generate a random floating-point number between 0 and 1| `random`                   | random.random()          |
 | randint  | Generate a random integer within a specified range    | `1 6 randint`              | random.randint(1, 6)     |
 | uniform  | Generate a random floating-point number within a specified range | `1 2 uniform` | random.uniform(1, 2) |
 | dice     | Roll dice (e.g., 3d6)                                 | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | Remove the element at the specified index             | `2 delete`                 | Remove the element at index 2 from the stack  |
 | pluck    | Remove the element at the specified index and move it to the top of the stack | `2 pluck`              | Remove the element at index 2 and move it to the top of the stack  |
 | pick     | Copy the element at the specified index to the top of the stack | `2 pick`                   | Copy the element at index 2 to the top of the stack  |
@@ -141,20 +141,20 @@
 <br>
 <hr>
 
 
 ## Custom Functions::
 
 ### Example 1: Function to calculate the average of two numbers (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
 
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (Note that the function definition syntax is a custom RPN-like syntax）
 
 <br>
 <hr>
 
 
@@ -383,14 +383,15 @@
 | asinh  | 逆双曲線正弦                                          | `1 asinh`                  | math.asinh(1)            |
 | acosh  | 逆双曲線余弦                                          | `2 acosh`                  | math.acosh(2)            |
 | atanh  | 逆双曲線正接                                          | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt   | 平方根                                                | `9 sqrt`                   | math.sqrt(9)             |
 | ceil   | 切り上げ                                              | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor  | 切り捨て                                              | `3.8 floor`                | math.floor(3.8)          |
 | round  | 四捨五入                                              | `3.5 round`                | round(3.5)               |
+| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | float  | 浮動小数点数に変換                                    | `5 float`                  | 5.0                      |
 | int    | 整数に変換                                            | `3.14 int`                 | 3                        |
 | ==     | 等しい                                                | `1 1 ==`                   | True                     |
 | !=     | 等しくない                                            | `1 0 !=`                   | True                     |
 | <      | より小さい                                            | `1 2 <`                    | True                     |
 | <=     | 以下                                                  | `3 3 <=`                   | True                     |
 | >      | より大きい                                            | `2 1 >`                    | True                     |
@@ -404,15 +405,14 @@
 | bin    | ２進数表示 (結果はstring)                             | `5 bin`                    | '0b101'                  |
 | oct    | 8進数表示 (結果はstring)                              | `10 oct`                   | '0o12'                   |
 | dec    | 10進数表示 (結果はinteger)                            | `0b101010 dec`             | 42                       |
 | hex    | 16進数表示 (結果はstring)                             | `255 hex`                  | '0xff'                   |
 | gcd    | 最大公約数                                            | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !      | 階乗                                                  | `4 !`                      | math.factorial(4)        |
 | radians| 度数法から弧度法へ変換                                | `180 radians`              | math.radians(180)        |
-| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | random | 0と1の間の乱数を生成                                  | `random`                   | random.random()          |
 | randint| 指定した範囲内の整数乱数を生成                        | `1 6 randint`              | random.randint(1, 6)     |
 | uniform| 指定した範囲内の浮動小数点数乱数を生成                | `1 2 uniform`              | random.uniform(1, 2)     |
 | dice   | サイコロを振る (例：3d6)                              | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | 指定のindexを削除                                     | `2 delete`               | スタックからindex 2の要素を削除  |
 | pluck    | 指定のindexを削除し、スタックのトップに移動           | `2 pluck`                | index 2の要素を削除し、スタックのトップに移動  |
 | pick     | 指定されたインデックスの要素をスタックのトップにコピー | `2 pick`                | index 2の要素をスタックのトップにコピー  |
@@ -454,19 +454,19 @@
 
 <br>
 <hr>
 
 ## 自作関数:
 
 ### 例 1: 二つの数の平均を計算する関数 (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (関数定義の構文はRPN構文っぽい独自定義の構文)
 
 <br>
 <hr>
 
 ## プラグインの使い方
```

### Comparing `pystacker-1.2.4/pystacker.egg-info/PKG-INFO` & `pystacker-1.2.5/pystacker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystacker
-Version: 1.2.4
+Version: 1.2.5
 Summary: Stacker: RPN Calculator in Python
 Home-page: https://github.com/remokasu/stacker
 Author: remokasu
 License: MIT License
         
         Copyright (c) 2023 Remokasu
         
@@ -99,14 +99,15 @@
 | asinh    | Inverse hyperbolic sine                               | `1 asinh`                  | math.asinh(1)            |
 | acosh    | Inverse hyperbolic cosine                             | `2 acosh`                  | math.acosh(2)            |
 | atanh    | Inverse hyperbolic tangent                            | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt     | Square root                                           | `9 sqrt`                   | math.sqrt(9)             |
 | ceil     | Ceiling                                               | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor    | Floor                                                 | `3.8 floor`                | math.floor(3.8)          |
 | round    | Round                                                 | `3.5 round`                | round(3.5)               |
+| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | float    | Convert to floating-point number                      | `5 float`                  | 5.0                      |
 | int      | Convert to integer                                    | `3.14 int`                 | 3                        |
 | ==       | Equal                                                 | `1 1 ==`                   | True                     |
 | !=       | Not equal                                             | `1 0 !=`                   | True                     |
 | <        | Less than                                             | `1 2 <`                    | True                     |
 | <=       | Less than or equal to                                 | `3 3 <=`                   | True                     |
 | >        | Greater than                                          | `2 1 >`                    | True                     |
@@ -120,15 +121,14 @@
 | bin      | Binary representation (result is a string)            | `5 bin`                    | '0b101'                  |
 | oct      | Octal representation (result is a string)             | `10 oct`                   | '0o12'                   |
 | dec      | Decimal representation (result is an integer)         | `0b101010 dec`             | 42                       |
 | hex      | Hexadecimal representation (result is a string)       | `255 hex`                  | '0xff'                   |
 | gcd      | Greatest common divisor                               | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !        | Factorial                                             | `4 !`                      | math.factorial(4)        |
 | radians  | Convert degrees to radians                            | `180 radians`              | math.radians(180)        |
-| roundn   | Round to specified decimal places                     | `3.51 1 roundn`            | round(3.51, 1)           |
 | random   | Generate a random floating-point number between 0 and 1| `random`                   | random.random()          |
 | randint  | Generate a random integer within a specified range    | `1 6 randint`              | random.randint(1, 6)     |
 | uniform  | Generate a random floating-point number within a specified range | `1 2 uniform` | random.uniform(1, 2) |
 | dice     | Roll dice (e.g., 3d6)                                 | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | Remove the element at the specified index             | `2 delete`                 | Remove the element at index 2 from the stack  |
 | pluck    | Remove the element at the specified index and move it to the top of the stack | `2 pluck`              | Remove the element at index 2 and move it to the top of the stack  |
 | pick     | Copy the element at the specified index to the top of the stack | `2 pick`                   | Copy the element at index 2 to the top of the stack  |
@@ -173,20 +173,20 @@
 <br>
 <hr>
 
 
 ## Custom Functions::
 
 ### Example 1: Function to calculate the average of two numbers (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
 
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (Note that the function definition syntax is a custom RPN-like syntax）
 
 <br>
 <hr>
 
 
@@ -415,14 +415,15 @@
 | asinh  | 逆双曲線正弦                                          | `1 asinh`                  | math.asinh(1)            |
 | acosh  | 逆双曲線余弦                                          | `2 acosh`                  | math.acosh(2)            |
 | atanh  | 逆双曲線正接                                          | `0.5 atanh`                | math.atanh(0.5)          |
 | sqrt   | 平方根                                                | `9 sqrt`                   | math.sqrt(9)             |
 | ceil   | 切り上げ                                              | `3.2 ceil`                 | math.ceil(3.2)           |
 | floor  | 切り捨て                                              | `3.8 floor`                | math.floor(3.8)          |
 | round  | 四捨五入                                              | `3.5 round`                | round(3.5)               |
+| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | float  | 浮動小数点数に変換                                    | `5 float`                  | 5.0                      |
 | int    | 整数に変換                                            | `3.14 int`                 | 3                        |
 | ==     | 等しい                                                | `1 1 ==`                   | True                     |
 | !=     | 等しくない                                            | `1 0 !=`                   | True                     |
 | <      | より小さい                                            | `1 2 <`                    | True                     |
 | <=     | 以下                                                  | `3 3 <=`                   | True                     |
 | >      | より大きい                                            | `2 1 >`                    | True                     |
@@ -436,15 +437,14 @@
 | bin    | ２進数表示 (結果はstring)                             | `5 bin`                    | '0b101'                  |
 | oct    | 8進数表示 (結果はstring)                              | `10 oct`                   | '0o12'                   |
 | dec    | 10進数表示 (結果はinteger)                            | `0b101010 dec`             | 42                       |
 | hex    | 16進数表示 (結果はstring)                             | `255 hex`                  | '0xff'                   |
 | gcd    | 最大公約数                                            | `4 2 gcd`                  | math.gcd(4, 2)           |
 | !      | 階乗                                                  | `4 !`                      | math.factorial(4)        |
 | radians| 度数法から弧度法へ変換                                | `180 radians`              | math.radians(180)        |
-| roundn | 指定した小数点以下の桁数で四捨五入                    | `3.51 1 roundn`            | round(3.51, 1)           |
 | random | 0と1の間の乱数を生成                                  | `random`                   | random.random()          |
 | randint| 指定した範囲内の整数乱数を生成                        | `1 6 randint`              | random.randint(1, 6)     |
 | uniform| 指定した範囲内の浮動小数点数乱数を生成                | `1 2 uniform`              | random.uniform(1, 2)     |
 | dice   | サイコロを振る (例：3d6)                              | `3 6 dice`                 | sum(random.randint(1, 6) for _ in range(3)) |
 | delete   | 指定のindexを削除                                     | `2 delete`               | スタックからindex 2の要素を削除  |
 | pluck    | 指定のindexを削除し、スタックのトップに移動           | `2 pluck`                | index 2の要素を削除し、スタックのトップに移動  |
 | pick     | 指定されたインデックスの要素をスタックのトップにコピー | `2 pick`                | index 2の要素をスタックのトップにコピー  |
@@ -486,19 +486,19 @@
 
 <br>
 <hr>
 
 ## 自作関数:
 
 ### 例 1: 二つの数の平均を計算する関数 (average)
-    ~~~ bash
-    stacker:0> x y average => x y + 2 /
-    stacker:1> 2 6 average
-    [4.0]
-    ~~~
+~~~ bash
+stacker:0> x y average => x y + 2 /
+stacker:1> 2 6 average
+[4.0]
+~~~
 
 (関数定義の構文はRPN構文っぽい独自定義の構文)
 
 <br>
 <hr>
 
 ## プラグインの使い方
```

### Comparing `pystacker-1.2.4/setup.py` & `pystacker-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     install_requires = f.read()
 
 setup(
     author='remokasu',
     name="pystacker",
-    version="1.2.4",
+    version="1.2.5",
     license=license,
     url='https://github.com/remokasu/stacker',
     install_requires=install_requires,
     packages=find_packages(),
     package_data={'stacker': ['data/*', 'plugins/*']},
     description='Stacker: RPN Calculator in Python',
     long_description=long_description,
```

### Comparing `pystacker-1.2.4/stacker/data/about.txt` & `pystacker-1.2.5/stacker/data/about.txt`

 * *Files identical despite different names*

### Comparing `pystacker-1.2.4/stacker/data/help-jp.txt` & `pystacker-1.2.5/stacker/data/help-jp.txt`

 * *Files identical despite different names*

### Comparing `pystacker-1.2.4/stacker/data/help.txt` & `pystacker-1.2.5/stacker/data/help.txt`

 * *Files identical despite different names*

### Comparing `pystacker-1.2.4/stacker/plugins/set_color.py` & `pystacker-1.2.5/stacker/plugins/set_color.py`

 * *Files identical despite different names*

### Comparing `pystacker-1.2.4/stacker/stacker.py` & `pystacker-1.2.5/stacker/stacker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import ast
 import cmath
 import copy
 import importlib
 import math
 import os
 import random
 import re
@@ -82,20 +83,25 @@
 
 
 def delete_history():
     if history_file_path.exists():
         history_file_path.unlink()
 
 
-def evaluate_token_or_return_str(input_str: str) -> int | float | str:
+# def evaluate_token_or_return_str(input_str: str) -> int | float | str:
+#     try:
+#         return eval(input_str)
+#     except (SyntaxError, NameError, TypeError, ZeroDivisionError):
+#         pass
+#     return input_str
+def evaluate_token_or_return_str(token):
     try:
-        return eval(input_str)
-    except (SyntaxError, NameError, TypeError, ZeroDivisionError):
-        pass
-    return input_str
+        return ast.literal_eval(token)
+    except (ValueError, SyntaxError):
+        return token
 
 
 def convert_to_base(value, base):
     value = str(value)
 
     # 2進数 (0b...)
     binary_pattern = re.compile(r'^0b[01]+$')
@@ -166,79 +172,79 @@
 
 
 class StackerCore:
     def __init__(self, plugin_dir: str = plugins_dir_path):
         self.stack = []  # スタックを追加
         self.last_pop = None  # pop コマンド(ユーザー入力)で取り出した値を一時的に格納。演算でpopする場合は対象外
         self.operator = {
-            "==": (lambda x1, x2: x1 == x2),  # 等しい
-            "!=": (lambda x1, x2: x1 != x2),  # 等しくない
-            "<": (lambda x1, x2: x1 < x2),  # より小さい
-            "<=": (lambda x1, x2: x1 <= x2),  # 以下
-            ">": (lambda x1, x2: x1 > x2),  # より大きい
-            ">=": (lambda x1, x2: x1 >= x2),  # 以上
-            "and": (lambda x1, x2: x1 and x2),  # 論理積
-            "or": (lambda x1, x2: x1 or x2),  # 論理和
-            "not": (lambda x: not x),  # 否定
-            "band": (lambda x1, x2: int(x1) & int(x2)),  # ビット毎の and
-            "bor": (lambda x1, x2: int(x1) | int(x2)),  # ビット毎の or
-            "bxor": (lambda x1, x2: int(x1) ^ int(x2)),  # ビット毎の xor
-            "bin": (lambda value: convert_to_base(value, 2)),  # 2進数表示
-            "oct": (lambda value: convert_to_base(value, 8)),  # 8進数表
-            "dec": (lambda value: convert_to_base(value, 10)),  # 10進数表示
-            "hex": (lambda value: convert_to_base(value, 16)),  # 16進表示
-            "+": (lambda x1, x2: x1 + x2),  # 加算
-            "-": (lambda x1, x2: x1 - x2),  # 減算
-            "*": (lambda x1, x2: x1 * x2),  # 乗算
-            "/": (lambda x1, x2: x1 / x2),  # 除算
-            "//": (lambda x1, x2: x1 // x2),  # 整数除算
-            "%": (lambda x1, x2: x1 % x2),  # 剰余
-            "^": (lambda x1, x2: math_pow(x1, x2)),  # べき乗
-            "gcd": (lambda x1, x2: math.gcd(int(x1), int(x2))),  # 最大公約数
+            "==": (lambda x1, x2: x1 == x2),    # Equal
+            "!=": (lambda x1, x2: x1 != x2),    # Not equal
+            "<": (lambda x1, x2: x1 < x2),      # Less than
+            "<=": (lambda x1, x2: x1 <= x2),    # Less than or equal to
+            ">": (lambda x1, x2: x1 > x2),      # Greater than
+            ">=": (lambda x1, x2: x1 >= x2),    # Greater than or equal to
+            "and": (lambda x1, x2: x1 and x2),  # Logical and
+            "or": (lambda x1, x2: x1 or x2),    # Logical or
+            "not": (lambda x: not x),           # Logical not
+            "band": (lambda x1, x2: int(x1) & int(x2)),  # Bitwise and
+            "bor": (lambda x1, x2: int(x1) | int(x2)),   # Bitwise or
+            "bxor": (lambda x1, x2: int(x1) ^ int(x2)),  # Bitwise xor
+            "bin": (lambda value: convert_to_base(value, 2)),   # Binary representation
+            "oct": (lambda value: convert_to_base(value, 8)),   # Octal representation
+            "dec": (lambda value: convert_to_base(value, 10)),  # Decimal representation
+            "hex": (lambda value: convert_to_base(value, 16)),  # Hexadecimal representation
+            "+": (lambda x1, x2: x1 + x2),    # Add
+            "-": (lambda x1, x2: x1 - x2),    # Subtract
+            "*": (lambda x1, x2: x1 * x2),    # Multiply
+            "/": (lambda x1, x2: x1 / x2),    # Divide
+            "//": (lambda x1, x2: x1 // x2),  # Integer divide
+            "%": (lambda x1, x2: x1 % x2),    # Modulus
+            "^": (lambda x1, x2: math_pow(x1, x2)),  # Power
+            "gcd": (lambda x1, x2: math.gcd(int(x1), int(x2))),  # Greatest common divisor
             "lcm": (lambda x1, x2: math.lcm(int(x1), int(x2))),  # 最小公倍数
-            "neg": (lambda x: -x),  # 符号反転
-            "abs": (lambda x: abs(x)),  # 絶対値
-            "exp": (lambda x: math_exp(x)),  # 指数関数
-            "log": (lambda x: math_log(x)),  # 自然対数
-            "log10": (lambda x: math_log10(x)),  # 常用対数（底が10）
-            "log2": (lambda x: math_log2(x)),  # 常用対数（底が10）
-            "sin": (lambda x: math_sin(x)),  # 正弦関数
-            "cos": (lambda x: math_cos(x)),  # 余弦関数
-            "tan": (lambda x: math_tan(x)),  # 正接関数
-            "asin": (lambda x: math_asin(x)),  # アークサイン
-            "acos": (lambda x: math_acos(x)),  # アークコサイン
-            "atan": (lambda x: math_atan(x)),  # アークタンジェント
-            "sinh": (lambda x: math_sinh(x)),  # 双曲線正弦
-            "cosh": (lambda x: math_cosh(x)),  # 双曲線余弦
-            "tanh": (lambda x: math_tanh(x)),  # 双曲線正接
-            "asinh": (lambda x: math_asinh(x)),  # 双曲線正弦の逆関数
-            "acosh": (lambda x: math_acosh(x)),  # 双曲線余弦の逆関数
-            "atanh": (lambda x: math_atanh(x)),  # 双曲線正接の逆関数
-            "sqrt": (lambda x: math_sqrt(x)),  # 平方根
-            "radians":  (lambda deg: math.radians(deg)),  # ディグリー(度、Degree)からラジアン(弧度、Radian)に変換
-            "!": (lambda x: math.factorial(int(x))),  # 階乗
+            "neg": (lambda x: -x),  # Negate
+            "abs": (lambda x: abs(x)),  # Absolute value
+            "exp": (lambda x: math_exp(x)),  # Exponential
+            "log": (lambda x: math_log(x)),  # Natural logarithm
+            "log10": (lambda x: math_log10(x)),  # Common logarithm (base 10)
+            "log2": (lambda x: math_log2(x)),  # Logarithm base 2
+            "sin": (lambda x: math_sin(x)),  # Sine
+            "cos": (lambda x: math_cos(x)),  # Cosine
+            "tan": (lambda x: math_tan(x)),  # Tangent
+            "asin": (lambda x: math_asin(x)),  # Arcsine
+            "acos": (lambda x: math_acos(x)),  # Arccosine
+            "atan": (lambda x: math_atan(x)),  # Arctangent
+            "sinh": (lambda x: math_sinh(x)),  # Hyperbolic sine
+            "cosh": (lambda x: math_cosh(x)),  # Hyperbolic cosine
+            "tanh": (lambda x: math_tanh(x)),  # Hyperbolic tangent
+            "asinh": (lambda x: math_asinh(x)),  # Inverse hyperbolic sine
+            "acosh": (lambda x: math_acosh(x)),  # Inverse hyperbolic cosine
+            "atanh": (lambda x: math_atanh(x)),  # Inverse hyperbolic tangent
+            "sqrt": (lambda x: math_sqrt(x)),  # Square root
+            "radians": (lambda deg: math.radians(deg)),  # Convert degrees to radians
+            "!": (lambda x: math.factorial(int(x))),  # Factorial
             "cbrt": (lambda x: pow(x, 1/3)),  # 立方根
             "ncr": (lambda n, k: math.comb(int(n), int(k))),  # 組み合わせ (nCr)
             "npr": (lambda n, k: math.perm(int(n), int(k))),  # 順列 (nPr)
-            "float": (lambda x: float(x)),  # 整数を浮動小数点数に変換
-            "int": (lambda x: int(x)),  # 浮動小数点数を整数に変換
-            "ceil": (lambda x: math.ceil(x)),    # 小数点以下を切り上げた最小の整数
-            "floor": (lambda x: math.floor(x)),  # 小数点以下を切り捨てた最大の整数
-            "round": (lambda x: round(x)),  # 最も近い整数に四捨五入
-            "roundn": (lambda x1, x2: round(x1, int(x2))),  # 任意の桁数で丸める
-            "random": (lambda: random.random()),  # 0から1までの範囲でランダムな浮動小数点数を生成
-            "randint": (lambda x1, x2: random.randint(int(x1), int(x2))),  # 指定された範囲でランダムな整数を生成
-            "uniform": (lambda x1, x2: random.uniform(x1, x2)),  # 指定された範囲でランダムな浮動小数点数を生成
-            "dice": (lambda num_dice, num_faces: sum(random.randint(1, int(num_faces)) for _ in range(int(num_dice)))),  # ダイスロール(例 3d6)
-            "delete": (lambda index: self.stack.pop(index)),  # 指定のindexを削除
-            "pluck": (lambda index: self.stack.pop(index)),  # 指定のindexを削除し、スタックのトップに移動
-            "pick": (lambda index: self.stack.append((self.stack[index]))),  # 指定されたインデックスの要素をスタックのトップにコピー
+            "float": (lambda x: float(x)),  # Convert to floating-point number
+            "int": (lambda x: int(x)),  # Convert to integer
+            "ceil": (lambda x: math.ceil(x)),    # Ceiling
+            "floor": (lambda x: math.floor(x)),  # Floor
+            "round": (lambda x: round(x)),  # Round
+            "roundn": (lambda x1, x2: round(x1, int(x2))),  # Round to specified decimal places
+            "random": (lambda: random.random()),  # Generate a random floating-point number between 0 and 1|
+            "randint": (lambda x1, x2: random.randint(int(x1), int(x2))),  # Generate a random integer within a specified range
+            "uniform": (lambda x1, x2: random.uniform(x1, x2)),  # Generate a random floating-point number within a specified range
+            "dice": (lambda num_dice, num_faces: sum(random.randint(1, int(num_faces)) for _ in range(int(num_dice)))),  # Roll dice (e.g., 3d6) 
+            "delete": (lambda index: self.stack.pop(index)),  # Remove the element at the specified index
+            "pluck": (lambda index: self.stack.pop(index)),  # Remove the element at the specified index and move it to the top of the stack
+            "pick": (lambda index: self.stack.append((self.stack[index]))),  # Copy the element at the specified index to the top of the stack
             "pop": (lambda: self.stack.pop()),  # pop
-            "exec": (lambda command: exec(command, globals())),  # 指定のPythonコードを実行
-            "eval": (lambda command: eval(command)),  # 指定のPython式を評価
+            "exec": (lambda command: exec(command, globals())),  # Execute the specified Python code
+            "eval": (lambda command: eval(command)),  # Evaluate the specified Python expression
         }
         self.plugins = {}
         self.plugin_descriptions = {}
         self.plugin_dir = plugin_dir
 
     def get_n_args_for_operator(self, token):
         # token(演算子)に必要な引数の数
@@ -274,15 +280,23 @@
         """
         Evaluates a given RPN expression.
         Returns the result of the evaluation.
         """
         if stack is None:
             stack = []
 
-        # tokens = expression.split()
+        # List or Tuple
+        try:
+            value = ast.literal_eval(expression)
+            if isinstance(value, (list, tuple)):
+                stack.append(value)
+                return stack
+        except (ValueError, SyntaxError):
+            pass  # 入力がリテラルではない場合、処理を継続
+
         tokens = shlex.split(expression)
         for token in tokens:
             # token: (str)
             if token in self.operator:
                 self.apply_operator(token, stack)
             elif token == "=>":
                 continue
```

### Comparing `pystacker-1.2.4/stacker/test.py` & `pystacker-1.2.5/stacker/test.py`

 * *Files identical despite different names*

