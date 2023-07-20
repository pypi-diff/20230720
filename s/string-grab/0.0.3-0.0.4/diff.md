# Comparing `tmp/string_grab-0.0.3.tar.gz` & `tmp/string_grab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-0.0.3.tar", last modified: Thu Jul 20 11:01:35 2023, max compression
+gzip compressed data, was "string_grab-0.0.4.tar", last modified: Thu Jul 20 16:35:55 2023, max compression
```

## Comparing `string_grab-0.0.3.tar` & `string_grab-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.3/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1028 2023-07-20 11:01:35.226476 string_grab-0.0.3/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      639 2023-07-20 11:00:34.000000 string_grab-0.0.3/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 11:01:35.226476 string_grab-0.0.3/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-20 11:00:56.000000 string_grab-0.0.3/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.3/string_grab/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     1587 2023-07-20 11:00:34.000000 string_grab-0.0.3/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 11:01:35.226476 string_grab-0.0.3/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1028 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-20 11:01:35.000000 string_grab-0.0.3/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 16:35:55.947119 string_grab-0.0.4/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.4/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-20 16:35:55.947119 string_grab-0.0.4/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-0.0.4/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 16:35:55.947119 string_grab-0.0.4/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-20 16:35:50.000000 string_grab-0.0.4/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 16:35:55.947119 string_grab-0.0.4/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.4/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     1587 2023-07-20 11:00:34.000000 string_grab-0.0.4/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 16:35:55.947119 string_grab-0.0.4/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-20 16:35:55.000000 string_grab-0.0.4/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-20 16:35:55.000000 string_grab-0.0.4/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 16:35:55.000000 string_grab-0.0.4/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-20 16:35:55.000000 string_grab-0.0.4/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-0.0.3/LICENSE` & `string_grab-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.3/PKG-INFO` & `string_grab-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -21,18 +21,18 @@
        Mobile: 715-563-3967
        Street: 4674 Lynn Avenue
        City, State, Zip: Eau Claire, Wisconsin(WI), 54701"""
 ```
 ```python
 from string_grab import grab
 
-birthday = grab(text, start="Birthday: ", end="\n")
+birthday = grab(text, start="Birthday: ", end=" (")
 print(birthday)
 
->> "3/23/1973 (50 years old)"
+>> "3/23/1973"
 ```
 ```python
 from string_grab import grab_all
 
 for number in grab_all(text, start="Mobile: ", end="\n"):
     print(number)
```

### Comparing `string_grab-0.0.3/README.md` & `string_grab-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,18 @@
        Mobile: 715-563-3967
        Street: 4674 Lynn Avenue
        City, State, Zip: Eau Claire, Wisconsin(WI), 54701"""
 ```
 ```python
 from string_grab import grab
 
-birthday = grab(text, start="Birthday: ", end="\n")
+birthday = grab(text, start="Birthday: ", end=" (")
 print(birthday)
 
->> "3/23/1973 (50 years old)"
+>> "3/23/1973"
 ```
 ```python
 from string_grab import grab_all
 
 for number in grab_all(text, start="Mobile: ", end="\n"):
     print(number)
```

### Comparing `string_grab-0.0.3/setup.py` & `string_grab-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="0.0.3",
+    version="0.0.4",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
     description=("Extract one or multiple substrings "
                  "between two start and end strings."),
```

### Comparing `string_grab-0.0.3/string_grab/string_grab.py` & `string_grab-0.0.4/string_grab/string_grab.py`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.3/string_grab.egg-info/PKG-INFO` & `string_grab-0.0.4/string_grab.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -21,18 +21,18 @@
        Mobile: 715-563-3967
        Street: 4674 Lynn Avenue
        City, State, Zip: Eau Claire, Wisconsin(WI), 54701"""
 ```
 ```python
 from string_grab import grab
 
-birthday = grab(text, start="Birthday: ", end="\n")
+birthday = grab(text, start="Birthday: ", end=" (")
 print(birthday)
 
->> "3/23/1973 (50 years old)"
+>> "3/23/1973"
 ```
 ```python
 from string_grab import grab_all
 
 for number in grab_all(text, start="Mobile: ", end="\n"):
     print(number)
```

