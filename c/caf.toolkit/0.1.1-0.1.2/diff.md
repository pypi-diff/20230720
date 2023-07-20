# Comparing `tmp/caf.toolkit-0.1.1.tar.gz` & `tmp/caf.toolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.toolkit-0.1.1.tar", last modified: Tue Apr 25 07:11:53 2023, max compression
+gzip compressed data, was "caf.toolkit-0.1.2.tar", last modified: Thu Jul 20 09:19:22 2023, max compression
```

## Comparing `caf.toolkit-0.1.1.tar` & `caf.toolkit-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/caf/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/array_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/config_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/df_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/numpy_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    41797 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/caf/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/array_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/config_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21770 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/df_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/numpy_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29378 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41120 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_translation.py
```

### Comparing `caf.toolkit-0.1.1/LICENSE` & `caf.toolkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/PKG-INFO` & `caf.toolkit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.1 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.2 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `caf.toolkit-0.1.1/README.md` & `caf.toolkit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/pyproject.toml` & `caf.toolkit-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "too-many-lines",
     "use-dict-literal",
     "use-list-literal",
 ]
 
 # Pylint settings
 [tool.pylint.basic]
-good-names = ["df", "fn", "ca", "tp", "to", "x", "i", "f", "q"]
+good-names = ["df", "fn", "ca", "tp", "to", "x", "x1", "x2", "i", "f", "q"]
 extension-pkg-allow-list = ["pydantic"]
 
 [tool.pylint.main]
 ignore = ["__init__.py", "_version.py", "versioneer.py"]
 
 [tool.pylint.design]
 max-args = 10
```

### Comparing `caf.toolkit-0.1.1/setup.cfg` & `caf.toolkit-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/array_utils.py` & `caf.toolkit-0.1.2/src/caf/toolkit/array_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py` & `caf.toolkit-0.1.2/src/caf/toolkit/concurrency/multiprocessing_wrapper.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/config_base.py` & `caf.toolkit-0.1.2/src/caf/toolkit/config_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -120,14 +120,39 @@
             Path to YAML file to output.
         """
         # pylint: disable = unspecified-encoding
         with open(path, "wt") as file:
             file.write(self.to_yaml())
         # pylint: enable = unspecified-encoding
 
+    @classmethod
+    def write_example(cls, path_: Path, /, **examples: str) -> None:
+        """Write examples to a config file.
+
+        Parameters
+        ----------
+        path_ : Path
+            Path to the YAML file to write.
+        examples : str
+            Fields of the config to write, any missing fields
+            are filled in with their default value (if they have
+            one) or 'REQUIRED' / 'OPTIONAL'.
+        """
+        data = {}
+        for name, field in cls.__fields__.items():
+            if field.default is not None:
+                value = field.default
+            else:
+                value = "REQUIRED" if field.required else "OPTIONAL"
+
+            data[name] = examples.get(name, value)
+
+        example = cls.construct(_fields_set=None, **data)
+        example.save_yaml(path_)
+
 
 # # # FUNCTIONS # # #
 def _remove_none_dict(data: dict) -> dict:
     """Remove items recursively from dictionary which are None."""
     filtered = {}
 
     for key, value in data.items():
```

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/cost_utils.py` & `caf.toolkit-0.1.2/src/caf/toolkit/cost_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/io.py` & `caf.toolkit-0.1.2/src/caf/toolkit/io.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/iterative_proportional_fitting.py` & `caf.toolkit-0.1.2/src/caf/toolkit/iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/math_utils.py` & `caf.toolkit-0.1.2/src/caf/toolkit/math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/df_handling.py` & `caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/df_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,27 +417,27 @@
     df: pd.DataFrame,
     index_dict: Mapping[str, Optional[list[Any]]],
     infill: Any = 0,
     check_totals: bool = False,
 ) -> pd.DataFrame:
     """Infill columns with a complete product of one another.
 
-    Infills missing values of df in `index_cols.keys()` columns by generating
+    Infills missing values of df in `index_dict.keys()` columns by generating
     a new MultiIndex from a product of the values in `index_cols.values()`.
-    Where a None-like values is given, all unique values are taken from `df`
+    Where a None-like value is given, all unique values are taken from `df`
     in that column.
 
     Parameters
     ----------
     df:
         The dataframe, in long format, to infill.
 
     index_dict:
         A dictionary mapping the columns of `df` to infill, and with what
-        values. Where a None-like values is given, all unique values are taken
+        values. Where a None-like value is given, all unique values are taken
         from `df` in that column.
         i.e, `df[index_col].unique()` will be used.
 
     infill:
         The value to use to infill any missing cells in the return DataFrame.
 
     check_totals:
@@ -598,15 +598,14 @@
 
     # Convert to wide
     df = df.pivot(
         index=index_col,
         columns=columns_col,
         values=values_col,
     )
-
     return df
 
 
 def wide_to_long_infill(
     df: pd.DataFrame,
     index_col_1_name: str,
     index_col_2_name: str,
```

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/numpy_conversions.py` & `caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/numpy_conversions.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/timing.py` & `caf.toolkit-0.1.2/src/caf/toolkit/timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/toolbox.py` & `caf.toolkit-0.1.2/src/caf/toolkit/toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/tqdm_utils.py` & `caf.toolkit-0.1.2/src/caf/toolkit/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/translation.py` & `caf.toolkit-0.1.2/src/caf/toolkit/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,16 +300,17 @@
             matrix=matrix,
             row_translation=row_translation,
             col_translation=col_translation,
         )
 
     # ## CONVERT DTYPES ## #
     if translation_dtype is None:
-        dtypes = [matrix.dtype, row_translation.dtype, col_translation.dtype]
-        translation_dtype = np.find_common_type(dtypes, [])
+        translation_dtype = np.promote_types(row_translation.dtype, col_translation.dtype)
+        translation_dtype = np.promote_types(translation_dtype, matrix.dtype)
+    assert translation_dtype is not None
     matrix = _convert_dtypes(
         arr=matrix,
         to_type=translation_dtype,
         arr_name="matrix",
     )
     row_translation = _convert_dtypes(
         arr=row_translation,
@@ -621,30 +622,23 @@
     col_translation = pd_utils.reindex_cols(
         df=col_translation,
         columns=columns,
         throw_error=True,
         dataframe_name="col_translation",
     )
 
-    # Check the matrix and translation dtypes match
-    if matrix.index.dtype != row_translation[translation_from_col].dtype:
-        raise ValueError(
-            "dtypes of `matrix.index` and `translation` in `from_zone_col` "
-            "must match.\n"
-            f"Matrix index data type: {matrix.index.dtype}\n"
-            f"Row Translation data type: {row_translation[translation_from_col].dtype}"
-        )
-
-    if matrix.columns.dtype != col_translation[translation_from_col].dtype:
-        raise ValueError(
-            "dtypes of `matrix.columns` and `col_translation` in `from_zone_col` "
-            "must match.\n"
-            f"Matrix column Dtype: {matrix.columns.dtype}\n"
-            f"Col Translation data type: {col_translation[translation_from_col].dtype}"
-        )
+    # Set the dtypes to match
+    matrix.index, row_translation[translation_from_col] = pd_utils.cast_to_common_type(
+        matrix.index,
+        row_translation[translation_from_col],
+    )
+    matrix.columns, col_translation[translation_from_col] = pd_utils.cast_to_common_type(
+        matrix.columns,
+        col_translation[translation_from_col],
+    )
 
     validators.unique_list(from_unique_index, name="from_unique_index")
     validators.unique_list(to_unique_index, name="to_unique_index")
 
     # Make sure the matrix only has the zones defined in from_unique_zones
     missing_rows = set(matrix.index.to_list()) - set(from_unique_index)
     if len(missing_rows) > 0:
@@ -723,14 +717,15 @@
     to_unique_index: list[Any],
     translation_dtype: Optional[np.dtype] = None,
     vector_infill: float = 0.0,
     translate_infill: float = 0.0,
     check_totals: bool = True,
 ) -> pd.Series:
     # pylint: disable=too-many-arguments
+    # pylint: disable=too-many-locals
     """Efficiently translates a pandas vector between index systems.
 
     Internally, checks and converts the pandas inputs into numpy arrays
     and calls `numpy_vector_zone_translation()`. The final output is then
     converted back into a pandas Series, using the same format as the input.
 
     Parameters
@@ -793,22 +788,19 @@
         if vector.shape[1] != 1:
             raise ValueError(
                 "`vector` must be a pandas.Series, or a pandas.DataFrame with "
                 f"one column. Got a DataFrame of shape {vector.shape} instead"
             )
         vector = vector[vector.columns[0]]
 
-    # Check the matrix and translation dtypes match
-    if vector.index.dtype != translation[translation_from_col].dtype:
-        raise ValueError(
-            "dtypes of `vector.index` and `translation` in `from_zone_col` "
-            "must match.\n"
-            f"vector index data type: {vector.index.dtype}\n"
-            f"translation[from_zone_col] data type: {translation[translation_from_col].dtype}"
-        )
+    # Set the dtypes to match
+    vector.index, translation[translation_from_col] = pd_utils.cast_to_common_type(
+        vector.index,
+        translation[translation_from_col],
+    )
 
     validators.unique_list(from_unique_index, name="from_unique_index")
     validators.unique_list(to_unique_index, name="to_unique_index")
 
     # Make sure the vector only has the zones defined in from_unique_zones
     missing_rows = set(vector.index.to_list()) - set(from_unique_index)
     if len(missing_rows) > 0:
```

### Comparing `caf.toolkit-0.1.1/src/caf/toolkit/validators.py` & `caf.toolkit-0.1.2/src/caf/toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/src/caf.toolkit.egg-info/PKG-INFO` & `caf.toolkit-0.1.2/src/caf.toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.1 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.2 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `caf.toolkit-0.1.1/src/caf.toolkit.egg-info/SOURCES.txt` & `caf.toolkit-0.1.2/src/caf.toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/caf/toolkit/concurrency/__init__.py
 src/caf/toolkit/concurrency/multiprocessing_wrapper.py
 src/caf/toolkit/core/__init__.py
 src/caf/toolkit/core/types.py
 src/caf/toolkit/pandas_utils/__init__.py
 src/caf/toolkit/pandas_utils/df_handling.py
 src/caf/toolkit/pandas_utils/numpy_conversions.py
+src/caf/toolkit/pandas_utils/utility.py
 tests/test_array_utils.py
 tests/test_config_base.py
 tests/test_cost_utils.py
 tests/test_io.py
 tests/test_iterative_proportional_fitting.py
 tests/test_math_utils.py
 tests/test_timing.py
```

### Comparing `caf.toolkit-0.1.1/tests/test_array_utils.py` & `caf.toolkit-0.1.2/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_config_base.py` & `caf.toolkit-0.1.2/tests/test_config_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Tests for the config_base module in caf.toolkit
 """
 # Built-Ins
 from pathlib import Path
 import dataclasses
+import pathlib
 
 # Third Party
 import pytest
 
 # pylint: disable=import-error
 from pydantic import ValidationError
 
@@ -227,8 +228,66 @@
         None
         """
         file_path = path / "save_test.yml"
         basic.save_yaml(file_path)
         assert ConfigTestClass.load_yaml(file_path) == basic
 
 
+class TestExample:
+    """Test writing the example file is correct."""
+
+    def write_example(self, path_: pathlib.Path, /, **kwargs) -> str:
+        """Run `ConfigTestClass.write_example` and read output."""
+        example_file = path_ / "test_example.yml"
+        ConfigTestClass.write_example(example_file, **kwargs)
+
+        with open(example_file, "rt", encoding="utf-8") as file:
+            return file.read()
+
+    def test_default_example(self, path: pathlib.Path) -> None:
+        """Write example without descriptions."""
+        example = self.write_example(path)
+
+        expected = (
+            "dictionary: REQUIRED\n"
+            "path: REQUIRED\n"
+            "list: REQUIRED\n"
+            "set: REQUIRED\n"
+            "tuple: REQUIRED\n"
+            "sub: OPTIONAL\n"
+            "default: yes\n"
+            "option: OPTIONAL\n"
+        )
+
+        assert example == expected, "Write example without descriptions"
+
+    def test_example(self, path: pathlib.Path) -> None:
+        """Write example with descriptions."""
+        example_values = dict(
+            dictionary="This is a dictionary",
+            path="This is a path",
+            list="This is a list",
+            set="This is a set",
+            tuple="Two paths to files",
+            sub=TestSubClass("integer value", "decimal value"),
+            default="This value defaults to true",
+            option="This value is optional",
+        )
+        example = self.write_example(path, **example_values)
+
+        expected = (
+            "dictionary: {dictionary}\n"
+            "path: {path}\n"
+            "list: {list}\n"
+            "set: {set}\n"
+            "tuple: {tuple}\n"
+            "sub:\n"
+            "  whole: integer value\n"
+            "  decimal: decimal value\n"
+            "default: {default}\n"
+            "option: {option}\n"
+        ).format(**example_values)
+
+        assert example == expected, "Write example with descriptions"
+
+
 # # # FUNCTIONS # # #
```

### Comparing `caf.toolkit-0.1.1/tests/test_cost_utils.py` & `caf.toolkit-0.1.2/tests/test_cost_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_io.py` & `caf.toolkit-0.1.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_iterative_proportional_fitting.py` & `caf.toolkit-0.1.2/tests/test_iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_math_utils.py` & `caf.toolkit-0.1.2/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_timing.py` & `caf.toolkit-0.1.2/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_toolbox.py` & `caf.toolkit-0.1.2/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.1/tests/test_translation.py` & `caf.toolkit-0.1.2/tests/test_translation.py`

 * *Files 11% similar despite different names*

```diff
@@ -207,14 +207,17 @@
 
     def __post_init__(self, np_matrix: np.ndarray, np_expected_result: np.ndarray):
         """Convert numpy objects to pandas"""
         # Base from / to zones on translation
         self.from_unique_index = self.translation.unique_from
         self.to_unique_index = self.translation.unique_to
 
+        if self.col_translation is None:
+            self.col_translation = self.translation.copy()
+
         # Input and results
         self.mat = pd.DataFrame(
             data=np_matrix,
             index=self.from_unique_index,
             columns=self.from_unique_index,
         )
         self.expected_result = pd.DataFrame(
@@ -777,51 +780,14 @@
 
         # Run with errors
         with pytest.raises(ValueError, match=msg):
             translation.pandas_vector_zone_translation(
                 **(pd_vector_split.input_kwargs() | new_kwargs)
             )
 
-    @pytest.mark.parametrize("dtype1", [np.float64, np.int64, str])
-    @pytest.mark.parametrize("dtype2", [np.float64, np.int64, str])
-    def test_col_dtypes(
-        self,
-        pd_vector_split: PandasVectorResults,
-        dtype1: type,
-        dtype2: type,
-    ):
-        """Check that correct errors are thrown when types don't match"""
-        # Cast types
-        new_vector = pd_vector_split.vector.copy()
-        new_vector.index = new_vector.index.astype(dtype1)
-        new_trans = pd_vector_split.translation.copy()
-        new_trans.from_col = new_trans.from_col.astype(dtype2)
-        new_kwargs = {"vector": new_vector, "translation": new_trans.df}
-
-        if dtype1 == str and dtype2 == str:
-            # Pandas handles strings weirdly (as objects), making this hard to test
-            pass
-        elif dtype1 == dtype2:
-            # Should run normally with matching dtypes
-            result = translation.pandas_vector_zone_translation(
-                **(pd_vector_split.input_kwargs() | new_kwargs)
-            )
-            pd.testing.assert_series_equal(
-                result,
-                pd_vector_split.expected_result,
-                check_names=False,
-            )
-        else:
-            # Only throw error when not matching types
-            msg = "dtypes of `vector.index` and `translation` in `from_zone_col` must match."
-            with pytest.raises(ValueError, match=msg):
-                translation.pandas_vector_zone_translation(
-                    **(pd_vector_split.input_kwargs() | new_kwargs)
-                )
-
     def test_non_vector(self, pd_vector_split: PandasVectorResults):
         """Test that an error is thrown when a non-vector is passed in"""
         new_vector = pd.DataFrame(pd_vector_split.vector)
         new_vector[1] = new_vector[0].copy()
         with pytest.raises(ValueError, match="must be a pandas.Series"):
             translation.pandas_vector_zone_translation(
                 **(pd_vector_split.input_kwargs() | {"vector": new_vector})
@@ -857,14 +823,32 @@
         """
         pd_vector = request.getfixturevalue(pd_vector_str)
         result = translation.pandas_vector_zone_translation(
             **pd_vector.input_kwargs(check_totals=check_totals)
         )
         pd.testing.assert_series_equal(result, pd_vector.expected_result)
 
+    @pytest.mark.parametrize(
+        "pd_vector_str",
+        ["pd_vector_aggregation", "pd_vector_split"],
+    )
+    def test_check_allow_similar_types(
+        self,
+        pd_vector_str: str,
+        request,
+    ):
+        """Test that similar types are allowed in translation and data."""
+        pd_vector = request.getfixturevalue(pd_vector_str)
+        new_trans = pd_vector.translation.copy()
+        new_trans.from_col = new_trans.from_col.astype(np.int32)
+        result = translation.pandas_vector_zone_translation(
+            **(pd_vector.input_kwargs() | {"translation": new_trans.df})
+        )
+        pd.testing.assert_series_equal(result, pd_vector.expected_result)
+
 
 @pytest.mark.usefixtures(
     "np_matrix_aggregation",
     "np_matrix_aggregation2",
     "np_matrix_split",
     "np_matrix_dtype",
     "np_matrix_incomplete",
@@ -1038,67 +1022,14 @@
 
         # Run with errors
         with pytest.raises(ValueError, match=msg):
             translation.pandas_matrix_zone_translation(
                 **(pd_matrix_split.input_kwargs() | new_kwargs)
             )
 
-    @pytest.mark.parametrize("mat_dtype", [np.float64, np.int64, str])
-    @pytest.mark.parametrize("row_translation_dtype", [np.float64, np.int64, str])
-    def test_col_dtypes(
-        self,
-        pd_matrix_split: PandasMatrixResults,
-        mat_dtype: type,
-        row_translation_dtype: type,
-        col_translation_dtype: type = np.float64,
-    ):
-        """Check that correct errors are thrown when types don't match"""
-        # Cast types
-        new_matrix = pd_matrix_split.mat.copy()
-        new_matrix.index = new_matrix.index.astype(mat_dtype)
-        new_matrix.columns = new_matrix.columns.astype(mat_dtype)
-
-        new_trans = pd_matrix_split.translation.copy()
-        new_trans.from_col = new_trans.from_col.astype(row_translation_dtype)
-        col_trans = pd_matrix_split.translation.copy()
-        col_trans.from_col = col_trans.from_col.astype(col_translation_dtype)
-        new_kwargs = {
-            "matrix": new_matrix,
-            "translation": new_trans.df,
-            "col_translation": col_trans.df,
-        }
-
-        if mat_dtype == str and row_translation_dtype == str:
-            # Pandas handles strings weirdly (as objects), making this hard to test
-            pass
-        elif mat_dtype == row_translation_dtype == col_translation_dtype:
-            # Should run normally with matching dtypes
-            result = translation.pandas_matrix_zone_translation(
-                **(pd_matrix_split.input_kwargs() | new_kwargs)
-            )
-            pd.testing.assert_frame_equal(
-                result,
-                pd_matrix_split.expected_result,
-                check_names=False,
-            )
-        elif mat_dtype == row_translation_dtype:
-            # If the row matches, but the column doesn't
-            msg = "dtypes of `matrix.columns` and `col_translation` in `from_zone_col` must match."
-            with pytest.raises(ValueError, match=msg):
-                translation.pandas_matrix_zone_translation(
-                    **(pd_matrix_split.input_kwargs() | new_kwargs)
-                )
-        else:
-            # If row row and data dtypes don't match
-            msg = "dtypes of `matrix.index` and `translation` in `from_zone_col` must match."
-            with pytest.raises(ValueError, match=msg):
-                translation.pandas_matrix_zone_translation(
-                    **(pd_matrix_split.input_kwargs() | new_kwargs)
-                )
-
     @pytest.mark.parametrize(
         "pd_matrix_str",
         [
             "pd_matrix_aggregation",
             "pd_matrix_aggregation2",
             "pd_matrix_split",
             "pd_matrix_dtype",
@@ -1145,7 +1076,82 @@
         translation splitting.
         """
         pd_mat = request.getfixturevalue(pd_matrix_str)
         result = translation.pandas_matrix_zone_translation(
             **pd_mat.input_kwargs(check_totals=check_totals)
         )
         pd.testing.assert_frame_equal(result, pd_mat.expected_result)
+
+    @pytest.mark.parametrize(
+        "pd_matrix_str",
+        [
+            "pd_matrix_aggregation",
+            "pd_matrix_aggregation2",
+            "pd_matrix_split",
+            "pd_matrix_dtype",
+        ],
+    )
+    @pytest.mark.parametrize("row", [True, False])
+    def test_check_allow_similar_types(
+        self,
+        pd_matrix_str: str,
+        row: bool,
+        request,
+    ):
+        """Test that similar types are allowed in translation and data."""
+        pd_mat = request.getfixturevalue(pd_matrix_str)
+
+        # Change the dtype of the row / col
+        if row:
+            new_trans = pd_mat.translation.copy()
+            keyword = "translation"
+        else:
+            new_trans = pd_mat.col_translation.copy()
+            keyword = "col_translation"
+
+        # Run the translation
+        new_trans.from_col = new_trans.from_col.astype(np.int32)
+        result = translation.pandas_matrix_zone_translation(
+            **(pd_mat.input_kwargs() | {keyword: new_trans.df})
+        )
+        pd.testing.assert_frame_equal(result, pd_mat.expected_result)
+
+    @pytest.mark.parametrize(
+        "pd_matrix_str",
+        [
+            "pd_matrix_aggregation",
+            "pd_matrix_aggregation2",
+            "pd_matrix_split",
+            "pd_matrix_dtype",
+        ],
+    )
+    @pytest.mark.parametrize("row", [True, False])
+    @pytest.mark.parametrize("trans_dtype", [str, int, float])
+    @pytest.mark.parametrize("matrix_dtype", [str, int, float])
+    def test_allow_different_types(
+        self,
+        pd_matrix_str: str,
+        row: bool,
+        trans_dtype: type,
+        matrix_dtype: type,
+        request,
+    ):
+        """Test that similar types are allowed in translation and data."""
+        pd_mat = request.getfixturevalue(pd_matrix_str)
+
+        # Change the dtype of the row / col
+        new_matrix = pd_mat.mat.copy()
+        if row:
+            new_trans = pd_mat.translation.copy()
+            keyword = "translation"
+            new_matrix.index = new_matrix.index.astype(matrix_dtype)
+        else:
+            new_trans = pd_mat.col_translation.copy()
+            keyword = "col_translation"
+            new_matrix.columns = new_matrix.columns.astype(matrix_dtype)
+
+        # Run the translation
+        new_trans.from_col = new_trans.from_col.astype(trans_dtype)
+        result = translation.pandas_matrix_zone_translation(
+            **(pd_mat.input_kwargs() | {keyword: new_trans.df})
+        )
+        pd.testing.assert_frame_equal(result, pd_mat.expected_result)
```

