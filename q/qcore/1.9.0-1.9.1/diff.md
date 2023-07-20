# Comparing `tmp/qcore-1.9.0.tar.gz` & `tmp/qcore-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcore-1.9.0.tar", last modified: Fri May 26 03:43:20 2023, max compression
+gzip compressed data, was "qcore-1.9.1.tar", last modified: Thu Jul 20 18:36:18 2023, max compression
```

## Comparing `qcore-1.9.0.tar` & `qcore-1.9.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-26 03:43:16.000000 qcore-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-26 03:43:20.008219 qcore-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-26 03:43:16.000000 qcore-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 03:43:16.000000 qcore-1.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/asserts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/disallow_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/disallow_inheritance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspectable_class.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspectable_class.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/testing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_disallow_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_inspectable_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_microtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:43:20.008219 qcore-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-26 03:43:16.000000 qcore-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:36:18.707202 qcore-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 18:36:13.000000 qcore-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-20 18:36:18.707202 qcore-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-20 18:36:13.000000 qcore-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 18:36:13.000000 qcore-1.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:36:18.707202 qcore-1.9.1/qcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/asserts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/caching.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/caching.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/decorators.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/disallow_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/disallow_inheritance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/events.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/helpers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/inspectable_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/inspectable_class.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/inspection.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/microtime.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/microtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/microtime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/testing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:36:18.707202 qcore-1.9.1/qcore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_disallow_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_inspectable_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_microtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-20 18:36:13.000000 qcore-1.9.1/qcore/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:36:18.707202 qcore-1.9.1/qcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-20 18:36:18.000000 qcore-1.9.1/qcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-20 18:36:18.000000 qcore-1.9.1/qcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:36:18.000000 qcore-1.9.1/qcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 18:36:18.000000 qcore-1.9.1/qcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 18:36:18.000000 qcore-1.9.1/qcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:36:18.707202 qcore-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-20 18:36:13.000000 qcore-1.9.1/setup.py
```

### Comparing `qcore-1.9.0/LICENSE` & `qcore-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/PKG-INFO` & `qcore-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcore
-Version: 1.9.0
+Version: 1.9.1
 Summary: Quora's core utility library
 Home-page: https://github.com/quora/qcore
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
 Keywords: quora core common utility
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qcore-1.9.0/README.rst` & `qcore-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/__init__.py` & `qcore-1.9.1/qcore/__init__.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/__init__.pyi` & `qcore-1.9.1/qcore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/asserts.py` & `qcore-1.9.1/qcore/asserts.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/asserts.pyi` & `qcore-1.9.1/qcore/asserts.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/caching.pxd` & `qcore-1.9.1/qcore/caching.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/caching.py` & `qcore-1.9.1/qcore/caching.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/caching.pyi` & `qcore-1.9.1/qcore/caching.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/debug.py` & `qcore-1.9.1/qcore/debug.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/debug.pyi` & `qcore-1.9.1/qcore/debug.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/decorators.pxd` & `qcore-1.9.1/qcore/decorators.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/decorators.py` & `qcore-1.9.1/qcore/decorators.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/decorators.pyi` & `qcore-1.9.1/qcore/decorators.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/disallow_inheritance.py` & `qcore-1.9.1/qcore/disallow_inheritance.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/enum.py` & `qcore-1.9.1/qcore/enum.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/enum.pyi` & `qcore-1.9.1/qcore/enum.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/errors.py` & `qcore-1.9.1/qcore/errors.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/errors.pyi` & `qcore-1.9.1/qcore/errors.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/events.pxd` & `qcore-1.9.1/qcore/events.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/events.py` & `qcore-1.9.1/qcore/events.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/events.pyi` & `qcore-1.9.1/qcore/events.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/helpers.pxd` & `qcore-1.9.1/qcore/helpers.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/helpers.py` & `qcore-1.9.1/qcore/helpers.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/helpers.pyi` & `qcore-1.9.1/qcore/helpers.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/inspectable_class.py` & `qcore-1.9.1/qcore/inspectable_class.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/inspection.pxd` & `qcore-1.9.1/qcore/inspection.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/inspection.py` & `qcore-1.9.1/qcore/inspection.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/inspection.pyi` & `qcore-1.9.1/qcore/inspection.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/microtime.pxd` & `qcore-1.9.1/qcore/microtime.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/microtime.py` & `qcore-1.9.1/qcore/microtime.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/microtime.pyi` & `qcore-1.9.1/qcore/microtime.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/testing.py` & `qcore-1.9.1/qcore/testing.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_asserts.py` & `qcore-1.9.1/qcore/tests/test_asserts.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_caching.py` & `qcore-1.9.1/qcore/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_debug.py` & `qcore-1.9.1/qcore/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_decorators.py` & `qcore-1.9.1/qcore/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_enum.py` & `qcore-1.9.1/qcore/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_errors.py` & `qcore-1.9.1/qcore/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_events.py` & `qcore-1.9.1/qcore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_examples.py` & `qcore-1.9.1/qcore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_helpers.py` & `qcore-1.9.1/qcore/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_inspectable_class.py` & `qcore-1.9.1/qcore/tests/test_inspectable_class.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_inspection.py` & `qcore-1.9.1/qcore/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_microtime.py` & `qcore-1.9.1/qcore/tests/test_microtime.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore/tests/test_testing.py` & `qcore-1.9.1/qcore/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/qcore.egg-info/PKG-INFO` & `qcore-1.9.1/qcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcore
-Version: 1.9.0
+Version: 1.9.1
 Summary: Quora's core utility library
 Home-page: https://github.com/quora/qcore
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
 Keywords: quora core common utility
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qcore-1.9.0/qcore.egg-info/SOURCES.txt` & `qcore-1.9.1/qcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qcore-1.9.0/setup.py` & `qcore-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 DATA_FILES = (
     ["py.typed"]
     + ["%s.pxd" % module for module in CYTHON_MODULES]
     + [os.path.relpath(f, "qcore/") for f in glob.glob("qcore/*.pyi")]
 )
 
 
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 
 
 EXTENSIONS = [
     Extension("qcore.%s" % module, ["qcore/%s.py" % module])
     for module in CYTHON_MODULES
 ]
 
@@ -68,10 +68,10 @@
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
         keywords="quora core common utility",
         packages=["qcore", "qcore.tests"],
         package_data={"qcore": DATA_FILES},
         ext_modules=EXTENSIONS,
-        setup_requires=["Cython"],
+        setup_requires=["Cython==0.29.36"],
         install_requires=["Cython"],
     )
```

