# Comparing `tmp/pesic-0.1.0.tar.gz` & `tmp/pesic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pesic-0.1.0.tar", last modified: Thu Jul 20 08:54:58 2023, max compression
+gzip compressed data, was "pesic-0.1.2.tar", last modified: Thu Jul 20 10:56:34 2023, max compression
```

## Comparing `pesic-0.1.0.tar` & `pesic-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:58.730124 pesic-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 08:54:47.000000 pesic-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-20 08:54:58.730124 pesic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-20 08:54:47.000000 pesic-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:58.726124 pesic-0.1.0/pesic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:47.000000 pesic-0.1.0/pesic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-20 08:54:47.000000 pesic-0.1.0/pesic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 08:54:47.000000 pesic-0.1.0/pesic/custom_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-20 08:54:47.000000 pesic-0.1.0/pesic/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:58.730124 pesic-0.1.0/pesic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-20 08:54:58.000000 pesic-0.1.0/pesic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 08:54:58.000000 pesic-0.1.0/pesic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:54:58.000000 pesic-0.1.0/pesic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 08:54:58.000000 pesic-0.1.0/pesic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 08:54:58.000000 pesic-0.1.0/pesic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:54:58.730124 pesic-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 08:54:47.000000 pesic-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:56:34.660823 pesic-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 10:56:22.000000 pesic-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-20 10:56:34.660823 pesic-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-20 10:56:22.000000 pesic-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:56:34.660823 pesic-0.1.2/pesic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:56:22.000000 pesic-0.1.2/pesic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-20 10:56:22.000000 pesic-0.1.2/pesic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 10:56:22.000000 pesic-0.1.2/pesic/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-20 10:56:22.000000 pesic-0.1.2/pesic/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:56:34.660823 pesic-0.1.2/pesic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-20 10:56:34.000000 pesic-0.1.2/pesic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 10:56:34.000000 pesic-0.1.2/pesic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:56:34.000000 pesic-0.1.2/pesic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 10:56:34.000000 pesic-0.1.2/pesic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 10:56:34.000000 pesic-0.1.2/pesic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:56:34.660823 pesic-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 10:56:22.000000 pesic-0.1.2/setup.py
```

### Comparing `pesic-0.1.0/LICENSE` & `pesic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pesic-0.1.0/PKG-INFO` & `pesic-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pesic
-Version: 0.1.0
+Version: 0.1.2
 Summary: PetroElectroSbyt API Wrapper
 Home-page: https://github.com/StanislavBolshakov/pesic
 Author: Stanislav Bolshakov
 Author-email: st.bolshakov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pesic-0.1.0/README.md` & `pesic-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pesic-0.1.0/pesic/client.py` & `pesic-0.1.2/pesic/client.py`

 * *Files identical despite different names*

### Comparing `pesic-0.1.0/pesic/custom_exceptions.py` & `pesic-0.1.2/pesic/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `pesic-0.1.0/pesic/wrapper.py` & `pesic-0.1.2/pesic/wrapper.py`

 * *Files identical despite different names*

### Comparing `pesic-0.1.0/pesic.egg-info/PKG-INFO` & `pesic-0.1.2/pesic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pesic
-Version: 0.1.0
+Version: 0.1.2
 Summary: PetroElectroSbyt API Wrapper
 Home-page: https://github.com/StanislavBolshakov/pesic
 Author: Stanislav Bolshakov
 Author-email: st.bolshakov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pesic-0.1.0/setup.py` & `pesic-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="pesic",
-    version="0.1.0",
+    version="0.1.2",
     author="Stanislav Bolshakov",
     author_email="st.bolshakov@gmail.com",
     url="https://github.com/StanislavBolshakov/pesic",
     description="PetroElectroSbyt API Wrapper",
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

