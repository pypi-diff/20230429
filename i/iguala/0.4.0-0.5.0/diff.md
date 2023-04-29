# Comparing `tmp/iguala-0.4.0.tar.gz` & `tmp/iguala-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguala-0.4.0.tar", last modified: Wed Dec 21 23:01:58 2022, max compression
+gzip compressed data, was "iguala-0.5.0.tar", last modified: Sat Apr 29 18:48:38 2023, max compression
```

## Comparing `iguala-0.4.0.tar` & `iguala-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:01:58.439601 iguala-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-21 23:01:46.000000 iguala-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-21 23:01:46.000000 iguala-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-21 23:01:46.000000 iguala-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2022-12-21 23:01:58.435601 iguala-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2022-12-21 23:01:46.000000 iguala-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:01:58.435601 iguala-0.4.0/iguala/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-21 23:01:46.000000 iguala-0.4.0/iguala/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2022-12-21 23:01:46.000000 iguala-0.4.0/iguala/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18886 2022-12-21 23:01:46.000000 iguala-0.4.0/iguala/matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2022-12-21 23:01:46.000000 iguala-0.4.0/iguala/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:01:58.435601 iguala-0.4.0/iguala.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2022-12-21 23:01:58.000000 iguala-0.4.0/iguala.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-21 23:01:58.000000 iguala-0.4.0/iguala.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 23:01:58.000000 iguala-0.4.0/iguala.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-21 23:01:58.000000 iguala-0.4.0/iguala.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 23:01:58.439601 iguala-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-12-21 23:01:46.000000 iguala-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-29 18:48:26.000000 iguala-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-29 18:48:26.000000 iguala-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 18:48:26.000000 iguala-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-04-29 18:48:38.963733 iguala-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-04-29 18:48:26.000000 iguala-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/iguala/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/iguala.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:48:38.963733 iguala-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-29 18:48:26.000000 iguala-0.5.0/setup.py
```

### Comparing `iguala-0.4.0/LICENSE` & `iguala-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iguala-0.4.0/PKG-INFO` & `iguala-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.4.0
+Version: 0.5.0
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
@@ -54,26 +54,35 @@
 NOTE: in this document, the term `matcher` and `pattern` are used to refer to the same thing, but a matcher matches a single small entity while a pattern defines a composition of matchers (or a single matcher).
 
 ```python
 # we consider that "MyObject" is an already known type
 # and "instance" and instance of it with att1 = att2 = 4 and name = 'foo'
 from iguala import match, is_not
 
-pattern = match(MyObject) % {  # must be an instance of MyObject
+pattern = match(MyObject)[  # must be an instance of MyObject
     "att1": "@value",  # with att1 stored in "value"
     "att2": "@value",   # and att2 with the same value as the one from att1
     "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
-}
+]
+
 print(pattern.match(instance))
 # displays: <True: [{'value': 4, 'name': 'foo'}]>
 
 # An equivalent Python code would be:
 if type(instance) == MyObject and instance.att1 == instance.att2 and instance.name != "bar":
     value = instance.att1
     name = instance.name
+
+# As an alternative syntax, here is how you can write the same pattern
+# You can choose the one you prefer, there is pros and cons with both
+pattern = match(MyObject) % {  # must be an instance of MyObject
+    "att1": "@value",  # with att1 stored in "value"
+    "att2": "@value",   # and att2 with the same value as the one from att1
+    "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
+}
 ```
 
 ## Installation
 
 ```sh
 pip install iguala
 ```
@@ -121,22 +130,23 @@
 
 ### Matchers/pattern operators
 
 There is few pattern operators.
 
 * `match(...)` with a type as parameter matches exactly a type, e.g: `match(A) % {}` means, match an instance of `A` (but not subclasses).
 * `~` used in front of an object matcher expresses "and all its subclasses", e.g: `~match(object) % {}` means, match an instance of `object` or from its subclasses.
+* `matcher[...]` with slices as indexes which expresses the properties of an object, e.g: `match(A)['name': 'foo']` means, match an instance of `A` where the `name` equals `foo`.
 * `%` with a dictionnary on its right expresses the properties of an object, e.g: `match(A) % {'name': 'foo'}` means, match an instance of `A` where the `name` equals `foo`.
-* `@` stores a data into a dedicated name, e.g: `match(A) % {'name': 'foo'} @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
-* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A) % {'name': is_not('foo')}`, means match an instance of `A` where the `name` is not equal to `foo`,
-* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A) % {'name': regex('[A-Z].*')}`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
-    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A) % {'name': regex('[A-Z].*') >> 'match_result'}` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
-    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A) % {'name': regex('[A-Z].*', label='match_result')}`. Using the operator or not is a matter of taste, the effect is exactly the same.
-* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A) % {'x': range(0, 5)}` means, match an instance of `A` where `x` is in the range `[0..4]`.
-* `|` expresses a logical "or" between two patterns, e.g: `match(A) % {'name': is_not(m('foo') | 'bar')}`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
+* `@` stores a data into a dedicated name, e.g: `match(A)['name': 'foo'] @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
+* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A)['name': is_not('foo')]`, means match an instance of `A` where the `name` is not equal to `foo`,
+* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A)['name': regex('[A-Z].*')]`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
+    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A)['name': regex('[A-Z].*') >> 'match_result']` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
+    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A)['name': regex('[A-Z].*', label='match_result')]`. Using the operator or not is a matter of taste, the effect is exactly the same.
+* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A)['x': range(0, 5)]` means, match an instance of `A` where `x` is in the range `[0..4]`.
+* `|` expresses a logical "or" between two patterns, e.g: `match(A)['name': is_not(m('foo') | 'bar')]`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
 
 ### Collections patterns
 
 Here is a list of some examples of patterns that can be applied to collections:
 
 * `[]`, means empty collection
 * `[3]` means a collection with only one value: `3`
@@ -154,26 +164,26 @@
 * `is_not([..., '@x', ..., is_not('@x'), ...])` means a collection where there is no elements that are not the same (a collection where all elements are the same)
 
 ### Lambda based matchers
 
 Lambdas are used to express patterns over captured variables:
 
 * `lambda VAR1, VAR2, ....: SOMETHINGS WITHS VARS` is a matcher generator.
-Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A): {'x': '@x', 'y': lambda x: x + 1}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A)['x': '@x', 'y': lambda x: x + 1]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `cond(lambda ....)` is a condition matcher (needs to be imported `from iguala import cond`).
-Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A): {'x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A)['x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `__self__` is a meta-variable that can be passed as arguments of the matcher generator or conditional matcher. This variable resolves to the object currently matched.
 
 Matcher generators and conditional matchers also works with sequence matchers, negative matchers, range matcher, regex matcher...etc.
 Here is some examples:
 
 * `[..., '@x', lambda x: x + 1, ...]` means a collection where one element is followed by its successor.
 * `[..., '@x', is_not(lambda x: x + 1), ...]` means a collection where one element is not followed by its successor.
 * `is_not([..., '@x', is_not(lambda x: x + 1), ...])` means a collection where there is no element that is not followed by its successor (a collection that is sorted).
-* `match(A) % {'x': '@x', 'y': lambda x: range(0, x + 1)}` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
+* `match(A)['x': '@x', 'y': lambda x: range(0, x + 1)]` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
 
 
 NOTE: Argument names of the function used for the matcher generator or the conditional matcher have to match the name of variables defined in the pattern.
 If other names are used, `iguala` will ignore the matcher, but will generate a warning message stating what are the missing variables and their positions in the pattern.
 
 ## Walkthrough - Draw me a pattern on an Object
 
@@ -224,34 +234,34 @@
 # displays: <False - []>
 ```
 No suprises, `a1` and `a2` are instances of `A` while `b` is not.
 
 Let's now see if those objects are instances of `A` with an attribute `z` that equals 4, then if they own an attribute `x` equals to 4.
 
 ```python
-pattern = match(A) % { 'z': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'z': 4 ]  # is it an instance of A with 'z' == 4?
 
 print(pattern.match(a1))  # and a2, b
 # displays: <False - []>, they don't have 'z' properties
 
-pattern = match(A) % { 'x': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'x': 4 ]  # is it an instance of A with 'z' == 4?
 print(pattern.match(a1))
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{}]>
 ```
 
 Now, let's deconstruct to get the value of `x`.
 We will express in our pattern that the data should be an instance of `A` with an attribute `x` and that we want to store the value of `x` in a variable named `value`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <True - [{'value': 3}]>
 print(result.bindings[0]['value'])
 # displays: 3
 
@@ -263,101 +273,101 @@
 
 Each right side of the property dictionnary that starts with an `@` means that it's a variable.
 If the name is found again in the pattern, then, it means that the data needs to have the same value for those variable in those positions.
 
 Let's use that to check now if each data is an instance of `A` where `x` and `y` have the same value.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
     'y': '@value'  # with an attribute "y" with the same value as "x"
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{'value': 4}]>
 ```
 
 Let's check now if we have an instance of `A` with a `2` in the collection `l`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': 2  # does "l" contains a 2?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{}, {}]>, there is two 2 in "l", so two combination, this information is returned by the matcher
 
 print(pattern.match(a2))
 # displays: <True - [{}]>, here there is only one 2 in "l"
 ```
 
 Let's try more precise questions over the collection `l`:
 
 ```python
 #
 # Patterns over collections
 #
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [2]  # does "l" contains only a 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., 2]  # does the last element of "l" is 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value']  # does "l" has a last element?
-}
+]
 print(pattern.match(a1))
 # displays: <True: [{'value': 5}]>
 
 print(pattern.match(a2))
 # displays: <True: [{'value': 2}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', '@value', ...]  # does "l" has two times the same element that follow each other?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True: [{'value': 2}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', ..., '@value', ...]  # does "l" has at least two times the same element?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{'value': 2}, {'value': 3}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': ["*l1", '@value', "*l2", '@value', "*l3"]  # does "l" has at least two times the same element? and store the collections around
-}
+]
 
 print(pattern.match(a1))
 # input for l was: [1, 2, 2, 3, 4, 3, 5]
 # displays: <True - [
 #    {'l1': [1], 'value': 2, 'l2': [], 'l3': [3, 4, 3, 5]},
 #    {'l1': [1, 2, 2], 'value': 3, 'l2': [4], 'l3': [5]}
 # ]>
@@ -373,17 +383,17 @@
 a3 = A(x=3, y=4, l=[])
 col = [a1, a2, b, a3, b]
 
 # does the collection contains two instances of A that have the same value for x
 # and store the nodes in 'inst1' and 'inst2'
 matcher = as_matcher(
     [...,
-     match(A) % {'x': '@x'} @ 'inst1',
+     match(A)['x': '@x'] @ 'inst1',
      ...,
-     match(A) % {'x': '@x'} @ 'inst2',
+     match(A)['x': '@x'] @ 'inst2',
      ...]
 )
 
 print(matcher.match(col))
 # displays: <True - [{'inst1': A(x=3, y=4, l=[1, 2, 2, 3, 4, 3, 5]), 'x': 3, 'inst2': A(x=3, y=4, l=[])}]>
 ```
 The `@` operator stores the results when a combination is found.
@@ -424,21 +434,21 @@
 ### Do we match something that has this shape?
 
 Let's try to see if this module contains classes, which means: does the `tree` variable have the shape of a Module that contains Classes in this body?
 Let's define the pattern to check that:
 
 ```python
 # Pattern example 1
-pattern = match(Module) % {  # we want a Module
+pattern = match(Module)[  # we want a Module
     'body': match(ClassDef)  # that contains a ClassDef in 'body'
-}
+]
 ```
 This pattern expresses that we want to match a `Module` using `match(Module)`, and in the `body` relation of this `Module`, must contain a `ClassDef`.
-To express the content of a class instance, we use the `%` operator follows by a dictionnary where the key is the name of the relation and the value is against what the value needs to be matched.
-The key is considered as a "path", we will see later what it means, while the value is a matcher.
+To express the content of a class instance, we use the collection acces notation where each index is a slice with the start of the slice that is the name of the relation and the value is against what the value needs to be matched (the stop of the slice).
+The key (start) is considered as a "path", we will see later what it means, while the value is a matcher.
 In this case, `body` will yield a collection of ast nodes for `Module`.
 Even if the path will resolve as a collection, as we use a simple matcher here, the semantic is equivalent to "contains".
 Consequently, we can read this as does `body` contains a `ClassDef`.
 
 Now that we have our matcher, we "execute it" against the `tree` object.
 
 ```python
@@ -458,17 +468,17 @@
 ### Deconstruct/extract information from a pattern
 
 Knowing if an object matches against a pattern is nice, but it's even better to be able to gather some data.
 To have more details about what was matched by the pattern, we will introduce variables/wildcards.
 
 ```python
 # Pattern example 2
-pattern = match(Module) % {  # we want a Module
-    'body': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    'body': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}]
 ```
@@ -476,17 +486,17 @@
 Obviously, we only have the classes that are directly under `body` in the module.
 If we want all the modules, whereever there are defined, we will use instead the children recursive path operator.
 
 NOTE: if you execute this code in IPython, it could be long, `parse(...)` seems to behave a little bit different in interactive environement.
 
 ```python
 # Pattern exmaple 3
-pattern = match(Module) % {  # we want a Module
-    '*': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    '*': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}, {'name': 'InnerCls'}]
 ```
@@ -497,28 +507,28 @@
 Now, we will go further by trying to match a module that contains classes that contains a `__init__` method and the `__init__` method should have assignment with the form `self.XXX = SOMETHING`.
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{'name': 'A', 'attr': 'x'},
 #  {'name': 'A', 'attr': 'y'},
 #  {'name': 'A', 'attr': 'z'},
@@ -531,30 +541,30 @@
 
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'args>*': match(arg) % { '*': '@attr'},  # among the args, there is one that a field equals to "attr"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'args>*': match(arg)['*': '@attr'],  # among the args, there is one that a field equals to "attr"
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
                 'value>id': "@attr",  # and the "id" of the "value" of the assignment as is equivalent to "attr"
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{"name": "A", "attr": "x"},
 #  {"name": "A", "attr": "y"},
 #  {"name": "B", "attr": "w"}]
@@ -587,16 +597,16 @@
 
 To overcome this "limitation" (it's not a limitation, but in our case, it can feel like it), we will define a class with all the patterns we want as class variable.
 
 ```python
 from iguala import as_matcher as m
 
 class Patterns(object):
-    case1 = match(A) % {"x": "@x"}
-    case2 = match(B) % {"y": 4}
+    case1 = match(A)[ "x": "@x" ]
+    case2 = match(B)[ "y": 4 ]
     case3 = m([1, "*value", 3, ...])  # we want that the list starts with 1, then there is a bunch of 3 inside at any position
 ```
 
 ### Integrating `iguala` patterns with Python `case` syntax
 
 Then, from here, we can pass them to the `case` syntax:
```

### Comparing `iguala-0.4.0/README.md` & `iguala-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,35 @@
 NOTE: in this document, the term `matcher` and `pattern` are used to refer to the same thing, but a matcher matches a single small entity while a pattern defines a composition of matchers (or a single matcher).
 
 ```python
 # we consider that "MyObject" is an already known type
 # and "instance" and instance of it with att1 = att2 = 4 and name = 'foo'
 from iguala import match, is_not
 
-pattern = match(MyObject) % {  # must be an instance of MyObject
+pattern = match(MyObject)[  # must be an instance of MyObject
     "att1": "@value",  # with att1 stored in "value"
     "att2": "@value",   # and att2 with the same value as the one from att1
     "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
-}
+]
+
 print(pattern.match(instance))
 # displays: <True: [{'value': 4, 'name': 'foo'}]>
 
 # An equivalent Python code would be:
 if type(instance) == MyObject and instance.att1 == instance.att2 and instance.name != "bar":
     value = instance.att1
     name = instance.name
+
+# As an alternative syntax, here is how you can write the same pattern
+# You can choose the one you prefer, there is pros and cons with both
+pattern = match(MyObject) % {  # must be an instance of MyObject
+    "att1": "@value",  # with att1 stored in "value"
+    "att2": "@value",   # and att2 with the same value as the one from att1
+    "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
+}
 ```
 
 ## Installation
 
 ```sh
 pip install iguala
 ```
@@ -98,22 +107,23 @@
 
 ### Matchers/pattern operators
 
 There is few pattern operators.
 
 * `match(...)` with a type as parameter matches exactly a type, e.g: `match(A) % {}` means, match an instance of `A` (but not subclasses).
 * `~` used in front of an object matcher expresses "and all its subclasses", e.g: `~match(object) % {}` means, match an instance of `object` or from its subclasses.
+* `matcher[...]` with slices as indexes which expresses the properties of an object, e.g: `match(A)['name': 'foo']` means, match an instance of `A` where the `name` equals `foo`.
 * `%` with a dictionnary on its right expresses the properties of an object, e.g: `match(A) % {'name': 'foo'}` means, match an instance of `A` where the `name` equals `foo`.
-* `@` stores a data into a dedicated name, e.g: `match(A) % {'name': 'foo'} @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
-* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A) % {'name': is_not('foo')}`, means match an instance of `A` where the `name` is not equal to `foo`,
-* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A) % {'name': regex('[A-Z].*')}`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
-    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A) % {'name': regex('[A-Z].*') >> 'match_result'}` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
-    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A) % {'name': regex('[A-Z].*', label='match_result')}`. Using the operator or not is a matter of taste, the effect is exactly the same.
-* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A) % {'x': range(0, 5)}` means, match an instance of `A` where `x` is in the range `[0..4]`.
-* `|` expresses a logical "or" between two patterns, e.g: `match(A) % {'name': is_not(m('foo') | 'bar')}`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
+* `@` stores a data into a dedicated name, e.g: `match(A)['name': 'foo'] @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
+* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A)['name': is_not('foo')]`, means match an instance of `A` where the `name` is not equal to `foo`,
+* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A)['name': regex('[A-Z].*')]`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
+    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A)['name': regex('[A-Z].*') >> 'match_result']` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
+    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A)['name': regex('[A-Z].*', label='match_result')]`. Using the operator or not is a matter of taste, the effect is exactly the same.
+* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A)['x': range(0, 5)]` means, match an instance of `A` where `x` is in the range `[0..4]`.
+* `|` expresses a logical "or" between two patterns, e.g: `match(A)['name': is_not(m('foo') | 'bar')]`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
 
 ### Collections patterns
 
 Here is a list of some examples of patterns that can be applied to collections:
 
 * `[]`, means empty collection
 * `[3]` means a collection with only one value: `3`
@@ -131,26 +141,26 @@
 * `is_not([..., '@x', ..., is_not('@x'), ...])` means a collection where there is no elements that are not the same (a collection where all elements are the same)
 
 ### Lambda based matchers
 
 Lambdas are used to express patterns over captured variables:
 
 * `lambda VAR1, VAR2, ....: SOMETHINGS WITHS VARS` is a matcher generator.
-Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A): {'x': '@x', 'y': lambda x: x + 1}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A)['x': '@x', 'y': lambda x: x + 1]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `cond(lambda ....)` is a condition matcher (needs to be imported `from iguala import cond`).
-Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A): {'x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A)['x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `__self__` is a meta-variable that can be passed as arguments of the matcher generator or conditional matcher. This variable resolves to the object currently matched.
 
 Matcher generators and conditional matchers also works with sequence matchers, negative matchers, range matcher, regex matcher...etc.
 Here is some examples:
 
 * `[..., '@x', lambda x: x + 1, ...]` means a collection where one element is followed by its successor.
 * `[..., '@x', is_not(lambda x: x + 1), ...]` means a collection where one element is not followed by its successor.
 * `is_not([..., '@x', is_not(lambda x: x + 1), ...])` means a collection where there is no element that is not followed by its successor (a collection that is sorted).
-* `match(A) % {'x': '@x', 'y': lambda x: range(0, x + 1)}` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
+* `match(A)['x': '@x', 'y': lambda x: range(0, x + 1)]` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
 
 
 NOTE: Argument names of the function used for the matcher generator or the conditional matcher have to match the name of variables defined in the pattern.
 If other names are used, `iguala` will ignore the matcher, but will generate a warning message stating what are the missing variables and their positions in the pattern.
 
 ## Walkthrough - Draw me a pattern on an Object
 
@@ -201,34 +211,34 @@
 # displays: <False - []>
 ```
 No suprises, `a1` and `a2` are instances of `A` while `b` is not.
 
 Let's now see if those objects are instances of `A` with an attribute `z` that equals 4, then if they own an attribute `x` equals to 4.
 
 ```python
-pattern = match(A) % { 'z': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'z': 4 ]  # is it an instance of A with 'z' == 4?
 
 print(pattern.match(a1))  # and a2, b
 # displays: <False - []>, they don't have 'z' properties
 
-pattern = match(A) % { 'x': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'x': 4 ]  # is it an instance of A with 'z' == 4?
 print(pattern.match(a1))
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{}]>
 ```
 
 Now, let's deconstruct to get the value of `x`.
 We will express in our pattern that the data should be an instance of `A` with an attribute `x` and that we want to store the value of `x` in a variable named `value`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <True - [{'value': 3}]>
 print(result.bindings[0]['value'])
 # displays: 3
 
@@ -240,101 +250,101 @@
 
 Each right side of the property dictionnary that starts with an `@` means that it's a variable.
 If the name is found again in the pattern, then, it means that the data needs to have the same value for those variable in those positions.
 
 Let's use that to check now if each data is an instance of `A` where `x` and `y` have the same value.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
     'y': '@value'  # with an attribute "y" with the same value as "x"
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{'value': 4}]>
 ```
 
 Let's check now if we have an instance of `A` with a `2` in the collection `l`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': 2  # does "l" contains a 2?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{}, {}]>, there is two 2 in "l", so two combination, this information is returned by the matcher
 
 print(pattern.match(a2))
 # displays: <True - [{}]>, here there is only one 2 in "l"
 ```
 
 Let's try more precise questions over the collection `l`:
 
 ```python
 #
 # Patterns over collections
 #
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [2]  # does "l" contains only a 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., 2]  # does the last element of "l" is 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value']  # does "l" has a last element?
-}
+]
 print(pattern.match(a1))
 # displays: <True: [{'value': 5}]>
 
 print(pattern.match(a2))
 # displays: <True: [{'value': 2}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', '@value', ...]  # does "l" has two times the same element that follow each other?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True: [{'value': 2}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', ..., '@value', ...]  # does "l" has at least two times the same element?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{'value': 2}, {'value': 3}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': ["*l1", '@value', "*l2", '@value', "*l3"]  # does "l" has at least two times the same element? and store the collections around
-}
+]
 
 print(pattern.match(a1))
 # input for l was: [1, 2, 2, 3, 4, 3, 5]
 # displays: <True - [
 #    {'l1': [1], 'value': 2, 'l2': [], 'l3': [3, 4, 3, 5]},
 #    {'l1': [1, 2, 2], 'value': 3, 'l2': [4], 'l3': [5]}
 # ]>
@@ -350,17 +360,17 @@
 a3 = A(x=3, y=4, l=[])
 col = [a1, a2, b, a3, b]
 
 # does the collection contains two instances of A that have the same value for x
 # and store the nodes in 'inst1' and 'inst2'
 matcher = as_matcher(
     [...,
-     match(A) % {'x': '@x'} @ 'inst1',
+     match(A)['x': '@x'] @ 'inst1',
      ...,
-     match(A) % {'x': '@x'} @ 'inst2',
+     match(A)['x': '@x'] @ 'inst2',
      ...]
 )
 
 print(matcher.match(col))
 # displays: <True - [{'inst1': A(x=3, y=4, l=[1, 2, 2, 3, 4, 3, 5]), 'x': 3, 'inst2': A(x=3, y=4, l=[])}]>
 ```
 The `@` operator stores the results when a combination is found.
@@ -401,21 +411,21 @@
 ### Do we match something that has this shape?
 
 Let's try to see if this module contains classes, which means: does the `tree` variable have the shape of a Module that contains Classes in this body?
 Let's define the pattern to check that:
 
 ```python
 # Pattern example 1
-pattern = match(Module) % {  # we want a Module
+pattern = match(Module)[  # we want a Module
     'body': match(ClassDef)  # that contains a ClassDef in 'body'
-}
+]
 ```
 This pattern expresses that we want to match a `Module` using `match(Module)`, and in the `body` relation of this `Module`, must contain a `ClassDef`.
-To express the content of a class instance, we use the `%` operator follows by a dictionnary where the key is the name of the relation and the value is against what the value needs to be matched.
-The key is considered as a "path", we will see later what it means, while the value is a matcher.
+To express the content of a class instance, we use the collection acces notation where each index is a slice with the start of the slice that is the name of the relation and the value is against what the value needs to be matched (the stop of the slice).
+The key (start) is considered as a "path", we will see later what it means, while the value is a matcher.
 In this case, `body` will yield a collection of ast nodes for `Module`.
 Even if the path will resolve as a collection, as we use a simple matcher here, the semantic is equivalent to "contains".
 Consequently, we can read this as does `body` contains a `ClassDef`.
 
 Now that we have our matcher, we "execute it" against the `tree` object.
 
 ```python
@@ -435,17 +445,17 @@
 ### Deconstruct/extract information from a pattern
 
 Knowing if an object matches against a pattern is nice, but it's even better to be able to gather some data.
 To have more details about what was matched by the pattern, we will introduce variables/wildcards.
 
 ```python
 # Pattern example 2
-pattern = match(Module) % {  # we want a Module
-    'body': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    'body': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}]
 ```
@@ -453,17 +463,17 @@
 Obviously, we only have the classes that are directly under `body` in the module.
 If we want all the modules, whereever there are defined, we will use instead the children recursive path operator.
 
 NOTE: if you execute this code in IPython, it could be long, `parse(...)` seems to behave a little bit different in interactive environement.
 
 ```python
 # Pattern exmaple 3
-pattern = match(Module) % {  # we want a Module
-    '*': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    '*': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}, {'name': 'InnerCls'}]
 ```
@@ -474,28 +484,28 @@
 Now, we will go further by trying to match a module that contains classes that contains a `__init__` method and the `__init__` method should have assignment with the form `self.XXX = SOMETHING`.
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{'name': 'A', 'attr': 'x'},
 #  {'name': 'A', 'attr': 'y'},
 #  {'name': 'A', 'attr': 'z'},
@@ -508,30 +518,30 @@
 
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'args>*': match(arg) % { '*': '@attr'},  # among the args, there is one that a field equals to "attr"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'args>*': match(arg)['*': '@attr'],  # among the args, there is one that a field equals to "attr"
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
                 'value>id': "@attr",  # and the "id" of the "value" of the assignment as is equivalent to "attr"
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{"name": "A", "attr": "x"},
 #  {"name": "A", "attr": "y"},
 #  {"name": "B", "attr": "w"}]
@@ -564,16 +574,16 @@
 
 To overcome this "limitation" (it's not a limitation, but in our case, it can feel like it), we will define a class with all the patterns we want as class variable.
 
 ```python
 from iguala import as_matcher as m
 
 class Patterns(object):
-    case1 = match(A) % {"x": "@x"}
-    case2 = match(B) % {"y": 4}
+    case1 = match(A)[ "x": "@x" ]
+    case2 = match(B)[ "y": 4 ]
     case3 = m([1, "*value", 3, ...])  # we want that the list starts with 1, then there is a bunch of 3 inside at any position
 ```
 
 ### Integrating `iguala` patterns with Python `case` syntax
 
 Then, from here, we can pass them to the `case` syntax:
```

### Comparing `iguala-0.4.0/iguala/helpers.py` & `iguala-0.5.0/iguala/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
         self.matcher = ObjectMatcher(cls)
         self.matcher.properties = {}
 
     def __mod__(self, properties):
         self.matcher.properties = properties
         return self.matcher
 
+    def __getitem__(self, keys):
+        self.matcher.properties = keys if isinstance(keys, tuple) else [keys]
+        return self.matcher
+
     def __matmul__(self, alias):
         from .matchers import SaveNodeMatcher
 
         return SaveNodeMatcher(alias, self.matcher)
 
     def __invert__(self):
         self.matcher.subclassmatch = True
```

### Comparing `iguala-0.4.0/iguala/matchers.py` & `iguala-0.5.0/iguala/matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import MutableMapping
+import itertools
 from re import compile
 from types import LambdaType
 
 from .helpers import flat
 from .paths import as_path
 
 
@@ -105,14 +106,17 @@
         result.add_contexts(contexts)
         result.analyse_contexts()
         return result
 
     def __or__(self, right):
         return OrMatcher(self, as_matcher(right))
 
+    def __ror__(self, left):
+        return OrMatcher(as_matcher(left), self)
+
     def save_as(self, alias):
         return SaveNodeMatcher(alias, self)
 
     def __matmul__(self, alias):
         return SaveNodeMatcher(alias, self)
 
     def __eq__(self, other):
@@ -193,25 +197,24 @@
 
 class OrMatcher(Matcher):
     def __init__(self, left, right):
         self.left = left
         self.right = right
 
     def match_context(self, obj, context):
-        contexts = self.left.match_context(obj, context)
-        if any(c.is_match for c in contexts):
-            return contexts
-        return self.right.match_context(obj, context)
+        left_contexts = self.left.match_context(obj, context.copy())
+        right_contexts = self.right.match_context(obj, context.copy())
+        return [c for c in left_contexts + right_contexts if c.is_match]
 
 
 class KeyValueMatcher(object):
     def match_context(self, obj, context):
         context.is_match = True
         new_contexts = [context]
-        for path, matcher in self.properties.items():
+        for path, matcher in self.properties:
             results = []
             for context in new_contexts:
                 if matcher.is_collection_matcher:
                     cpy = context.copy()
                     results.extend(matcher.match_context(path.resolve_from(obj), cpy))
                 else:
                     results.extend(
@@ -247,17 +250,20 @@
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, properties):
         if properties is None:
             self._properties = {}
+            return
+        elif isinstance(properties, dict):
+            props = [(as_path(k), as_matcher(v)) for k, v in properties.items()]
         else:
-            props = {as_path(k): as_matcher(v) for k, v in properties.items()}
-            self._properties = props
+            props = [(as_path(sl.start), as_matcher(sl.stop)) for sl in properties]
+        self._properties = props
 
 
 class DictMatcher(KeyValueMatcher, Matcher):
     def __init__(self, d):
         self.properties = {
             as_path(k, dictkey=True): as_matcher(v) for k, v in d.items()
         }
```

### Comparing `iguala-0.4.0/iguala/paths.py` & `iguala-0.5.0/iguala/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # from types import LambdaType
+from functools import lru_cache
 
 from .helpers import IdentitySet, flat
 
 
 class ObjectPath(object):
     def as_path(self):
         return self
```

### Comparing `iguala-0.4.0/iguala.egg-info/PKG-INFO` & `iguala-0.5.0/iguala.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.4.0
+Version: 0.5.0
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
@@ -54,26 +54,35 @@
 NOTE: in this document, the term `matcher` and `pattern` are used to refer to the same thing, but a matcher matches a single small entity while a pattern defines a composition of matchers (or a single matcher).
 
 ```python
 # we consider that "MyObject" is an already known type
 # and "instance" and instance of it with att1 = att2 = 4 and name = 'foo'
 from iguala import match, is_not
 
-pattern = match(MyObject) % {  # must be an instance of MyObject
+pattern = match(MyObject)[  # must be an instance of MyObject
     "att1": "@value",  # with att1 stored in "value"
     "att2": "@value",   # and att2 with the same value as the one from att1
     "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
-}
+]
+
 print(pattern.match(instance))
 # displays: <True: [{'value': 4, 'name': 'foo'}]>
 
 # An equivalent Python code would be:
 if type(instance) == MyObject and instance.att1 == instance.att2 and instance.name != "bar":
     value = instance.att1
     name = instance.name
+
+# As an alternative syntax, here is how you can write the same pattern
+# You can choose the one you prefer, there is pros and cons with both
+pattern = match(MyObject) % {  # must be an instance of MyObject
+    "att1": "@value",  # with att1 stored in "value"
+    "att2": "@value",   # and att2 with the same value as the one from att1
+    "name": is_not("bar") @ "name" # and name is not "bar", store the name in "name"
+}
 ```
 
 ## Installation
 
 ```sh
 pip install iguala
 ```
@@ -121,22 +130,23 @@
 
 ### Matchers/pattern operators
 
 There is few pattern operators.
 
 * `match(...)` with a type as parameter matches exactly a type, e.g: `match(A) % {}` means, match an instance of `A` (but not subclasses).
 * `~` used in front of an object matcher expresses "and all its subclasses", e.g: `~match(object) % {}` means, match an instance of `object` or from its subclasses.
+* `matcher[...]` with slices as indexes which expresses the properties of an object, e.g: `match(A)['name': 'foo']` means, match an instance of `A` where the `name` equals `foo`.
 * `%` with a dictionnary on its right expresses the properties of an object, e.g: `match(A) % {'name': 'foo'}` means, match an instance of `A` where the `name` equals `foo`.
-* `@` stores a data into a dedicated name, e.g: `match(A) % {'name': 'foo'} @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
-* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A) % {'name': is_not('foo')}`, means match an instance of `A` where the `name` is not equal to `foo`,
-* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A) % {'name': regex('[A-Z].*')}`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
-    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A) % {'name': regex('[A-Z].*') >> 'match_result'}` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
-    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A) % {'name': regex('[A-Z].*', label='match_result')}`. Using the operator or not is a matter of taste, the effect is exactly the same.
-* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A) % {'x': range(0, 5)}` means, match an instance of `A` where `x` is in the range `[0..4]`.
-* `|` expresses a logical "or" between two patterns, e.g: `match(A) % {'name': is_not(m('foo') | 'bar')}`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
+* `@` stores a data into a dedicated name, e.g: `match(A)['name': 'foo'] @ 'inst'` means, match an instance of `A` where the `name` equals `foo` and store the instance of `A` in `inst` for further usage.
+* `is_not(...)` expresses a negation (needs to be imported `from iguala import is_not`), e.g: `match(A)['name': is_not('foo')]`, means match an instance of `A` where the `name` is not equal to `foo`,
+* `regex(...)` expresses a regular expression matcher (needs to be imported `from iguala import regex`). The regex to match needs to be passed as a string, e.g: `match(A)['name': regex('[A-Z].*')]`, means match an instance of `A` where the `name` matches the regex `[A-Z].*`.
+    * This matcher supports an additional operator `>>` that is used to store the matching result for further usage. This mecomes really handy to get matched groups (especially if named match group are used), e.g: `match(A)['name': regex('[A-Z].*') >> 'match_result']` will store the "match" object obtained during the regex matching operation under the label `match_result`. This variable will be accessible as all variables, in the result procuded by `iguala`.
+    * The same behavior as describe above can be achieved without using the `>>` by passing an extra argument to `regex(...)`, e.g: `match(A)['name': regex('[A-Z].*', label='match_result')]`. Using the operator or not is a matter of taste, the effect is exactly the same.
+* `range(...)`, if you use the `range(...)` constructor (from builtins), a special "range matcher" is created, e.g: `match(A)['x': range(0, 5)]` means, match an instance of `A` where `x` is in the range `[0..4]`.
+* `|` expresses a logical "or" between two patterns, e.g: `match(A)['name': is_not(m('foo') | 'bar')]`, means match an instance of `A` where `name` is neither `foo` nor `bar`. In this example, `m` is a renaming of the `as_matcher` function made this way: `from iguala import as_matcher as m`.
 
 ### Collections patterns
 
 Here is a list of some examples of patterns that can be applied to collections:
 
 * `[]`, means empty collection
 * `[3]` means a collection with only one value: `3`
@@ -154,26 +164,26 @@
 * `is_not([..., '@x', ..., is_not('@x'), ...])` means a collection where there is no elements that are not the same (a collection where all elements are the same)
 
 ### Lambda based matchers
 
 Lambdas are used to express patterns over captured variables:
 
 * `lambda VAR1, VAR2, ....: SOMETHINGS WITHS VARS` is a matcher generator.
-Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A): {'x': '@x', 'y': lambda x: x + 1}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Matcher generators uses captured variable to generate new matchers that are executed when all necessary variables have been captured, e.g: `match(A)['x': '@x', 'y': lambda x: x + 1]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `cond(lambda ....)` is a condition matcher (needs to be imported `from iguala import cond`).
-Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A): {'x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)}` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
+Condition matchers uses captured variable to execute a function and use the result as matching result. Consequently, the return type of the function must be a boolean, e.g: `match(A)['x': '@x', 'y': cond(lambda x, __self__: x ==  __self__ + 1)]` means, match an instance of `A` that have an attribute `x` and an attribute `y` that is equals to `x + 1`.
 * `__self__` is a meta-variable that can be passed as arguments of the matcher generator or conditional matcher. This variable resolves to the object currently matched.
 
 Matcher generators and conditional matchers also works with sequence matchers, negative matchers, range matcher, regex matcher...etc.
 Here is some examples:
 
 * `[..., '@x', lambda x: x + 1, ...]` means a collection where one element is followed by its successor.
 * `[..., '@x', is_not(lambda x: x + 1), ...]` means a collection where one element is not followed by its successor.
 * `is_not([..., '@x', is_not(lambda x: x + 1), ...])` means a collection where there is no element that is not followed by its successor (a collection that is sorted).
-* `match(A) % {'x': '@x', 'y': lambda x: range(0, x + 1)}` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
+* `match(A)['x': '@x', 'y': lambda x: range(0, x + 1)]` means match an instance of `A` which has an `x` value and a `y` value contained in the `[0..x]` interval.
 
 
 NOTE: Argument names of the function used for the matcher generator or the conditional matcher have to match the name of variables defined in the pattern.
 If other names are used, `iguala` will ignore the matcher, but will generate a warning message stating what are the missing variables and their positions in the pattern.
 
 ## Walkthrough - Draw me a pattern on an Object
 
@@ -224,34 +234,34 @@
 # displays: <False - []>
 ```
 No suprises, `a1` and `a2` are instances of `A` while `b` is not.
 
 Let's now see if those objects are instances of `A` with an attribute `z` that equals 4, then if they own an attribute `x` equals to 4.
 
 ```python
-pattern = match(A) % { 'z': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'z': 4 ]  # is it an instance of A with 'z' == 4?
 
 print(pattern.match(a1))  # and a2, b
 # displays: <False - []>, they don't have 'z' properties
 
-pattern = match(A) % { 'x': 4 }  # is it an instance of A with 'z' == 4?
+pattern = match(A)[ 'x': 4 ]  # is it an instance of A with 'z' == 4?
 print(pattern.match(a1))
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{}]>
 ```
 
 Now, let's deconstruct to get the value of `x`.
 We will express in our pattern that the data should be an instance of `A` with an attribute `x` and that we want to store the value of `x` in a variable named `value`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <True - [{'value': 3}]>
 print(result.bindings[0]['value'])
 # displays: 3
 
@@ -263,101 +273,101 @@
 
 Each right side of the property dictionnary that starts with an `@` means that it's a variable.
 If the name is found again in the pattern, then, it means that the data needs to have the same value for those variable in those positions.
 
 Let's use that to check now if each data is an instance of `A` where `x` and `y` have the same value.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'x': '@value'  # with an attribute "x"? (stored in "value")
     'y': '@value'  # with an attribute "y" with the same value as "x"
-}
+]
 
 result = pattern.match(a1)
 print(result)
 # displays: <False - []>
 
 print(pattern.match(a2))
 # displays: <True - [{'value': 4}]>
 ```
 
 Let's check now if we have an instance of `A` with a `2` in the collection `l`.
 
 ```python
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': 2  # does "l" contains a 2?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{}, {}]>, there is two 2 in "l", so two combination, this information is returned by the matcher
 
 print(pattern.match(a2))
 # displays: <True - [{}]>, here there is only one 2 in "l"
 ```
 
 Let's try more precise questions over the collection `l`:
 
 ```python
 #
 # Patterns over collections
 #
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [2]  # does "l" contains only a 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., 2]  # does the last element of "l" is 2?
-}
+]
 print(pattern.match(a1))
 # displays: <False: []>
 
 print(pattern.match(a2))
 # displays: <True: [{}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value']  # does "l" has a last element?
-}
+]
 print(pattern.match(a1))
 # displays: <True: [{'value': 5}]>
 
 print(pattern.match(a2))
 # displays: <True: [{'value': 2}]>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', '@value', ...]  # does "l" has two times the same element that follow each other?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True: [{'value': 2}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': [..., '@value', ..., '@value', ...]  # does "l" has at least two times the same element?
-}
+]
 
 print(pattern.match(a1))
 # displays: <True - [{'value': 2}, {'value': 3}]>
 
 print(pattern.match(a2))
 # displays: <False: []>
 
-pattern = match(A) % {  # is it an instance of A?
+pattern = match(A)[  # is it an instance of A?
     'l': ["*l1", '@value', "*l2", '@value', "*l3"]  # does "l" has at least two times the same element? and store the collections around
-}
+]
 
 print(pattern.match(a1))
 # input for l was: [1, 2, 2, 3, 4, 3, 5]
 # displays: <True - [
 #    {'l1': [1], 'value': 2, 'l2': [], 'l3': [3, 4, 3, 5]},
 #    {'l1': [1, 2, 2], 'value': 3, 'l2': [4], 'l3': [5]}
 # ]>
@@ -373,17 +383,17 @@
 a3 = A(x=3, y=4, l=[])
 col = [a1, a2, b, a3, b]
 
 # does the collection contains two instances of A that have the same value for x
 # and store the nodes in 'inst1' and 'inst2'
 matcher = as_matcher(
     [...,
-     match(A) % {'x': '@x'} @ 'inst1',
+     match(A)['x': '@x'] @ 'inst1',
      ...,
-     match(A) % {'x': '@x'} @ 'inst2',
+     match(A)['x': '@x'] @ 'inst2',
      ...]
 )
 
 print(matcher.match(col))
 # displays: <True - [{'inst1': A(x=3, y=4, l=[1, 2, 2, 3, 4, 3, 5]), 'x': 3, 'inst2': A(x=3, y=4, l=[])}]>
 ```
 The `@` operator stores the results when a combination is found.
@@ -424,21 +434,21 @@
 ### Do we match something that has this shape?
 
 Let's try to see if this module contains classes, which means: does the `tree` variable have the shape of a Module that contains Classes in this body?
 Let's define the pattern to check that:
 
 ```python
 # Pattern example 1
-pattern = match(Module) % {  # we want a Module
+pattern = match(Module)[  # we want a Module
     'body': match(ClassDef)  # that contains a ClassDef in 'body'
-}
+]
 ```
 This pattern expresses that we want to match a `Module` using `match(Module)`, and in the `body` relation of this `Module`, must contain a `ClassDef`.
-To express the content of a class instance, we use the `%` operator follows by a dictionnary where the key is the name of the relation and the value is against what the value needs to be matched.
-The key is considered as a "path", we will see later what it means, while the value is a matcher.
+To express the content of a class instance, we use the collection acces notation where each index is a slice with the start of the slice that is the name of the relation and the value is against what the value needs to be matched (the stop of the slice).
+The key (start) is considered as a "path", we will see later what it means, while the value is a matcher.
 In this case, `body` will yield a collection of ast nodes for `Module`.
 Even if the path will resolve as a collection, as we use a simple matcher here, the semantic is equivalent to "contains".
 Consequently, we can read this as does `body` contains a `ClassDef`.
 
 Now that we have our matcher, we "execute it" against the `tree` object.
 
 ```python
@@ -458,17 +468,17 @@
 ### Deconstruct/extract information from a pattern
 
 Knowing if an object matches against a pattern is nice, but it's even better to be able to gather some data.
 To have more details about what was matched by the pattern, we will introduce variables/wildcards.
 
 ```python
 # Pattern example 2
-pattern = match(Module) % {  # we want a Module
-    'body': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    'body': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}]
 ```
@@ -476,17 +486,17 @@
 Obviously, we only have the classes that are directly under `body` in the module.
 If we want all the modules, whereever there are defined, we will use instead the children recursive path operator.
 
 NOTE: if you execute this code in IPython, it could be long, `parse(...)` seems to behave a little bit different in interactive environement.
 
 ```python
 # Pattern exmaple 3
-pattern = match(Module) % {  # we want a Module
-    '*': match(ClassDef) % {"name": "@name"} # that contains a ClassDef in 'body' and has a "name"
-}
+pattern = match(Module)[  # we want a Module
+    '*': match(ClassDef)["name": "@name"] # that contains a ClassDef in 'body' and has a "name"
+]
 
 # Let's match the "tree"
 result = pattern.match(tree)
 print(result.is_match)  # True
 print(result.bindings)
 # displays: [{'name': 'A'}, {'name': 'B'}, {'name': 'InnerCls'}]
 ```
@@ -497,28 +507,28 @@
 Now, we will go further by trying to match a module that contains classes that contains a `__init__` method and the `__init__` method should have assignment with the form `self.XXX = SOMETHING`.
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{'name': 'A', 'attr': 'x'},
 #  {'name': 'A', 'attr': 'y'},
 #  {'name': 'A', 'attr': 'z'},
@@ -531,30 +541,30 @@
 
 
 ```python
 from iguala import match
 
 # defines the pattern we want to look for
 # we want a Module
-pattern = match(Module) % {
+pattern = match(Module)[
     # that owns in all its children, recursively (i.e: somewhere, at any depth)
     # a ClassDef instance
-    '*': match(ClassDef) % {
+    '*': match(ClassDef)[
         'name': '@name',  # where name is equivalent to "name" (store the node)
-        'body': match(FunctionDef) % {  # that has a FunctionDef in body
+        'body': match(FunctionDef)[  # that has a FunctionDef in body
             'name': '__init__',  # that is named "__init__"
-            'args>*': match(arg) % { '*': '@attr'},  # among the args, there is one that a field equals to "attr"
-            'body>*': match(Assign) % {  # and that has an Assign in it's body, somewhere (at any depth)
+            'args>*': match(arg)['*': '@attr'],  # among the args, there is one that a field equals to "attr"
+            'body>*': match(Assign)[  # and that has an Assign in it's body, somewhere (at any depth)
                 'targets>value>id': 'self',  # where the target is "self"
                 'targets>attr': '@attr',  # where the attr is equivalent to "attr" (store the node)
                 'value>id': "@attr",  # and the "id" of the "value" of the assignment as is equivalent to "attr"
-            }
-        }
-    }
-}
+            ]
+        ]
+    ]
+]
 result = matcher.match(tree)  # Find all combinations
 print(result)
 print(result.is_match)  # displays True
 print(result.bindings)  # displays
 # [{"name": "A", "attr": "x"},
 #  {"name": "A", "attr": "y"},
 #  {"name": "B", "attr": "w"}]
@@ -587,16 +597,16 @@
 
 To overcome this "limitation" (it's not a limitation, but in our case, it can feel like it), we will define a class with all the patterns we want as class variable.
 
 ```python
 from iguala import as_matcher as m
 
 class Patterns(object):
-    case1 = match(A) % {"x": "@x"}
-    case2 = match(B) % {"y": 4}
+    case1 = match(A)[ "x": "@x" ]
+    case2 = match(B)[ "y": 4 ]
     case3 = m([1, "*value", 3, ...])  # we want that the list starts with 1, then there is a bunch of 3 inside at any position
 ```
 
 ### Integrating `iguala` patterns with Python `case` syntax
 
 Then, from here, we can pass them to the `case` syntax:
```

### Comparing `iguala-0.4.0/setup.py` & `iguala-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if version < (3, 7):
     sys.exit('Sorry, Python < 3.7 is not supported')
 
 packages = ['iguala']
 
 setup(
     name='iguala',
-    version='0.4.0',
+    version='0.5.0',
     description=("Non-linear pattern matching for Python's objects, or rexep-like for objects"),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='pattern matching matcher regexp graph query term rewriting',
     url='https://github.com/aranega/iguala',
     author='Vincent Aranega',
     author_email='vincent.aranega@gmail.com',
```

