# Comparing `tmp/phoenixtools-1.2.0.tar.gz` & `tmp/phoenixtools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixtools-1.2.0.tar", last modified: Thu Jul 20 05:20:30 2023, max compression
+gzip compressed data, was "phoenixtools-1.2.1.tar", last modified: Thu Jul 20 05:23:31 2023, max compression
```

## Comparing `phoenixtools-1.2.0.tar` & `phoenixtools-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 05:20:30.773129 phoenixtools-1.2.0/
--rw-rw-rw-   0        0        0      642 2023-07-20 05:20:30.772134 phoenixtools-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 05:20:30.755569 phoenixtools-1.2.0/phoenixtools/
--rw-rw-rw-   0        0        0     1314 2023-07-20 05:16:34.000000 phoenixtools-1.2.0/phoenixtools/__init__.py
--rw-rw-rw-   0        0        0      203 2023-07-11 09:48:52.000000 phoenixtools-1.2.0/phoenixtools/colors.py
--rw-rw-rw-   0        0        0      538 2023-07-13 03:52:49.000000 phoenixtools-1.2.0/phoenixtools/encryption.py
--rw-rw-rw-   0        0        0      705 2023-07-13 04:38:37.000000 phoenixtools-1.2.0/phoenixtools/iptools.py
--rw-rw-rw-   0        0        0      280 2023-07-11 09:48:52.000000 phoenixtools-1.2.0/phoenixtools/math.py
--rw-rw-rw-   0        0        0     4216 2023-07-13 04:52:57.000000 phoenixtools-1.2.0/phoenixtools/steamkeygen.py
--rw-rw-rw-   0        0        0      152 2023-07-20 05:16:34.000000 phoenixtools-1.2.0/phoenixtools/writemodes.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:20:30.771134 phoenixtools-1.2.0/phoenixtools.egg-info/
--rw-rw-rw-   0        0        0      642 2023-07-20 05:20:30.000000 phoenixtools-1.2.0/phoenixtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-07-20 05:20:30.000000 phoenixtools-1.2.0/phoenixtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 05:20:30.000000 phoenixtools-1.2.0/phoenixtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 05:20:30.000000 phoenixtools-1.2.0/phoenixtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 05:20:30.000000 phoenixtools-1.2.0/phoenixtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 05:20:30.773129 phoenixtools-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1157 2023-07-20 05:20:05.000000 phoenixtools-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 05:23:31.269024 phoenixtools-1.2.1/
+-rw-rw-rw-   0        0        0      642 2023-07-20 05:23:31.268010 phoenixtools-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 05:23:31.252743 phoenixtools-1.2.1/phoenixtools/
+-rw-rw-rw-   0        0        0     1314 2023-07-20 05:16:34.000000 phoenixtools-1.2.1/phoenixtools/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-11 09:48:52.000000 phoenixtools-1.2.1/phoenixtools/colors.py
+-rw-rw-rw-   0        0        0      538 2023-07-13 03:52:49.000000 phoenixtools-1.2.1/phoenixtools/encryption.py
+-rw-rw-rw-   0        0        0      705 2023-07-13 04:38:37.000000 phoenixtools-1.2.1/phoenixtools/iptools.py
+-rw-rw-rw-   0        0        0      280 2023-07-11 09:48:52.000000 phoenixtools-1.2.1/phoenixtools/math.py
+-rw-rw-rw-   0        0        0     4216 2023-07-13 04:52:57.000000 phoenixtools-1.2.1/phoenixtools/steamkeygen.py
+-rw-rw-rw-   0        0        0      152 2023-07-20 05:16:34.000000 phoenixtools-1.2.1/phoenixtools/writemodes.py
+drwxrwxrwx   0        0        0        0 2023-07-20 05:23:31.266998 phoenixtools-1.2.1/phoenixtools.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-07-20 05:23:31.000000 phoenixtools-1.2.1/phoenixtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-20 05:23:31.000000 phoenixtools-1.2.1/phoenixtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 05:23:31.000000 phoenixtools-1.2.1/phoenixtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-20 05:23:31.000000 phoenixtools-1.2.1/phoenixtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 05:23:31.269024 phoenixtools-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2023-07-20 05:22:48.000000 phoenixtools-1.2.1/setup.py
```

### Comparing `phoenixtools-1.2.0/PKG-INFO` & `phoenixtools-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: phoenixtools
-Version: 1.2.0
+Version: 1.2.1
 Summary: A fun little python package including tools such as math, encryption, and ANSI color codes.
 Author: Jack B.
 Author-email: <BurrJ22@outlook.com>
 Keywords: python,encryption,PyPi,math,Steam Keygen
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 
-NOTE: THIS VERSION (v1.2.0) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.
+NOTE: THIS VERSION (v1.2.1) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.
```

### Comparing `phoenixtools-1.2.0/phoenixtools/__init__.py` & `phoenixtools-1.2.1/phoenixtools/__init__.py`

 * *Files identical despite different names*

### Comparing `phoenixtools-1.2.0/phoenixtools/encryption.py` & `phoenixtools-1.2.1/phoenixtools/encryption.py`

 * *Files identical despite different names*

### Comparing `phoenixtools-1.2.0/phoenixtools/iptools.py` & `phoenixtools-1.2.1/phoenixtools/iptools.py`

 * *Files identical despite different names*

### Comparing `phoenixtools-1.2.0/phoenixtools/steamkeygen.py` & `phoenixtools-1.2.1/phoenixtools/steamkeygen.py`

 * *Files identical despite different names*

### Comparing `phoenixtools-1.2.0/phoenixtools.egg-info/PKG-INFO` & `phoenixtools-1.2.1/phoenixtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: phoenixtools
-Version: 1.2.0
+Version: 1.2.1
 Summary: A fun little python package including tools such as math, encryption, and ANSI color codes.
 Author: Jack B.
 Author-email: <BurrJ22@outlook.com>
 Keywords: python,encryption,PyPi,math,Steam Keygen
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 
-NOTE: THIS VERSION (v1.2.0) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.
+NOTE: THIS VERSION (v1.2.1) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.
```

### Comparing `phoenixtools-1.2.0/setup.py` & `phoenixtools-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION="v1.2.0"
+VERSION="v1.2.1"
 DESCRIPTION = 'A fun little python package including tools such as math, encryption, and ANSI color codes.'
-LONG_DESCRIPTION = 'NOTE: THIS VERSION (v1.2.0) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.'
+LONG_DESCRIPTION = 'NOTE: THIS VERSION (v1.2.1) IS THE FIRST STABLE VERSION. OTHER VERSIONS HAVE IMPORTING ISSUES AND ERRORS IN CODE. DO NOT USE THEM.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="phoenixtools", 
         version=VERSION,
         author="Jack B.",
         author_email="<BurrJ22@outlook.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['math','zipfile'], # add any additional packages that 
+        install_requires=[], # add any additional packages that 
         # need to be installed along with your package. Eg: 'caer'
         
         keywords=['python','encryption','PyPi','math','Steam Keygen'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

