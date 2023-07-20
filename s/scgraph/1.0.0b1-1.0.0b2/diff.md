# Comparing `tmp/scgraph-1.0.0b1.tar.gz` & `tmp/scgraph-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-1.0.0b1.tar", last modified: Thu Jul 20 20:19:22 2023, max compression
+gzip compressed data, was "scgraph-1.0.0b2.tar", last modified: Thu Jul 20 20:32:36 2023, max compression
```

## Comparing `scgraph-1.0.0b1.tar` & `scgraph-1.0.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.0.0b1/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     6084 2023-07-20 20:14:59.000000 scgraph-1.0.0b1/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      109 2023-07-20 20:16:30.000000 scgraph-1.0.0b1/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-07-20 20:10:57.000000 scgraph-1.0.0b1/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    20565 2023-07-20 19:09:42.000000 scgraph-1.0.0b1/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:10:31.000000 scgraph-1.0.0b1/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143458 2023-07-20 20:16:35.000000 scgraph-1.0.0b1/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2150 2023-07-20 18:43:41.000000 scgraph-1.0.0b1/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      286 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      973 2023-07-20 20:19:15.000000 scgraph-1.0.0b1/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.0.0b2/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     6084 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      109 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    20565 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:28:13.000000 scgraph-1.0.0b2/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143458 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2150 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      286 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      953 2023-07-20 20:32:23.000000 scgraph-1.0.0b2/setup.py
```

### Comparing `scgraph-1.0.0b1/LICENSE` & `scgraph-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b1/PKG-INFO` & `scgraph-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b1.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `scgraph-1.0.0b1/README.md` & `scgraph-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b1/scgraph/core.py` & `scgraph-1.0.0b2/scgraph/core.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b1/scgraph/geographs/marnet.py` & `scgraph-1.0.0b2/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b1/scgraph/utils.py` & `scgraph-1.0.0b2/scgraph/utils.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b1/scgraph.egg-info/PKG-INFO` & `scgraph-1.0.0b2/scgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b1.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `scgraph-1.0.0b1/setup.py` & `scgraph-1.0.0b2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from distutils.core import setup
-from setuptools import find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scgraph',
-  packages = find_packages(),
-  version = '1.0.0b1',
+  packages = ['scgraph', 'scgraph.geographs'],
+  version = '1.0.0b2',
   license='MIT',
   description = 'Determine an approximate route between two points on earth',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/connor-makowski/scgraph',
-  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b1.tar.gz',
+  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz',
   keywords = ['scgraph'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

