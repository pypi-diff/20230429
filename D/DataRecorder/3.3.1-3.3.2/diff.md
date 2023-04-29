# Comparing `tmp/DataRecorder-3.3.1.tar.gz` & `tmp/DataRecorder-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataRecorder-3.3.1.tar", last modified: Sun Mar 26 03:48:39 2023, max compression
+gzip compressed data, was "DataRecorder-3.3.2.tar", last modified: Sat Apr 29 17:50:09 2023, max compression
```

## Comparing `DataRecorder-3.3.1.tar` & `DataRecorder-3.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 03:48:39.700929 DataRecorder-3.3.1/
-drwxrwxrwx   0        0        0        0 2023-03-26 03:48:39.673806 DataRecorder-3.3.1/DataRecorder/
--rw-rw-rw-   0        0        0      138 2022-06-16 13:39:46.000000 DataRecorder-3.3.1/DataRecorder/__init__.py
--rw-rw-rw-   0        0        0    17067 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/base.py
--rw-rw-rw-   0        0        0     3469 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/base.pyi
--rw-rw-rw-   0        0        0     1576 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      474 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     4759 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/db_recorder.py
--rw-rw-rw-   0        0        0      703 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    17399 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/filler.py
--rw-rw-rw-   0        0        0     3312 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/filler.pyi
--rw-rw-rw-   0        0        0     5072 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/recorder.py
--rw-rw-rw-   0        0        0      461 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/recorder.pyi
--rw-rw-rw-   0        0        0     3142 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/tools.py
--rw-rw-rw-   0        0        0      368 2023-03-26 03:46:22.000000 DataRecorder-3.3.1/DataRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2023-03-26 03:48:39.700929 DataRecorder-3.3.1/DataRecorder.egg-info/
--rw-rw-rw-   0        0        0     5062 2023-03-26 03:48:39.000000 DataRecorder-3.3.1/DataRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-03-26 03:48:39.000000 DataRecorder-3.3.1/DataRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 03:48:39.000000 DataRecorder-3.3.1/DataRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-26 03:48:39.000000 DataRecorder-3.3.1/DataRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-26 03:48:39.000000 DataRecorder-3.3.1/DataRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2022-01-26 11:22:47.000000 DataRecorder-3.3.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-26 03:46:04.000000 DataRecorder-3.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5062 2023-03-26 03:48:39.700929 DataRecorder-3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4563 2022-12-14 14:48:56.000000 DataRecorder-3.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-26 03:48:39.700929 DataRecorder-3.3.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-03-26 03:46:49.000000 DataRecorder-3.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:50:09.554826 DataRecorder-3.3.2/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:50:09.514066 DataRecorder-3.3.2/DataRecorder/
+-rw-rw-rw-   0        0        0      138 2022-06-16 13:39:46.000000 DataRecorder-3.3.2/DataRecorder/__init__.py
+-rw-rw-rw-   0        0        0    17067 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/base.py
+-rw-rw-rw-   0        0        0     3469 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1576 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      474 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     4759 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0      703 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    17399 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/filler.py
+-rw-rw-rw-   0        0        0     3312 2023-03-26 03:46:22.000000 DataRecorder-3.3.2/DataRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     7179 2023-04-29 17:49:39.000000 DataRecorder-3.3.2/DataRecorder/recorder.py
+-rw-rw-rw-   0        0        0      884 2023-04-29 16:44:32.000000 DataRecorder-3.3.2/DataRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0     4870 2023-04-29 16:44:32.000000 DataRecorder-3.3.2/DataRecorder/tools.py
+-rw-rw-rw-   0        0        0     1173 2023-04-29 17:42:18.000000 DataRecorder-3.3.2/DataRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2023-04-29 17:50:09.545815 DataRecorder-3.3.2/DataRecorder.egg-info/
+-rw-rw-rw-   0        0        0     5062 2023-04-29 17:50:09.000000 DataRecorder-3.3.2/DataRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-04-29 17:50:09.000000 DataRecorder-3.3.2/DataRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:50:09.000000 DataRecorder-3.3.2/DataRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 17:50:09.000000 DataRecorder-3.3.2/DataRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 17:50:09.000000 DataRecorder-3.3.2/DataRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2022-01-26 11:22:47.000000 DataRecorder-3.3.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-26 03:46:04.000000 DataRecorder-3.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5062 2023-04-29 17:50:09.545815 DataRecorder-3.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4563 2022-12-14 14:48:56.000000 DataRecorder-3.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:50:09.554826 DataRecorder-3.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-04-29 17:49:39.000000 DataRecorder-3.3.2/setup.py
```

### Comparing `DataRecorder-3.3.1/DataRecorder/base.py` & `DataRecorder-3.3.2/DataRecorder/base.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/base.pyi` & `DataRecorder-3.3.2/DataRecorder/base.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/byte_recorder.py` & `DataRecorder-3.3.2/DataRecorder/byte_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/db_recorder.py` & `DataRecorder-3.3.2/DataRecorder/db_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/db_recorder.pyi` & `DataRecorder-3.3.2/DataRecorder/db_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/filler.py` & `DataRecorder-3.3.2/DataRecorder/filler.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/filler.pyi` & `DataRecorder-3.3.2/DataRecorder/filler.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/DataRecorder/recorder.py` & `DataRecorder-3.3.2/DataRecorder/tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,153 @@
 # -*- coding:utf-8 -*-
-from pathlib import Path
-from time import sleep
-from typing import Union
-
-from openpyxl import Workbook, load_workbook
+from copy import copy
+from csv import reader as csv_reader, writer as csv_writer
 
-from .base import BaseRecorder, ok_list
+from pathlib import Path
+from re import search, sub
 
 
-class Recorder(BaseRecorder):
-    """用于缓存并记录数据，可在达到一定数量时自动记录，以降低文件读写次数，减少开销。
-    退出时能自动记录数据（xlsx格式除外），避免因异常丢失。
+class CellStyle(object):
+    def __init__(self, from_cell=None):
+        if from_cell:
+            self._style = copy(from_cell._style)
+            self._font = copy(from_cell.font)
+            self._border = copy(from_cell.border)
+            self._fill = copy(from_cell.fill)
+            self._number_format = copy(from_cell.number_format)
+            self._protection = copy(from_cell.protection)
+            self._alignment = copy(from_cell.alignment)
+        else:
+            self._style = None
+            self._font = None
+            self._border = None
+            self._fill = None
+            self._number_format = None
+            self._protection = None
+            self._alignment = None
+
+    def set_alignment(self, alignment):
+        self._alignment = alignment
+
+    def set_font(self, font):
+        self._font = font
+
+    def set_border(self, border):
+        self._border = border
+
+    def set_fill(self, fill):
+        self._fill = fill
+
+    def set_number_format(self, number_format):
+        self._number_format = number_format
+
+    def set_protection(self, protection):
+        self._protection = protection
+
+    def to_cell(self, cell):
+        """把当前样式复制到目标单元格"""
+        if self._style:
+            cell._style = self._style
+        if self._alignment:
+            cell.alignment = self._alignment
+        if self._font:
+            cell.font = self._font
+        if self._border:
+            cell.border = self._border
+        if self._fill:
+            cell.fill = self._fill
+        if self._number_format:
+            cell.number_format = self._number_format
+        if self._protection:
+            cell.protection = self._protection
+
+
+def align_csv(path, encoding='utf-8', delimiter=',', quotechar='"'):
+    """补全csv文件，使其每行列数一样多，用于pandas读取时避免出错
+    :param path: 要处理的文件路径
+    :param encoding: 文件编码
+    :param delimiter: 分隔符
+    :param quotechar: 引用符
+    :return: None
+    """
+    with open(path, 'r', encoding=encoding) as f:
+        reader = csv_reader(f, delimiter=delimiter, quotechar=quotechar)
+        lines = list(reader)
+        lines_data = {}
+        max_len = 0
+
+        # 把每行列数用字典记录，并找到最长的一行
+        for k, i in enumerate(lines):
+            line_len = len(i)
+            if line_len > max_len:
+                max_len = line_len
+            lines_data[k] = line_len
+
+        # 把所有行用空值补全到和最长一行一样
+        for i in lines_data:
+            lines[i].extend([None] * (max_len - lines_data[i]))
+
+        writer = csv_writer(open(path, 'w', encoding=encoding, newline=''), delimiter=delimiter, quotechar=quotechar)
+        writer.writerows(lines)
+
+
+def get_usable_path(path):
+    """检查文件或文件夹是否有重名，并返回可以使用的路径
+    :param path: 文件或文件夹路径
+    :return: 可用的路径，Path对象
     """
-    SUPPORTS = ('any',)
+    path = Path(path)
+    parent = path.parent
+    path = parent / make_valid_file_name(path.name)
+    name = path.stem if path.is_file() else path.name
+    ext = path.suffix if path.is_file() else ''
 
-    def add_data(self, data):
-        """添加数据，可一次添加多条数据
-        :param data: 插入的数据，元组或列表
-        :return: None
-        """
-        while self._pause_add:  # 等待其它线程写入结束
-            sleep(.1)
-
-        if not isinstance(data, (list, tuple, dict)):
-            data = (data,)
-        if not data:
-            data = (None,)
-        # 一维数组
-        if (isinstance(data, (list, tuple)) and not isinstance(data[0], (list, tuple, dict))) or isinstance(data, dict):
-            self._data.append(data)
-        else:  # 二维数组
-            self._data.extend(data)
-
-        if 0 < self.cache_size <= len(self._data):
-            self.record()
-
-    def _record(self):
-        """记录数据"""
-        if self.type == 'xlsx':
-            self._to_xlsx()
-        elif self.type == 'csv':
-            self._to_csv()
-        elif self.type == 'json':
-            self._to_json()
-        else:
-            self._to_txt()
+    first_time = True
 
-    def _to_xlsx(self):
-        """记录数据到xlsx文件"""
-        if Path(self.path).exists():
-            wb = load_workbook(self.path)
-            if self.table:
-                ws = wb[self.table] if self.table in [i.title for i in wb.worksheets] else wb.create_sheet(
-                    title=self.table)
-            else:
-                ws = wb.active
+    while path.exists():
+        r = search(r'(.*)_(\d+)$', name)
 
+        if not r or (r and first_time):
+            src_name, num = name, '1'
         else:
-            wb = Workbook(write_only=True)
-            ws = wb.create_sheet(title=self.table)
-            title = _get_title(self._data[0], self._before, self._after)
-            if title is not None:
-                ws.append(ok_list(title, True))
-
-        for i in self._data:
-            ws.append(ok_list(self._data_to_list(i), True))
-
-        wb.save(self.path)
-        wb.close()
-
-    def _to_csv(self):
-        """记录数据到csv文件"""
-        from csv import writer
-        title = _get_title(self._data[0], self._before, self._after) if not Path(self.path).exists() else None
-
-        with open(self.path, 'a+', newline='', encoding=self.encoding) as f:
-            csv_write = writer(f, delimiter=self.delimiter, quotechar=self.quote_char)
-            if title:
-                csv_write.writerow(ok_list(title))
-            for i in self._data:
-                csv_write.writerow(ok_list(self._data_to_list(i)))
-
-    def _to_txt(self):
-        """记录数据到txt文件"""
-        with open(self.path, 'a+', encoding=self.encoding) as f:
-            all_data = [' '.join(ok_list(self._data_to_list_or_dict(i), as_str=True)) for i in self._data]
-            f.write('\n'.join(all_data) + '\n')
-
-    def _to_json(self):
-        """记录数据到json文件"""
-        from json import load, dump
-        if Path(self.path).exists():
-            with open(self.path, 'r', encoding=self.encoding) as f:
-                json_data = load(f)
+            src_name, num = r.group(1), int(r.group(2)) + 1
 
-            for i in self._data:
-                json_data.append(ok_list(self._data_to_list_or_dict(i)))
+        name = f'{src_name}_{num}'
+        path = parent / f'{name}{ext}'
+        first_time = None
 
-        else:
-            json_data = [ok_list(self._data_to_list_or_dict(i)) for i in self._data]
+    return path
 
-        with open(self.path, 'w', encoding=self.encoding) as f:
-            dump(json_data, f)
 
-    def _data_to_list_or_dict(self, data):
-        """将传入的数据转换为列表或字典形式，添加前后列数据，用于记录到txt或json
-        :param data: 要处理的数据
-        :return: 转变成列表或字典形式的数据
-        """
-        if isinstance(data, (list, tuple)):
-            return self._data_to_list(data)
-
-        elif isinstance(data, dict):
-            if isinstance(self.before, dict):
-                data = {**self.before, **data}
-
-            if isinstance(self.after, dict):
-                data = {**data, **self.after}
-
-            return data
-
-
-def _get_title(data: Union[list, dict],
-               before: Union[list, dict, None] = None,
-               after: Union[list, dict, None] = None) -> Union[list, None]:
-    """获取表头列表
-    :param data: 数据列表或字典
-    :param before: 数据前的列
-    :param after: 数据后的列
-    :return: 表头列表
+def make_valid_file_name(full_name):
+    """获取有效的文件名
+    :param full_name: 文件名
+    :return: 可用的文件名
     """
-    if isinstance(data, (tuple, list)):
-        return None
+    # ----------------去除前后空格----------------
+    full_name = full_name.strip()
 
-    return_list = []
-    for i in (before, data, after):
-        if isinstance(i, dict):
-            return_list.extend(list(i))
-        elif i is None:
-            pass
-        elif isinstance(i, list):
-            return_list.extend(['' for _ in range(len(i))])
-        else:
-            return_list.extend([''])
-
-    return return_list
+    # ----------------使总长度不大于255个字符（一个汉字是2个字符）----------------
+    r = search(r'(.*)(\.[^.]+$)', full_name)  # 拆分文件名和后缀名
+    if r:
+        name, ext = r.group(1), r.group(2)
+        ext_long = len(ext)
+    else:
+        name, ext = full_name, ''
+        ext_long = 0
+
+    while _get_long(name) > 255 - ext_long:
+        name = name[:-1]
+
+    full_name = f'{name}{ext}'
+
+    # ----------------去除不允许存在的字符----------------
+    return sub(r'[<>/\\|:*?\n]', ' ', full_name)
+
+
+def _get_long(txt) -> int:
+    """返回字符串中字符个数（一个汉字是2个字符）
+    :param txt: 字符串
+    :return: 字符个数
+    """
+    txt_len = len(txt)
+    return int((len(txt.encode('utf-8')) - txt_len) / 2 + txt_len)
```

### Comparing `DataRecorder-3.3.1/DataRecorder.egg-info/PKG-INFO` & `DataRecorder-3.3.2/DataRecorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.3.1
+Version: 3.3.2
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.3.1/DataRecorder.egg-info/SOURCES.txt` & `DataRecorder-3.3.2/DataRecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/LICENSE` & `DataRecorder-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/PKG-INFO` & `DataRecorder-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.3.1
+Version: 3.3.2
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.3.1/README.md` & `DataRecorder-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.3.1/setup.py` & `DataRecorder-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DataRecorder",
-    version="3.3.1",
+    version="3.3.2",
     author="g1879",
     author_email="g1879@qq.com",
     description="用于记录数据的模块。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="DataRecorder",
```

