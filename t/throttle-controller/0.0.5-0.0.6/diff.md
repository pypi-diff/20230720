# Comparing `tmp/throttle-controller-0.0.5.tar.gz` & `tmp/throttle-controller-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle-controller-0.0.5.tar", last modified: Mon Jan  9 12:13:12 2023, max compression
+gzip compressed data, was "throttle-controller-0.0.6.tar", last modified: Thu Jul 20 14:42:35 2023, max compression
```

## Comparing `throttle-controller-0.0.5.tar` & `throttle-controller-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.527131 throttle-controller-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    16488 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/tests/test_utils_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/throttle_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/throttle_controller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/utils/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-09 12:12:46.000000 throttle-controller-0.0.5/throttle_controller/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:13:12.531131 throttle-controller-0.0.5/throttle_controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-09 12:13:12.000000 throttle-controller-0.0.5/throttle_controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    39914 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-20 14:42:35.101082 throttle-controller-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/tests/test_utils_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/throttle_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/throttle_controller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 14:42:00.000000 throttle-controller-0.0.6/throttle_controller/utils/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:35.097082 throttle-controller-0.0.6/throttle_controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 14:42:35.000000 throttle-controller-0.0.6/throttle_controller.egg-info/top_level.txt
```

### Comparing `throttle-controller-0.0.5/.gitignore` & `throttle-controller-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `throttle-controller-0.0.5/LICENSE` & `throttle-controller-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle-controller-0.0.5/PKG-INFO` & `throttle-controller-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle-controller
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple throttling controller
 Home-page: https://github.com/kitsuyui/python-throttle-controller
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `throttle-controller-0.0.5/README.md` & `throttle-controller-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `throttle-controller-0.0.5/setup.cfg` & `throttle-controller-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `throttle-controller-0.0.5/tests/test_simple.py` & `throttle-controller-0.0.6/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `throttle-controller-0.0.5/throttle_controller/protocol.py` & `throttle-controller-0.0.6/throttle_controller/protocol.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import contextlib
 import datetime
-from typing import Generator, Hashable, Protocol
+import sys
+from typing import Generator, Hashable
+
+if sys.version_info >= (3, 8):
+    from typing import Protocol
+else:
+    from typing_extensions import Protocol  # pragma: no cover
+
 
 Key = Hashable
 
 
 class ThrottleController(Protocol):  # pragma: no cover
     def cooldown_time_for(self, key: Key) -> datetime.timedelta:
         ...
```

### Comparing `throttle-controller-0.0.5/throttle_controller/simple.py` & `throttle-controller-0.0.6/throttle_controller/simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import datetime
 import time
 from dataclasses import dataclass, field
-from typing import Dict
 
 from .protocol import Key, ThrottleController
 from .utils.interval import Interval, interval_to_timedelta
 
 
 @dataclass
 class SimpleThrottleController(ThrottleController):
     default_cooldown_time: datetime.timedelta
-    last_use_times: Dict[Key, datetime.datetime] = field(default_factory=dict)
-    cooldown_times: Dict[Key, datetime.timedelta] = field(default_factory=dict)
+    last_use_times: dict[Key, datetime.datetime] = field(default_factory=dict)
+    cooldown_times: dict[Key, datetime.timedelta] = field(default_factory=dict)
 
     @classmethod
-    def create(cls, *, default_cooldown_time: Interval) -> SimpleThrottleController:
-        return cls(default_cooldown_time=interval_to_timedelta(default_cooldown_time))
+    def create(
+        cls, *, default_cooldown_time: Interval
+    ) -> SimpleThrottleController:
+        return cls(
+            default_cooldown_time=interval_to_timedelta(default_cooldown_time)
+        )
 
     def cooldown_time_for(self, key: Key) -> datetime.timedelta:
         return self.cooldown_times.get(key, self.default_cooldown_time)
 
     def record_use_time(self, key: Key, use_time: datetime.datetime) -> None:
         self.last_use_times[key] = use_time
```

### Comparing `throttle-controller-0.0.5/throttle_controller.egg-info/PKG-INFO` & `throttle-controller-0.0.6/throttle_controller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throttle-controller
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple throttling controller
 Home-page: https://github.com/kitsuyui/python-throttle-controller
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `throttle-controller-0.0.5/throttle_controller.egg-info/SOURCES.txt` & `throttle-controller-0.0.6/throttle_controller.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 .coveragerc
 .gitignore
 .gitignore.in
 LICENSE
-Makefile
-Pipfile
-Pipfile.lock
 README.md
-mypy.ini
+poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
-setup.py
+.github/renovate.json5
+.github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 tests/__init__.py
 tests/test_simple.py
 tests/test_utils_interval.py
 throttle_controller/__init__.py
 throttle_controller/_version.py
 throttle_controller/protocol.py
 throttle_controller/py.typed
 throttle_controller/simple.py
-throttle_controller/version.py
 throttle_controller.egg-info/PKG-INFO
 throttle_controller.egg-info/SOURCES.txt
 throttle_controller.egg-info/dependency_links.txt
 throttle_controller.egg-info/requires.txt
 throttle_controller.egg-info/top_level.txt
 throttle_controller/utils/__init__.py
 throttle_controller/utils/interval.py
```

