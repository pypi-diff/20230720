# Comparing `tmp/string_grab-0.0.2.tar.gz` & `tmp/string_grab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-0.0.2.tar", last modified: Thu Jul 20 10:54:27 2023, max compression
+gzip compressed data, was "string_grab-0.0.3.tar", last modified: Thu Jul 20 11:01:35 2023, max compression
```

## Comparing `string_grab-0.0.2.tar` & `string_grab-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 10:54:27.878491 string_grab-0.0.2/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 10:30:29.000000 string_grab-0.0.2/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1027 2023-07-20 10:54:27.878491 string_grab-0.0.2/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      639 2023-07-20 10:49:37.000000 string_grab-0.0.2/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 10:54:27.878491 string_grab-0.0.2/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      542 2023-07-20 10:54:15.000000 string_grab-0.0.2/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 10:54:27.874491 string_grab-0.0.2/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 10:23:26.000000 string_grab-0.0.2/string_grab/__init__.py
--rwxr-xr-x   0 omega     (1000) omega     (1000)     1587 2023-07-20 09:48:59.000000 string_grab-0.0.2/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 10:54:27.878491 string_grab-0.0.2/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1027 2023-07-20 10:54:27.000000 string_grab-0.0.2/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-20 10:54:27.000000 string_grab-0.0.2/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 10:54:27.000000 string_grab-0.0.2/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-20 10:54:27.000000 string_grab-0.0.2/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.3/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1028 2023-07-20 11:01:35.226476 string_grab-0.0.3/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      639 2023-07-20 11:00:34.000000 string_grab-0.0.3/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 11:01:35.226476 string_grab-0.0.3/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-20 11:00:56.000000 string_grab-0.0.3/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.3/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     1587 2023-07-20 11:00:34.000000 string_grab-0.0.3/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1028 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-0.0.2/LICENSE` & `string_grab-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.2/PKG-INFO` & `string_grab-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 0.0.2
-Summary: Extract one or multiple substringsbetween two start and end strings.
+Version: 0.0.3
+Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
 Description-Content-Type: text/markdown
```

### Comparing `string_grab-0.0.2/README.md` & `string_grab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.2/setup.py` & `string_grab-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="0.0.2",
+    version="0.0.3",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
-    description=("Extract one or multiple substrings"
+    description=("Extract one or multiple substrings "
                  "between two start and end strings."),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="GPLv2",
     packages=["string_grab"])
```

### Comparing `string_grab-0.0.2/string_grab/string_grab.py` & `string_grab-0.0.3/string_grab/string_grab.py`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.2/string_grab.egg-info/PKG-INFO` & `string_grab-0.0.3/string_grab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 0.0.2
-Summary: Extract one or multiple substringsbetween two start and end strings.
+Version: 0.0.3
+Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
 Description-Content-Type: text/markdown
```

