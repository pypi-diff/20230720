# Comparing `tmp/alpaka-job-coverage-1.3.4.tar.gz` & `tmp/alpaka-job-coverage-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.3.4.tar", last modified: Wed Jul 19 12:56:51 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.3.5.tar", last modified: Thu Jul 20 15:01:25 2023, max compression
```

## Comparing `alpaka-job-coverage-1.3.4.tar` & `alpaka-job-coverage-1.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.647751 alpaka-job-coverage-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-19 12:56:51.647751 alpaka-job-coverage-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:56:51.647751 alpaka-job-coverage-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.639752 alpaka-job-coverage-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.643751 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.643751 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-19 12:56:51.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 12:56:51.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:56:51.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 12:56:51.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 12:56:51.000000 alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.647751 alpaka-job-coverage-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    40729 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 12:56:30.000000 alpaka-job-coverage-1.3.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41654 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/version.txt
```

### Comparing `alpaka-job-coverage-1.3.4/LICENSE` & `alpaka-job-coverage-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/PKG-INFO` & `alpaka-job-coverage-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.4
+Version: 1.3.5
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.4/README.md` & `alpaka-job-coverage-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/setup.py` & `alpaka-job-coverage-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,35 @@
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
 from alpaka_job_coverage.util import (
     row_check_name,
     row_check_version,
     row_check_backend_version,
     backend_is_not_in_row,
 )
+from typing import List, Tuple, Union
+from typeguard import typechecked
+
+
+@typechecked
+def compiler_backend_filter_typed(
+    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]]
+) -> bool:
+    """Type checked version of compiler_backend_filter(). Should be only used for
+    testing or tooling. The type check adds a big overhead, which slows down
+    pair-wise generator by the factor 30.
+
+    Args:
+        row (List[Union[Tuple[str, str], List[Tuple[str, str]]]]): Combination
+        to verify. The row can contain up to all combination fields and at least
+         two items.
+
+    Returns:
+        bool: True, if combination is valid, otherwise False.
+    """
+    return compiler_backend_filter(row)
 
 
 def compiler_backend_filter(row: List) -> bool:
     """Filter rules basing on backend names and versions.
 
     Args:
         row (List): Combination to verify. The row can contain
```

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 """Filter rules basing on host and device compiler names and versions.
 """
 
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
 from alpaka_job_coverage.util import row_check_name, row_check_version, is_in_row
 
 from packaging import version as pk_version
+from typing import List, Tuple, Union
+from typeguard import typechecked
+
+
+@typechecked
+def compiler_version_filter_typed(
+    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]]
+) -> bool:
+    """Type checked version of compiler_version_filter(). Should be only used for
+    testing or tooling. The type check adds a big overhead, which slows down
+    pair-wise generator by the factor 30.
+
+    Args:
+        row (List[Union[Tuple[str, str], List[Tuple[str, str]]]]): Combination
+        to verify. The row can contain up to all combination fields and at least
+         two items.
+
+    Returns:
+        bool: True, if combination is valid, otherwise False.
+    """
+    return compiler_version_filter(row)
 
 
 def compiler_version_filter(row: List) -> bool:
     """Filter rules basing on host and device compiler names and versions.
 
     Args:
         row (List): Combination to verify. The row can contain
```

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,35 @@
     row_check_backend_version,
     row_check_name,
     row_check_version,
     is_in_row,
 )
 
 from packaging import version as pk_version
+from typing import List, Tuple, Union
+from typeguard import typechecked
+
+
+@typechecked
+def software_dependency_filter_typed(
+    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]]
+) -> bool:
+    """Type checked version of software_dependency_filter(). Should be only used for
+    testing or tooling. The type check adds a big overhead, which slows down
+    pair-wise generator by the factor 30.
+
+    Args:
+        row (List[Union[Tuple[str, str], List[Tuple[str, str]]]]): Combination
+        to verify. The row can contain up to all combination fields and at least
+         two items.
+
+    Returns:
+        bool: True, if combination is valid, otherwise False.
+    """
+    return software_dependency_filter(row)
 
 
 def software_dependency_filter(row: List) -> bool:
     """Filter rules handling software dependencies and compiler settings.
 
     Args:
         row (List): Combination to verify. The row can contain
@@ -120,20 +141,25 @@
     # a bug in CMAKE 3.18 avoids the correct usage of the variable CMAKE_CUDA_ARCHITECTURE if the
     # CUDA compiler is Clang++
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA) and row_check_version(
         row, CMAKE, "<", "3.19"
     ):
         return False
 
-    # disable nvcc 11.3 + gcc 10 + Ubuntu 20.04
+    # disable nvcc 11.0-11.3 + gcc 10 + Ubuntu 20.04
     # Ubuntu 20.04 provides only gcc 10.3 and not 10.4 or 10.5
     # this combination does not work: https://github.com/alpaka-group/alpaka/issues/1297
     if (
         row_check_name(row, DEVICE_COMPILER, "==", NVCC)
-        and row_check_version(row, DEVICE_COMPILER, "==", "11.3")
+        and (
+            row_check_version(row, DEVICE_COMPILER, "==", "11.0")
+            or row_check_version(row, DEVICE_COMPILER, "==", "11.1")
+            or row_check_version(row, DEVICE_COMPILER, "==", "11.2")
+            or row_check_version(row, DEVICE_COMPILER, "==", "11.3")
+        )
         and row_check_name(row, HOST_COMPILER, "==", GCC)
         and row_check_version(row, HOST_COMPILER, "==", "10")
         and row_check_version(row, UBUNTU, "==", "20.04")
     ):
         return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.4
+Version: 1.3.5
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.4/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.4/tests/test_compiler_names.py` & `alpaka-job-coverage-1.3.5/tests/test_compiler_names.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
-from alpaka_job_coverage.filter_compiler_name import general_compiler_filter
+from alpaka_job_coverage.filter_compiler_name import general_compiler_filter_typed
 
 
 # Test all compiler names except nvcc and clang-cuda. This is tested in
 # test_cuda_sdk.py
 class TestHostDeviceCompiler(unittest.TestCase):
     def setUp(self):
         global param_map
@@ -23,18 +23,18 @@
         valid_combs = [
             [(GCC, "0"), (GCC, "0")],
             [(CLANG, "0"), (CLANG, "0")],
             [(HIPCC, "0"), (HIPCC, "0")],
         ]
 
         for comb in valid_combs:
-            self.assertTrue(general_compiler_filter(comb))
+            self.assertTrue(general_compiler_filter_typed(comb))
 
         invalid_combs = [
             [(GCC, "0"), (CLANG, "0")],
             [(GCC, "0"), (CLANG, "0")],
             [(GCC, "0"), (HIPCC, "0")],
             [(HIPCC, "0"), (CLANG, "0")],
         ]
 
         for comb in invalid_combs:
-            self.assertFalse(general_compiler_filter(comb))
+            self.assertFalse(general_compiler_filter_typed(comb))
```

### Comparing `alpaka-job-coverage-1.3.4/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.3.5/tests/test_cuda_sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import unittest
 
-from alpaka_job_coverage.filter_compiler_name import general_compiler_filter
-from alpaka_job_coverage.filter_compiler_version import compiler_version_filter
-from alpaka_job_coverage.filter_backend_version import compiler_backend_filter
-from alpaka_job_coverage.filter_software_dependency import software_dependency_filter
+from alpaka_job_coverage.filter_compiler_name import general_compiler_filter_typed
+from alpaka_job_coverage.filter_compiler_version import compiler_version_filter_typed
+from alpaka_job_coverage.filter_backend_version import compiler_backend_filter_typed
+from alpaka_job_coverage.filter_software_dependency import (
+    software_dependency_filter_typed,
+)
 from alpaka_job_coverage.globals import *
 
 
 def full_filter_chain(row) -> bool:
     return (
-        general_compiler_filter(row)
-        and compiler_version_filter(row)
-        and compiler_backend_filter(row)
-        and software_dependency_filter(row)
+        general_compiler_filter_typed(row)
+        and compiler_version_filter_typed(row)
+        and compiler_backend_filter_typed(row)
+        and software_dependency_filter_typed(row)
     )
 
 
 class TestHostDeviceCompiler(unittest.TestCase):
     def setUp(self):
         global param_map
         # set param_map, that filters expect the following parameters in the
@@ -35,265 +37,265 @@
         valid_combs = [
             [(GCC, "0"), (NVCC, "0")],
             [(CLANG, "0"), (NVCC, "0")],
             [(CLANG_CUDA, "0"), (CLANG_CUDA, "0")],
         ]
 
         for comb in valid_combs:
-            self.assertTrue(general_compiler_filter(comb))
+            self.assertTrue(general_compiler_filter_typed(comb))
 
         invalid_combs = [
             # NVCC is not allowed as host compiler
             [(NVCC, "0"), (NVCC, "0")],
             [(NVCC, "0"), (GCC, "0")],
             [(NVCC, "0"), (CLANG, "0")],
             # only GCC and Clang are allowed as host compiler for nvcc
             [(CLANG_CUDA, "0"), (NVCC, "0")],
             [(HIPCC, "0"), (NVCC, "0")],
         ]
 
         for comb in invalid_combs:
-            self.assertFalse(general_compiler_filter(comb))
+            self.assertFalse(general_compiler_filter_typed(comb))
 
 
 class TestGeneralFilterFunctionality(unittest.TestCase):
     def setUp(self):
         global param_map
         # set param_map, that filters expect the following parameters in the
         # order
         param_map[HOST_COMPILER] = 0
         param_map[DEVICE_COMPILER] = 1
         param_map[BACKENDS] = 2
         # UBUNTU and CXX_STANDARD are only required, because
-        # software_dependency_filter do a look up in param_map for it
+        # software_dependency_filter_typed do a look up in param_map for it
         param_map[CXX_STANDARD] = 3
         param_map[UBUNTU] = 4
 
     def setDown(self):
         global param_map
         # reset param_map for following up tests
         param_map = {}
 
     def test_if_backend_is_not_set(self):
-        # general_compiler_filter should be always return true, because
+        # general_compiler_filter_typed should be always return true, because
         # GCC is a valid host compiler and NVCC a valid device compiler
 
-        # compiler_backend_filter should always return true for the valid
+        # compiler_backend_filter_typed should always return true for the valid
         # combination, because if the backend parameter
         # (ALPAKA_ACC_GPU_CUDA_ENABLE, "11.2") is added, it becomes a valid
         # combination
 
-        # compiler_version_filter filters invalid combination depending of
+        # compiler_version_filter_typed filters invalid combination depending of
         # host and device compiler version
 
-        # no rule in software_dependency_filter should affect this test
+        # no rule in software_dependency_filter_typed should affect this test
 
         comb_valid_1 = [(GCC, "9"), (NVCC, "11.2")]
 
-        self.assertTrue(general_compiler_filter(comb_valid_1))
-        self.assertTrue(compiler_backend_filter(comb_valid_1))
-        self.assertTrue(compiler_version_filter(comb_valid_1))
-        self.assertTrue(software_dependency_filter(comb_valid_1))
+        self.assertTrue(general_compiler_filter_typed(comb_valid_1))
+        self.assertTrue(compiler_backend_filter_typed(comb_valid_1))
+        self.assertTrue(compiler_version_filter_typed(comb_valid_1))
+        self.assertTrue(software_dependency_filter_typed(comb_valid_1))
         self.assertTrue(full_filter_chain(comb_valid_1))
 
         comb_invalid_1 = [(GCC, "13"), (NVCC, "11.2")]
 
-        self.assertTrue(general_compiler_filter(comb_invalid_1))
-        self.assertTrue(compiler_backend_filter(comb_invalid_1))
-        self.assertFalse(compiler_version_filter(comb_invalid_1))
-        self.assertTrue(software_dependency_filter(comb_invalid_1))
+        self.assertTrue(general_compiler_filter_typed(comb_invalid_1))
+        self.assertTrue(compiler_backend_filter_typed(comb_invalid_1))
+        self.assertFalse(compiler_version_filter_typed(comb_invalid_1))
+        self.assertTrue(software_dependency_filter_typed(comb_invalid_1))
         self.assertFalse(full_filter_chain(comb_invalid_1))
 
         comb_valid_2 = [(CLANG, "9"), (NVCC, "11.2")]
 
-        self.assertTrue(general_compiler_filter(comb_valid_2))
-        self.assertTrue(compiler_backend_filter(comb_valid_2))
-        self.assertTrue(compiler_version_filter(comb_valid_2))
-        self.assertTrue(software_dependency_filter(comb_valid_2))
+        self.assertTrue(general_compiler_filter_typed(comb_valid_2))
+        self.assertTrue(compiler_backend_filter_typed(comb_valid_2))
+        self.assertTrue(compiler_version_filter_typed(comb_valid_2))
+        self.assertTrue(software_dependency_filter_typed(comb_valid_2))
         self.assertTrue(full_filter_chain(comb_valid_2))
 
         comb_invalid_2 = [(CLANG, "17"), (NVCC, "11.2")]
 
-        self.assertTrue(general_compiler_filter(comb_invalid_2))
-        self.assertTrue(compiler_backend_filter(comb_invalid_2))
-        self.assertFalse(compiler_version_filter(comb_invalid_2))
-        self.assertTrue(software_dependency_filter(comb_invalid_2))
+        self.assertTrue(general_compiler_filter_typed(comb_invalid_2))
+        self.assertTrue(compiler_backend_filter_typed(comb_invalid_2))
+        self.assertFalse(compiler_version_filter_typed(comb_invalid_2))
+        self.assertTrue(software_dependency_filter_typed(comb_invalid_2))
         self.assertFalse(full_filter_chain(comb_invalid_2))
 
     def test_if_backend_is_disabled(self):
-        # because the backend is off, compiler_backend_filter should return
+        # because the backend is off, compiler_backend_filter_typed should return
         # False every time
 
         comb_valid_1 = [
             (GCC, "9"),
             (NVCC, "11.2"),
             [(ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER)],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_valid_1))
-        self.assertFalse(compiler_backend_filter(comb_valid_1))
-        self.assertTrue(compiler_version_filter(comb_valid_1))
-        self.assertTrue(software_dependency_filter(comb_valid_1))
+        self.assertTrue(general_compiler_filter_typed(comb_valid_1))
+        self.assertFalse(compiler_backend_filter_typed(comb_valid_1))
+        self.assertTrue(compiler_version_filter_typed(comb_valid_1))
+        self.assertTrue(software_dependency_filter_typed(comb_valid_1))
         self.assertFalse(full_filter_chain(comb_valid_1))
 
         comb_valid_2 = [
             (GCC, "9"),
             (NVCC, "11.2"),
             [
                 (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                 (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                 (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
             ],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_valid_2))
-        self.assertFalse(compiler_backend_filter(comb_valid_2))
-        self.assertTrue(compiler_version_filter(comb_valid_2))
-        self.assertTrue(software_dependency_filter(comb_valid_2))
+        self.assertTrue(general_compiler_filter_typed(comb_valid_2))
+        self.assertFalse(compiler_backend_filter_typed(comb_valid_2))
+        self.assertTrue(compiler_version_filter_typed(comb_valid_2))
+        self.assertTrue(software_dependency_filter_typed(comb_valid_2))
         self.assertFalse(full_filter_chain(comb_valid_2))
 
         comb_valid_3 = [
             (CLANG, "9"),
             (NVCC, "11.2"),
             [
                 (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                 (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                 (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
             ],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_valid_3))
-        self.assertFalse(compiler_backend_filter(comb_valid_3))
-        self.assertTrue(compiler_version_filter(comb_valid_3))
-        self.assertTrue(software_dependency_filter(comb_valid_3))
+        self.assertTrue(general_compiler_filter_typed(comb_valid_3))
+        self.assertFalse(compiler_backend_filter_typed(comb_valid_3))
+        self.assertTrue(compiler_version_filter_typed(comb_valid_3))
+        self.assertTrue(software_dependency_filter_typed(comb_valid_3))
         self.assertFalse(full_filter_chain(comb_valid_3))
 
         comb_invalid_1 = [
             (GCC, "13"),
             (NVCC, "11.2"),
             [(ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER)],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_invalid_1))
-        self.assertFalse(compiler_backend_filter(comb_invalid_1))
-        self.assertFalse(compiler_version_filter(comb_invalid_1))
-        self.assertTrue(software_dependency_filter(comb_invalid_1))
+        self.assertTrue(general_compiler_filter_typed(comb_invalid_1))
+        self.assertFalse(compiler_backend_filter_typed(comb_invalid_1))
+        self.assertFalse(compiler_version_filter_typed(comb_invalid_1))
+        self.assertTrue(software_dependency_filter_typed(comb_invalid_1))
         self.assertFalse(full_filter_chain(comb_invalid_1))
 
         comb_invalid_2 = [
             (GCC, "13"),
             (NVCC, "11.2"),
             [
                 (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                 (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                 (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
             ],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_invalid_2))
-        self.assertFalse(compiler_backend_filter(comb_invalid_2))
-        self.assertFalse(compiler_version_filter(comb_invalid_2))
-        self.assertTrue(software_dependency_filter(comb_invalid_2))
+        self.assertTrue(general_compiler_filter_typed(comb_invalid_2))
+        self.assertFalse(compiler_backend_filter_typed(comb_invalid_2))
+        self.assertFalse(compiler_version_filter_typed(comb_invalid_2))
+        self.assertTrue(software_dependency_filter_typed(comb_invalid_2))
         self.assertFalse(full_filter_chain(comb_invalid_2))
 
         comb_invalid_3 = [
             (CLANG, "13"),
             (NVCC, "11.2"),
             [
                 (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                 (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                 (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
             ],
         ]
 
-        self.assertTrue(general_compiler_filter(comb_invalid_3))
-        self.assertFalse(compiler_backend_filter(comb_invalid_3))
-        self.assertFalse(compiler_version_filter(comb_invalid_3))
-        self.assertTrue(software_dependency_filter(comb_invalid_3))
+        self.assertTrue(general_compiler_filter_typed(comb_invalid_3))
+        self.assertFalse(compiler_backend_filter_typed(comb_invalid_3))
+        self.assertFalse(compiler_version_filter_typed(comb_invalid_3))
+        self.assertTrue(software_dependency_filter_typed(comb_invalid_3))
         self.assertFalse(full_filter_chain(comb_invalid_3))
 
     def test_backend_versions(self):
         # for NVCC, the compiler version needs to be equal to the backend version
         for version in ["10.2", "11.0", "12.2"]:
             comb1 = [
                 (GCC, "9"),
                 (NVCC, version),
                 [(ALPAKA_ACC_GPU_CUDA_ENABLE, version)],
             ]
-            self.assertTrue(compiler_backend_filter(comb1))
+            self.assertTrue(compiler_backend_filter_typed(comb1))
 
             comb2 = [
                 (CLANG, "9"),
                 (NVCC, version),
                 [(ALPAKA_ACC_GPU_CUDA_ENABLE, version)],
             ]
-            self.assertTrue(compiler_backend_filter(comb2))
+            self.assertTrue(compiler_backend_filter_typed(comb2))
 
             comb3 = [
                 (GCC, "9"),
                 (NVCC, version),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, version),
                 ],
             ]
-            self.assertTrue(compiler_backend_filter(comb3))
+            self.assertTrue(compiler_backend_filter_typed(comb3))
 
             comb4 = [
                 (CLANG, "9"),
                 (NVCC, version),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, version),
                 ],
             ]
-            self.assertTrue(compiler_backend_filter(comb4))
+            self.assertTrue(compiler_backend_filter_typed(comb4))
 
         for nvcc_version, backend_version in [
             ("10.1", "10.2"),
             ("11.0", "11.5"),
             ("11.8", "12.2"),
         ]:
             comb1 = [
                 (GCC, "9"),
                 (NVCC, nvcc_version),
                 [(ALPAKA_ACC_GPU_CUDA_ENABLE, backend_version)],
             ]
-            self.assertFalse(compiler_backend_filter(comb1))
+            self.assertFalse(compiler_backend_filter_typed(comb1))
 
             comb2 = [
                 (CLANG, "9"),
                 (NVCC, nvcc_version),
                 [(ALPAKA_ACC_GPU_CUDA_ENABLE, backend_version)],
             ]
-            self.assertFalse(compiler_backend_filter(comb2))
+            self.assertFalse(compiler_backend_filter_typed(comb2))
 
             comb3 = [
                 (GCC, "9"),
                 (NVCC, nvcc_version),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, backend_version),
                 ],
             ]
-            self.assertFalse(compiler_backend_filter(comb3))
+            self.assertFalse(compiler_backend_filter_typed(comb3))
 
             comb4 = [
                 (CLANG, "9"),
                 (NVCC, nvcc_version),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, backend_version),
                 ],
             ]
-            self.assertFalse(compiler_backend_filter(comb4))
+            self.assertFalse(compiler_backend_filter_typed(comb4))
 
 
 class TestNvccGccCompatibility(unittest.TestCase):
     def setUp(self):
         global param_map
         # set param_map, that filters expect the following parameters in the
         # order
@@ -325,15 +327,17 @@
             ("11.0", "9", True),
             ("11.0", "10", False),
             ("11.0", "12", False),
         ]
 
         for nvcc_version, gcc_version, expected_value in expected_results:
             self.assertEqual(
-                compiler_version_filter([(NVCC, nvcc_version), (GCC, gcc_version)]),
+                compiler_version_filter_typed(
+                    [(NVCC, nvcc_version), (GCC, gcc_version)]
+                ),
                 expected_value,
                 f"nvcc {nvcc_version} + gcc {gcc_version} -> {expected_value}",
             )
 
     # Test the combination of GCC version and CUDA SDK version.
     # Validate the combinations, which are defined in the release notes of the
     # CUDA SDK.
@@ -367,15 +371,17 @@
             ("12.0", "13", False),
             ("12.1", "12", True),
             ("12.1", "13", False),
         ]
 
         for nvcc_version, gcc_version, expected_value in expected_results:
             self.assertEqual(
-                compiler_version_filter([(NVCC, nvcc_version), (GCC, gcc_version)]),
+                compiler_version_filter_typed(
+                    [(NVCC, nvcc_version), (GCC, gcc_version)]
+                ),
                 expected_value,
                 f"nvcc {nvcc_version} + gcc {gcc_version} -> {expected_value}",
             )
 
     # Test if a unknown CUDA SDK version returns always true.
     # This avoid behavior avoids, that valid combinations are silently disabled
     # if a new CUDA SDK version is released.
@@ -384,15 +390,17 @@
             ("42.0", "45", True),
         ]
 
         # TODO: add is_supported_sw_version to verify that our test version is not supported
 
         for nvcc_version, gcc_version, expected_value in expected_results:
             self.assertEqual(
-                compiler_version_filter([(NVCC, nvcc_version), (GCC, gcc_version)]),
+                compiler_version_filter_typed(
+                    [(NVCC, nvcc_version), (GCC, gcc_version)]
+                ),
                 expected_value,
                 f"nvcc {nvcc_version} + gcc {gcc_version} -> {expected_value}",
             )
 
 
 class TestNvccClangCompatibility(unittest.TestCase):
     def setUp(self):
@@ -441,15 +449,17 @@
             ("12.0", "15", False),
             ("12.1", "15", True),
             ("12.1", "16", False),
         ]
 
         for nvcc_version, clang_version, expected_value in expected_results:
             self.assertEqual(
-                compiler_version_filter([(NVCC, nvcc_version), (CLANG, clang_version)]),
+                compiler_version_filter_typed(
+                    [(NVCC, nvcc_version), (CLANG, clang_version)]
+                ),
                 expected_value,
                 f"nvcc {nvcc_version} + clang {clang_version} -> {expected_value}",
             )
 
     # Test if a unknown CUDA SDK version returns always true.
     # This avoid behavior avoids, that valid combinations are silently disabled
     # if a new CUDA SDK version is released.
@@ -458,15 +468,17 @@
             ("42.0", "45", True),
         ]
 
         # TODO: add is_supported_sw_version to verify that our test version is not supported
 
         for nvcc_version, clang_version, expected_value in expected_results:
             self.assertEqual(
-                compiler_version_filter([(NVCC, nvcc_version), (CLANG, clang_version)]),
+                compiler_version_filter_typed(
+                    [(NVCC, nvcc_version), (CLANG, clang_version)]
+                ),
                 expected_value,
                 f"nvcc {nvcc_version} + clang {clang_version} -> {expected_value}",
             )
 
 
 class TestNvccCxxStandard(unittest.TestCase):
     def setUp(self):
@@ -501,20 +513,20 @@
             ("12.2", 32),
             ("13.0", 32),
         ]:
             for cxx_version in [11, 14, 17, 20, 23, 26, 29, 32]:
                 comb = [(NVCC, nvcc_version), (CXX_STANDARD, str(cxx_version))]
                 if cxx_version <= max_cxx:
                     self.assertTrue(
-                        software_dependency_filter(comb),
+                        software_dependency_filter_typed(comb),
                         f"NVCC {nvcc_version} + CXX {cxx_version}",
                     )
                 else:
                     self.assertFalse(
-                        software_dependency_filter(comb),
+                        software_dependency_filter_typed(comb),
                         f"NVCC {nvcc_version} + CXX {cxx_version}",
                     )
 
 
 # tests for Clang as CUDA compiler
 class TestClangCUDA(unittest.TestCase):
     def setUp(self):
@@ -534,29 +546,29 @@
         # reset param_map for following up tests
         param_map = {}
 
     # standalone CLANG_CUDA as host compiler should pass all tests
     def test_host_compiler_name(self):
         comb = [(CLANG_CUDA, "99")]
 
-        self.assertTrue(general_compiler_filter(comb))
-        self.assertTrue(compiler_version_filter(comb))
-        self.assertTrue(compiler_backend_filter(comb))
-        self.assertTrue(software_dependency_filter(comb))
+        self.assertTrue(general_compiler_filter_typed(comb))
+        self.assertTrue(compiler_version_filter_typed(comb))
+        self.assertTrue(compiler_backend_filter_typed(comb))
+        self.assertTrue(software_dependency_filter_typed(comb))
         self.assertTrue(full_filter_chain(comb))
 
     # CLANG_CUDA as host compiler can be only used with CLANG_CUDA as device
     # compiler an vice vera
     def test_host_device_compiler_name(self):
         valid_comb = [(CLANG_CUDA, "99"), (CLANG_CUDA, "99")]
 
-        self.assertTrue(general_compiler_filter(valid_comb))
-        self.assertTrue(compiler_version_filter(valid_comb))
-        self.assertTrue(compiler_backend_filter(valid_comb))
-        self.assertTrue(software_dependency_filter(valid_comb))
+        self.assertTrue(general_compiler_filter_typed(valid_comb))
+        self.assertTrue(compiler_version_filter_typed(valid_comb))
+        self.assertTrue(compiler_backend_filter_typed(valid_comb))
+        self.assertTrue(software_dependency_filter_typed(valid_comb))
         self.assertTrue(full_filter_chain(valid_comb))
 
         invalid_combs = [
             [(CLANG_CUDA, "99"), (GCC, "99")],
             [(CLANG_CUDA, "99"), (CLANG, "99")],
             [(CLANG_CUDA, "99"), (HIPCC, "99")],
             [(CLANG_CUDA, "99"), (NVCC, "99")],
@@ -564,27 +576,27 @@
             [(CLANG, "99"), (CLANG_CUDA, "99")],
             [(HIPCC, "99"), (CLANG_CUDA, "99")],
             [(NVCC, "99"), (CLANG_CUDA, "99")],
         ]
 
         for comb in invalid_combs:
             self.assertFalse(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
 
@@ -595,30 +607,30 @@
             [(CLANG_CUDA, "16"), (CLANG_CUDA, "16")],
             [(CLANG_CUDA, "20"), (CLANG_CUDA, "20")],
             [(CLANG_CUDA, "99"), (CLANG_CUDA, "99")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -630,30 +642,30 @@
             # only Clang 14 and newer are supported as CUDA compiler
             [(CLANG_CUDA, "9"), (CLANG_CUDA, "9")],
             [(CLANG_CUDA, "13"), (CLANG_CUDA, "13")],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertFalse(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -684,33 +696,33 @@
                     (ALPAKA_ACC_GPU_HIP_ENABLE, OFF_VER),
                 ],
             ],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
@@ -743,33 +755,33 @@
                     (ALPAKA_ACC_GPU_HIP_ENABLE, "5.0"),
                 ],
             ],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertFalse(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
@@ -819,61 +831,61 @@
                     (CLANG_CUDA, str(clang_version)),
                     (CLANG_CUDA, str(clang_version)),
                     [(ALPAKA_ACC_GPU_CUDA_ENABLE, str(cuda_version))],
                 ]
 
                 if cuda_version > supported_versions[clang_version]:
                     self.assertFalse(
-                        compiler_backend_filter(comb),
+                        compiler_backend_filter_typed(comb),
                         f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                         f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                         f"BACKENDS: {comb[2]}",
                     )
                 else:
                     self.assertTrue(
-                        compiler_backend_filter(comb),
+                        compiler_backend_filter_typed(comb),
                         f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                         f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                         f"BACKENDS: {comb[2]}",
                     )
 
         # test if combination of non released clang version and released CUDA
         # SDK is allowed
         self.assertTrue(
-            compiler_backend_filter(
+            compiler_backend_filter_typed(
                 [
                     (CLANG_CUDA, "30"),
                     (CLANG_CUDA, "30"),
                     [(ALPAKA_ACC_GPU_CUDA_ENABLE, "11.5")],
                 ]
             ),
             f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
             f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
             f"BACKENDS: {comb[2]}",
         )
 
         # test if combination of non released clang version and non released
         # CUDA SDK is allowed
         self.assertTrue(
-            compiler_backend_filter(
+            compiler_backend_filter_typed(
                 [
                     (CLANG_CUDA, "30"),
                     (CLANG_CUDA, "30"),
                     [(ALPAKA_ACC_GPU_CUDA_ENABLE, "30.0")],
                 ]
             ),
             f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
             f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
             f"BACKENDS: {comb[2]}",
         )
 
         # test if combination of released clang version and non released
         # CUDA SDK is not allowed
         self.assertFalse(
-            compiler_backend_filter(
+            compiler_backend_filter_typed(
                 [
                     (CLANG_CUDA, "15"),
                     (CLANG_CUDA, "15"),
                     [(ALPAKA_ACC_GPU_CUDA_ENABLE, "30.0")],
                 ]
             ),
             f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
@@ -888,46 +900,46 @@
                 comb = [
                     (CLANG_CUDA, str(clang_version)),
                     (CLANG_CUDA, str(clang_version)),
                     [(ALPAKA_ACC_GPU_CUDA_ENABLE, "9.2")],
                     (CXX_STANDARD, str(cxx_version)),
                 ]
                 self.assertTrue(
-                    general_compiler_filter(comb),
+                    general_compiler_filter_typed(comb),
                     f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                     f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                     f"C++: {comb[3]}",
                 )
 
-                # does not test compiler_version_filter(), because of the filter
+                # does not test compiler_version_filter_typed(), because of the filter
                 # rule, that Clang 13 and older is not allowed as CUDA compiler
 
                 self.assertTrue(
-                    compiler_backend_filter(comb),
+                    compiler_backend_filter_typed(comb),
                     f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                     f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                     f"C++: {comb[3]}",
                 )
 
                 if clang_version <= 9 and cxx_version > 17:
                     self.assertFalse(
-                        software_dependency_filter(comb),
+                        software_dependency_filter_typed(comb),
                         f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                         f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                         f"C++: {comb[3]}",
                     )
                     self.assertFalse(
                         full_filter_chain(comb),
                         f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                         f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                         f"C++: {comb[3]}",
                     )
                 else:
                     self.assertTrue(
-                        software_dependency_filter(comb),
+                        software_dependency_filter_typed(comb),
                         f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                         f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                         f"C++: {comb[3]}",
                     )
 
     # Clang 11 and 12 is not available in the Ubuntu 18.04 ppa
     def test_ubuntu1804_ppa(self):
@@ -937,43 +949,43 @@
                 (CLANG_CUDA, str(clang_version)),
                 [(ALPAKA_ACC_GPU_CUDA_ENABLE, "9.2")],
                 (CXX_STANDARD, "17"),
                 (UBUNTU, "18.04"),
             ]
 
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"Ubuntu: {comb[4]}",
             )
 
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"Ubuntu: {comb[4]}",
             )
 
             if clang_version == 11 or clang_version == 12:
                 self.assertFalse(
-                    software_dependency_filter(comb),
+                    software_dependency_filter_typed(comb),
                     f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                     f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                     f"Ubuntu: {comb[4]}",
                 )
                 self.assertFalse(
                     full_filter_chain(comb),
                     f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                     f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                     f"Ubuntu: {comb[4]}",
                 )
             else:
                 self.assertTrue(
-                    software_dependency_filter(comb),
+                    software_dependency_filter_typed(comb),
                     f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                     f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                     f"Ubuntu: {comb[4]}",
                 )
 
     # CMake 3.18 and older does not support Clang as CUDA compiler
     def test_cmake_version(self):
@@ -994,33 +1006,33 @@
                 (UBUNTU, "20.04"),
                 (CMAKE, "3.22"),
             ],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
@@ -1053,33 +1065,33 @@
                 (UBUNTU, "20.04"),
                 (CMAKE, "3.18.3"),
             ],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertFalse(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"CMAKE: {comb[5][1]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
```

### Comparing `alpaka-job-coverage-1.3.4/tests/test_hipcc.py` & `alpaka-job-coverage-1.3.5/tests/test_hipcc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import unittest
 
-from alpaka_job_coverage.filter_compiler_name import general_compiler_filter
-from alpaka_job_coverage.filter_compiler_version import compiler_version_filter
-from alpaka_job_coverage.filter_backend_version import compiler_backend_filter
-from alpaka_job_coverage.filter_software_dependency import software_dependency_filter
+from alpaka_job_coverage.filter_compiler_name import general_compiler_filter_typed
+from alpaka_job_coverage.filter_compiler_version import compiler_version_filter_typed
+from alpaka_job_coverage.filter_backend_version import compiler_backend_filter_typed
+from alpaka_job_coverage.filter_software_dependency import (
+    software_dependency_filter_typed,
+)
 from alpaka_job_coverage.globals import *
 
 
 def full_filter_chain(row) -> bool:
     return (
-        general_compiler_filter(row)
-        and compiler_version_filter(row)
-        and compiler_backend_filter(row)
-        and software_dependency_filter(row)
+        general_compiler_filter_typed(row)
+        and compiler_version_filter_typed(row)
+        and compiler_backend_filter_typed(row)
+        and software_dependency_filter_typed(row)
     )
 
 
 class TestHipccHostDeviceCompilerBackend(unittest.TestCase):
     def setUp(self):
         global param_map
         # set param_map, that filters expect the following parameters in the
@@ -38,27 +40,27 @@
             [(HIPCC, "4.8")],
             [(HIPCC, "5.0")],
             [(HIPCC, "5.5")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
 
@@ -67,27 +69,27 @@
     def test_host_device_compiler_name(self):
         valid_combs = [
             [(HIPCC, "0"), (HIPCC, "0")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
 
@@ -101,27 +103,27 @@
             [(GCC, "0"), (HIPCC, "0")],
             [(CLANG, "0"), (HIPCC, "0")],
             [(CLANG_CUDA, "0"), (HIPCC, "0")],
         ]
 
         for comb in invalid_combs:
             self.assertFalse(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
 
@@ -132,30 +134,30 @@
             [(HIPCC, "4.8"), (HIPCC, "4.8")],
             [(HIPCC, "5.0"), (HIPCC, "5.0")],
             [(HIPCC, "5.5"), (HIPCC, "5.5")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -165,30 +167,30 @@
             [(HIPCC, "4.4"), (HIPCC, "4.8")],
             [(HIPCC, "5.0"), (HIPCC, "5.2")],
             [(HIPCC, "5.5"), (HIPCC, "4.4")],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertFalse(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -221,33 +223,33 @@
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
                 ],
             ],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
@@ -279,33 +281,33 @@
                     (ALPAKA_ACC_GPU_HIP_ENABLE, "5.5"),
                 ],
             ],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
-                general_compiler_filter(comb),
+                general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                compiler_version_filter(comb),
+                compiler_version_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertFalse(
-                compiler_backend_filter(comb),
+                compiler_backend_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertTrue(
-                software_dependency_filter(comb),
+                software_dependency_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
             self.assertFalse(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
```

### Comparing `alpaka-job-coverage-1.3.4/tests/test_single_rules.py` & `alpaka-job-coverage-1.3.5/tests/test_single_rules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import unittest
 
-from alpaka_job_coverage.filter_compiler_name import general_compiler_filter
-from alpaka_job_coverage.filter_compiler_version import compiler_version_filter
-from alpaka_job_coverage.filter_backend_version import compiler_backend_filter
-from alpaka_job_coverage.filter_software_dependency import software_dependency_filter
+from alpaka_job_coverage.filter_compiler_name import general_compiler_filter_typed
+from alpaka_job_coverage.filter_compiler_version import compiler_version_filter_typed
+from alpaka_job_coverage.filter_backend_version import compiler_backend_filter_typed
+from alpaka_job_coverage.filter_software_dependency import (
+    software_dependency_filter_typed,
+)
 from alpaka_job_coverage.globals import *
 
 # The files contains tests for single, specific rules
 
 
 def full_filter_chain(row) -> bool:
     return (
-        general_compiler_filter(row)
-        and compiler_version_filter(row)
-        and compiler_backend_filter(row)
-        and software_dependency_filter(row)
+        general_compiler_filter_typed(row)
+        and compiler_version_filter_typed(row)
+        and compiler_backend_filter_typed(row)
+        and software_dependency_filter_typed(row)
     )
 
 
-class TestNVCC113GCC103UBUNTU2004(unittest.TestCase):
+class TestNVCC11GCC103UBUNTU2004(unittest.TestCase):
     def setUp(self):
         global param_map
         # set param_map, that filters expect the following parameters in the
         # order
         param_map[HOST_COMPILER] = 0
         param_map[DEVICE_COMPILER] = 1
         param_map[UBUNTU] = 2
@@ -31,39 +33,51 @@
     def setDown(self):
         global param_map
         # reset param_map for following up tests
         param_map = {}
 
     # test if nvcc 11.3 + gcc 10 + Ubuntu 20.04 is disabled
     def test_forbid_combination(self):
-        comb = [(GCC, "10"), (NVCC, "11.3"), (UBUNTU, "20.04")]
+        for nvcc_version in ["11.0", "11.1", "11.2", "11.3"]:
+            comb = [(GCC, "10"), (NVCC, nvcc_version), (UBUNTU, "20.04")]
 
-        self.assertTrue(
-            general_compiler_filter(comb),
-            f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
-            f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
-            f"UBUNTU: {comb[2][1]}",
-        )
-        self.assertTrue(
-            compiler_version_filter(comb),
-            f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
-            f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
-            f"UBUNTU: {comb[2][1]}",
-        )
-        self.assertTrue(
-            compiler_backend_filter(comb),
-            f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
-            f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
-            f"UBUNTU: {comb[2][1]}",
-        )
-        self.assertFalse(
-            software_dependency_filter(comb),
-            f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
-            f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
-            f"UBUNTU: {comb[2][1]}",
-        )
-        self.assertFalse(
-            full_filter_chain(comb),
-            f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
-            f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
-            f"UBUNTU: {comb[2][1]}",
-        )
+            self.assertTrue(
+                general_compiler_filter_typed(comb),
+                f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                f"UBUNTU: {comb[2][1]}",
+            )
+
+            # nvcc 11.0 does not support GCC 10
+            if nvcc_version != "11.0":
+                self.assertTrue(
+                    compiler_version_filter_typed(comb),
+                    f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                    f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                    f"UBUNTU: {comb[2][1]}",
+                )
+            else:
+                self.assertFalse(
+                    compiler_version_filter_typed(comb),
+                    f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                    f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                    f"UBUNTU: {comb[2][1]}",
+                )
+
+            self.assertTrue(
+                compiler_backend_filter_typed(comb),
+                f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                f"UBUNTU: {comb[2][1]}",
+            )
+            self.assertFalse(
+                software_dependency_filter_typed(comb),
+                f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                f"UBUNTU: {comb[2][1]}",
+            )
+            self.assertFalse(
+                full_filter_chain(comb),
+                f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
+                f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
+                f"UBUNTU: {comb[2][1]}",
+            )
```

### Comparing `alpaka-job-coverage-1.3.4/tests/test_util.py` & `alpaka-job-coverage-1.3.5/tests/test_util.py`

 * *Files identical despite different names*

