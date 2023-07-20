# Comparing `tmp/apparent-0.1.1.tar.gz` & `tmp/apparent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apparent-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apparent-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apparent-0.1.1.tar` & `apparent-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.1/LICENSE.txt
--rwxr-xr-x   0        0        0     5054 2023-07-20 20:01:34.669401 apparent-0.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.1/apparent/.DS_Store
--rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.1/apparent/__init__.py
--rw-r--r--   0        0        0     9337 2023-07-20 15:55:22.776212 apparent-0.1.1/apparent/timing.py
--rwxr-xr-x   0        0        0       92 2023-07-20 16:31:06.798096 apparent-0.1.1/bin/install-dev
--rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.1/bin/test
--rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.1/bin/test-coverage
--rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.1/doc/K.svg
--rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.1/doc/diffs.svg
--rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.1/doc/variance.md
--rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.1/doc/variance.svg
--rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.1/doc/variance_calc.svg
--rwxr-xr-x   0        0        0     1025 2023-07-20 20:54:35.784460 apparent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.1/tests/timer_results_tests.py
--rw-r--r--   0        0        0     6049 2023-07-19 19:30:18.766728 apparent-0.1.1/tests/timer_tests.py
--rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.1/tests/variance_tests.py
--rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 apparent-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.2/LICENSE.txt
+-rwxr-xr-x   0        0        0     5054 2023-07-20 20:01:34.669401 apparent-0.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.2/apparent/.DS_Store
+-rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.2/apparent/__init__.py
+-rw-r--r--   0        0        0     9362 2023-07-20 21:27:03.306883 apparent-0.1.2/apparent/timing.py
+-rwxr-xr-x   0        0        0       92 2023-07-20 16:31:06.798096 apparent-0.1.2/bin/install-dev
+-rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.2/bin/test
+-rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.2/bin/test-coverage
+-rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.2/doc/K.svg
+-rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.2/doc/diffs.svg
+-rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.2/doc/variance.md
+-rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.2/doc/variance.svg
+-rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.2/doc/variance_calc.svg
+-rwxr-xr-x   0        0        0     1025 2023-07-20 21:27:49.647195 apparent-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.2/tests/timer_results_tests.py
+-rw-r--r--   0        0        0     6049 2023-07-19 19:30:18.766728 apparent-0.1.2/tests/timer_tests.py
+-rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.2/tests/variance_tests.py
+-rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 apparent-0.1.2/PKG-INFO
```

### Comparing `apparent-0.1.1/.gitignore` & `apparent-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/LICENSE.txt` & `apparent-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/README.md` & `apparent-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/apparent/.DS_Store` & `apparent-0.1.2/apparent/.DS_Store`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/apparent/timing.py` & `apparent-0.1.2/apparent/timing.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """The main module for explicit timing measurement support. See @timed"""
 import math
 from contextlib import AbstractContextManager
 from dataclasses import asdict, dataclass
 from enum import Enum
 from functools import wraps
 from time import perf_counter
-from typing import Protocol, Type
+from typing import Protocol, Type, Union
 
 
 class Units(Enum):
     MIN = 'min'
     SEC = 'sec'
     MSEC = 'msec'
 
@@ -224,22 +224,22 @@
 
     def reset(self, name: str):
         ...
 
 
 class Timed:
     """A simple class to associate a timer registry with the timed decorator. Rarely used."""
-    _registry: TimerRegistryType | Type[TimerRegistry] = TimerRegistry
+    _registry: Union[TimerRegistryType, Type[TimerRegistry]] = TimerRegistry
 
     @classmethod
-    def registry(cls) -> TimerRegistryType | Type[TimerRegistry]:
+    def registry(cls) -> Union[TimerRegistryType, Type[TimerRegistry]]:
         return cls._registry
 
     @classmethod
-    def set_registry(cls, registry: TimerRegistryType | Type[TimerRegistry]):
+    def set_registry(cls, registry: Union[TimerRegistryType, Type[TimerRegistry]]):
         cls._registry = registry
 
 
 def timed(f):
     """A decorator for timing a function.
     The decorated function will be called with a timer context manager to
     record the time spent in the decorated function.
```

### Comparing `apparent-0.1.1/doc/K.svg` & `apparent-0.1.2/doc/K.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/doc/diffs.svg` & `apparent-0.1.2/doc/diffs.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/doc/variance.md` & `apparent-0.1.2/doc/variance.md`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/doc/variance.svg` & `apparent-0.1.2/doc/variance.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/doc/variance_calc.svg` & `apparent-0.1.2/doc/variance_calc.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/pyproject.toml` & `apparent-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apparent"
-version = "0.1.1"
+version = "0.1.2"
 description = "A toolkit for code observability in-process data collection: timing, counters, and metrics."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = ["apparent", "observability", "monitoring", "timers", "timing", "counters", "metrics"]
 authors = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
 maintainers = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
```

### Comparing `apparent-0.1.1/tests/timer_results_tests.py` & `apparent-0.1.2/tests/timer_results_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/tests/timer_tests.py` & `apparent-0.1.2/tests/timer_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/tests/variance_tests.py` & `apparent-0.1.2/tests/variance_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.1/PKG-INFO` & `apparent-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apparent
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit for code observability in-process data collection: timing, counters, and metrics.
 Keywords: apparent,observability,monitoring,timers,timing,counters,metrics
 Author-email: Arnon Moscona <arnon@moscona.com>
 Maintainer-email: Arnon Moscona <arnon@moscona.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

