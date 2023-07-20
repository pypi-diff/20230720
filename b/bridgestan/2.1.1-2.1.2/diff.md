# Comparing `tmp/bridgestan-2.1.1.tar.gz` & `tmp/bridgestan-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgestan-2.1.1.tar", last modified: Fri Jun 30 18:36:30 2023, max compression
+gzip compressed data, was "bridgestan-2.1.2.tar", last modified: Thu Jul 20 14:10:13 2023, max compression
```

## Comparing `bridgestan-2.1.1.tar` & `bridgestan-2.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 18:36:30.485672 bridgestan-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 18:33:56.000000 bridgestan-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/bridgestan/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 18:35:45.000000 bridgestan-2.1.1/bridgestan/__version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25859 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/bridgestan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 18:33:56.000000 bridgestan-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-30 18:36:30.485672 bridgestan-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 18:33:56.000000 bridgestan-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25485 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_stanmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:13.236772 bridgestan-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 14:10:13.236772 bridgestan-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-20 14:07:00.000000 bridgestan-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:13.232772 bridgestan-2.1.2/bridgestan/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 14:09:27.000000 bridgestan-2.1.2/bridgestan/__version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25859 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-20 14:07:00.000000 bridgestan-2.1.2/bridgestan/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:13.236772 bridgestan-2.1.2/bridgestan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 14:10:13.000000 bridgestan-2.1.2/bridgestan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 14:10:13.000000 bridgestan-2.1.2/bridgestan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:10:13.000000 bridgestan-2.1.2/bridgestan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 14:10:13.000000 bridgestan-2.1.2/bridgestan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 14:10:13.000000 bridgestan-2.1.2/bridgestan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 14:07:00.000000 bridgestan-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 14:10:13.240772 bridgestan-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 14:07:00.000000 bridgestan-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:10:13.236772 bridgestan-2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 14:07:00.000000 bridgestan-2.1.2/test/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-20 14:07:00.000000 bridgestan-2.1.2/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-07-20 14:07:00.000000 bridgestan-2.1.2/test/test_stanmodel.py
```

### Comparing `bridgestan-2.1.1/PKG-INFO` & `bridgestan-2.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.1.1
+Version: 2.1.2
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.1.1/bridgestan/compile.py` & `bridgestan-2.1.2/bridgestan/compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.1/bridgestan/download.py` & `bridgestan-2.1.2/bridgestan/download.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.1/bridgestan/model.py` & `bridgestan-2.1.2/bridgestan/model.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.1/bridgestan.egg-info/PKG-INFO` & `bridgestan-2.1.2/bridgestan.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.1.1
+Version: 2.1.2
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.1.1/test/test_compile.py` & `bridgestan-2.1.2/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.1/test/test_stanmodel.py` & `bridgestan-2.1.2/test/test_stanmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         bs.StanModel(bernoulli_so, "nope, not going to find it.json")
 
     # test data load exception
     throw_data_so = str(STAN_FOLDER / "throw_data" / "throw_data_model.so")
     with pytest.raises(RuntimeError, match="find this text: datafails"):
         b4 = bs.StanModel(throw_data_so)
 
+    load_sundials = str(STAN_FOLDER / "ode_sundials" / "ode_sundials_model.so")
+    ode_sundials_data = (
+        STAN_FOLDER / "ode_sundials" / "ode_sundials.data.json"
+    ).read_text()
+    bs.StanModel(load_sundials, ode_sundials_data)
+
 
 def test_name():
     std_so = str(STAN_FOLDER / "stdnormal" / "stdnormal_model.so")
     b = bs.StanModel(std_so)
     np.testing.assert_equal("stdnormal_model", b.name())
```

