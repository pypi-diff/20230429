# Comparing `tmp/bumbag-4.1.0.tar.gz` & `tmp/bumbag-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumbag-4.1.0.tar", max compression
+gzip compressed data, was "bumbag-5.0.0.tar", max compression
```

## Comparing `bumbag-4.1.0.tar` & `bumbag-5.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1523 2023-03-07 19:13:48.927733 bumbag-4.1.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-03-07 19:13:48.927733 bumbag-4.1.0/LICENSES/
--rw-r--r--   0        0        0     2890 2023-03-07 19:13:48.927733 bumbag-4.1.0/LICENSES/DATEUTIL_LICENSE
--rw-r--r--   0        0        0     1492 2023-03-07 19:13:48.927733 bumbag-4.1.0/LICENSES/TOOLZ_LICENSE
--rw-r--r--   0        0        0     3219 2023-03-07 19:13:48.927733 bumbag-4.1.0/README.md
--rw-r--r--   0        0        0     1323 2023-03-07 19:15:06.976864 bumbag-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      281 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/__init__.py
--rw-r--r--   0        0        0    11242 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/core.py
--rw-r--r--   0        0        0     5488 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/io.py
--rw-r--r--   0        0        0     3156 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/math.py
--rw-r--r--   0        0        0     4411 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/random.py
--rw-r--r--   0        0        0     4466 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/string.py
--rw-r--r--   0        0        0    13073 2023-03-07 19:13:48.927733 bumbag-4.1.0/src/bumbag/time.py
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 bumbag-4.1.0/setup.py
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 bumbag-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-04-29 11:34:12.262915 bumbag-5.0.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-04-29 11:34:12.262915 bumbag-5.0.0/LICENSES/
+-rw-r--r--   0        0        0     2890 2023-04-29 11:34:12.262915 bumbag-5.0.0/LICENSES/DATEUTIL_LICENSE
+-rw-r--r--   0        0        0     1492 2023-04-29 11:34:12.262915 bumbag-5.0.0/LICENSES/TOOLZ_LICENSE
+-rw-r--r--   0        0        0     3203 2023-04-29 11:34:12.262915 bumbag-5.0.0/README.md
+-rw-r--r--   0        0        0     1323 2023-04-29 11:35:28.598801 bumbag-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/__init__.py
+-rw-r--r--   0        0        0    14331 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/core.py
+-rw-r--r--   0        0        0     5528 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/io.py
+-rw-r--r--   0        0        0     3802 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/math.py
+-rw-r--r--   0        0        0     4444 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/random.py
+-rw-r--r--   0        0        0     5861 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/string.py
+-rw-r--r--   0        0        0    13554 2023-04-29 11:34:12.266915 bumbag-5.0.0/src/bumbag/time.py
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 bumbag-5.0.0/setup.py
+-rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 bumbag-5.0.0/PKG-INFO
```

### Comparing `bumbag-4.1.0/LICENSE` & `bumbag-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bumbag-4.1.0/LICENSES/DATEUTIL_LICENSE` & `bumbag-5.0.0/LICENSES/DATEUTIL_LICENSE`

 * *Files identical despite different names*

### Comparing `bumbag-4.1.0/LICENSES/TOOLZ_LICENSE` & `bumbag-5.0.0/LICENSES/TOOLZ_LICENSE`

 * *Files identical despite different names*

### Comparing `bumbag-4.1.0/README.md` & `bumbag-5.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ['one', 2, 3, 4, 'five', 'six', 'seven', 8, 9, 'ten']
 ```
 
 Use [`highlight_string_differences`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.highlight_string_differences) to see differences between two strings easily:
 
 ```python
 >>> import bumbag
->>> print(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall"))
+>>> print(bumbag.highlight_string_differences("hello", "hall"))
 hello
  |  |
 hall
 ```
 
 Quickly compare two Python sets with [`two_set_summary`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.two_set_summary):
```

#### html2text {}

```diff
@@ -10,16 +10,16 @@
 irregular list: ```python >>> import bumbag >>> irregular_list = [ ... ["one",
 2], ... 3, ... [(4, "five")], ... [[["six"]]], ... "seven", ... [], ... ] >>>
 list(bumbag.flatten(irregular_list, 8, [9, ("ten",)])) ['one', 2, 3, 4, 'five',
 'six', 'seven', 8, 9, 'ten'] ``` Use [`highlight_string_differences`](https://
 bumbag.readthedocs.io/en/stable/autoapi/bumbag/
 index.html#bumbag.highlight_string_differences) to see differences between two
 strings easily: ```python >>> import bumbag >>> print
-(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall")) hello |
-| hall ``` Quickly compare two Python sets with [`two_set_summary`](https://
+(bumbag.highlight_string_differences("hello", "hall")) hello | | hall ```
+Quickly compare two Python sets with [`two_set_summary`](https://
 bumbag.readthedocs.io/en/stable/autoapi/bumbag/
 index.html#bumbag.two_set_summary): ```python >>> import bumbag >>> x = {"a",
 "c", "b", "g", "h"} >>> y = {"c", "d", "e", "f", "g"} >>> summary =
 bumbag.two_set_summary(x, y) >>> print(summary["report"]) x (n=5): {'a', 'b',
 'c', ...} y (n=5): {'c', 'd', 'e', ...} x | y (n=8): {'a', 'b', 'c', ...} x & y
 (n=2): {'c', 'g'} x - y (n=3): {'a', 'b', 'h'} y - x (n=3): {'d', 'e', 'f'} x ^
 y (n=6): {'a', 'b', 'd', ...} jaccard = 0.25 overlap = 0.4 dice = 0.4
```

### Comparing `bumbag-4.1.0/pyproject.toml` & `bumbag-5.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bumbag"
-version = "4.1.0"
+version = "5.0.0"
 description = "A package for Python utility functions."
 authors = ["BumBag Developers"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/bumbag"
 documentation = "https://bumbag.readthedocs.io/en/stable/"
 include = ["LICENSES/"]
```

### Comparing `bumbag-4.1.0/src/bumbag/core.py` & `bumbag-5.0.0/src/bumbag/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,104 @@
+import functools
 import inspect
 import math
 import operator
 from collections import Counter
 from typing import Iterator, Sequence
 
 from toolz import curried
 
 __all__ = (
+    "all_predicate_true",
+    "any_predicate_true",
     "extend_range",
     "flatten",
     "freq",
     "get_function_name",
     "get_source_code",
+    "numberformat",
     "op",
+    "setred",
     "sig",
     "two_set_summary",
 )
 
 
 @curried.curry
-def extend_range(min_value, max_value, min_factor=0.05, max_factor=0.05):
+def all_predicate_true(predicates, x, /):
+    """Check if all predicates are true.
+
+    Parameters
+    ----------
+    predicates : Iterable of Callable[[Any], bool]]
+        Collection of predicates to check.
+    x : Any
+        Specify the value to evaluate the predicates on.
+
+    Returns
+    -------
+    bool
+        ``True`` if all predicates evaluate to ``True`` else ``False``.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> is_divisible_by_3_and_5 = bumbag.all_predicate_true(
+    ...     [lambda n: n % 3 == 0, lambda n: n % 5 == 0]
+    ... )
+    >>> is_divisible_by_3_and_5(60)
+    True
+    >>> is_divisible_by_3_and_5(9)
+    False
+    """
+    return all(predicate(x) for predicate in predicates)
+
+
+@curried.curry
+def any_predicate_true(predicates, x, /):
+    """Check if any predicate is true.
+
+    Parameters
+    ----------
+    predicates : Iterable of Callable[[Any], bool]]
+        Collection of predicates to check.
+    x : Any
+        Specify the value to evaluate the predicates on.
+
+    Returns
+    -------
+    bool
+        ``True`` if any predicate evaluates to ``True`` else ``False``.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> is_divisible_by_3_or_5 = bumbag.any_predicate_true(
+    ...     [lambda n: n % 3 == 0, lambda n: n % 5 == 0]
+    ... )
+    >>> is_divisible_by_3_or_5(60)
+    True
+    >>> is_divisible_by_3_or_5(9)
+    True
+    >>> is_divisible_by_3_or_5(13)
+    False
+    """
+    return any(predicate(x) for predicate in predicates)
+
+
+@curried.curry
+def extend_range(min_value, max_value, /, *, min_factor=0.05, max_factor=0.05):
     """Extend value range by a factor.
 
     The value range is defined as ``max_value - min_value``.
 
     Parameters
     ----------
     min_value : int, float
@@ -47,15 +122,15 @@
 
     Examples
     --------
     >>> import bumbag
     >>> bumbag.extend_range(0, 1)
     (-0.05, 1.05)
 
-    >>> bumbag.extend_range(0, 1, 0.1, 0.2)
+    >>> bumbag.extend_range(0, 1, min_factor=0.1, max_factor=0.2)
     (-0.1, 1.2)
     """
     if not isinstance(min_factor, float) or min_factor < 0:
         raise ValueError(f"{min_factor=} - must be a non-negative number")
 
     if not isinstance(max_factor, float) or max_factor < 0:
         raise ValueError(f"{max_factor=} - must be a non-negative number")
@@ -215,15 +290,15 @@
     ...
     >>> my_test_function()
     'my_test_function'
     """
     return inspect.stack()[1].function
 
 
-def get_source_code(obj):
+def get_source_code(obj, /):
     """Get source code of an object.
 
     Parameters
     ----------
     obj : module, class, method, function, traceback, frame, or code object
         Object to get source code from.
 
@@ -242,14 +317,39 @@
     def my_test_function():
         return "Hello, World!"
     <BLANKLINE>
     """
     return inspect.getsource(obj)
 
 
+def numberformat(number, /):
+    """Format numeric literals with underscores.
+
+    Parameters
+    ----------
+    number : int or float
+        Number to format.
+
+    Returns
+    -------
+    str
+        A string representation with underscores of a numeric literal.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> bumbag.numberformat(1000000)
+    '1_000_000'
+
+    >>> bumbag.numberformat(100000.0)
+    '100_000.0'
+    """
+    return f"{number:,}".replace(",", "_")
+
+
 @curried.curry
 def op(func, x, y):
     """Apply an operator function that takes two inputs.
 
     Parameters
     ----------
     func : function
@@ -280,15 +380,57 @@
     >>> inc(10)
     11
     """
     return func(x, y)
 
 
 @curried.curry
-def sig(number, digits=3):
+def setred(func, *sets):
+    """Apply a set function to reduce a sequence of sets.
+
+    Parameters
+    ----------
+    func : function
+        Specify the set function.
+    sets : set
+        A sequence of Python set objects to reduce.
+
+    Returns
+    -------
+    set
+        A reduced set according to the set function.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> x = {0, 1, 2, 3}
+    >>> y = {2, 4, 6}
+    >>> z = {2, 6, 8}
+    >>> bumbag.setred(set.intersection, x, y, z)
+    {2}
+
+    >>> bumbag.setred(set.union, x, y, z)
+    {0, 1, 2, 3, 4, 6, 8}
+
+    >>> bumbag.setred(set.difference, x, y, z)
+    {0, 1, 3}
+
+    >>> sym_diff = bumbag.setred(set.symmetric_difference)
+    >>> sym_diff(x, y, z)
+    {0, 1, 2, 3, 4, 8}
+    """
+    return functools.reduce(func, map(set, sets))
+
+
+@curried.curry
+def sig(number, /, *, digits=3):
     """Round number to its significant digits.
 
     Parameters
     ----------
     number : int, float
         Number to round.
     digits : int, default=3
@@ -310,31 +452,31 @@
 
     Examples
     --------
     >>> import bumbag
     >>> bumbag.sig(987654321)
     988000000
 
-    >>> bumbag.sig(14393237.76, 2)
+    >>> bumbag.sig(14393237.76, digits=2)
     14000000.0
 
-    >>> bumbag.sig(14393237.76, 3)
+    >>> bumbag.sig(14393237.76, digits=3)
     14400000.0
     """
     if not isinstance(digits, int) or digits < 1:
         raise ValueError(f"{digits=} - must be a positive integer")
 
     if not math.isfinite(number) or math.isclose(number, 0.0):
         return number
 
     digits -= math.ceil(math.log10(abs(number)))
     return round(number, digits)
 
 
-def two_set_summary(x, y, show=3):
+def two_set_summary(x, y, /, *, show=3):
     """Compute two set summary.
 
     Given two sets, calculate multiple key set operations like union,
     intersection, difference, and more.
 
     Parameters
     ----------
```

### Comparing `bumbag-4.1.0/src/bumbag/io.py` & `bumbag-5.0.0/src/bumbag/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __all__ = (
     "archive_files",
     "lazy_read_lines",
     "query_yes_no",
 )
 
 
-def archive_files(wildcards=None, target_dir=None, name=None, kind="zip"):
+def archive_files(*, wildcards=None, target_dir=None, name=None, kind="zip"):
     """Archive files in target directory.
 
     Parameters
     ----------
     wildcards : None, list of str, default=None
         Specify a wildcard to archive files. If ``wildcards`` is None,
         all files in target directory are archived.
@@ -37,15 +37,15 @@
         Function has no return value. However, the archive of files of
         the target directory is stored in the current working directory.
 
     Examples
     --------
     >>> # Archive all Python files and Notebooks in current working directory
     >>> import bumbag
-    >>> bumbag.archive_files(["*.py", "*.ipynb"])  # doctest: +SKIP
+    >>> bumbag.archive_files(wildcards=["*.py", "*.ipynb"])  # doctest: +SKIP
     """
     wildcards = wildcards or ["**/*"]
     target_dir = target_dir or "."
     target_dir = Path(target_dir).resolve()
     timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
     name = name or f"{timestamp}_{target_dir.stem}"
 
@@ -60,15 +60,15 @@
                 dst_dir = str(src_file.parent).replace(str(target_dir), tmpdir)
                 os.makedirs(dst_dir, exist_ok=True)
                 shutil.copy(str(src_file), dst_file)
 
         shutil.make_archive(name, kind, tmpdir)
 
 
-def lazy_read_lines(path, encoding=None, errors=None, newline=None):
+def lazy_read_lines(path, /, *, encoding=None, errors=None, newline=None):
     """Lazily read text file line by line.
 
     Parameters
     ----------
     path : str or Path
         Path to the text file to read from.
     encoding : str, default=None
@@ -108,26 +108,26 @@
         errors=errors,
         newline=newline,
     ) as lines:
         for line in lines:
             yield line
 
 
-def query_yes_no(question, default=None):
+def query_yes_no(question, /, *, default=None):
     """Prompt user a yes/no question.
 
     Parameters
     ----------
     question : str
         Specify a yes/no question to prompt the user.
     default : None, str, default=None
         Define default answer:
          - If ``default`` is None, an explicit answer is needed from the user.
          - If ``default`` is "yes" or "no", the presumed answer, indicated by
-           a capitial letter, is accepted when pressing <enter>.
+           a capital letter, is accepted when pressing <enter>.
 
     Returns
     -------
     bool
         ``True`` if user's answer is "yes" else ``False``.
 
     Raises
@@ -138,19 +138,19 @@
     Examples
     --------
     >>> import bumbag
     >>> bumbag.query_yes_no("Is all clear?")  # doctest: +SKIP
     Is all clear? [y/n] y<enter>
     True
 
-    >>> bumbag.query_yes_no("Do you like BumBag?", "yes")  # doctest: +SKIP
+    >>> bumbag.query_yes_no("Do you like BumBag?", default="yes")  # doctest: +SKIP
     Do you like BumBag? [Y/n] <enter>
     True
 
-    >>> bumbag.query_yes_no("Do you like BumBag?", "yes")  # doctest: +SKIP
+    >>> bumbag.query_yes_no("Do you like BumBag?", default="yes")  # doctest: +SKIP
     Do you like BumBag? [Y/n] yay<enter>
     Do you like BumBag? Please respond with 'yes' [Y] or 'no' [n] <enter>
     True
     """
     prompt = (
         "[y/n]"
         if default is None
```

### Comparing `bumbag-4.1.0/src/bumbag/math.py` & `bumbag-5.0.0/src/bumbag/math.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import toolz
 
 __all__ = (
     "collatz",
     "fibonacci",
+    "isdivisibleby",
     "iseven",
     "isodd",
 )
 
 
-def collatz(number):
+def collatz(number, /):
     """Generate the Collatz sequence for a positive integer.
 
     The famous 3n + 1 conjecture. Given a positive integer :math:`n > 0`,
     the next term in the Collatz sequence is half of :math:`n`
     if :math:`n` is even; otherwise, if :math:`n` is odd,
     the next term is 3 times :math:`n` plus 1.
     Symbolically,
@@ -100,15 +101,51 @@
 
     while True:
         lag0 = lag1 + lag2
         yield lag0
         lag1, lag2 = lag0, lag1
 
 
-def iseven(number):
+@toolz.curry
+def isdivisibleby(x, number, /):
+    """Is number evenly divisible by x.
+
+    Parameters
+    ----------
+    x : int
+        Specify the divisor.
+    number : int
+        Specify the number to check.
+
+    Returns
+    -------
+    bool
+        ``True`` if number is evenly divisible by x else ``False``.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> bumbag.isdivisibleby(2, 10)
+    True
+
+    >>> bumbag.isdivisibleby(2, 9)
+    False
+
+    >>> iseven = bumbag.isdivisibleby(2)
+    >>> iseven(10)
+    True
+    """
+    return number % x == 0
+
+
+def iseven(number, /):
     """Check if number is even.
 
     Parameters
     ----------
     number : int
         Number to check.
 
@@ -122,18 +159,18 @@
     >>> import bumbag
     >>> bumbag.iseven(2)
     True
 
     >>> bumbag.iseven(3)
     False
     """
-    return number % 2 == 0
+    return isdivisibleby(2)(number)
 
 
-def isodd(number):
+def isodd(number, /):
     """Check if number is odd.
 
     Parameters
     ----------
     number : int
         Number to check.
```

### Comparing `bumbag-4.1.0/src/bumbag/random.py` & `bumbag-5.0.0/src/bumbag/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "coinflip",
     "get_random_character",
     "get_random_instance",
     "get_random_integer",
 )
 
 
-def coinflip(bias=0.5, seed=None):
+def coinflip(*, bias=0.5, seed=None):
     """Flip a coin.
 
     Parameters
     ----------
     bias : float, default=0.5
         Specify the bias of the coin:
          - A ``bias`` of 0.5 corresponds to a fair coin.
@@ -39,19 +39,19 @@
     --------
     >>> import bumbag
     >>> {bumbag.coinflip() for _ in range(30)} == {True, False}
     True
     """
     if not (0 <= bias <= 1):
         raise ValueError(f"{bias=} - must be a float in [0, 1]")
-    rng = get_random_instance(seed)
+    rng = get_random_instance(seed=seed)
     return rng.random() < bias
 
 
-def get_random_character(alphabet=None, seed=None):
+def get_random_character(alphabet=None, /, *, seed=None):
     """Get a random character from a given alphabet.
 
     Parameters
     ----------
     alphabet : str, default=None
         Set of characters to sample from.
         If None, the default alphabet is made of [a-zA-Z0-9] characters.
@@ -71,20 +71,20 @@
     >>> import bumbag
     >>> rnd_char = bumbag.get_random_character("bumbag")
     >>> isinstance(rnd_char, str)
     True
     >>> rnd_char in "bumbag"
     True
     """
-    rng = get_random_instance(seed)
+    rng = get_random_instance(seed=seed)
     alphabet = alphabet or string.ascii_letters + string.digits
     return rng.sample(population=alphabet, k=len(alphabet))[0]
 
 
-def get_random_instance(seed=None):
+def get_random_instance(*, seed=None):
     """Turn seed into a random.Random instance.
 
     Parameters
     ----------
     seed : None, int, random.Random, default=None
         Value to seed an instance:
          - If ``seed`` is None, return random module's singleton.
@@ -123,15 +123,15 @@
     elif isinstance(seed, random.Random):
         return seed
 
     else:
         raise ValueError(f"{seed=} cannot be used to seed a Random instance")
 
 
-def get_random_integer(a=0, b=2147483647, seed=None):
+def get_random_integer(a=0, b=2147483647, /, *, seed=None):
     """Get a random integer from interval [a, b].
 
     Setting default values for the arguments of ``random.randint``.
 
     Parameters
     ----------
     a : int, default=0
@@ -154,9 +154,9 @@
     >>> import bumbag
     >>> rnd_int = bumbag.get_random_integer()
     >>> isinstance(rnd_int, int)
     True
     >>> 0 <= rnd_int <= 2147483647
     True
     """
-    rng = get_random_instance(seed)
+    rng = get_random_instance(seed=seed)
     return rng.randint(a, b)
```

### Comparing `bumbag-4.1.0/src/bumbag/string.py` & `bumbag-5.0.0/src/bumbag/string.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,61 @@
 import itertools
 import re
 import string as builtin_string_module
 
 import toolz
 
 __all__ = (
+    "concat_strings",
     "filter_regex",
+    "headline",
     "highlight_string_differences",
     "map_regex",
     "remove_punctuation",
 )
 
 
 @toolz.curry
-def filter_regex(pattern, strings, flags=re.IGNORECASE):
+def concat_strings(strings, /, *, sep=" "):
+    """Concatenate strings.
+
+    Parameters
+    ----------
+    strings : Iterable of str
+        Strings to concatenate.
+    sep : str, default=" "
+        Specify the separator.
+
+    Returns
+    -------
+    str
+        A concatenated string.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> bumbag.concat_strings(["Hello", "World"])
+    'Hello World'
+
+    >>> hyphen_concat = bumbag.concat_strings(sep="-")
+    >>> hyphen_concat(["Hello", "World"])
+    'Hello-World'
+
+    >>> list(map(bumbag.concat_strings, [["Hello", "World"]]))
+    ['Hello World']
+    """
+    return sep.join(strings)
+
+
+@toolz.curry
+def filter_regex(pattern, strings, /, *, flags=re.IGNORECASE):
     """Filter an iterable of strings with a regex pattern.
 
     Parameters
     ----------
     pattern : str
         Regex pattern to use.
     strings : Iterable of str
@@ -53,15 +91,46 @@
     >>> filter_python_regex = bumbag.filter_regex("python")
     >>> list(filter_python_regex(list_of_strings))
     ["Guiding principles for Python's design: The Zen of Python"]
     """
     return filter(functools.partial(re.findall, pattern, flags=flags), strings)
 
 
-def highlight_string_differences(lft_str, rgt_str):
+@toolz.curry
+def headline(string, /, *, length=88, character="-"):
+    """Generate a headline string.
+
+    Parameters
+    ----------
+    string : str
+        Specify headline text.
+    length : int, default=88
+        Specify the length of the headline string.
+    character : str, default="-"
+        Specify the character to fill the missing space on each side.
+
+    Returns
+    -------
+    str
+        A headline string.
+
+    Notes
+    -----
+    Function is curried.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> bumbag.headline("Hello, World!", length=30)
+    '------- Hello, World! --------'
+    """
+    return f" {string} ".center(length, character)
+
+
+def highlight_string_differences(lft_str, rgt_str, /):
     """Highlight differences between two strings.
 
     Parameters
     ----------
     lft_str : str
         Left string.
     rgt_str : str
@@ -76,20 +145,20 @@
     Notes
     -----
     In case of uneven string lengths, the comparison is done up until the longer string.
 
     Examples
     --------
     >>> import bumbag
-    >>> print(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hello"))
+    >>> print(bumbag.highlight_string_differences("hello", "hello"))
     hello
     <BLANKLINE>
     hello
 
-    >>> print(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall"))
+    >>> print(bumbag.highlight_string_differences("hello", "hall"))
     hello
      |  |
     hall
     """
     lines = (
         lft_str,
         "".join(
@@ -98,15 +167,15 @@
         ),
         rgt_str,
     )
     return "\n".join(lines)
 
 
 @toolz.curry
-def map_regex(pattern, strings, flags=re.IGNORECASE):
+def map_regex(pattern, strings, /, *, flags=re.IGNORECASE):
     """Map regex pattern to an iterable of strings.
 
     Parameters
     ----------
     pattern : str
         Regex pattern to use.
     strings : Iterable of str
@@ -143,15 +212,15 @@
     >>> map_python_regex = bumbag.map_regex("python")
     >>> list(map_python_regex(list_of_strings))
     [['Python', 'Python'], [], [], []]
     """
     return map(functools.partial(re.findall, pattern, flags=flags), strings)
 
 
-def remove_punctuation(string):
+def remove_punctuation(string, /):
     """Remove punctuation from a string.
 
     Parameters
     ----------
     string : str
         String to process.
```

### Comparing `bumbag-4.1.0/src/bumbag/time.py` & `bumbag-5.0.0/src/bumbag/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 import math
 import operator
 from datetime import date, datetime, timedelta
 
 import toolz
 from dateutil.relativedelta import relativedelta
 
-from bumbag.core import op
+from bumbag import core
 
 __all__ = (
     "datedelta",
     "daterange",
-    "day_of_week",
     "days_between_dates",
     "daycount",
     "humantime",
     "last_date_of_month",
     "months_between_dates",
     "to_date",
     "to_str",
+    "weekday",
 )
 
 
-def datedelta(reference, days):
+def datedelta(reference_date, /, *, days):
     """Compute date relative to reference date.
 
     The reference date and relative date are the inclusive endpoints of the
     corresponding, consecutive date sequence. As a result, the reference date
     and relative date can, for example, directly be used in a BETWEEN statement
     of a SQL query.
 
     Parameters
     ----------
-    reference : datetime.date
-        The reference date.
+    reference_date : datetime.date
+        Specify reference date.
     days : int
         Size of the delta expressed in number of days:
          - If ``days == 0``, returns the reference date.
          - If ``days > 0``, returns the date ahead w.r.t. the reference date.
          - If ``days < 0``, returns the date ago w.r.t. the reference date.
         The value of ``days`` equals the length of the corresponding sequence of
         consecutive dates with inclusive endpoints.
@@ -48,34 +48,35 @@
     datetime.date
         Relative date.
 
     Examples
     --------
     >>> import bumbag
     >>> from datetime import date
-    >>> bumbag.datedelta(date(2022, 1, 1), 0)
+    >>> reference_date = date(2022, 1, 1)
+    >>> bumbag.datedelta(reference_date, days=0)
     datetime.date(2022, 1, 1)
 
-    >>> bumbag.datedelta(date(2022, 1, 1), 3)
+    >>> bumbag.datedelta(reference_date, days=3)
     datetime.date(2022, 1, 3)
 
-    >>> bumbag.datedelta(date(2022, 1, 1), -3)
+    >>> bumbag.datedelta(reference_date, days=-3)
     datetime.date(2021, 12, 30)
     """
-    relative_date = reference + timedelta(days=days)
+    relative_date = reference_date + timedelta(days=days)
     return (
         relative_date
         if days == 0
         else relative_date - timedelta(days=1)
         if days > 0
         else relative_date + timedelta(days=1)
     )
 
 
-def daterange(start, end, include_start=True, include_end=True):
+def daterange(start, end, /, *, include_start=True, include_end=True):
     """Generate a sequence of consecutive days between two dates.
 
     Parameters
     ----------
     start : datetime.date
         Start of the sequence.
     end : datetime.date
@@ -103,32 +104,41 @@
     >>> d1 = date(2022, 1, 1)
     >>> d2 = date(2022, 1, 3)
 
     >>> curried.pipe(bumbag.daterange(d1, d2), curried.map(bumbag.to_str), list)
     ['2022-01-01', '2022-01-02', '2022-01-03']
 
     >>> curried.pipe(
-    ...     bumbag.daterange(d1, d2, False, True), curried.map(bumbag.to_str), list
+    ...     bumbag.daterange(d1, d2, include_start=False, include_end=True),
+    ...     curried.map(bumbag.to_str),
+    ...     list,
     ... )
     ['2022-01-02', '2022-01-03']
 
     >>> curried.pipe(
-    ...     bumbag.daterange(d1, d2, True, False), curried.map(bumbag.to_str), list
+    ...     bumbag.daterange(d1, d2, include_start=True, include_end=False),
+    ...     curried.map(bumbag.to_str),
+    ...     list,
     ... )
     ['2022-01-01', '2022-01-02']
 
     >>> curried.pipe(
-    ...     bumbag.daterange(d1, d2, False, False), curried.map(bumbag.to_str), list
+    ...     bumbag.daterange(d1, d2, include_start=False, include_end=False),
+    ...     curried.map(bumbag.to_str),
+    ...     list,
     ... )
     ['2022-01-02']
 
     >>> curried.pipe(bumbag.daterange(date(2022, 1, 1), date(2022, 1, 1)), list)
     [datetime.date(2022, 1, 1)]
 
-    >>> curried.pipe(bumbag.daterange(date(2022, 1, 1), date(2022, 1, 1), False), list)
+    >>> curried.pipe(
+    ...     bumbag.daterange(date(2022, 1, 1), date(2022, 1, 1), include_start=False),
+    ...     list,
+    ... )
     []
 
     >>> curried.pipe(bumbag.daterange(d2, d1), curried.map(bumbag.to_str), list)
     ['2022-01-01', '2022-01-02', '2022-01-03']
 
     >>> # month sequence - first date
     >>> curried.pipe(
@@ -151,46 +161,15 @@
     """
     start, end = sorted([start, end])
     start = start if include_start else start + timedelta(1)
     end = end if include_end else end - timedelta(1)
     return itertools.takewhile(lambda d: d <= end, daycount(start))
 
 
-def day_of_week(date_to_name):
-    """Get the day of the week.
-
-    Parameters
-    ----------
-    date_to_name : datetime.date
-        Date object to extract day name from.
-
-    Returns
-    -------
-    str
-        Day name of the week.
-
-    Examples
-    --------
-    >>> import bumbag
-    >>> from datetime import date
-    >>> d1 = date(2022, 8, 1)
-    >>> d2 = date(2022, 8, 5)
-    >>> list(map(bumbag.day_of_week, bumbag.daterange(d1, d2)))
-    ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday']
-
-    >>> bumbag.day_of_week(date(2022, 8, 6))
-    'Saturday'
-
-    >>> bumbag.day_of_week(date(2022, 8, 7))
-    'Sunday'
-    """
-    return date_to_name.strftime("%A")
-
-
-def days_between_dates(date1, date2, include_last_date=False):
+def days_between_dates(date1, date2, /, *, include_last_date=False):
     """Compute the number of days between two dates.
 
     Parameters
     ----------
     date1 : datetime.date
         First reference date.
     date2 : datetime.date
@@ -211,33 +190,37 @@
 
     Examples
     --------
     >>> import bumbag
     >>> from datetime import date
     >>> bumbag.days_between_dates(date(2022, 8, 1), date(2022, 8, 1))
     0
-    >>> bumbag.days_between_dates(date(2022, 8, 1), date(2022, 8, 1), True)
+    >>> bumbag.days_between_dates(
+    ...     date(2022, 8, 1), date(2022, 8, 1), include_last_date=True
+    ... )
     1
 
     >>> bumbag.days_between_dates(date(2022, 8, 1), date(2022, 8, 7))
     6
-    >>> bumbag.days_between_dates(date(2022, 8, 1), date(2022, 8, 7), True)
+    >>> bumbag.days_between_dates(
+    ...     date(2022, 8, 1), date(2022, 8, 7), include_last_date=True
+    ... )
     7
     """
     start, end = sorted([date1, date2])
     return (end - start).days + 1 if include_last_date else (end - start).days
 
 
-def daycount(start, forward=True):
+def daycount(start_date, /, *, forward=True):
     """Generate an in principle infinite sequence of consecutive dates.
 
     Parameters
     ----------
-    start : datetime.date
-        Start of the sequence.
+    start_date : datetime.date
+        Specify the start date of the sequence.
     forward : bool, default=True
         Specify if dates should be generated in a forward or backward manner.
 
     Yields
     ------
     datetime.date
         A generator of the date sequence.
@@ -255,23 +238,23 @@
 
     >>> curried.pipe(
     ...     bumbag.daycount(d1), curried.map(bumbag.to_str), curried.take(3), list
     ... )
     ['2022-01-01', '2022-01-02', '2022-01-03']
 
     >>> curried.pipe(
-    ...     bumbag.daycount(d1, False),
+    ...     bumbag.daycount(d1, forward=False),
     ...     curried.map(bumbag.to_str),
     ...     curried.take(3),
     ...     list,
     ... )
     ['2022-01-01', '2021-12-31', '2021-12-30']
 
     >>> curried.pipe(
-    ...     bumbag.daycount(d1, False),
+    ...     bumbag.daycount(d1, forward=False),
     ...     curried.map(bumbag.to_str),
     ...     curried.take(3),
     ...     list,
     ... )
     ['2022-01-01', '2021-12-31', '2021-12-30']
 
     >>> # month sequence - first date
@@ -294,15 +277,15 @@
     ...     list,
     ... )
     ['2022-01-31', '2022-02-28', '2022-03-31', '2022-04-30', '2022-05-31']
 
     >>> # Monday sequence
     >>> curried.pipe(
     ...     bumbag.daycount(d1),
-    ...     curried.filter(lambda d: day_of_week(d) == "Monday"),
+    ...     curried.filter(lambda d: weekday(d) == "Mon"),
     ...     curried.map(bumbag.to_str),
     ...     curried.take(5),
     ...     list,
     ... )
     ['2022-01-03', '2022-01-10', '2022-01-17', '2022-01-24', '2022-01-31']
 
     >>> # pick every 7th day
@@ -311,19 +294,19 @@
     ...     curried.take_nth(7),
     ...     curried.map(bumbag.to_str),
     ...     curried.take(5),
     ...     list,
     ... )
     ['2022-01-01', '2022-01-08', '2022-01-15', '2022-01-22', '2022-01-29']
     """
-    successor = op(operator.add if forward else operator.sub, y=timedelta(1))
-    return toolz.iterate(successor, start)
+    successor = core.op(operator.add if forward else operator.sub, y=timedelta(1))
+    return toolz.iterate(successor, start_date)
 
 
-def humantime(seconds):
+def humantime(seconds, /):
     """Convert seconds to human-readable time.
 
     Parameters
     ----------
     seconds : int, float
         Seconds to convert, a non-negative number.
 
@@ -387,15 +370,15 @@
 
     if seconds:
         output.append(f"{seconds}s")
 
     return " ".join(output)
 
 
-def last_date_of_month(year, month):
+def last_date_of_month(year, month, /):
     """Get last date of month.
 
     Parameters
     ----------
     year : int
         Year of date.
     month : int
@@ -412,23 +395,23 @@
     >>> bumbag.last_date_of_month(2022, 1)
     datetime.date(2022, 1, 31)
     """
     _, number_days_in_month = calendar.monthrange(year, month)
     return date(year, month, number_days_in_month)
 
 
-def months_between_dates(date1, date2, include_last_date=False):
+def months_between_dates(date1, date2, /, *, include_last_date=False):
     """Compute the number of months between two dates.
 
     Parameters
     ----------
     date1 : datetime.date
-        First reference date.
+        Specify the first reference date.
     date2 : datetime.date
-        Second reference date.
+        Specify the second reference date.
     include_last_date : bool, default=False
         Specify if the larger date should be included in the computation:
          - If ``False``, number of days based on date interval [date1, date2).
          - If ``True``, number of days based on date interval [date1, date2].
 
     Notes
     -----
@@ -441,29 +424,33 @@
 
     Examples
     --------
     >>> import bumbag
     >>> from datetime import date
     >>> bumbag.months_between_dates(date(2022, 1, 1), date(2022, 1, 1))
     0
-    >>> bumbag.months_between_dates(date(2022, 1, 1), date(2022, 1, 1), True)
+    >>> bumbag.months_between_dates(
+    ...     date(2022, 1, 1), date(2022, 1, 1), include_last_date=True
+    ... )
     1
 
     >>> bumbag.months_between_dates(date(2022, 1, 1), date(2022, 8, 31))
     7
-    >>> bumbag.months_between_dates(date(2022, 1, 1), date(2022, 8, 1), True)
+    >>> bumbag.months_between_dates(
+    ...     date(2022, 1, 1), date(2022, 8, 1), include_last_date=True
+    ... )
     8
     """
     start, end = sorted([date1, date2])
     difference = relativedelta(end, start)
     n_months = difference.months + 12 * difference.years
     return n_months + 1 if include_last_date else n_months
 
 
-def to_date(string_to_cast):
+def to_date(string_to_cast, /):
     """Cast an ISO date string to a date object.
 
     Parameters
     ----------
     string_to_cast : str
         Date string in ISO format (YYYY-MM-DD) to cast.
 
@@ -477,15 +464,15 @@
     >>> import bumbag
     >>> bumbag.to_date("2022-01-01")
     datetime.date(2022, 1, 1)
     """
     return datetime.strptime(string_to_cast, "%Y-%m-%d").date()
 
 
-def to_str(date_to_cast):
+def to_str(date_to_cast, /):
     """Cast a date object to an ISO date string.
 
     Parameters
     ----------
     date_to_cast : datetime.date
         Date object to cast.
 
@@ -498,7 +485,38 @@
     --------
     >>> import bumbag
     >>> from datetime import date
     >>> bumbag.to_str(date(2022, 1, 1))
     '2022-01-01'
     """
     return date_to_cast.isoformat()
+
+
+def weekday(a_date, /):
+    """Get name of the weekday.
+
+    Parameters
+    ----------
+    a_date : datetime.date
+        Specify date to extract weekday name from.
+
+    Returns
+    -------
+    str
+        Name of the weekday.
+
+    Examples
+    --------
+    >>> import bumbag
+    >>> from datetime import date
+    >>> d1 = date(2022, 8, 1)
+    >>> d2 = date(2022, 8, 5)
+    >>> list(map(bumbag.weekday, bumbag.daterange(d1, d2)))
+    ['Mon', 'Tue', 'Wed', 'Thu', 'Fri']
+
+    >>> bumbag.weekday(date(2022, 8, 6))
+    'Sat'
+
+    >>> bumbag.weekday(date(2022, 8, 7))
+    'Sun'
+    """
+    return a_date.strftime("%a")
```

### Comparing `bumbag-4.1.0/setup.py` & `bumbag-5.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dateutil>=2.8.2,<3.0.0', 'toolz>=0.12.0,<0.13.0']
 
 setup_kwargs = {
     'name': 'bumbag',
-    'version': '4.1.0',
+    'version': '5.0.0',
     'description': 'A package for Python utility functions.',
-    'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/estripling/bumbag/main/docs/source/_static/logo.png" width="180" alt="The BumBag logo.">\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/bumbag"><img alt="pypi" src="https://img.shields.io/pypi/v/bumbag"></a>\n<a href="https://readthedocs.org/projects/bumbag/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/bumbag/badge/?version=latest"></a>\n<a href="https://github.com/estripling/bumbag/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/bumbag/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/bumbag"><img alt="coverage" src="https://codecov.io/github/estripling/bumbag/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/bumbag/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/bumbag"></a>\n</p>\n\n## About\n\nBumBag is a collection of Python utility functions:\n\n- [Documentation](https://bumbag.readthedocs.io/en/stable/index.html)\n- [Example usage](https://bumbag.readthedocs.io/en/stable/example.html)\n- [API Reference](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html)\n\n## Installation\n\n`bumbag` is available on [PyPI](https://pypi.org/project/bumbag/) for Python 3.8+:\n\n```shell\npip install bumbag\n```\n\n## Examples\n\nEasily [`flatten`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.flatten) an irregular list:\n\n```python\n>>> import bumbag\n>>> irregular_list = [\n...     ["one", 2],\n...     3,\n...     [(4, "five")],\n...     [[["six"]]],\n...     "seven",\n...     [],\n... ]\n>>> list(bumbag.flatten(irregular_list, 8, [9, ("ten",)]))\n[\'one\', 2, 3, 4, \'five\', \'six\', \'seven\', 8, 9, \'ten\']\n```\n\nUse [`highlight_string_differences`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.highlight_string_differences) to see differences between two strings easily:\n\n```python\n>>> import bumbag\n>>> print(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall"))\nhello\n |  |\nhall\n```\n\nQuickly compare two Python sets with [`two_set_summary`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.two_set_summary):\n\n```python\n>>> import bumbag\n>>> x = {"a", "c", "b", "g", "h"}\n>>> y = {"c", "d", "e", "f", "g"}\n>>> summary = bumbag.two_set_summary(x, y)\n>>> print(summary["report"])\n    x (n=5): {\'a\', \'b\', \'c\', ...}\n    y (n=5): {\'c\', \'d\', \'e\', ...}\nx | y (n=8): {\'a\', \'b\', \'c\', ...}\nx & y (n=2): {\'c\', \'g\'}\nx - y (n=3): {\'a\', \'b\', \'h\'}\ny - x (n=3): {\'d\', \'e\', \'f\'}\nx ^ y (n=6): {\'a\', \'b\', \'d\', ...}\njaccard = 0.25\noverlap = 0.4\ndice = 0.4\ndisjoint?: False\nx == y: False\nx <= y: False\nx <  y: False\ny <= x: False\ny <  x: False\n```\n\n## Contributing to BumBag\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://bumbag.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://bumbag.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://bumbag.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`bumbag` was created by the BumBag Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
+    'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/estripling/bumbag/main/docs/source/_static/logo.png" width="180" alt="The BumBag logo.">\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/bumbag"><img alt="pypi" src="https://img.shields.io/pypi/v/bumbag"></a>\n<a href="https://readthedocs.org/projects/bumbag/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/bumbag/badge/?version=latest"></a>\n<a href="https://github.com/estripling/bumbag/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/bumbag/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/bumbag"><img alt="coverage" src="https://codecov.io/github/estripling/bumbag/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/bumbag/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/bumbag"></a>\n</p>\n\n## About\n\nBumBag is a collection of Python utility functions:\n\n- [Documentation](https://bumbag.readthedocs.io/en/stable/index.html)\n- [Example usage](https://bumbag.readthedocs.io/en/stable/example.html)\n- [API Reference](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html)\n\n## Installation\n\n`bumbag` is available on [PyPI](https://pypi.org/project/bumbag/) for Python 3.8+:\n\n```shell\npip install bumbag\n```\n\n## Examples\n\nEasily [`flatten`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.flatten) an irregular list:\n\n```python\n>>> import bumbag\n>>> irregular_list = [\n...     ["one", 2],\n...     3,\n...     [(4, "five")],\n...     [[["six"]]],\n...     "seven",\n...     [],\n... ]\n>>> list(bumbag.flatten(irregular_list, 8, [9, ("ten",)]))\n[\'one\', 2, 3, 4, \'five\', \'six\', \'seven\', 8, 9, \'ten\']\n```\n\nUse [`highlight_string_differences`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.highlight_string_differences) to see differences between two strings easily:\n\n```python\n>>> import bumbag\n>>> print(bumbag.highlight_string_differences("hello", "hall"))\nhello\n |  |\nhall\n```\n\nQuickly compare two Python sets with [`two_set_summary`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.two_set_summary):\n\n```python\n>>> import bumbag\n>>> x = {"a", "c", "b", "g", "h"}\n>>> y = {"c", "d", "e", "f", "g"}\n>>> summary = bumbag.two_set_summary(x, y)\n>>> print(summary["report"])\n    x (n=5): {\'a\', \'b\', \'c\', ...}\n    y (n=5): {\'c\', \'d\', \'e\', ...}\nx | y (n=8): {\'a\', \'b\', \'c\', ...}\nx & y (n=2): {\'c\', \'g\'}\nx - y (n=3): {\'a\', \'b\', \'h\'}\ny - x (n=3): {\'d\', \'e\', \'f\'}\nx ^ y (n=6): {\'a\', \'b\', \'d\', ...}\njaccard = 0.25\noverlap = 0.4\ndice = 0.4\ndisjoint?: False\nx == y: False\nx <= y: False\nx <  y: False\ny <= x: False\ny <  x: False\n```\n\n## Contributing to BumBag\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://bumbag.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://bumbag.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://bumbag.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`bumbag` was created by the BumBag Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
     'author': 'BumBag Developers',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/estripling/bumbag',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['bumbag'] package_data = \ {'': ['*']} install_requires =
 \ ['python-dateutil>=2.8.2,<3.0.0', 'toolz>=0.12.0,<0.13.0'] setup_kwargs =
-{ 'name': 'bumbag', 'version': '4.1.0', 'description': 'A package for Python
+{ 'name': 'bumbag', 'version': '5.0.0', 'description': 'A package for Python
 utility functions.', 'long_description': '
                             \n[The BumBag logo.]\n
 \n\n
             \n[pypi]\n[docs]\n[ci_status]\n[coverage]\n[license]\n
 \n\n## About\n\nBumBag is a collection of Python utility functions:\n\n-
 [Documentation](https://bumbag.readthedocs.io/en/stable/index.html)\n- [Example
 usage](https://bumbag.readthedocs.io/en/stable/example.html)\n- [API Reference]
@@ -17,19 +17,19 @@
 bumbag\n>>> irregular_list = [\n... ["one", 2],\n... 3,\n... [(4,
 "five")],\n... [[["six"]]],\n... "seven",\n... [],\n... ]\n>>> list
 (bumbag.flatten(irregular_list, 8, [9, ("ten",)]))\n[\'one\', 2, 3, 4,
 \'five\', \'six\', \'seven\', 8, 9, \'ten\']\n```\n\nUse
 [`highlight_string_differences`](https://bumbag.readthedocs.io/en/stable/
 autoapi/bumbag/index.html#bumbag.highlight_string_differences) to see
 differences between two strings easily:\n\n```python\n>>> import bumbag\n>>>
-print(bumbag.highlight_string_differences(lft_str="hello",
-rgt_str="hall"))\nhello\n | |\nhall\n```\n\nQuickly compare two Python sets
-with [`two_set_summary`](https://bumbag.readthedocs.io/en/stable/autoapi/
-bumbag/index.html#bumbag.two_set_summary):\n\n```python\n>>> import bumbag\n>>>
-x = {"a", "c", "b", "g", "h"}\n>>> y = {"c", "d", "e", "f", "g"}\n>>> summary =
+print(bumbag.highlight_string_differences("hello", "hall"))\nhello\n |
+|\nhall\n```\n\nQuickly compare two Python sets with [`two_set_summary`](https:
+//bumbag.readthedocs.io/en/stable/autoapi/bumbag/
+index.html#bumbag.two_set_summary):\n\n```python\n>>> import bumbag\n>>> x =
+{"a", "c", "b", "g", "h"}\n>>> y = {"c", "d", "e", "f", "g"}\n>>> summary =
 bumbag.two_set_summary(x, y)\n>>> print(summary["report"])\n x (n=5): {\'a\',
 \'b\', \'c\', ...}\n y (n=5): {\'c\', \'d\', \'e\', ...}\nx | y (n=8): {\'a\',
 \'b\', \'c\', ...}\nx & y (n=2): {\'c\', \'g\'}\nx - y (n=3): {\'a\', \'b\',
 \'h\'}\ny - x (n=3): {\'d\', \'e\', \'f\'}\nx ^ y (n=6): {\'a\', \'b\', \'d\',
 ...}\njaccard = 0.25\noverlap = 0.4\ndice = 0.4\ndisjoint?: False\nx == y:
 False\nx <= y: False\nx < y: False\ny <= x: False\ny < x: False\n```\n\n##
 Contributing to BumBag\n\nYour contribution is greatly appreciated!\nSee the
```

### Comparing `bumbag-4.1.0/PKG-INFO` & `bumbag-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumbag
-Version: 4.1.0
+Version: 5.0.0
 Summary: A package for Python utility functions.
 Home-page: https://github.com/estripling/bumbag
 License: BSD-3-Clause
 Keywords: utility functions,bumbag
 Author: BumBag Developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -69,15 +69,15 @@
 ['one', 2, 3, 4, 'five', 'six', 'seven', 8, 9, 'ten']
 ```
 
 Use [`highlight_string_differences`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.highlight_string_differences) to see differences between two strings easily:
 
 ```python
 >>> import bumbag
->>> print(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall"))
+>>> print(bumbag.highlight_string_differences("hello", "hall"))
 hello
  |  |
 hall
 ```
 
 Quickly compare two Python sets with [`two_set_summary`](https://bumbag.readthedocs.io/en/stable/autoapi/bumbag/index.html#bumbag.two_set_summary):
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bumbag Version: 4.1.0 Summary: A package for Python
+Metadata-Version: 2.1 Name: bumbag Version: 5.0.0 Summary: A package for Python
 utility functions. Home-page: https://github.com/estripling/bumbag License:
 BSD-3-Clause Keywords: utility functions,bumbag Author: BumBag Developers
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
@@ -24,16 +24,16 @@
 irregular list: ```python >>> import bumbag >>> irregular_list = [ ... ["one",
 2], ... 3, ... [(4, "five")], ... [[["six"]]], ... "seven", ... [], ... ] >>>
 list(bumbag.flatten(irregular_list, 8, [9, ("ten",)])) ['one', 2, 3, 4, 'five',
 'six', 'seven', 8, 9, 'ten'] ``` Use [`highlight_string_differences`](https://
 bumbag.readthedocs.io/en/stable/autoapi/bumbag/
 index.html#bumbag.highlight_string_differences) to see differences between two
 strings easily: ```python >>> import bumbag >>> print
-(bumbag.highlight_string_differences(lft_str="hello", rgt_str="hall")) hello |
-| hall ``` Quickly compare two Python sets with [`two_set_summary`](https://
+(bumbag.highlight_string_differences("hello", "hall")) hello | | hall ```
+Quickly compare two Python sets with [`two_set_summary`](https://
 bumbag.readthedocs.io/en/stable/autoapi/bumbag/
 index.html#bumbag.two_set_summary): ```python >>> import bumbag >>> x = {"a",
 "c", "b", "g", "h"} >>> y = {"c", "d", "e", "f", "g"} >>> summary =
 bumbag.two_set_summary(x, y) >>> print(summary["report"]) x (n=5): {'a', 'b',
 'c', ...} y (n=5): {'c', 'd', 'e', ...} x | y (n=8): {'a', 'b', 'c', ...} x & y
 (n=2): {'c', 'g'} x - y (n=3): {'a', 'b', 'h'} y - x (n=3): {'d', 'e', 'f'} x ^
 y (n=6): {'a', 'b', 'd', ...} jaccard = 0.25 overlap = 0.4 dice = 0.4
```

