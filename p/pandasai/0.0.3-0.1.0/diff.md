# Comparing `tmp/pandasai-0.0.3.tar.gz` & `tmp/pandasai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.0.3.tar", last modified: Thu Apr 27 09:19:18 2023, max compression
+gzip compressed data, was "pandasai-0.1.0.tar", max compression
```

## Comparing `pandasai-0.0.3.tar` & `pandasai-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,11 @@
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.641090 pandasai-0.0.3/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1055 2023-04-24 05:55:05.000000 pandasai-0.0.3/LICENSE
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)       28 2023-04-24 09:50:53.000000 pandasai-0.0.3/MANIFEST.in
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3144 2023-04-27 09:19:18.640906 pandasai-0.0.3/PKG-INFO
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2763 2023-04-27 09:18:21.000000 pandasai-0.0.3/README.md
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.635156 pandasai-0.0.3/pandasai/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2982 2023-04-27 09:09:37.000000 pandasai-0.0.3/pandasai/__init__.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.636325 pandasai-0.0.3/pandasai/__pycache__/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2660 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3017 2023-04-27 09:14:30.000000 pandasai-0.0.3/pandasai/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.637782 pandasai-0.0.3/pandasai/llm/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        0 2023-04-24 11:19:15.000000 pandasai-0.0.3/pandasai/llm/__init__.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.640469 pandasai-0.0.3/pandasai/llm/__pycache__/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      160 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/llm/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      160 2023-04-24 11:19:33.000000 pandasai-0.0.3/pandasai/llm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1416 2023-04-24 16:52:07.000000 pandasai-0.0.3/pandasai/llm/__pycache__/alpaca.cpython-38.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1416 2023-04-24 21:08:19.000000 pandasai-0.0.3/pandasai/llm/__pycache__/alpaca.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2353 2023-04-24 20:56:38.000000 pandasai-0.0.3/pandasai/llm/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2380 2023-04-24 21:08:19.000000 pandasai-0.0.3/pandasai/llm/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      903 2023-04-24 12:44:16.000000 pandasai-0.0.3/pandasai/llm/__pycache__/fake.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1547 2023-04-26 21:59:03.000000 pandasai-0.0.3/pandasai/llm/__pycache__/open_assistant.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2502 2023-04-24 22:45:27.000000 pandasai-0.0.3/pandasai/llm/__pycache__/openai.cpython-39.pyc
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1065 2023-04-24 13:43:47.000000 pandasai-0.0.3/pandasai/llm/alpaca.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     1760 2023-04-24 21:08:02.000000 pandasai-0.0.3/pandasai/llm/base.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      300 2023-04-24 13:34:20.000000 pandasai-0.0.3/pandasai/llm/fake.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      907 2023-04-24 13:34:14.000000 pandasai-0.0.3/pandasai/llm/open_assistant.py
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     2533 2023-04-24 22:45:22.000000 pandasai-0.0.3/pandasai/llm/openai.py
-drwxr-xr-x   0 gabrieleventuri   (501) staff       (20)        0 2023-04-27 09:19:18.635935 pandasai-0.0.3/pandasai.egg-info/
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)     3144 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/PKG-INFO
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      850 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        1 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)        9 2023-04-27 09:19:18.000000 pandasai-0.0.3/pandasai.egg-info/top_level.txt
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)       38 2023-04-27 09:19:18.641143 pandasai-0.0.3/setup.cfg
--rw-r--r--   0 gabrieleventuri   (501) staff       (20)      626 2023-04-27 09:18:57.000000 pandasai-0.0.3/setup.py
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2923 2023-04-29 12:25:55.311311 pandasai-0.1.0/README.md
+-rw-r--r--   0        0        0     3326 2023-04-29 12:22:08.974103 pandasai-0.1.0/pandasai/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:19:15.318272 pandasai-0.1.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1065 2023-04-24 13:43:47.784698 pandasai-0.1.0/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     1938 2023-04-29 12:22:08.974865 pandasai-0.1.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      324 2023-04-29 12:22:08.975266 pandasai-0.1.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      965 2023-04-29 12:22:08.975718 pandasai-0.1.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2908 2023-04-29 12:22:08.976312 pandasai-0.1.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      579 2023-04-29 13:04:33.234577 pandasai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 pandasai-0.1.0/PKG-INFO
```

### Comparing `pandasai-0.0.3/LICENSE` & `pandasai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.3/PKG-INFO` & `pandasai-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,42 @@
-Metadata-Version: 2.1
-Name: pandasai
-Version: 0.0.3
-Summary: A wrapper around pandas to make it conversational
-Author: Gabriele Venturi
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PandasAI 🐼
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
+<!-- Add images/pandas-ai.png -->
+
+![PandasAI](images/pandas-ai.png?raw=true)
+
 ## Installation
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
 PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
-from pandas_ai import PandasAI
+from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [21400000, 2940000, 2830000, 3870000, 2160000, 1350000, 1780000, 1320000, 516000, 14000000],
     "happiness_index": [7.3, 7.2, 6.5, 7.0, 6.0, 6.3, 7.3, 7.3, 5.9, 5.0]
 })
 
 # Instantiate a LLM
-from llm.openai import OpenAI
+from pandasai.llm.openai import OpenAI
 llm = OpenAI()
 
-pandas_ai = PandasAI(df, llm)
-pandas_ai.run('Which are the 5 happiest countries?')
+pandas_ai = PandasAI(llm)
+pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 0     United States
 6            Canada
@@ -54,15 +45,15 @@
 3           Germany
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai.run('What is the sum of the GDPs of the 2 unhappiest countries?')
+pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 14516000
 ```
@@ -99,8 +90,10 @@
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add CI/CD
+- [ ] Add unit tests
+- [ ] Add contributing guidelines
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.0.3/README.md` & `pandasai-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,59 @@
+Metadata-Version: 2.1
+Name: pandasai
+Version: 0.1.0
+Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
+License: MIT
+Author: Gabriele Venturi
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # PandasAI 🐼
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
+<!-- Add images/pandas-ai.png -->
+
+![PandasAI](images/pandas-ai.png?raw=true)
+
 ## Installation
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
 PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
-from pandas_ai import PandasAI
+from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [21400000, 2940000, 2830000, 3870000, 2160000, 1350000, 1780000, 1320000, 516000, 14000000],
     "happiness_index": [7.3, 7.2, 6.5, 7.0, 6.0, 6.3, 7.3, 7.3, 5.9, 5.0]
 })
 
 # Instantiate a LLM
-from llm.openai import OpenAI
+from pandasai.llm.openai import OpenAI
 llm = OpenAI()
 
-pandas_ai = PandasAI(df, llm)
-pandas_ai.run('Which are the 5 happiest countries?')
+pandas_ai = PandasAI(llm)
+pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 0     United States
 6            Canada
@@ -41,15 +62,15 @@
 3           Germany
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai.run('What is the sum of the GDPs of the 2 unhappiest countries?')
+pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 14516000
 ```
@@ -86,8 +107,11 @@
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add CI/CD
+- [ ] Add unit tests
+- [ ] Add contributing guidelines
 - [x] Add support for conversational responses
+
```

### Comparing `pandasai-0.0.3/pandasai/__init__.py` & `pandasai-0.1.0/pandasai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,106 @@
 import pandas as pd
 from .llm.base import LLM
 import io
 import sys
 
+
 class PandasAI:
-  """PandasAI is a wrapper around a LLM to make dataframes convesational"""
+    """PandasAI is a wrapper around a LLM to make dataframes convesational"""
 
-  _task_instruction: str = """
+    _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
 This is the result of `print(df.head())`:
 {df_head}.
 
 Return the python code (do not import anything) to get the answer to the following question:
 """
-  _response_instruction: str = """
+    _response_instruction: str = """
 Question: {question}
 Answer: {answer}
 
 Rewrite the answer to the question in a conversational way.
 """
-  _llm: LLM
-  _verbose: bool = False
-  _is_conversational_answer: bool = True
-  last_code_generated: str = None
-  code_output: str = None
-
-  def __init__(self, llm = None, conversational = True, verbose = False):
-    if llm is None:
-      raise Exception("An LLM should be provided to instantiate a PandasAI instance")
-    self._llm = llm
-    self._is_conversational_answer = conversational
-    self._verbose = verbose
-
-  def conversational_answer(self, question: str, code: str, answer: str) -> str:
-    """Return the conversational answer"""
-    instruction = self._response_instruction.format(question = question, code = code, answer = answer)
-    return self._llm.call(instruction, answer)
-
-  def run(self, df: pd.DataFrame, prompt: str, is_conversational_answer: bool = None) -> str:
-    """Run the LLM with the given prompt"""
-    self.log(f"Running PandasAI with {self._llm._type} LLM...")
-
-    code = self._llm.generate_code(self._task_instruction.format(df_head = df.head()), prompt)
-    self.last_code_generated = code
-    self.log(f"""
+    _llm: LLM
+    _verbose: bool = False
+    _is_conversational_answer: bool = True
+    last_code_generated: str = None
+    code_output: str = None
+
+    def __init__(self, llm=None, conversational=True, verbose=False):
+        if llm is None:
+            raise Exception(
+                "An LLM should be provided to instantiate a PandasAI instance"
+            )
+        self._llm = llm
+        self._is_conversational_answer = conversational
+        self._verbose = verbose
+
+    def conversational_answer(self, question: str, code: str, answer: str) -> str:
+        """Return the conversational answer"""
+        instruction = self._response_instruction.format(
+            question=question, code=code, answer=answer
+        )
+        return self._llm.call(instruction, answer)
+
+    def run(
+        self, df: pd.DataFrame, prompt: str, is_conversational_answer: bool = None
+    ) -> str:
+        """Run the LLM with the given prompt"""
+        self.log(f"Running PandasAI with {self._llm._type} LLM...")
+
+        code = self._llm.generate_code(
+            self._task_instruction.format(df_head=df.head()), prompt
+        )
+        self.last_code_generated = code
+        self.log(
+            f"""
 Code generated:
 ```
 {code}
-```""")
+```"""
+        )
 
-    answer = self.run_code(code, df)
-    self.code_output = answer
-    self.log(f"Answer: {answer}")
-
-    if is_conversational_answer is None:
-      is_conversational_answer = self._is_conversational_answer
-    if is_conversational_answer:
-      answer = self.conversational_answer(prompt, code, answer)
-      self.log(f"Conversational answer: {answer}")
-    return answer
-
-  def run_code(self, code: str, df: pd.DataFrame):
-    """Run the code in the current context and return the result"""
-
-    # Redirect standard output to a StringIO buffer
-    output = io.StringIO()
-    sys.stdout = output
-
-    # Execute the code
-    exec(code)
-
-    # Restore standard output and get the captured output
-    sys.stdout = sys.__stdout__
-    captured_output = output.getvalue()
-
-    # Evaluate the last line and return its value or the captured output
-    lines = code.strip().split('\n')
-    last_line = lines[-1].strip()
-    if last_line.startswith('print(') and last_line.endswith(')'):
-      # Last line is already printing
-      return eval(last_line[6:-1])
-    else:
-      # Evaluate last line and return its value or the captured output
-      try:
-        result = eval(last_line)
-        return result
-      except:
-        return captured_output
-
-  def log(self, message: str):
-    """Log a message"""
-    if self._verbose:
-      print(message)
+        answer = self.run_code(code, df)
+        self.code_output = answer
+        self.log(f"Answer: {answer}")
+
+        if is_conversational_answer is None:
+            is_conversational_answer = self._is_conversational_answer
+        if is_conversational_answer:
+            answer = self.conversational_answer(prompt, code, answer)
+            self.log(f"Conversational answer: {answer}")
+        return answer
+
+    def run_code(self, code: str, df: pd.DataFrame):
+        """Run the code in the current context and return the result"""
+
+        # Redirect standard output to a StringIO buffer
+        output = io.StringIO()
+        sys.stdout = output
+
+        # Execute the code
+        exec(code)
+
+        # Restore standard output and get the captured output
+        sys.stdout = sys.__stdout__
+        captured_output = output.getvalue()
+
+        # Evaluate the last line and return its value or the captured output
+        lines = code.strip().split("\n")
+        last_line = lines[-1].strip()
+        if last_line.startswith("print(") and last_line.endswith(")"):
+            # Last line is already printing
+            return eval(last_line[6:-1])
+        else:
+            # Evaluate last line and return its value or the captured output
+            try:
+                result = eval(last_line)
+                return result
+            except:
+                return captured_output
+
+    def log(self, message: str):
+        """Log a message"""
+        if self._verbose:
+            print(message)
```

### Comparing `pandasai-0.0.3/pandasai/llm/alpaca.py` & `pandasai-0.1.0/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.0.3/pandasai/llm/base.py` & `pandasai-0.1.0/pandasai/llm/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import re
 import ast
 import astor
 
+
 class LLM:
-  @property
-  def _type(self) -> str:
-    """Return type of llm."""
-    raise Exception("Type has not been implemented")
-  
-  def _remove_imports(self, code: str) -> str:
-    tree = ast.parse(code)
-    new_body = []
-
-    for node in tree.body:
-        if not isinstance(node, (ast.Import, ast.ImportFrom)):
-            new_body.append(node)
-
-    new_tree = ast.Module(body=new_body)
-    return astor.to_source(new_tree)
-
-  def _polish_code(self, code: str) -> str:
-    """Polish the code:
-    - remove the leading "python" or "py"
-    - remove the imports
-    - remove trailing spaces and new lines
-    """
-
-    if re.match(r"^(python|py)", code):
-      code = re.sub(r"^(python|py)", "", code)
-    if re.match(r"^`.*`$", code):
-      code = re.sub(r"^`(.*)`$", r"\1", code)
-    self._remove_imports(code)
-    code = code.strip()
-    return code
-  
-  def _is_python_code(self, string):
-    try:
-      ast.parse(string)
-      return True
-    except SyntaxError:
-      return False
-
-  def _extract_code(self, response: str, separator: str = "```") -> str:
-    """Extract the code from the response"""
-
-    code = response
-    if len(response.split(separator)) > 1:
-      code = response.split(separator)[1]
-    code = self._polish_code(code)
-    if not self._is_python_code(code):
-      raise Exception("No code found in the response")
-
-    return code
-
-  def call(self, instruction: str, input: str) -> str:
-    """Execute the llm with the given prompt"""
-
-    raise Exception("Call method has not been implemented")
-  
-  def generate_code(self, instruction: str, prompt: str) -> str:
-    """Generate the code based on the instruction and the prompt"""
+    @property
+    def _type(self) -> str:
+        """Return type of llm."""
+        raise Exception("Type has not been implemented")
+
+    def _remove_imports(self, code: str) -> str:
+        tree = ast.parse(code)
+        new_body = []
+
+        for node in tree.body:
+            if not isinstance(node, (ast.Import, ast.ImportFrom)):
+                new_body.append(node)
+
+        new_tree = ast.Module(body=new_body)
+        return astor.to_source(new_tree)
+
+    def _polish_code(self, code: str) -> str:
+        """Polish the code:
+        - remove the leading "python" or "py"
+        - remove the imports
+        - remove trailing spaces and new lines
+        """
+
+        if re.match(r"^(python|py)", code):
+            code = re.sub(r"^(python|py)", "", code)
+        if re.match(r"^`.*`$", code):
+            code = re.sub(r"^`(.*)`$", r"\1", code)
+        self._remove_imports(code)
+        code = code.strip()
+        return code
+
+    def _is_python_code(self, string):
+        try:
+            ast.parse(string)
+            return True
+        except SyntaxError:
+            return False
+
+    def _extract_code(self, response: str, separator: str = "```") -> str:
+        """Extract the code from the response"""
+
+        code = response
+        if len(response.split(separator)) > 1:
+            code = response.split(separator)[1]
+        code = self._polish_code(code)
+        if not self._is_python_code(code):
+            raise Exception("No code found in the response")
+
+        return code
+
+    def call(self, instruction: str, input: str) -> str:
+        """Execute the llm with the given prompt"""
+
+        raise Exception("Call method has not been implemented")
+
+    def generate_code(self, instruction: str, prompt: str) -> str:
+        """Generate the code based on the instruction and the prompt"""
 
-    return self._extract_code(self.call(instruction, prompt))
+        return self._extract_code(self.call(instruction, prompt))
```

### Comparing `pandasai-0.0.3/pandasai/llm/open_assistant.py` & `pandasai-0.1.0/pandasai/llm/open_assistant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import requests
 import os
 from dotenv import load_dotenv
 from .base import LLM
 
 load_dotenv()
 
+
 class OpenAssistant(LLM):
-  api_token: str
+    api_token: str
 
-  def __init__(self, api_token: str = None):
-    self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
-    if (self.api_token is None):
-      raise Exception("HuggingFace Hub API key is required")
-
-  def query(self, payload):
-    API_URL = "https://api-inference.huggingface.co/models/OpenAssistant/oasst-sft-1-pythia-12b"
-    headers = {"Authorization": "Bearer {}".format(self.api_token)}
-    
-    response = requests.post(API_URL, headers=headers, json=payload)
-    return response.json()
-
-  def call(self, instruction: str, input: str) -> str:
-    output = self.query({
-      "inputs": "<|prompter|>" + instruction + input + "<|endoftext|>"
-    })
-    return output[0]["generated_text"]
-
-  @property
-  def _type(self) -> str:
-      return "open-assistant"
+    def __init__(self, api_token: str = None):
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
+        if self.api_token is None:
+            raise Exception("HuggingFace Hub API key is required")
+
+    def query(self, payload):
+        API_URL = "https://api-inference.huggingface.co/models/OpenAssistant/oasst-sft-1-pythia-12b"
+        headers = {"Authorization": "Bearer {}".format(self.api_token)}
+
+        response = requests.post(API_URL, headers=headers, json=payload)
+        return response.json()
+
+    def call(self, instruction: str, input: str) -> str:
+        output = self.query(
+            {"inputs": "<|prompter|>" + instruction + input + "<|endoftext|>"}
+        )
+        return output[0]["generated_text"]
+
+    @property
+    def _type(self) -> str:
+        return "open-assistant"
```

### Comparing `pandasai-0.0.3/pandasai/llm/openai.py` & `pandasai-0.1.0/pandasai/llm/openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,96 @@
 import os
 from dotenv import load_dotenv
 from .base import LLM
 import openai
 
 load_dotenv()
 
+
 class OpenAI(LLM):
-  api_token: str
-  model: str = "gpt-3.5-turbo"
-  temperature: float = 0
-  max_tokens: int = 512
-  top_p: float = 1
-  frequency_penalty: float = 0
-  presence_penalty: float = 0.6
-  stop: str = None
-
-  def __init__(self, api_token: str = None, model: str = None, temperature: float = None, max_tokens: int = None, top_p: float = None, frequency_penalty: float = None, presence_penalty: float = None, stop: str = None):
-    self.api_token = api_token or os.getenv("OPENAI_API_KEY")
-    if (self.api_token is None):
-      raise Exception("OpenAI API key is required")
-    openai.api_key = self.api_token
-    
-    self.model = model or self.model
-    self.temperature = temperature or self.temperature
-    self.max_tokens = max_tokens or self.max_tokens
-    self.top_p = top_p or self.top_p
-    self.frequency_penalty = frequency_penalty or self.frequency_penalty
-    self.presence_penalty = presence_penalty or self.presence_penalty
-    self.stop = stop or self.stop
-  
-  def completion(self, prompt: str) -> str:
-    params = {
-      "model": self.model,
-      "prompt": prompt,
-      "temperature": self.temperature,
-      "max_tokens": self.max_tokens,
-      "top_p": self.top_p,
-      "frequency_penalty": self.frequency_penalty,
-      "presence_penalty": self.presence_penalty
-    }
-
-    if self.stop is not None:
-        params["stop"] = [self.stop]
-
-    response = openai.Completion.create(**params)
-
-    return response["choices"][0]["text"]
-  
-  def chat_completion(self, prompt: str) -> str:
-    params = {
-      "model": self.model,
-      "temperature": self.temperature,
-      "max_tokens": self.max_tokens,
-      "top_p": self.top_p,
-      "frequency_penalty": self.frequency_penalty,
-      "presence_penalty": self.presence_penalty,
-      "messages": [{
-        "role": "system",
-        "content": prompt,
-      }]
-    }
-
-    if self.stop is not None:
-        params["stop"] = [self.stop]
-
-    response = openai.ChatCompletion.create(**params)
-
-    return response["choices"][0]["message"]["content"]
-
-  def call(self, instruction: str, input: str) -> str:
-    if (self.model == "text-davinci-003"):
-      response = self.completion(str(instruction) + str(input))
-    elif (self.model == "gpt-3.5-turbo"):
-      response = self.chat_completion(str(instruction) + str(input))
-    else:
-      raise Exception("Unsupported model")
-
-    return response
-
-  @property
-  def _type(self) -> str:
-      return "openai"
+    api_token: str
+    model: str = "gpt-3.5-turbo"
+    temperature: float = 0
+    max_tokens: int = 512
+    top_p: float = 1
+    frequency_penalty: float = 0
+    presence_penalty: float = 0.6
+    stop: str = None
+
+    def __init__(
+        self,
+        api_token: str = None,
+        model: str = None,
+        temperature: float = None,
+        max_tokens: int = None,
+        top_p: float = None,
+        frequency_penalty: float = None,
+        presence_penalty: float = None,
+        stop: str = None,
+    ):
+        self.api_token = api_token or os.getenv("OPENAI_API_KEY")
+        if self.api_token is None:
+            raise Exception("OpenAI API key is required")
+        openai.api_key = self.api_token
+
+        self.model = model or self.model
+        self.temperature = temperature or self.temperature
+        self.max_tokens = max_tokens or self.max_tokens
+        self.top_p = top_p or self.top_p
+        self.frequency_penalty = frequency_penalty or self.frequency_penalty
+        self.presence_penalty = presence_penalty or self.presence_penalty
+        self.stop = stop or self.stop
+
+    def completion(self, prompt: str) -> str:
+        params = {
+            "model": self.model,
+            "prompt": prompt,
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+            "top_p": self.top_p,
+            "frequency_penalty": self.frequency_penalty,
+            "presence_penalty": self.presence_penalty,
+        }
+
+        if self.stop is not None:
+            params["stop"] = [self.stop]
+
+        response = openai.Completion.create(**params)
+
+        return response["choices"][0]["text"]
+
+    def chat_completion(self, prompt: str) -> str:
+        params = {
+            "model": self.model,
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+            "top_p": self.top_p,
+            "frequency_penalty": self.frequency_penalty,
+            "presence_penalty": self.presence_penalty,
+            "messages": [
+                {
+                    "role": "system",
+                    "content": prompt,
+                }
+            ],
+        }
+
+        if self.stop is not None:
+            params["stop"] = [self.stop]
+
+        response = openai.ChatCompletion.create(**params)
+
+        return response["choices"][0]["message"]["content"]
+
+    def call(self, instruction: str, input: str) -> str:
+        if self.model == "text-davinci-003":
+            response = self.completion(str(instruction) + str(input))
+        elif self.model == "gpt-3.5-turbo":
+            response = self.chat_completion(str(instruction) + str(input))
+        else:
+            raise Exception("Unsupported model")
+
+        return response
+
+    @property
+    def _type(self) -> str:
+        return "openai"
```

