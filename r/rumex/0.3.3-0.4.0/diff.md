# Comparing `tmp/rumex-0.3.3.tar.gz` & `tmp/rumex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumex-0.3.3.tar", max compression
+gzip compressed data, was "rumex-0.4.0.tar", max compression
```

## Comparing `rumex-0.3.3.tar` & `rumex-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.3.3/LICENSE
--rw-r--r--   0        0        0     4537 2023-04-04 21:27:51.312254 rumex-0.3.3/README.rst
--rw-r--r--   0        0        0      916 2023-04-23 21:55:25.650645 rumex-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/__init__.py
--rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.3.3/rumex/parsing/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/builder.py
--rw-r--r--   0        0        0      899 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/parsing/core.py
--rw-r--r--   0        0        0     7405 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/parser.py
--rw-r--r--   0        0        0      990 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/parsing/table.py
--rw-r--r--   0        0        0     2363 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/tokenizer.py
--rw-r--r--   0        0        0     9814 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/runner.py
--rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/tests/__init__.py
--rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/tests/test_data.py
--rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_error_reporting.py
--rw-r--r--   0        0        0     5554 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_no_execution_cases.py
--rw-r--r--   0        0        0     5022 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_simple_execution.py
--rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.3.3/rumex/utils.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 rumex-0.3.3/setup.py
--rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 rumex-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1520 2023-04-23 22:18:05.688768 rumex-0.4.0/README.rst
+-rw-r--r--   0        0        0      916 2023-04-29 00:59:13.547098 rumex-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-04-29 00:59:13.547098 rumex-0.4.0/rumex/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.4.0/rumex/parsing/__init__.py
+-rw-r--r--   0        0        0     3271 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/builder.py
+-rw-r--r--   0        0        0      947 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/core.py
+-rw-r--r--   0        0        0     8365 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/parser.py
+-rw-r--r--   0        0        0      990 2023-04-04 00:34:13.843051 rumex-0.4.0/rumex/parsing/table.py
+-rw-r--r--   0        0        0     2642 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/tokenizer.py
+-rw-r--r--   0        0        0    11047 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/runner.py
+-rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.4.0/rumex/tests/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.4.0/rumex/tests/test_data.py
+-rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.4.0/rumex/tests/test_error_reporting.py
+-rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.4.0/rumex/tests/test_no_execution_cases.py
+-rw-r--r--   0        0        0     6710 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/tests/test_simple_execution.py
+-rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.4.0/rumex/utils.py
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 rumex-0.4.0/PKG-INFO
```

### Comparing `rumex-0.3.3/LICENSE` & `rumex-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/pyproject.toml` & `rumex-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "rumex"
-version = "0.3.3"
+version = "0.4.0"
 
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 bandit = "^1.7.4"
-mypy = "^0.971"
+mypy = "^1.2.0"
 flake8 = "^5.0.4"
 pylint = "^2.15.0"
 toml = "^0.10.2"
 types-toml = "^0.10.8"
 twine = "^4.0.2"
```

### Comparing `rumex-0.3.3/rumex/parsing/builder.py` & `rumex-0.4.0/rumex/parsing/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import textwrap
 
-from .core import File, Scenario, Step
+from .core import ParsedFile, Scenario, Step
 from .table import parse_table_line
 
 
 class TableBuilder:
 
     def __init__(self):
         self._header = None
@@ -68,14 +68,15 @@
 
 class ScenarioBuilder:
 
     def __init__(self, name):
         self.name = name
         self._step_builders = []
         self.description = []
+        self.tags = []
 
     @property
     def current_step_builder(self):
         return self._step_builders[-1]
 
     def new_step(self, sentence):
         self._step_builders.append(StepBuilder(sentence))
@@ -87,38 +88,39 @@
         else:
             formatted_description = None
 
         return Scenario(
                 name=self.name,
                 description=formatted_description,
                 steps=[builder.get_built() for builder in self._step_builders],
+                tags=tuple(self.tags),
         )
 
 
 class FileBuilder:
 
     def __init__(self):
         self.name = None
         self.description = []
         self._scenario_builders = []
 
     @property
     def current_scenario_builder(self):
         return self._scenario_builders[-1]
 
-    def new_scenario(self, scenario_name):
-        self._scenario_builders.append(ScenarioBuilder(scenario_name))
+    def new_scenario(self, name=None):
+        self._scenario_builders.append(ScenarioBuilder(name))
 
     def get_built(self, *, uri):
         if self.description:
             formatted_description = textwrap.dedent(
                     '\n'.join(self.description)).strip()
         else:
             formatted_description = None
 
-        return File(
+        return ParsedFile(
             name=self.name,
             description=formatted_description,
             scenarios=[
                 builder.get_built() for builder in self._scenario_builders],
             uri=uri,
         )
```

### Comparing `rumex-0.3.3/rumex/parsing/core.py` & `rumex-0.4.0/rumex/parsing/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Protocol
+from typing import Protocol, Sequence
 
 
 @dataclass(frozen=True, kw_only=True)
 class InputFile:
     """Container for a test file to be parsed.
 
     Does not have to represent an actual file.
@@ -30,23 +30,24 @@
 
 
 @dataclass(frozen=True, kw_only=True)
 class Scenario:
 
     name: str
     description: str
-    steps: tuple[Step, ...]
+    steps: Sequence[Step]
+    tags: Sequence[str]
 
 
 @dataclass(frozen=True, kw_only=True)
-class File:
+class ParsedFile:
 
     name: str
     description: str
-    scenarios: list[Scenario]
+    scenarios: Sequence[Scenario]
     uri: str
 
 
 class ParserProto(Protocol):
 
-    def __call__(self, input_file: InputFile, /) -> File:
+    def __call__(self, input_file: InputFile, /) -> ParsedFile:
         """Build test files."""
```

### Comparing `rumex-0.3.3/rumex/parsing/table.py` & `rumex-0.4.0/rumex/parsing/table.py`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/rumex/parsing/tokenizer.py` & `rumex-0.4.0/rumex/parsing/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CannotTokenizeLine(Exception):
     pass
 
 
 class TokenKind(Enum):
+    """Basic identifiers for syntactic meaning of a (part of) line."""
 
     NAME_KW = auto()
     SCENARIO_KW = auto()
     STEP_KW = auto()
     BLANK_LINE = auto()
     DESCRIPTION = auto()
     TRIPLE_QUOTE = auto()
+    SCENARIO_TAG = auto()
 
 
 @dataclass(frozen=True, kw_only=True)
 class Token:
     """Every line must map to a `Token`."""
 
     kind: Hashable
@@ -33,14 +35,20 @@
 
 def match_keyword(keyword, *, line):
     if match_ := re.match(fr'^\s*{keyword}:\s*(.*)$', line):
         value, = match_.groups()
         return value
 
 
+def match_scenario_tag(line):
+    if match_ := re.match(r'^\s*@(\w+)\s*$', line):
+        tag, = match_.groups()
+        return TokenKind.SCENARIO_TAG, tag
+
+
 def match_scenario(line):
     if name := match_keyword('Scenario', line=line):
         return TokenKind.SCENARIO_KW, name
 
 
 def match_name(line):
     if name := match_keyword('Name', line=line):
@@ -82,17 +90,18 @@
         return self._fns[item]
 
     def __len__(self):
         return len(self._fns)
 
 
 default_tokenizers = Tokenizers(
+    match_triple_quote,
     match_name,
+    match_scenario_tag,
     match_scenario,
-    match_triple_quote,
     match_step,
     match_blank_line,
     match_description,
 )
 
 
 def iter_tokens(text, tokenizers=default_tokenizers):
```

### Comparing `rumex-0.3.3/rumex/runner.py` & `rumex-0.4.0/rumex/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from __future__ import annotations
-
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from typing import Any, Callable, Protocol, TypeAlias
 import inspect
 import re
 
-from .parsing.core import InputFile, File, ParserProto, Scenario
+from .parsing.core import InputFile, ParsedFile, ParserProto, Scenario
 from .parsing.parser import parse
 
 
-class HookAlreadyRegistered(Exception):
+class RumexException(Exception):
+    pass
+
+
+class HookAlreadyRegistered(RumexException):
+    pass
+
+
+class MatchingFunctionNotFound(RumexException):
     pass
 
 
 @dataclass(frozen=True, kw_only=True)
 class _ExecutedStep:
     sentence: str
 
@@ -38,25 +44,25 @@
 
 @dataclass(frozen=True, kw_only=True)
 class ExecutedScenario:
 
     name: str
     description: str
     steps: Sequence[ExecutedStep]
-
-    def __new__(cls, *, steps, **_):
-        if all(s.success for s in steps):
-            return super().__new__(PassedScenario)
-        return super().__new__(FailedScenario)
+    tags: Sequence[str]
 
 
 class PassedScenario(ExecutedScenario):
     success = True
 
 
+class SkippedScenario(PassedScenario):
+    pass
+
+
 class FailedScenario(ExecutedScenario):
     success = False
 
 
 @dataclass(frozen=True, kw_only=True)
 class ExecutedFile:
 
@@ -102,75 +108,144 @@
         # pylint: disable=comparison-with-callable
         if getattr(self, run_hook_name) is None:
             setattr(self, run_hook_name, _Hook(name=hook_name, fn=fn))
         else:
             raise HookAlreadyRegistered(hook_name)
 
 
+class ContextCallable(Protocol):
+
+    def __call__(self, context: Any) -> None:
+        ...
+
+
+class ExecutableStep:
+
+    def __init__(self, *, sentence: str, callable_: ContextCallable):
+        self.sentence = sentence
+        self._callable = callable_
+
+    def __call__(self, *, context: Any) -> None:
+        self._callable(context=context)
+
+
+@dataclass(frozen=True, kw_only=True)
+class MissingStep:
+
+    sentence: str
+
+
+class StepMapperProto(Protocol):
+
+    def iter_steps(
+            self,
+            scenario: Scenario,
+    ) -> Iterable[ExecutableStep | MissingStep]:
+        """Build callables representing steps of a scenario.
+
+        Each callable takes one argument `context`.
+
+        Params
+        ------
+        scenario: The scenario to which the step callables pertain.
+        """
+
+
 class ExecutorProto(Protocol):
 
     def __call__(
             self,
-            parsed: File,
+            parsed: ParsedFile,
             /,
             *,
             steps: StepMapperProto,
             context_maker: Callable[[], Any] | None,
     ) -> ExecutedFile:
         """Run the tests."""
 
 
 def execute_scenario(
         scenario,
         *,
-        context,
+        context_maker,
         steps,
+        skip_scenario_tag,
 ):
     executed_steps = []
-    failed = False
-    for executable_step in steps.iter_steps(scenario):
-        if failed:
-            executed = IgnoredStep(sentence=executable_step.sentence)
-        else:
-            try:
-                executable_step(context=context)
-            except Exception as exc:  # pylint: disable=broad-except
+    if skip_scenario_tag in scenario.tags:
+        cls = SkippedScenario
+    else:
+        failed = False
+        context = context_maker()
+        for step_ in steps.iter_steps(scenario):
+            if isinstance(step_, MissingStep):
                 failed = True
                 executed = FailedStep(
-                        exception=exc,
-                        sentence=executable_step.sentence,
+                    exception=MatchingFunctionNotFound(step_.sentence),
+                    sentence=step_.sentence,
                 )
+            elif failed:
+                executed = IgnoredStep(sentence=step_.sentence)
             else:
-                executed = PassedStep(sentence=executable_step.sentence)
-        executed_steps.append(executed)
+                try:
+                    step_(context=context)
+                except Exception as exc:  # pylint: disable=broad-except
+                    failed = True
+                    executed = FailedStep(
+                            exception=exc,
+                            sentence=step_.sentence,
+                    )
+                else:
+                    executed = PassedStep(sentence=step_.sentence)
+            executed_steps.append(executed)
+        cls = FailedScenario if failed else PassedScenario
 
-    return ExecutedScenario(
+    return cls(
             name=scenario.name,
             description=scenario.description,
             steps=tuple(executed_steps),
+            tags=scenario.tags,
     )
 
 
 def execute_file(
-        parsed_file: File,
+        parsed_file: ParsedFile,
         /,
         *,
         context_maker: Callable[[], Any] | None,
         steps: StepMapperProto,
+        skip_scenario_tag: str | None = None,
 ):
-    """Executed a single test file."""
+    """Executed a single test file.
+
+    Params
+    ------
+    parsed_file: File to be executed.
+
+    context_maker:
+        Callable returning context object
+        that will be passed to steps.
+
+    steps:
+        Step mapper that can generate executable steps
+        for all the steps defined in the `parsed_file`.
+
+    skip_scenario_tag:
+        If a scenario in the `parsed_file` contains
+        this tag, the scenario will not be executed.
+    """
 
     context_maker = context_maker or (lambda: None)
     executed_scenarios: list[ExecutedScenario] = []
     for scenario in parsed_file.scenarios:
-        context = context_maker()
         executed_scenario = execute_scenario(
                 scenario,
                 steps=steps,
-                context=context,
+                context_maker=context_maker,
+                skip_scenario_tag=skip_scenario_tag,
         )
         executed_scenarios.append(executed_scenario)
 
     return ExecutedFile(
             scenarios=tuple(executed_scenarios),
             uri=parsed_file.uri,
             name=parsed_file.name,
@@ -203,18 +278,18 @@
     steps: See `StepMapper` or `StepMapperProto` for more info.
 
     context_maker:
         A callable that returns an object that can be passed
         to step functions.
 
     parser:
-        A callable that takes `InputFile` and returns `File`.
+        A callable that takes `InputFile` and returns `ParsedFile`.
 
     executor:
-        A callable that takes `File`
+        A callable that takes `ParsedFile`
         `steps` and `context_maker` and returns `ExecutedFile`.
 
     reporter:
         A callable that takes the collection of all executed files.
         This can be as simple as raising an exception if any
         of the executed files is a `FailedFile`.
 
@@ -231,43 +306,14 @@
                     context_maker=context_maker,
             ),
             parsed_files,
     )
     return reporter(executed)
 
 
-class ContextCallable(Protocol):
-
-    def __call__(self, context: Any) -> None:
-        ...
-
-
-class ExecutableStep:
-
-    def __init__(self, *, sentence: str, callable_: ContextCallable):
-        self.sentence = sentence
-        self._callable = callable_
-
-    def __call__(self, *, context: Any) -> None:
-        self._callable(context=context)
-
-
-class StepMapperProto(Protocol):
-
-    def iter_steps(self, scenario: Scenario) -> Iterable[ExecutableStep]:
-        """Build callables representing steps of a scenario.
-
-        Each callable takes one argument `context`.
-
-        Params
-        ------
-        scenario: The scenario to which the step callables pertain.
-        """
-
-
 class StepMapper:
     """Prepare step functions."""
 
     def __init__(self):
         self._hooks = _Hooks()
         self._pattern_to_fn = {}
 
@@ -357,18 +403,24 @@
                 ]
                 return self._wrap_mapped_function(
                     fn_spec=spec,
                     fn=fn,
                     mapped_args=mapped_args,
                     data=step_.data,
                     )
-        raise Exception('TODO')
 
-    def iter_steps(self, scenario: Scenario) -> Iterable[ExecutableStep]:
+        return None
+
+    def iter_steps(
+            self,
+            scenario: Scenario,
+    ) -> Iterable[ExecutableStep | MissingStep]:
         """See documentation of `StepMapperProto`."""
         if (hook := self._hooks.run_before_scenario):
             yield ExecutableStep(sentence=hook.name, callable_=hook.fn)
         for step_ in scenario.steps:
             if (hook := self._hooks.run_before_step):
                 yield ExecutableStep(sentence=hook.name, callable_=hook.fn)
-            fn = self._prepare_step(step_)
-            yield ExecutableStep(sentence=step_.sentence, callable_=fn)
+            if (fn := self._prepare_step(step_)):
+                yield ExecutableStep(sentence=step_.sentence, callable_=fn)
+            else:
+                yield MissingStep(sentence=step_.sentence)
```

### Comparing `rumex-0.3.3/rumex/tests/__init__.py` & `rumex-0.4.0/rumex/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/rumex/tests/test_data.py` & `rumex-0.4.0/rumex/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/rumex/tests/test_error_reporting.py` & `rumex-0.4.0/rumex/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/rumex/tests/test_no_execution_cases.py` & `rumex-0.4.0/rumex/tests/test_no_execution_cases.py`

 * *Files identical despite different names*

### Comparing `rumex-0.3.3/rumex/tests/test_simple_execution.py` & `rumex-0.4.0/rumex/tests/test_simple_execution.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 import textwrap
 
 from rumex.parsing.parser import InputFile
+from rumex.runner import IgnoredStep, MatchingFunctionNotFound
 
 from .test_no_execution_cases import Reporter
 
 # pylint: disable=unbalanced-tuple-unpacking
 
 
 def test_scenario_is_failed_when_step_fails(run, get_step_mapper, **_):
@@ -207,7 +208,77 @@
     )
 
     executed_file, = reporter.reported
     assert executed_file.success
     scenario, = executed_file.scenarios
     assert scenario.success
     assert scenario.description == 'First a description, then a step.'
+
+
+def test_2_scenarios(run, get_step_mapper, **_):
+    text = textwrap.dedent('''
+        Name: Test file.
+
+        Scenario: My scenario.
+            Given something
+
+        Scenario: My 2nd scenario.
+            Given anything
+    ''')
+    uri = 'test_file'
+
+    steps = get_step_mapper()
+
+    @steps(r'thing')
+    def given_():
+        pass
+
+    reporter = Reporter()
+    run(
+        files=[InputFile(uri=uri, text=text)],
+        reporter=reporter,
+        steps=steps,
+    )
+
+    executed, = reporter.reported
+
+    scenario_1, scenario_2 = executed.scenarios
+    assert scenario_1.name == 'My scenario.'
+    assert scenario_2.name == 'My 2nd scenario.'
+
+
+def test_unimplemented_scenario(run, get_step_mapper, **_):
+    text = textwrap.dedent('''
+        Name: Test file.
+
+        Scenario: My scenario.
+            Given stuff
+            And anything
+            And more stuff
+            Then something
+    ''')
+    uri = 'test_file'
+
+    steps = get_step_mapper()
+
+    @steps(r'stuff')
+    def given_():
+        pass
+
+    reporter = Reporter()
+    run(
+        files=[InputFile(uri=uri, text=text)],
+        reporter=reporter,
+        steps=steps,
+    )
+
+    executed, = reporter.reported
+    scenario, = executed.scenarios
+    assert not scenario.success
+    passed, failed_1, ignored, failed_2 = scenario.steps
+    assert passed.success
+    assert not failed_1.success
+    assert isinstance(failed_1.exception, MatchingFunctionNotFound)
+    assert not ignored.success
+    assert isinstance(ignored, IgnoredStep)
+    assert not failed_2.success
+    assert isinstance(failed_2.exception, MatchingFunctionNotFound)
```

### Comparing `rumex-0.3.3/rumex/utils.py` & `rumex-0.4.0/rumex/utils.py`

 * *Files identical despite different names*

