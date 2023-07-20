# Comparing `tmp/up_nextflap-0.0.6.tar.gz` & `tmp/up_nextflap-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_nextflap-0.0.6.tar", last modified: Thu Jul 20 16:56:50 2023, max compression
+gzip compressed data, was "up_nextflap-0.0.8.tar", last modified: Thu Jul 20 17:27:17 2023, max compression
```

## Comparing `up_nextflap-0.0.6.tar` & `up_nextflap-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 16:56:50.248149 up_nextflap-0.0.6/
--rw-rw-rw-   0        0        0    11357 2023-06-24 19:12:50.000000 up_nextflap-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      340 2023-07-20 16:56:50.248149 up_nextflap-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-07-20 15:53:16.000000 up_nextflap-0.0.6/README.md
--rw-rw-rw-   0        0        0 16222656 2023-05-06 22:33:43.000000 up_nextflap-0.0.6/libz3.dll
--rw-rw-rw-   0        0        0   781312 2023-07-20 15:06:45.000000 up_nextflap-0.0.6/nextflap.pyd
--rw-rw-rw-   0        0        0       42 2023-07-20 16:56:50.248149 up_nextflap-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      652 2023-07-20 16:56:17.000000 up_nextflap-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:56:50.235318 up_nextflap-0.0.6/up_nextflap/
--rw-rw-rw-   0        0        0       38 2023-07-04 14:38:59.000000 up_nextflap-0.0.6/up_nextflap/__init__.py
--rw-rw-rw-   0        0        0    47569 2023-07-20 13:39:27.000000 up_nextflap-0.0.6/up_nextflap/up_nextflap.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:56:50.247147 up_nextflap-0.0.6/up_nextflap.egg-info/
--rw-rw-rw-   0        0        0      340 2023-07-20 16:56:50.000000 up_nextflap-0.0.6/up_nextflap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-20 16:56:50.000000 up_nextflap-0.0.6/up_nextflap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 16:56:50.000000 up_nextflap-0.0.6/up_nextflap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-20 16:56:50.000000 up_nextflap-0.0.6/up_nextflap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 16:56:50.000000 up_nextflap-0.0.6/up_nextflap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 17:27:17.436154 up_nextflap-0.0.8/
+-rw-rw-rw-   0        0        0    11357 2023-06-24 19:12:50.000000 up_nextflap-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      414 2023-07-20 17:27:17.436154 up_nextflap-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-07-20 15:53:16.000000 up_nextflap-0.0.8/README.md
+-rw-rw-rw-   0        0        0 16222656 2023-05-06 22:33:43.000000 up_nextflap-0.0.8/libz3.dll
+-rw-rw-rw-   0        0        0   781312 2023-07-20 15:06:45.000000 up_nextflap-0.0.8/nextflap.pyd
+-rw-rw-rw-   0        0        0       42 2023-07-20 17:27:17.436154 up_nextflap-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-07-20 17:27:02.000000 up_nextflap-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:27:17.420536 up_nextflap-0.0.8/up_nextflap/
+-rw-rw-rw-   0        0        0       38 2023-07-04 14:38:59.000000 up_nextflap-0.0.8/up_nextflap/__init__.py
+-rw-rw-rw-   0        0        0    47569 2023-07-20 13:39:27.000000 up_nextflap-0.0.8/up_nextflap/up_nextflap.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:27:17.436154 up_nextflap-0.0.8/up_nextflap.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-07-20 17:27:17.000000 up_nextflap-0.0.8/up_nextflap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-20 17:27:17.000000 up_nextflap-0.0.8/up_nextflap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 17:27:17.000000 up_nextflap-0.0.8/up_nextflap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-20 17:27:17.000000 up_nextflap-0.0.8/up_nextflap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 17:27:17.000000 up_nextflap-0.0.8/up_nextflap.egg-info/top_level.txt
```

### Comparing `up_nextflap-0.0.6/LICENSE` & `up_nextflap-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.6/README.md` & `up_nextflap-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.6/libz3.dll` & `up_nextflap-0.0.8/libz3.dll`

 * *Files identical despite different names*

### Comparing `up_nextflap-0.0.6/setup.py` & `up_nextflap-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 """============================================================
     UP_NEXTFLAP
  ============================================================
 """
 
 setup(
     name='up_nextflap',
-    version='0.0.6',
+    version='0.0.8',
     description='up_nextflap',
     long_description=long_description,
     long_description_content_type ="text/markdown",
     author='Oscar Sapena',
     author_email='ossaver@upv.es',
+    url = "https://github.com/aiplan4eu/up-nextflap",
+    packages=['up_nextflap'],
+    platforms=['win_amd64'],
     options = {
         'build_apps': {
             'platforms': ['win_amd64',],
         }
     },
     data_files=[('.', ['libz3.dll', 'nextflap.pyd'])],
     install_requires=[
```

### Comparing `up_nextflap-0.0.6/up_nextflap/up_nextflap.py` & `up_nextflap-0.0.8/up_nextflap/up_nextflap.py`

 * *Files identical despite different names*

