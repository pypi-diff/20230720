# Comparing `tmp/buscador-0.6.tar.gz` & `tmp/buscador-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.6.tar", last modified: Thu Jul 20 14:41:39 2023, max compression
+gzip compressed data, was "buscador-0.7.tar", last modified: Thu Jul 20 15:52:35 2023, max compression
```

## Comparing `buscador-0.6.tar` & `buscador-0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.845123 buscador-0.6/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.6/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 14:41:39.845371 buscador-0.6/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      697 2023-07-20 13:47:30.000000 buscador-0.6/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.841645 buscador-0.6/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.6/buscador/__init__.py
--rw-r--r--   0 samcook    (501) staff       (20)      485 2023-07-20 14:41:31.000000 buscador-0.6/buscador/classFindValue.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 14:41:39.844658 buscador-0.6/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       13 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 14:41:39.000000 buscador-0.6/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 14:41:39.845971 buscador-0.6/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)      964 2023-07-20 14:41:31.000000 buscador-0.6/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.071670 buscador-0.7/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.7/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 15:52:35.071945 buscador-0.7/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      760 2023-07-20 14:43:59.000000 buscador-0.7/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.065380 buscador-0.7/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)       88 2023-07-20 14:51:08.000000 buscador-0.7/buscador/__init__.py
+-rw-r--r--   0 samcook    (501) staff       (20)     1213 2023-07-20 15:34:17.000000 buscador-0.7/buscador/classJsonStuff.py
+-rw-r--r--   0 samcook    (501) staff       (20)     3019 2023-07-20 15:49:46.000000 buscador-0.7/buscador/classS3Stuff.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.070352 buscador-0.7/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      272 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       25 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 15:52:35.072832 buscador-0.7/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)      998 2023-07-20 15:52:19.000000 buscador-0.7/setup.py
```

### Comparing `buscador-0.6/LICENSE.txt` & `buscador-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buscador-0.6/PKG-INFO` & `buscador-0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.6
+Version: 0.7
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.6.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.6/README.md` & `buscador-0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,7 +7,10 @@
 https://dillinger.io
 
 New Version*
 . Simply upload your new code to github, create a new release, then adapt the setup.py file (new download_url — according to your new release tag, new version), then run the setup.py and the twin command again (navigate to your folder first!)
 
 - python setup.py sdist
 - twine upload dist/*
+
+or if Vs already exist 
+- twine upload --skip-existing dist/*
```

### Comparing `buscador-0.6/buscador.egg-info/PKG-INFO` & `buscador-0.7/buscador.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.6
+Version: 0.7
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.6.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.6/setup.py` & `buscador-0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from distutils.core import setup
 
 setup(
     name="buscador",
     packages=["buscador"],
-    version="0.6",
+    version="0.7",
     license="MIT",
     description="Just a collection of helpful tools",
     author="Samuel Cook",
     author_email="samcook23@hotmail.com",
     url="https://github.com/SamuelBCook",
-    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.6.tar.gz",
+    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz",
     keywords=["tools", "json", "easy"],
     install_requires=[
         "pandas",
         "boto3",
+        "botocore",
+        "io",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",  # either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
```

