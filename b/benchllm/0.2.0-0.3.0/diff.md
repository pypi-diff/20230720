# Comparing `tmp/benchllm-0.2.0.tar.gz` & `tmp/benchllm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchllm-0.2.0.tar", max compression
+gzip compressed data, was "benchllm-0.3.0.tar", max compression
```

## Comparing `benchllm-0.2.0.tar` & `benchllm-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1059 2023-07-13 15:45:09.119152 benchllm-0.2.0/LICENSE
--rw-r--r--   0        0        0     8869 2023-07-13 15:45:09.119152 benchllm-0.2.0/README.md
--rw-r--r--   0        0        0     1313 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/__init__.py
--rw-r--r--   0        0        0     3654 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cache.py
--rw-r--r--   0        0        0      285 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/__init__.py
--rw-r--r--   0        0        0      969 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/add_test.py
--rw-r--r--   0        0        0     1053 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/evaluate.py
--rw-r--r--   0        0        0     1283 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/list_tests.py
--rw-r--r--   0        0        0     1634 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/run_suite.py
--rw-r--r--   0        0        0      136 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/__init__.py
--rw-r--r--   0        0        0     1344 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/interactive.py
--rw-r--r--   0        0        0     1813 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/web.py
--rw-r--r--   0        0        0     5818 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/listener.py
--rw-r--r--   0        0        0     3790 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/main.py
--rw-r--r--   0        0        0     1502 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/utils.py
--rw-r--r--   0        0        0     1497 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/data_types.py
--rw-r--r--   0        0        0      198 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/__init__.py
--rw-r--r--   0        0        0     4502 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/evaluator.py
--rw-r--r--   0        0        0      671 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/semantic.py
--rw-r--r--   0        0        0     1013 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/evaluator/string_match.py
--rw-r--r--   0        0        0      276 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/input_types.py
--rw-r--r--   0        0        0     1086 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/listener.py
--rw-r--r--   0        0        0     1601 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/similarity.py
--rw-r--r--   0        0        0      743 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/singleton.py
--rw-r--r--   0        0        0     8813 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/tester.py
--rw-r--r--   0        0        0     2824 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/utils.py
--rw-r--r--   0        0        0     2065 2023-07-13 15:45:09.123152 benchllm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10173 1970-01-01 00:00:00.000000 benchllm-0.2.0/setup.py
--rw-r--r--   0        0        0     9883 1970-01-01 00:00:00.000000 benchllm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-20 12:55:50.762642 benchllm-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10070 2023-07-20 12:55:50.762642 benchllm-0.3.0/README.md
+-rw-r--r--   0        0        0     1398 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/__init__.py
+-rw-r--r--   0        0        0     3821 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cache.py
+-rw-r--r--   0        0        0      285 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/commands/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/commands/add_test.py
+-rw-r--r--   0        0        0     1053 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/commands/evaluate.py
+-rw-r--r--   0        0        0     1283 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/commands/list_tests.py
+-rw-r--r--   0        0        0     1634 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/commands/run_suite.py
+-rw-r--r--   0        0        0      136 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/evaluator/__init__.py
+-rw-r--r--   0        0        0     1653 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/evaluator/interactive.py
+-rw-r--r--   0        0        0     2089 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/evaluator/web.py
+-rw-r--r--   0        0        0     7483 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/listener.py
+-rw-r--r--   0        0        0     3790 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/main.py
+-rw-r--r--   0        0        0     1619 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/cli/utils.py
+-rw-r--r--   0        0        0     2241 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/data_types.py
+-rw-r--r--   0        0        0      340 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/evaluator/__init__.py
+-rw-r--r--   0        0        0     1471 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/evaluator/embedding.py
+-rw-r--r--   0        0        0     4679 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/evaluator/evaluator.py
+-rw-r--r--   0        0        0     1143 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/evaluator/semantic.py
+-rw-r--r--   0        0        0     1167 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/evaluator/string_match.py
+-rw-r--r--   0        0        0      276 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/input_types.py
+-rw-r--r--   0        0        0     1086 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/listener.py
+-rw-r--r--   0        0        0     1601 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/similarity.py
+-rw-r--r--   0        0        0      780 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/singleton.py
+-rw-r--r--   0        0        0    10746 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/tester.py
+-rw-r--r--   0        0        0     4474 2023-07-20 12:55:50.762642 benchllm-0.3.0/benchllm/utils.py
+-rw-r--r--   0        0        0     2065 2023-07-20 12:55:50.762642 benchllm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11392 1970-01-01 00:00:00.000000 benchllm-0.3.0/setup.py
+-rw-r--r--   0        0        0    11084 1970-01-01 00:00:00.000000 benchllm-0.3.0/PKG-INFO
```

### Comparing `benchllm-0.2.0/LICENSE` & `benchllm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/README.md` & `benchllm-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
 BenchLLM offers multiple evaluation methods to determine if the prediction matches the test case's expected values. You can use the `--evaluator` parameter to specify the evaluation method:
 
 There are multiple ways to evaluate if the test functions prediction matches the test cases expected values.
 By default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method
 
 - `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.
+- `embedding`, uses cosine distance between embedded vectors. Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.
 - `string-match`, checks if the strings are matching (case insensitive)
 - `interactive`, user manually accepts or fails tests in the terminal
 - `web`, uses pywebio fora simple local web interface
 
 The non interactive evaluators also supports `--workers N` to run in the evaluations in parallel
 
 ```bash
@@ -121,14 +122,29 @@
 - `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.
 - `none`, does not use any cache.
 
 ```bash
 $ bench run examples --cache memory
 ```
 
+When working on developing chains or training agent models, there may be instances where these models need to interact with external functions — for instance, querying a weather forecast or executing an SQL query. In such scenarios, BenchLLM facilitates the ability to mock these functions. This helps you make your tests more predictable and enables the discovery of unexpected function calls.
+
+```yml
+input: I live in London, can I expect rain today?
+expected: ["no"]
+calls:
+  - name: forecast.get_n_day_weather_forecast
+    returns: It's sunny in London.
+    arguments:
+      location: London
+      num_days: 1
+```
+
+In the example above, the function `get_n_day_weather_forecast` in the `forecast` module is mocked. In other words, every time this function is invoked, the model will receive `"It's sunny in London"`. BenchLLM also provides warnings if the function is invoked with argument values different from `get_n_day_weather_forecast(location=London, num_days=1)`. Please note, the provision of these argument parameters is optional.
+
 ### 🧮 Eval
 
 While _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
 
 ```bash
 $ bench run --no-eval
 ```
```

### Comparing `benchllm-0.2.0/benchllm/__init__.py` & `benchllm-0.3.0/benchllm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import inspect
 from pathlib import Path
 from typing import Callable, Type, TypeVar
 
 from .data_types import Evaluation, Prediction, Test  # noqa
-from .evaluator import Evaluator, SemanticEvaluator, StringMatchEvaluator  # noqa
+from .evaluator import (  # noqa
+    EmbeddingEvaluator,
+    Evaluator,
+    SemanticEvaluator,
+    StringMatchEvaluator,
+)
 from .input_types import ChatInput, SimilarityInput  # noqa
 from .similarity import semantically_similar  # noqa
 from .singleton import TestSingleton  # noqa
 from .tester import Tester  # noqa
 
 T = TypeVar("T")
 
@@ -16,20 +21,21 @@
     "Tester",
     "Prediction",
     "Test",
     "Evaluation",
     "StringMatchEvaluator",
     "SemanticEvaluator",
     "Evaluator",
+    "EmbeddingEvaluator",
 ]
 
 
-def test_wrapper(func: Callable[[T], str], type: Type[T], suite: Path) -> None:
+def test_wrapper(func: Callable[[T], str], input_type: Type[T], suite: Path) -> None:
     test_singleton = TestSingleton()
-    test_singleton.register(func, type=type, suite=suite)
+    test_singleton.register(func, input_type=input_type, suite=suite)
 
 
 def test(*, suite: str = ".") -> Callable[[Callable[[T], str]], None]:
     def test_decorator(func: Callable[[T], str]) -> None:
         suite_path = Path(suite)
         if not suite_path.is_absolute():
             suite_path = Path(inspect.getfile(func)).parent / suite
```

### Comparing `benchllm-0.2.0/benchllm/cache.py` & `benchllm-0.3.0/benchllm/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 import json
 from pathlib import Path
 from typing import Optional
 
+from pydantic import BaseModel
+
 from benchllm.data_types import Evaluation, Prediction
 from benchllm.evaluator import Evaluator
 from benchllm.input_types import Json
 from benchllm.listener import EvaluatorListener
 
 
+class MemoryValue(BaseModel):
+    passed: bool
+    score: float
+
+
 class MemoryCache(Evaluator):
     """Caches the results of the evaluator in memory"""
 
     def __init__(self, evaluator: Evaluator):
         super().__init__(workers=evaluator.workers)
         self._data: dict = {}
         self._evaluator = evaluator
         self._num_cache_misses = 0
         self._num_cache_hits = 0
 
     def _key(self, answer1: Json, answer2: Json) -> str:
         key1, key2 = json.dumps([answer1, answer2]), json.dumps([answer2, answer1])
         return key1 if key1 < key2 else key2
 
-    def lookup(self, answer1: Json, answer2: Json) -> Optional[bool]:
-        return self._data.get(self._key(answer1, answer2), None)
+    def lookup(self, answer1: Json, answer2: Json) -> Optional[MemoryValue]:
+        result = self._data.get(self._key(answer1, answer2), None)
+        if result:
+            return MemoryValue(**result)
+        return None
 
-    def store(self, answer1: Json, answer2: Json, value: bool) -> None:
+    def store(self, answer1: Json, answer2: Json, value: MemoryValue) -> None:
         key = self._key(answer1, answer2)
-        self._data[key] = value
+        self._data[key] = value.dict()
 
-    def evaluate_prediction(self, prediction: Prediction) -> Optional[Evaluator.Match]:
+    def evaluate_prediction(self, prediction: Prediction) -> list[Evaluator.Candidate]:
         uncached_expectations = []
+        candidates = []
         for expected in prediction.test.expected:
             lookup = self.lookup(expected, prediction.output)
             if lookup is None:
                 uncached_expectations.append(expected)
-            elif lookup:
-                # If we find a positive match we can stop comparing and just return.
-                # For negative matches we still need to check the other expected answers.
-                self._num_cache_hits += 1
-                return Evaluator.Match(prediction=prediction.output, expected=expected)
+            else:
+                candidates.append(Evaluator.Candidate(prediction=prediction.output, expected=expected, **lookup.dict()))
+
+        # If any of the cached candidates passed, we return them.
+        if any([candidate.passed for candidate in candidates]):
+            self._num_cache_hits += 1
+            return candidates
 
         # If all expectations were found in the cache but were negative matches,
         # we increment the cache hits counter and return None as there's no match.
         if not uncached_expectations:
             self._num_cache_hits += 1
-            return None
+            return candidates
 
         self._num_cache_misses += 1
         # set prediction.test.expected to only the ones that were not cached
         prediction = Prediction(**prediction.dict())
         prediction.test.expected = uncached_expectations
-        result = self._evaluator.evaluate_prediction(prediction)
-        if result:
-            self.store(result.expected, result.prediction, True)
-        else:
-            for expected in prediction.test.expected:
-                self.store(expected, prediction.output, False)
-        return result
+        candidates = self._evaluator.evaluate_prediction(prediction)
+        for candidate in candidates:
+            self.store(candidate.expected, candidate.prediction, MemoryValue(**candidate.dict()))
+        return candidates
 
     @property
     def num_cache_hits(self) -> int:
         return self._num_cache_hits
 
     @property
     def num_cache_misses(self) -> int:
```

### Comparing `benchllm-0.2.0/benchllm/cli/commands/add_test.py` & `benchllm-0.3.0/benchllm/cli/commands/add_test.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/cli/commands/evaluate.py` & `benchllm-0.3.0/benchllm/cli/commands/evaluate.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/cli/commands/list_tests.py` & `benchllm-0.3.0/benchllm/cli/commands/list_tests.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/cli/commands/run_suite.py` & `benchllm-0.3.0/benchllm/cli/commands/run_suite.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/cli/evaluator/interactive.py` & `benchllm-0.3.0/benchllm/cli/evaluator/interactive.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typer
 
 from benchllm.data_types import Prediction
 from benchllm.evaluator import Evaluator
 
 
 class InteractiveEvaluator(Evaluator):
-    def evaluate_prediction(self, prediction: Prediction) -> Optional[Evaluator.Match]:
+    def evaluate_prediction(self, prediction: Prediction) -> list[Evaluator.Candidate]:
         header = (
             f'{typer.style("Does ", bold=True)}'
             f"{typer.style(prediction.output, fg=typer.colors.BRIGHT_BLUE, bold=True)}"
             f'{typer.style(" match any of the following expected prompts?", bold=True)}'
         )
         typer.echo("")
         typer.echo(header)
@@ -23,9 +23,19 @@
 
         options = [str(idx) for idx, _ in enumerate(prediction.test.expected, start=1)] + ["n"]
 
         prompt_string = f"[{typer.style('matching number', fg=typer.colors.GREEN, bold=True)} or {typer.style('n', fg=typer.colors.RED, bold=True)}]"
         click_choice = click.Choice(options)
         response = typer.prompt(prompt_string, default="n", type=click_choice, show_choices=False).lower()
         if response == "n":
-            return None
-        return Evaluator.Match(prediction=prediction.output, expected=prediction.test.expected[int(response) - 1])
+            return [
+                Evaluator.Candidate(prediction=prediction.output, expected=expected, score=0.0, passed=False)
+                for expected in prediction.test.expected
+            ]
+        return [
+            Evaluator.Candidate(
+                prediction=prediction.output,
+                expected=prediction.test.expected[int(response) - 1],
+                score=1.0,
+                passed=True,
+            )
+        ]
```

### Comparing `benchllm-0.2.0/benchllm/cli/evaluator/web.py` & `benchllm-0.3.0/benchllm/cli/evaluator/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 f"The evaluation was interrupted. Run bench eval to start again", fg=typer.colors.RED, bold=True
             )
             # sys.exit doesn't work here, so we have to raise a signal to kill the process
             signal.raise_signal(signal.SIGINT)
 
         put_markdown("# BenchLLM Web Evaluator")
 
-    def evaluate_prediction(self, prediction: Prediction) -> Optional[Evaluator.Match]:
+    def evaluate_prediction(self, prediction: Prediction) -> list[Evaluator.Candidate]:
         test_name = prediction.test.file_path or prediction.test.id
 
         put_markdown(f"## {test_name}")
         put_markdown(f"*Question*: `{prediction.test.input}`")
         put_markdown(f"*Prediction*: `{prediction.output}`")
 
         table = [["Question:", f"{prediction.test.input}", ""], ["Prediction:", prediction.output], ""]
@@ -38,10 +38,17 @@
         options: list[dict[str, Optional[int | str]]] = [
             {"label": expected, "value": idx} for idx, expected in enumerate(prediction.test.expected)
         ]
         options.append({"label": "None", "value": None, "selected": True})
         answer = radio("Pick the matching answer", options=options, required=True)
 
         if answer and isinstance(answer, int):
-            return Evaluator.Match(prediction=prediction.output, expected=prediction.test.expected[answer])
+            return [
+                Evaluator.Candidate(
+                    prediction=prediction.output, expected=prediction.test.expected[answer], score=1.0, passed=True
+                )
+            ]
         else:
-            return None
+            return [
+                Evaluator.Candidate(prediction=prediction.output, expected=expected, score=0.0, passed=False)
+                for expected in prediction.test.expected
+            ]
```

### Comparing `benchllm-0.2.0/benchllm/cli/listener.py` & `benchllm-0.3.0/benchllm/cli/listener.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,17 +6,25 @@
 import typer
 from rich import print
 from rich.console import Console
 from rich.markup import render
 from rich.table import Table
 
 from benchllm.cache import MemoryCache
-from benchllm.data_types import Evaluation, FunctionID, Prediction, Test, TestFunction
+from benchllm.data_types import (
+    CallErrorType,
+    Evaluation,
+    FunctionID,
+    Prediction,
+    Test,
+    TestFunction,
+)
 from benchllm.evaluator import Evaluator
 from benchllm.listener import EvaluatorListener, TesterListener
+from benchllm.utils import collect_call_errors
 
 
 class ReportListener(TesterListener, EvaluatorListener):
     def __init__(self, *, output_dir: Path) -> None:
         super().__init__()
         self.output_dir = output_dir
 
@@ -103,26 +111,58 @@
             return
 
         if evaluation.passed:
             typer.secho(".", fg=typer.colors.GREEN, bold=True, nl=False)
         else:
             typer.secho("F", fg=typer.colors.RED, bold=True, nl=False)
 
+    def handle_call_error(self, evaluations) -> None:
+        predictions_with_calls = [
+            evaluation.prediction for evaluation in evaluations if evaluation.prediction.test.calls
+        ]
+        if not predictions_with_calls:
+            return
+
+        print_centered(" Call Warnings ")
+
+        for prediction in predictions_with_calls:
+            errors = collect_call_errors(prediction)
+            if not errors:
+                continue
+            relative_path = prediction.function_id.relative_str(self.root_dir)
+            print_centered(f" [yellow]{relative_path}[/yellow] :: [yellow]{prediction.test.file_path}[/yellow] ", "-")
+
+            for error in errors:
+                if error.error_type == CallErrorType.MISSING_ARGUMENT:
+                    print(
+                        f'[blue][bold]{error.function_name}[/bold][/blue] was never called with [blue][bold]"{error.argument_name}"[/bold][/blue]'
+                    )
+                elif error.error_type == CallErrorType.MISSING_FUNCTION:
+                    print(f"[blue][bold]{error.function_name}[/bold][/blue] was never declared")
+                elif error.error_type == CallErrorType.VALUE_MISMATCH:
+                    print(
+                        f'[blue][bold]{error.function_name}[/bold][/blue] was called with "{error.argument_name}=[red][bold]{error.actual_value}[/bold][/red]", expected "[green][bold]{error.expected_value}[/bold][/green]"'
+                    )
+
     def evaluate_ended(self, evaluations: list[Evaluation]) -> None:
+        self.handle_call_error(evaluations)
+
         failed = [evaluation for evaluation in evaluations if not evaluation.passed]
         total_test_time = (
             0.0 if self._eval_only else sum(evaluation.prediction.time_elapsed for evaluation in evaluations) or 0.0
         )
         total_eval_time = sum(evaluation.eval_time_elapsed for evaluation in evaluations) or 0.0
         if failed:
             print_centered(" Failures ")
             for failure in failed:
                 prediction = failure.prediction
                 relative_path = prediction.function_id.relative_str(self.root_dir)
-                print_centered(f" [red]{relative_path}[/red] :: [red]{prediction.test.file_path}[/red] ", "-")
+                print_centered(
+                    f" [red]{relative_path}[/red] :: [red]{prediction.test.file_path} ({failure.score:.2f})[/red] ", "-"
+                )
 
                 console = Console()
 
                 table = Table(show_header=False, show_lines=True)
                 table.add_row(f"Input", str(prediction.test.input))
                 table.add_row(f"Output", f"[red]{prediction.output}[/red]")
                 for i, answer in enumerate(prediction.test.expected):
```

### Comparing `benchllm-0.2.0/benchllm/cli/main.py` & `benchllm-0.3.0/benchllm/cli/main.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/cli/utils.py` & `benchllm-0.3.0/benchllm/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 from pathlib import Path
 
 from benchllm.cache import FileCache, MemoryCache
 from benchllm.cli.evaluator import InteractiveEvaluator, WebEvaluator
-from benchllm.evaluator import Evaluator, SemanticEvaluator, StringMatchEvaluator
+from benchllm.evaluator import (
+    EmbeddingEvaluator,
+    Evaluator,
+    SemanticEvaluator,
+    StringMatchEvaluator,
+)
 
 
 def output_dir_factory() -> Path:
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
     output_dir = Path.cwd() / "output" / str(timestamp)
     output_dir.mkdir(exist_ok=True, parents=True)
 
@@ -23,14 +28,16 @@
         return SemanticEvaluator(model=model, workers=workers)
     elif evaluator_name == "interactive":
         return InteractiveEvaluator()
     elif evaluator_name == "string-match":
         return StringMatchEvaluator(workers=workers)
     elif evaluator_name == "web":
         return WebEvaluator()
+    elif evaluator_name == "embedding":
+        return EmbeddingEvaluator()
     else:
         raise ValueError(f"Unknown evaluator {evaluator_name}")
 
 
 def add_cache(cache_name: str, evaluator: Evaluator, cache_path: Path) -> Evaluator:
     if cache_name == "file":
         return FileCache(evaluator, cache_path)
```

### Comparing `benchllm-0.2.0/benchllm/data_types.py` & `benchllm-0.3.0/benchllm/data_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,85 @@
+from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Generic, Optional, TypeVar
 from uuid import uuid4
 
 from pydantic import BaseModel, Field
 
 
+class TestCall(BaseModel):
+    __test__ = False
+    name: str
+    arguments: dict[str, Any]
+    returns: Any
+
+
 class Test(BaseModel):
     __test__ = False
     id: str = Field(default_factory=lambda: str(uuid4()))
     input: Any
     expected: list[str]
     file_path: Optional[Path] = None
+    calls: Optional[list[TestCall]] = None
 
 
 class FunctionID(BaseModel):
     module_path: Path
     line_number: int
+    name: str
 
     def __hash__(self) -> int:
         return hash((self.module_path, self.line_number))
 
     def __str__(self) -> str:
-        return f"{self.module_path}:{self.line_number}"
+        return f"{self.module_path}:{self.line_number} ({self.name})"
 
     def relative_str(self, root_dir: Path) -> str:
         try:
-            return str(FunctionID(module_path=self.module_path.relative_to(root_dir), line_number=self.line_number))
+            return str(
+                FunctionID(
+                    module_path=self.module_path.relative_to(root_dir), line_number=self.line_number, name=self.name
+                )
+            )
         except ValueError:
             # we can't be sure that the module_path loaded from json files is relative to the root_dir
-            return str(FunctionID(module_path=self.module_path, line_number=self.line_number))
+            return str(FunctionID(module_path=self.module_path, line_number=self.line_number, name=self.name))
 
     @staticmethod
     def default() -> "FunctionID":
-        return FunctionID(module_path=Path(""), line_number=0)
+        return FunctionID(module_path=Path(""), line_number=0, name="default")
 
 
 class Prediction(BaseModel):
     test: Test
     output: str
     time_elapsed: float
     function_id: FunctionID
+    calls: dict[str, list[dict[str, Any]]] = {}
+
+
+class CallErrorType(str, Enum):
+    MISSING_FUNCTION = "Missing function"
+    MISSING_ARGUMENT = "Missing argument"
+    VALUE_MISMATCH = "Value mismatch"
+
+
+class CallError(BaseModel):
+    function_name: str
+    argument_name: Optional[str] = None
+    expected_value: Optional[Any] = None
+    actual_value: Optional[Any] = None
+    error_type: CallErrorType
 
 
 class Evaluation(BaseModel):
     prediction: Prediction
     passed: bool
     eval_time_elapsed: float
+    score: float
 
 
 T = TypeVar("T")
 
 
 class TestFunction(BaseModel, Generic[T]):
     function: Callable[[T], Any]
```

### Comparing `benchllm-0.2.0/benchllm/evaluator/evaluator.py` & `benchllm-0.3.0/benchllm/evaluator/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 class Evaluator(ABC):
     def __init__(self, workers: int = 1):
         self._predictions: list[Prediction] = []
         self._listeners: list[EvaluatorListener] = []
         self._evaluations: list[Evaluation] = []
         self._workers: int = workers
 
-    class Match(BaseModel):
+    class Candidate(BaseModel):
         prediction: Json
         expected: Json
+        score: float
+        passed: bool
 
     def add_listener(self, listener: EvaluatorListener) -> None:
         self._listeners.append(listener)
 
     def load(self, predictions: list[Prediction]) -> None:
         self._predictions.extend(predictions)
 
@@ -54,18 +56,22 @@
                 self._broadcast_evaluate_module_ended()
             self._broadcast_evaluate_ended(self._evaluations)
         return self._evaluations
 
     def _run_evaluation(self, prediction: Prediction) -> Evaluation:
         self._broadcast_evaluate_prediction_started(prediction)
         start = timer()
-        match = self.evaluate_prediction(prediction)
+        candidates = self.evaluate_prediction(prediction)
         end = timer()
+
         evaluation = Evaluation(
-            prediction=prediction, passed=isinstance(match, Evaluator.Match), eval_time_elapsed=end - start
+            prediction=prediction,
+            passed=any([candidate.passed for candidate in candidates]),
+            eval_time_elapsed=end - start,
+            score=max([candidate.score for candidate in candidates], default=0.0),
         )
         self._broadcast_evaluate_prediction_ended(evaluation)
         return evaluation
 
     @property
     def passed(self) -> list[Evaluation]:
         return [evaluation for evaluation in self._evaluations if evaluation.passed]
@@ -83,15 +89,15 @@
         return self._workers
 
     @property
     def predictions(self) -> list[Prediction]:
         return self._predictions
 
     @abstractmethod
-    def evaluate_prediction(self, prediction: Prediction) -> Optional[Match]:
+    def evaluate_prediction(self, prediction: Prediction) -> list[Candidate]:
         """Evaluate a single prediction, return a Match if the prediction matches the expected output."""
         pass
 
     def max_threads(self) -> int:
         return 1
 
     def _broadcast_evaluate_started(self) -> None:
```

### Comparing `benchllm-0.2.0/benchllm/evaluator/string_match.py` & `benchllm-0.3.0/benchllm/evaluator/semantic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-import json
 from typing import Optional
 
 from benchllm.data_types import Prediction
 from benchllm.evaluator import Evaluator
+from benchllm.similarity import semantically_similar
 
 
-class StringMatchEvaluator(Evaluator):
-    def __init__(self, *, case_sensitive: bool = False, fuzzy: bool = False, workers: int = 1):
+class SemanticEvaluator(Evaluator):
+    def __init__(self, *, model: str = "gpt-3", workers: int = 1, early_quitting: bool = True):
         super().__init__(workers=workers)
+        self.model = model
+        self.early_quitting = early_quitting
 
-        self._case_sensitive = case_sensitive
-        self._fuzzy = fuzzy
-
-    def match_strings(self, expected: str, output: str) -> bool:
-        if not self._case_sensitive:
-            expected = expected.lower()
-            output = output.lower()
-
-        if self._fuzzy:
-            return expected in output or output in expected
-
-        return expected == output
-
-    def evaluate_prediction(self, prediction: Prediction) -> Optional[Evaluator.Match]:
-        output = prediction.output
+    def evaluate_prediction(self, prediction: Prediction) -> list[Evaluator.Candidate]:
+        candidates = []
         for expected in prediction.test.expected:
-            if self.match_strings(expected, output):
-                return Evaluator.Match(prediction=prediction.output, expected=expected)
-        return None
+            if semantically_similar(expected, prediction.output, model=self.model):
+                candidate = Evaluator.Candidate(prediction=prediction.output, expected=expected, score=1.0, passed=True)
+                if self.early_quitting:
+                    return [candidate]
+                else:
+                    candidates.append(candidate)
+            else:
+                candidates.append(
+                    Evaluator.Candidate(prediction=prediction.output, expected=expected, score=0.0, passed=False)
+                )
+        return candidates
```

### Comparing `benchllm-0.2.0/benchllm/listener.py` & `benchllm-0.3.0/benchllm/listener.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/similarity.py` & `benchllm-0.3.0/benchllm/similarity.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.2.0/benchllm/tester.py` & `benchllm-0.3.0/benchllm/tester.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import importlib.util
 import inspect
 import json
+import sys
 import uuid
+from contextlib import contextmanager
 from pathlib import Path
 from timeit import default_timer as timer
 from types import ModuleType
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Iterator, Optional, Union
 
 import yaml
 from pydantic import ValidationError, parse_obj_as
 
 from .data_types import FunctionID, Prediction, Test, TestFunction
 from .listener import TesterListener
 from .singleton import TestSingleton
@@ -56,29 +58,33 @@
     def load_module(self, path: Union[str, Path]) -> None:
         path = Path(path)
         test_singleton = TestSingleton()
         test_singleton.clear()
 
         import_module_from_file(path)
 
-        if not test_singleton.func or not test_singleton.type or not test_singleton.suite:
+        if not test_singleton.functions:
             raise NoBenchLLMTestFunction()
 
-        function_id = FunctionID(module_path=path, line_number=inspect.getsourcelines(test_singleton.func)[1])
-
-        self.add_test_function(
-            TestFunction(
-                function=test_singleton.func,
-                function_id=function_id,
-                input_type=test_singleton.type,
-                suite=test_singleton.suite,
+        for function in test_singleton.functions:
+            function_id = FunctionID(
+                module_path=path,
+                line_number=inspect.getsourcelines(function.func)[1],
+                name=function.func.__name__,
             )
-        )
 
-        self.load_tests(test_singleton.suite, function_id)
+            self.add_test_function(
+                TestFunction(
+                    function=function.func,
+                    function_id=function_id,
+                    input_type=function.type,
+                    suite=function.suite,
+                )
+            )
+            self.load_tests(function.suite, function_id)
 
     def run(self) -> list[Prediction]:
         """Runs each test through the test function and stores the result"""
 
         self._broadcast_test_run_started()
 
         if not self._test_functions:
@@ -103,18 +109,27 @@
                         input = parse_obj_as(test_function.input_type, test.input)
                     except ValidationError:
                         self._broadcast_test_skipped(test, error=True)
                         continue
 
                     self._broadcast_test_started(test)
                     start = timer()
-                    output = test_function.function(input)
+
+                    # set up mock functions for the test calls
+                    calls_made: dict[str, Any] = {}
+                    with setup_mocks(test, calls_made):
+                        output = test_function.function(input)
+
                     end = timer()
                     prediction = Prediction(
-                        test=test, output=output, time_elapsed=end - start, function_id=test_function.function_id
+                        test=test,
+                        output=output,
+                        time_elapsed=end - start,
+                        function_id=test_function.function_id,
+                        calls=calls_made,
                     )
                     self._predictions.append(prediction)
                     self._broadcast_test_ended(prediction)
             self._broadcast_test_function_ended()
         self._broadcast_test_run_ended(self._predictions)
         return self._predictions
 
@@ -218,12 +233,51 @@
 
     # Create a new module based on the spec.
     module = importlib.util.module_from_spec(spec)
 
     if not module:
         raise Exception(f"Failed to load module from {file_path}")
 
+    # Temporarly add the directory of the file to the system path so that the module can import other modules.
+    file_module = file_path.resolve().parent
+    old_sys_path = sys.path.copy()
+    sys.path.append(str(file_module))
+
     # Execute the module.
     spec.loader.exec_module(module)
 
+    # Restore the system path
+    sys.path = old_sys_path
+
     # Return the module.
     return module
+
+
+@contextmanager
+def setup_mocks(test: Test, calls_made: dict[str, Any]) -> Iterator[None]:
+    """Sets up mock functions for the test calls"""
+    old_functions = []
+    for call in test.calls or []:
+        mock_name = call.name
+        module_name, function_name = mock_name.rsplit(".", 1)
+        # we need to import the module before we can mock the function
+        module = importlib.import_module(module_name)
+        old_functions.append((module, function_name, getattr(module, function_name)))
+
+        def mock_function(*args: tuple, **kwargs: dict[str, Any]) -> Any:
+            assert not args, "Positional arguments are not supported"
+            if mock_name not in calls_made:
+                calls_made[mock_name] = []
+            calls_made[mock_name].append(kwargs)
+            return call.returns
+
+        try:
+            setattr(module, function_name, mock_function)
+        except AttributeError:
+            print(f"Function {function_name} doesn't exist in module {module_name}")
+
+    try:
+        yield
+    finally:
+        # restore the old function
+        for old_function in old_functions:
+            setattr(old_function[0], old_function[1], old_function[2])
```

### Comparing `benchllm-0.2.0/pyproject.toml` & `benchllm-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "benchllm"
-version = "0.2.0"
+version = "0.3.0"
 description = "Tool for testing LLMs"
 homepage = "https://github.com/v7labs/benchllm"
 authors = [ "Simon Edwardsson <simon@v7labs.com>", "Andrea Azzini <andrea@v7labs.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = []
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License",]
```

### Comparing `benchllm-0.2.0/setup.py` & `benchllm-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'test': ['pytest']}
 
 entry_points = \
 {'console_scripts': ['bench = benchllm.cli.main:main']}
 
 setup_kwargs = {
     'name': 'benchllm',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Tool for testing LLMs',
-    'long_description': '# 🏋️\u200d♂️ BenchLLM 🏋️\u200d♀️\n\n🦾 Continuous Integration for LLM powered applications 🦙🦅🤖\n\n[![GitHub Repo stars](https://img.shields.io/github/stars/v7labs/BenchLLM?style=social)](https://github.com/v7labs/BenchLLM/stargazers)\n[![Twitter Follow](https://img.shields.io/twitter/follow/V7Labs?style=social)](https://twitter.com/V7Labs)\n[![Discord Follow](https://dcbadge.vercel.app/api/server/x7ExfHb3bG?style=flat)](https://discord.gg/x7ExfHb3bG)\n\n[**BenchLLM**](https://benchllm.com/) is a Python-based open-source library that streamlines the testing of Large Language Models (LLMs) and AI-powered applications. It measures the accuracy of your model, agents, or chains by validating responses on any number of tests via LLMs.\n\nBenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and is now Open Sourced under MIT License to share with the wider community\n\n## 💡 Get help on [Discord](https://discord.gg/x7ExfHb3bG) or [Tweet at us](https://twitter.com/V7Labs)\n\n<hr/>\n\nUse BenchLLM to:\n\n- Test the responses of your LLM across any number of prompts.\n- Continuous integration for chains like [Langchain](https://github.com/hwchase17/langchain), agents like [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT), or LLM models like [Llama](https://github.com/facebookresearch/llama) or GPT-4.\n- Eliminate flaky chains and create confidence in your code.\n- Spot inaccurate responses and hallucinations in your application at every version.\n\n<hr/>\n\n> ⚠️ **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.\n>\n> For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.\n\n## 🧪 BenchLLM Testing Methodology\n\nBenchLLM implements a distinct two-step methodology for validating your machine learning models:\n\n1. **Testing**: This stage involves running your code against any number of expected responses and capturing the predictions produced by your model without immediate judgment or comparison.\n\n2. **Evaluation**: The recorded predictions are compared against the expected output using LLMs to verify factual similarity (or optionally manually). Detailed comparison reports, including pass/fail status and other metrics, are generated.\n\nThis methodical separation offers a comprehensive view of your model\'s performance and allows for better control and refinement of each step.\n\n## 🚀 Install\n\nTo install BenchLLM we use pip\n\n```\npip install benchllm\n```\n\n## 💻 Usage\n\nStart by importing the library and use the @benchllm.test decorator to mark the function you\'d like to test:\n\n```python\nimport benchllm\n\n# Your custom model implementation\ndef run_my_model(input):\n    # Your model\'s logic goes here.\n    return some_result\n\n@benchllm.test(suite="/path/to/test/suite") # If the tests are in the same directory, just use @benchllm.test.\ndef invoke_model(input: str):\n    return run_my_model(input)\n```\n\nNext, prepare your tests. These are YAML/JSON files structured as follows:\n\n```yml\ninput: What\'s 1+1? Be very terse, only numeric output\nexpected:\n  - 2\n  - 2.0\n```\n\nIn the above example, the `input` is the query or instruction that your model will process, and `expected` contains the potential responses that your model should return. It\'s important to note that `input` can be a simple `str` or a more complex nested dictionary; BenchLLM will extract the type of the `input` argument in the Python code and load the `input` field from the YAML file accordingly.\n\nBy default, BenchLLM uses OpenAI\'s GPT-3 model for the `semantic` evaluator. This requires setting the `OPENAI_API_KEY` environment variable. If you do not want to use this default evaluator, you can specify an alternative one (discussed in further detail below):\n\n```bash\nexport OPENAI_API_KEY=\'your-api-key\'\n```\n\nReplace \'your-api-key\' with your actual OpenAI API key.\n\nTo initiate testing, use the `bench run` command:\n\n```bash\n$ bench run\n```\n\nBy default, the bench run command looks for Python files implementing the @test decorator in the current directory. To target a specific file or folder, specify it directly:\n\n```bash\n$ bench run path/to/my/file.py or/path/to/folder/with/files\n```\n\nThe `--retry-count` parameter allows BenchLLM to run a test multiple times, useful for models that may have variability in their outputs:\n\n```bash\n$ bench run --retry-count 5\n```\n\nBenchLLM offers multiple evaluation methods to determine if the prediction matches the test case\'s expected values. You can use the `--evaluator` parameter to specify the evaluation method:\n\nThere are multiple ways to evaluate if the test functions prediction matches the test cases expected values.\nBy default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method\n\n- `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.\n- `string-match`, checks if the strings are matching (case insensitive)\n- `interactive`, user manually accepts or fails tests in the terminal\n- `web`, uses pywebio fora simple local web interface\n\nThe non interactive evaluators also supports `--workers N` to run in the evaluations in parallel\n\n```bash\n$ bench run --evaluator string-match --workers 5\n```\n\nTo accelerate the evaluation process, BenchLLM uses a cache. If a (prediction, expected) pair has been evaluated in the past and a cache was used, the evaluation output will be saved for future evaluations. There are several types of caches:\n\n- `memory`, only caches output values during the current run. This is particularly useful when running with `--retry-count N`\n- `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.\n- `none`, does not use any cache.\n\n```bash\n$ bench run examples --cache memory\n```\n\n### 🧮 Eval\n\nWhile _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.\n\n```bash\n$ bench run --no-eval\n```\n\nThis will generate json files in `output/latest/predictions`\nThen later you can evaluate them with\n\n```bash\n$ bench eval output/latest/predictions\n```\n\n## 🔌 API\n\nFor more detailed control, BenchLLM provides an API.\nYou are not required to add YML/JSON tests to be able to evaluate your model.\nYou can instead:\n\n- Instantiate `Test` objects\n- Use a `Tester` object to generate predictions\n- Use an `Evaluator` object to evaluate your model\n\n```python\nfrom benchllm import StringMatchEvaluator, Test, Tester\n\n# Instantiate your Test objects\ntests = [\n    Test(input="What\'s 1+1?", expected=["2", "It\'s 2"]),\n    Test(input="First rule of fight club?", expected=["Do not talk about fight club"]),\n]\n\n# Use a Tester object to generate predictions using any test functions\ntester = Tester(my_test_function)\ntester.add_tests(tests)\npredictions = tester.run()\n\n# Use an Evaluator object to evaluate your model\nevaluator = StringMatchEvaluator()\nevaluator.load(predictions)\nresults = evaluator.run()\n\nprint(results)\n```\n\nIf you want to incorporate caching and run multiple parallel evaluation jobs, you can modify your evaluator as follows:\n\n```python\nfrom benchllm.cache import FileCache\n\n...\n\nevaluator = FileCache(StringMatchEvaluator(workers=2), Path("path/to/cache.json"))\nevaluator.load(predictions)\nresults = evaluator.run()\n```\n\nIn this example, `FileCache` is used to enable caching, and the `workers` parameter of `StringMatchEvaluator` is set to `2` to allow for parallel evaluations. The cache results are saved in a file specified by `Path("path/to/cache.json")`.\n\n## ☕️ Commands\n\n- `bench add`: Add a new test to a suite.\n- `bench tests`: List all tests in a suite.\n- `bench run`: Run all or target test suites.\n- `bench eval`: Runs the evaluation of an existing test run.\n\n## 🙌 Contribute\n\nBenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment and pip >= 23. You can use conda or any other environment manager to set up the environment:\n\n```bash\n$ conda create --name benchllm python=3.10\n$ conda activate benchllm\n$ pip install -e ".[dev]"\n```\n\nTo run all the examples first install the examples extra dependencies\n\n```bash\n$ pip install -e ".[examples]"\n```\n\nContribution steps:\n\n1. Fork the repository.\n2. Create a new branch for your changes.\n3. Make your changes.\n4. Test your changes.\n5. Submit a pull request.\n\nWe adhere to the PEP8 style guide. Please follow this guide when contributing.\n\nIf you need any support, feel free to open an issue on our GitHub page.\n',
+    'long_description': '# 🏋️\u200d♂️ BenchLLM 🏋️\u200d♀️\n\n🦾 Continuous Integration for LLM powered applications 🦙🦅🤖\n\n[![GitHub Repo stars](https://img.shields.io/github/stars/v7labs/BenchLLM?style=social)](https://github.com/v7labs/BenchLLM/stargazers)\n[![Twitter Follow](https://img.shields.io/twitter/follow/V7Labs?style=social)](https://twitter.com/V7Labs)\n[![Discord Follow](https://dcbadge.vercel.app/api/server/x7ExfHb3bG?style=flat)](https://discord.gg/x7ExfHb3bG)\n\n[**BenchLLM**](https://benchllm.com/) is a Python-based open-source library that streamlines the testing of Large Language Models (LLMs) and AI-powered applications. It measures the accuracy of your model, agents, or chains by validating responses on any number of tests via LLMs.\n\nBenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and is now Open Sourced under MIT License to share with the wider community\n\n## 💡 Get help on [Discord](https://discord.gg/x7ExfHb3bG) or [Tweet at us](https://twitter.com/V7Labs)\n\n<hr/>\n\nUse BenchLLM to:\n\n- Test the responses of your LLM across any number of prompts.\n- Continuous integration for chains like [Langchain](https://github.com/hwchase17/langchain), agents like [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT), or LLM models like [Llama](https://github.com/facebookresearch/llama) or GPT-4.\n- Eliminate flaky chains and create confidence in your code.\n- Spot inaccurate responses and hallucinations in your application at every version.\n\n<hr/>\n\n> ⚠️ **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.\n>\n> For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.\n\n## 🧪 BenchLLM Testing Methodology\n\nBenchLLM implements a distinct two-step methodology for validating your machine learning models:\n\n1. **Testing**: This stage involves running your code against any number of expected responses and capturing the predictions produced by your model without immediate judgment or comparison.\n\n2. **Evaluation**: The recorded predictions are compared against the expected output using LLMs to verify factual similarity (or optionally manually). Detailed comparison reports, including pass/fail status and other metrics, are generated.\n\nThis methodical separation offers a comprehensive view of your model\'s performance and allows for better control and refinement of each step.\n\n## 🚀 Install\n\nTo install BenchLLM we use pip\n\n```\npip install benchllm\n```\n\n## 💻 Usage\n\nStart by importing the library and use the @benchllm.test decorator to mark the function you\'d like to test:\n\n```python\nimport benchllm\n\n# Your custom model implementation\ndef run_my_model(input):\n    # Your model\'s logic goes here.\n    return some_result\n\n@benchllm.test(suite="/path/to/test/suite") # If the tests are in the same directory, just use @benchllm.test.\ndef invoke_model(input: str):\n    return run_my_model(input)\n```\n\nNext, prepare your tests. These are YAML/JSON files structured as follows:\n\n```yml\ninput: What\'s 1+1? Be very terse, only numeric output\nexpected:\n  - 2\n  - 2.0\n```\n\nIn the above example, the `input` is the query or instruction that your model will process, and `expected` contains the potential responses that your model should return. It\'s important to note that `input` can be a simple `str` or a more complex nested dictionary; BenchLLM will extract the type of the `input` argument in the Python code and load the `input` field from the YAML file accordingly.\n\nBy default, BenchLLM uses OpenAI\'s GPT-3 model for the `semantic` evaluator. This requires setting the `OPENAI_API_KEY` environment variable. If you do not want to use this default evaluator, you can specify an alternative one (discussed in further detail below):\n\n```bash\nexport OPENAI_API_KEY=\'your-api-key\'\n```\n\nReplace \'your-api-key\' with your actual OpenAI API key.\n\nTo initiate testing, use the `bench run` command:\n\n```bash\n$ bench run\n```\n\nBy default, the bench run command looks for Python files implementing the @test decorator in the current directory. To target a specific file or folder, specify it directly:\n\n```bash\n$ bench run path/to/my/file.py or/path/to/folder/with/files\n```\n\nThe `--retry-count` parameter allows BenchLLM to run a test multiple times, useful for models that may have variability in their outputs:\n\n```bash\n$ bench run --retry-count 5\n```\n\nBenchLLM offers multiple evaluation methods to determine if the prediction matches the test case\'s expected values. You can use the `--evaluator` parameter to specify the evaluation method:\n\nThere are multiple ways to evaluate if the test functions prediction matches the test cases expected values.\nBy default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method\n\n- `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.\n- `embedding`, uses cosine distance between embedded vectors. Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.\n- `string-match`, checks if the strings are matching (case insensitive)\n- `interactive`, user manually accepts or fails tests in the terminal\n- `web`, uses pywebio fora simple local web interface\n\nThe non interactive evaluators also supports `--workers N` to run in the evaluations in parallel\n\n```bash\n$ bench run --evaluator string-match --workers 5\n```\n\nTo accelerate the evaluation process, BenchLLM uses a cache. If a (prediction, expected) pair has been evaluated in the past and a cache was used, the evaluation output will be saved for future evaluations. There are several types of caches:\n\n- `memory`, only caches output values during the current run. This is particularly useful when running with `--retry-count N`\n- `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.\n- `none`, does not use any cache.\n\n```bash\n$ bench run examples --cache memory\n```\n\nWhen working on developing chains or training agent models, there may be instances where these models need to interact with external functions — for instance, querying a weather forecast or executing an SQL query. In such scenarios, BenchLLM facilitates the ability to mock these functions. This helps you make your tests more predictable and enables the discovery of unexpected function calls.\n\n```yml\ninput: I live in London, can I expect rain today?\nexpected: ["no"]\ncalls:\n  - name: forecast.get_n_day_weather_forecast\n    returns: It\'s sunny in London.\n    arguments:\n      location: London\n      num_days: 1\n```\n\nIn the example above, the function `get_n_day_weather_forecast` in the `forecast` module is mocked. In other words, every time this function is invoked, the model will receive `"It\'s sunny in London"`. BenchLLM also provides warnings if the function is invoked with argument values different from `get_n_day_weather_forecast(location=London, num_days=1)`. Please note, the provision of these argument parameters is optional.\n\n### 🧮 Eval\n\nWhile _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.\n\n```bash\n$ bench run --no-eval\n```\n\nThis will generate json files in `output/latest/predictions`\nThen later you can evaluate them with\n\n```bash\n$ bench eval output/latest/predictions\n```\n\n## 🔌 API\n\nFor more detailed control, BenchLLM provides an API.\nYou are not required to add YML/JSON tests to be able to evaluate your model.\nYou can instead:\n\n- Instantiate `Test` objects\n- Use a `Tester` object to generate predictions\n- Use an `Evaluator` object to evaluate your model\n\n```python\nfrom benchllm import StringMatchEvaluator, Test, Tester\n\n# Instantiate your Test objects\ntests = [\n    Test(input="What\'s 1+1?", expected=["2", "It\'s 2"]),\n    Test(input="First rule of fight club?", expected=["Do not talk about fight club"]),\n]\n\n# Use a Tester object to generate predictions using any test functions\ntester = Tester(my_test_function)\ntester.add_tests(tests)\npredictions = tester.run()\n\n# Use an Evaluator object to evaluate your model\nevaluator = StringMatchEvaluator()\nevaluator.load(predictions)\nresults = evaluator.run()\n\nprint(results)\n```\n\nIf you want to incorporate caching and run multiple parallel evaluation jobs, you can modify your evaluator as follows:\n\n```python\nfrom benchllm.cache import FileCache\n\n...\n\nevaluator = FileCache(StringMatchEvaluator(workers=2), Path("path/to/cache.json"))\nevaluator.load(predictions)\nresults = evaluator.run()\n```\n\nIn this example, `FileCache` is used to enable caching, and the `workers` parameter of `StringMatchEvaluator` is set to `2` to allow for parallel evaluations. The cache results are saved in a file specified by `Path("path/to/cache.json")`.\n\n## ☕️ Commands\n\n- `bench add`: Add a new test to a suite.\n- `bench tests`: List all tests in a suite.\n- `bench run`: Run all or target test suites.\n- `bench eval`: Runs the evaluation of an existing test run.\n\n## 🙌 Contribute\n\nBenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment and pip >= 23. You can use conda or any other environment manager to set up the environment:\n\n```bash\n$ conda create --name benchllm python=3.10\n$ conda activate benchllm\n$ pip install -e ".[dev]"\n```\n\nTo run all the examples first install the examples extra dependencies\n\n```bash\n$ pip install -e ".[examples]"\n```\n\nContribution steps:\n\n1. Fork the repository.\n2. Create a new branch for your changes.\n3. Make your changes.\n4. Test your changes.\n5. Submit a pull request.\n\nWe adhere to the PEP8 style guide. Please follow this guide when contributing.\n\nIf you need any support, feel free to open an issue on our GitHub page.\n',
     'author': 'Simon Edwardsson',
     'author_email': 'simon@v7labs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/v7labs/benchllm',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `benchllm-0.2.0/PKG-INFO` & `benchllm-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchllm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tool for testing LLMs
 Home-page: https://github.com/v7labs/benchllm
 License: MIT
 Author: Simon Edwardsson
 Author-email: simon@v7labs.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -131,14 +131,15 @@
 
 BenchLLM offers multiple evaluation methods to determine if the prediction matches the test case's expected values. You can use the `--evaluator` parameter to specify the evaluation method:
 
 There are multiple ways to evaluate if the test functions prediction matches the test cases expected values.
 By default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method
 
 - `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.
+- `embedding`, uses cosine distance between embedded vectors. Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.
 - `string-match`, checks if the strings are matching (case insensitive)
 - `interactive`, user manually accepts or fails tests in the terminal
 - `web`, uses pywebio fora simple local web interface
 
 The non interactive evaluators also supports `--workers N` to run in the evaluations in parallel
 
 ```bash
@@ -151,14 +152,29 @@
 - `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.
 - `none`, does not use any cache.
 
 ```bash
 $ bench run examples --cache memory
 ```
 
+When working on developing chains or training agent models, there may be instances where these models need to interact with external functions — for instance, querying a weather forecast or executing an SQL query. In such scenarios, BenchLLM facilitates the ability to mock these functions. This helps you make your tests more predictable and enables the discovery of unexpected function calls.
+
+```yml
+input: I live in London, can I expect rain today?
+expected: ["no"]
+calls:
+  - name: forecast.get_n_day_weather_forecast
+    returns: It's sunny in London.
+    arguments:
+      location: London
+      num_days: 1
+```
+
+In the example above, the function `get_n_day_weather_forecast` in the `forecast` module is mocked. In other words, every time this function is invoked, the model will receive `"It's sunny in London"`. BenchLLM also provides warnings if the function is invoked with argument values different from `get_n_day_weather_forecast(location=London, num_days=1)`. Please note, the provision of these argument parameters is optional.
+
 ### 🧮 Eval
 
 While _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
 
 ```bash
 $ bench run --no-eval
 ```
```

