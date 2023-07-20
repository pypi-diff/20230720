# Comparing `tmp/regtricks-0.3.5.post1.tar.gz` & `tmp/regtricks-0.3.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regtricks-0.3.5.post1.tar", last modified: Thu Jul 20 21:23:44 2023, max compression
+gzip compressed data, was "regtricks-0.3.5.post2.tar", last modified: Thu Jul 20 21:25:27 2023, max compression
```

## Comparing `regtricks-0.3.5.post1.tar` & `regtricks-0.3.5.post2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.879392 regtricks-0.3.5.post1/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/LICENSE
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/MANIFEST.in
--rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:23:44.879155 regtricks-0.3.5.post1/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/README.md
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.877230 regtricks-0.3.5.post1/regtricks/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/__init__.py
--rw-r--r--   0 thomaskirk   (501) staff       (20)       77 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks/_version.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7424 2023-07-10 10:27:24.000000 regtricks-0.3.5.post1/regtricks/application_helpers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15302 2023-07-09 12:24:53.000000 regtricks-0.3.5.post1/regtricks/fnirt_coefficients.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11883 2023-07-10 10:23:15.000000 regtricks-0.3.5.post1/regtricks/image_space.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/multiplication.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.878972 regtricks-0.3.5.post1/regtricks/transforms/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/transforms/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11570 2023-07-09 13:14:48.000000 regtricks-0.3.5.post1/regtricks/transforms/linear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14424 2023-07-10 10:04:05.000000 regtricks-0.3.5.post1/regtricks/transforms/nonlinear.py
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     9434 2023-07-20 21:23:08.000000 regtricks-0.3.5.post1/regtricks/transforms/transform.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3238 2023-07-09 13:15:39.000000 regtricks-0.3.5.post1/regtricks/wrappers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/x5_interface.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.878108 regtricks-0.3.5.post1/regtricks.egg-info/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/SOURCES.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/dependency_links.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/requires.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/top_level.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/requirements.txt
--rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-20 21:23:44.879438 regtricks-0.3.5.post1/setup.cfg
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.5.post1/setup.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:25:27.133998 regtricks-0.3.5.post2/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/LICENSE
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/MANIFEST.in
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:25:27.133779 regtricks-0.3.5.post2/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/README.md
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:25:27.132076 regtricks-0.3.5.post2/regtricks/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/regtricks/__init__.py
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       77 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks/_version.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7424 2023-07-10 10:27:24.000000 regtricks-0.3.5.post2/regtricks/application_helpers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15302 2023-07-09 12:24:53.000000 regtricks-0.3.5.post2/regtricks/fnirt_coefficients.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11883 2023-07-10 10:23:15.000000 regtricks-0.3.5.post2/regtricks/image_space.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/regtricks/multiplication.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:25:27.133589 regtricks-0.3.5.post2/regtricks/transforms/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/regtricks/transforms/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11570 2023-07-09 13:14:48.000000 regtricks-0.3.5.post2/regtricks/transforms/linear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14424 2023-07-10 10:04:05.000000 regtricks-0.3.5.post2/regtricks/transforms/nonlinear.py
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     9437 2023-07-20 21:25:04.000000 regtricks-0.3.5.post2/regtricks/transforms/transform.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3238 2023-07-09 13:15:39.000000 regtricks-0.3.5.post2/regtricks/wrappers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/regtricks/x5_interface.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:25:27.132859 regtricks-0.3.5.post2/regtricks.egg-info/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks.egg-info/requires.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-20 21:25:27.000000 regtricks-0.3.5.post2/regtricks.egg-info/top_level.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.5.post2/requirements.txt
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-20 21:25:27.134049 regtricks-0.3.5.post2/setup.cfg
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.5.post2/setup.py
```

### Comparing `regtricks-0.3.5.post1/LICENSE` & `regtricks-0.3.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/PKG-INFO` & `regtricks-0.3.5.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.5.post1
+Version: 0.3.5.post2
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.5.post1/README.md` & `regtricks-0.3.5.post2/README.md`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/application_helpers.py` & `regtricks-0.3.5.post2/regtricks/application_helpers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/fnirt_coefficients.py` & `regtricks-0.3.5.post2/regtricks/fnirt_coefficients.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/image_space.py` & `regtricks-0.3.5.post2/regtricks/image_space.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/multiplication.py` & `regtricks-0.3.5.post2/regtricks/multiplication.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/linear.py` & `regtricks-0.3.5.post2/regtricks/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/nonlinear.py` & `regtricks-0.3.5.post2/regtricks/transforms/nonlinear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/transform.py` & `regtricks-0.3.5.post2/regtricks/transforms/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             super_ref = ref 
 
         if not ((data.ndim in (3,4)) and (np.array_equal(src.size, data.shape[:3]))): 
             raise ValueError("Data shape {} does not match source space {}"
                                 .format(data.shape, src.size))
 
         # Force to float data 
-        data = data.astype(float32)
+        data = data.astype(np.float32)
 
         # Only use multiprocessing on 4D data 
         if data.ndim == 3: 
             cores = 1 
         else: 
             cores = min([cores, data.shape[-1]])
```

### Comparing `regtricks-0.3.5.post1/regtricks/wrappers.py` & `regtricks-0.3.5.post2/regtricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/x5_interface.py` & `regtricks-0.3.5.post2/regtricks/x5_interface.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks.egg-info/PKG-INFO` & `regtricks-0.3.5.post2/regtricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.5.post1
+Version: 0.3.5.post2
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.5.post1/regtricks.egg-info/SOURCES.txt` & `regtricks-0.3.5.post2/regtricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/setup.py` & `regtricks-0.3.5.post2/setup.py`

 * *Files identical despite different names*

