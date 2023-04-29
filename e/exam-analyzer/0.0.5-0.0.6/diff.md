# Comparing `tmp/exam_analyzer-0.0.5-py3-none-any.whl.zip` & `tmp/exam_analyzer-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 30236 bytes, number of entries: 6
+Zip file size: 30969 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 exam_analyzer/__init__.py
--rw-r--r--  2.0 unx    12057 b- defN 20-Feb-02 00:00 exam_analyzer/main.py
-?rw-r--r--  2.0 unx    41684 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      487 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.5.dist-info/RECORD
-6 files, 89464 bytes uncompressed, 29356 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    12166 b- defN 20-Feb-02 00:00 exam_analyzer/main.py
+?rw-r--r--  2.0 unx    42488 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      487 b- defN 20-Feb-02 00:00 exam_analyzer-0.0.6.dist-info/RECORD
+6 files, 90377 bytes uncompressed, 30089 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: exam_analyzer/__init__.py
 Comment: 
 
 Filename: exam_analyzer/main.py
 Comment: 
 
-Filename: exam_analyzer-0.0.5.dist-info/METADATA
+Filename: exam_analyzer-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: exam_analyzer-0.0.5.dist-info/WHEEL
+Filename: exam_analyzer-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: exam_analyzer-0.0.5.dist-info/licenses/LICENSE
+Filename: exam_analyzer-0.0.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: exam_analyzer-0.0.5.dist-info/RECORD
+Filename: exam_analyzer-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## exam_analyzer/main.py

```diff
@@ -293,11 +293,12 @@
                 datas.append(read_and_analyze_PDF_file(file, class_name))  # 读取并分析某考生的成绩报告单，然后将数据保存起来供后续分析
             except Exception:
                 print(f"{file} 文件解析错误,请检查该文件.确保 pdf 文件是官方下载的！然后重新运行本程序.")
                 exit(0)
 
     analyze_and_save_to_excel(datas)  # 分析考生数据，然后存储到excel中，增加可视化
     beautify_excel()  # 美化表格
+    print("\033[0;32m程序运行完毕，已生成汇总文件：\033[0m" + "\033[0;31moutput.xlsx\033[0m")
 
 
 if __name__ == "__main__":
     run()
```

## Comparing `exam_analyzer-0.0.5.dist-info/METADATA` & `exam_analyzer-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: exam_analyzer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Analysis and Summary Tool for College Entrance Exam Grade Report
-Project-URL: Homepage, https://github.com/fearlessxjdx/exam-analyzer
-Project-URL: Bug Tracker, https://github.com/fearlessxjdx/exam-analyzer/issues
+Project-URL: Homepage, https://github.com/fearlessxjdx/ExamAnalyzer
+Project-URL: Bug Tracker, https://github.com/fearlessxjdx/ExamAnalyzer/issues
 Author-email: xjdx <fearlessxjdx@qq.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -677,29 +677,44 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pypdf2
 Description-Content-Type: text/markdown
 
-# 使用步骤
+# exam_analyzer
 
-## 1. 下载并安装 python 环境
+## 使用指南
+
+### 1. 安装 python 运行环境
+
+已经安装过 python，且 python 版本>=3.7 可以跳过此步骤
+
+python 版本低于 3.7 的，建议先卸载老版本的 python，再安装新版 python
 
 推荐下载 [python3.10](https://www.python.org/downloads/release/python-31011/)
 
 如果下载不动，请使用迅雷等下载工具
 
-## 2. 使用 pip 下载本工具库
+### 2. 建立班级文件夹，并放入学生的成绩报告单(PDF文件)
+
+以班级为单位，新建文件夹，文件夹必须以'班'字结尾，例如：301班、302班、303班、……
+
+然后将学生的 pdf 文件放入所在班级的文件夹，pdf 文件必须是官方网站下载的，否则可能出现解析错误，导致信息、分数不一致等情况。
+
+### 3. 双击 `生成.bat` 文件
+
+本着 `Pythonic` 理念，本人已将该工具包发布到 python 官方的 PyPI 上，感兴趣的老师欢迎加入开发。
+
+`生成.bat` 文件中，包含了几条命令，双击后会自动下载本人发布的工具库，下载完成后便会运行，老师们只需等待执行完成即可
```

## Comparing `exam_analyzer-0.0.5.dist-info/licenses/LICENSE` & `exam_analyzer-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

