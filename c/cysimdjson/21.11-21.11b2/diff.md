# Comparing `tmp/cysimdjson-21.11.tar.gz` & `tmp/cysimdjson-21.11b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cysimdjson-21.11.tar", last modified: Tue Mar 22 08:27:07 2022, max compression
+gzip compressed data, was "cysimdjson-21.11b2.tar", last modified: Fri Nov  5 16:23:06 2021, max compression
```

## Comparing `cysimdjson-21.11.tar` & `cysimdjson-21.11b2.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxr-xr-x   0 ateska     (501) staff       (20)        0 2022-03-22 08:27:07.713692 cysimdjson-21.11/
--rw-r--r--   0 ateska     (501) staff       (20)    11343 2021-03-09 21:00:36.000000 cysimdjson-21.11/LICENSE
--rw-r--r--   0 ateska     (501) staff       (20)     8814 2022-03-22 08:27:07.713945 cysimdjson-21.11/PKG-INFO
--rw-r--r--   0 ateska     (501) staff       (20)     6522 2022-03-22 08:01:02.000000 cysimdjson-21.11/README.md
-drwxr-xr-x   0 ateska     (501) staff       (20)        0 2022-03-22 08:27:07.699702 cysimdjson-21.11/cysimdjson/
--rw-r--r--   0 ateska     (501) staff       (20)      709 2021-12-27 19:50:46.000000 cysimdjson-21.11/cysimdjson/__init__.py
--rw-r--r--   0 ateska     (501) staff       (20)   467525 2021-11-05 17:14:06.000000 cysimdjson-21.11/cysimdjson/cysimdjson.cpp
--rw-r--r--   0 ateska     (501) staff       (20)      764 2021-11-05 17:14:06.000000 cysimdjson-21.11/cysimdjson/cysimdjson.h
--rw-r--r--   0 ateska     (501) staff       (20)    11798 2021-07-29 12:04:33.000000 cysimdjson-21.11/cysimdjson/cysimdjson.pyx
--rw-r--r--   0 ateska     (501) staff       (20)     5211 2021-08-02 09:57:57.000000 cysimdjson-21.11/cysimdjson/cysimdjsonc.cpp
--rw-r--r--   0 ateska     (501) staff       (20)     1303 2021-08-01 07:45:20.000000 cysimdjson-21.11/cysimdjson/cysimdjsonc.h
--rw-r--r--   0 ateska     (501) staff       (20)     1035 2021-07-28 10:08:08.000000 cysimdjson-21.11/cysimdjson/jsoninter.h
-drwxr-xr-x   0 ateska     (501) staff       (20)        0 2022-03-22 08:27:07.703047 cysimdjson-21.11/cysimdjson/pysimdjson/
--rw-r--r--   0 ateska     (501) staff       (20)     2783 2021-04-06 10:54:22.000000 cysimdjson-21.11/cysimdjson/pysimdjson/errors.cpp
--rw-r--r--   0 ateska     (501) staff       (20)      178 2021-03-27 12:20:17.000000 cysimdjson-21.11/cysimdjson/pysimdjson/errors.h
-drwxr-xr-x   0 ateska     (501) staff       (20)        0 2022-03-22 08:27:07.707881 cysimdjson-21.11/cysimdjson/simdjson/
--rw-r--r--   0 ateska     (501) staff       (20)   533449 2022-03-22 08:07:25.000000 cysimdjson-21.11/cysimdjson/simdjson/simdjson.cpp
--rw-r--r--   0 ateska     (501) staff       (20)  1189348 2022-03-22 08:07:25.000000 cysimdjson-21.11/cysimdjson/simdjson/simdjson.h
-drwxr-xr-x   0 ateska     (501) staff       (20)        0 2022-03-22 08:27:07.701689 cysimdjson-21.11/cysimdjson.egg-info/
--rw-r--r--   0 ateska     (501) staff       (20)     8814 2022-03-22 08:27:07.000000 cysimdjson-21.11/cysimdjson.egg-info/PKG-INFO
--rw-r--r--   0 ateska     (501) staff       (20)      489 2022-03-22 08:27:07.000000 cysimdjson-21.11/cysimdjson.egg-info/SOURCES.txt
--rw-r--r--   0 ateska     (501) staff       (20)        1 2022-03-22 08:27:07.000000 cysimdjson-21.11/cysimdjson.egg-info/dependency_links.txt
--rw-r--r--   0 ateska     (501) staff       (20)       11 2022-03-22 08:27:07.000000 cysimdjson-21.11/cysimdjson.egg-info/top_level.txt
--rw-r--r--   0 ateska     (501) staff       (20)       60 2021-03-08 22:58:43.000000 cysimdjson-21.11/pyproject.toml
--rw-r--r--   0 ateska     (501) staff       (20)       82 2022-03-22 08:27:07.714615 cysimdjson-21.11/setup.cfg
--rw-r--r--   0 ateska     (501) staff       (20)     1699 2022-03-22 08:22:04.000000 cysimdjson-21.11/setup.py
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2021-11-05 16:23:06.959733 cysimdjson-21.11b2/
+-rw-r--r--   0 ateska     (501) staff       (20)    11343 2021-03-09 21:00:36.000000 cysimdjson-21.11b2/LICENSE
+-rw-r--r--   0 ateska     (501) staff       (20)     8098 2021-11-05 16:23:06.960344 cysimdjson-21.11b2/PKG-INFO
+-rw-r--r--   0 ateska     (501) staff       (20)     6022 2021-07-28 15:22:15.000000 cysimdjson-21.11b2/README.md
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2021-11-05 16:23:06.950519 cysimdjson-21.11b2/cysimdjson/
+-rw-r--r--   0 ateska     (501) staff       (20)   467525 2021-11-05 15:32:33.000000 cysimdjson-21.11b2/cysimdjson/cysimdjson.cpp
+-rw-r--r--   0 ateska     (501) staff       (20)     5211 2021-08-02 09:57:57.000000 cysimdjson-21.11b2/cysimdjson/cysimdjsonc.cpp
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2021-11-05 16:23:06.952909 cysimdjson-21.11b2/cysimdjson/pysimdjson/
+-rw-r--r--   0 ateska     (501) staff       (20)     2783 2021-04-06 10:54:22.000000 cysimdjson-21.11b2/cysimdjson/pysimdjson/errors.cpp
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2021-11-05 16:23:06.953955 cysimdjson-21.11b2/cysimdjson/simdjson/
+-rw-rw-r--   0 ateska     (501) staff       (20)   533449 2021-11-05 15:29:29.000000 cysimdjson-21.11b2/cysimdjson/simdjson/simdjson.cpp
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2021-11-05 16:23:06.952484 cysimdjson-21.11b2/cysimdjson.egg-info/
+-rw-r--r--   0 ateska     (501) staff       (20)     8098 2021-11-05 16:23:06.000000 cysimdjson-21.11b2/cysimdjson.egg-info/PKG-INFO
+-rw-r--r--   0 ateska     (501) staff       (20)      306 2021-11-05 16:23:06.000000 cysimdjson-21.11b2/cysimdjson.egg-info/SOURCES.txt
+-rw-r--r--   0 ateska     (501) staff       (20)        1 2021-11-05 16:23:06.000000 cysimdjson-21.11b2/cysimdjson.egg-info/dependency_links.txt
+-rw-r--r--   0 ateska     (501) staff       (20)       11 2021-11-05 16:23:06.000000 cysimdjson-21.11b2/cysimdjson.egg-info/top_level.txt
+-rw-r--r--   0 ateska     (501) staff       (20)       60 2021-03-08 22:58:43.000000 cysimdjson-21.11b2/pyproject.toml
+-rw-r--r--   0 ateska     (501) staff       (20)       82 2021-11-05 16:23:06.962230 cysimdjson-21.11b2/setup.cfg
+-rw-r--r--   0 ateska     (501) staff       (20)     1434 2021-11-05 16:21:40.000000 cysimdjson-21.11b2/setup.py
```

### Comparing `cysimdjson-21.11/LICENSE` & `cysimdjson-21.11b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cysimdjson-21.11/PKG-INFO` & `cysimdjson-21.11b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cysimdjson
-Version: 21.11
+Version: 21.11b2
 Summary: Cython-based wrapper for SIMDJSON
 Home-page: https://github.com/TeskaLabs/cysimdjson
 Author: TeskaLabs Ltd
 Author-email: info@teskalabs.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/TeskaLabs/cysimdjson
 Project-URL: Tracker, https://github.com/TeskaLabs/cysimdjson/issues
@@ -54,25 +54,14 @@
         # Access using JSON Pointer
         print(json_parsed.json_parsed['foo'])
         ```
         
         The `json_parsed` is a read-only dictionary-like object, that provides an access to JSON data.
         
         
-        ## Trade-offs
-        
-        The speed of `cysimdjson` is based on these assumptions:
-        
-        1) The output of the parser is read-only, you cannot modify it
-        2) The output of the parser is not Python dictionary, but lazily evaluated dictionary-like object
-        3) If you convert the parser output into a Python dictionary, you will lose the speed
-        
-        If your design is not aligned with these assumptions, `cysimdjson` is not a good choice.
-        
-        
         ## Documentation
         
         `JSONParser.parse(json_bytes)`
         
         Parse JSON `json_bytes`, represented as `bytes`.
         
         
@@ -89,22 +78,20 @@
         
         `JSONParser.load(path)`
         
         
         ## Installation
         
         ```
+        pip3 install cython
         pip3 install cysimdjson
         ```
         
         Project `cysimdjson` is distributed via PyPI: https://pypi.org/project/cysimdjson/ .
         
-        If you want to install `cysimdjson` from source, you need to install Cython first: `pip3 install cython`.
-        
-        
         ## Performance
         
         ```
         ----------------------------------------------------------------
         # 'jsonexamples/test.json' 2397 bytes
         ----------------------------------------------------------------
         * cysimdjson parse          510291.81 EPS (  1.00)  1223.17 MB/s
@@ -194,15 +181,13 @@
         ## Manual build
         
         ```
         python3 setup.py build_ext --inplace
         ```
         
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `cysimdjson-21.11/README.md` & `cysimdjson-21.11b2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -44,25 +44,14 @@
 # Access using JSON Pointer
 print(json_parsed.json_parsed['foo'])
 ```
 
 The `json_parsed` is a read-only dictionary-like object, that provides an access to JSON data.
 
 
-## Trade-offs
-
-The speed of `cysimdjson` is based on these assumptions:
-
-1) The output of the parser is read-only, you cannot modify it
-2) The output of the parser is not Python dictionary, but lazily evaluated dictionary-like object
-3) If you convert the parser output into a Python dictionary, you will lose the speed
-
-If your design is not aligned with these assumptions, `cysimdjson` is not a good choice.
-
-
 ## Documentation
 
 `JSONParser.parse(json_bytes)`
 
 Parse JSON `json_bytes`, represented as `bytes`.
 
 
@@ -79,22 +68,20 @@
 
 `JSONParser.load(path)`
 
 
 ## Installation
 
 ```
+pip3 install cython
 pip3 install cysimdjson
 ```
 
 Project `cysimdjson` is distributed via PyPI: https://pypi.org/project/cysimdjson/ .
 
-If you want to install `cysimdjson` from source, you need to install Cython first: `pip3 install cython`.
-
-
 ## Performance
 
 ```
 ----------------------------------------------------------------
 # 'jsonexamples/test.json' 2397 bytes
 ----------------------------------------------------------------
 * cysimdjson parse          510291.81 EPS (  1.00)  1223.17 MB/s
```

### Comparing `cysimdjson-21.11/cysimdjson/cysimdjson.cpp` & `cysimdjson-21.11b2/cysimdjson/cysimdjson.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-21.11/cysimdjson/cysimdjsonc.cpp` & `cysimdjson-21.11b2/cysimdjson/cysimdjsonc.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-21.11/cysimdjson/pysimdjson/errors.cpp` & `cysimdjson-21.11b2/cysimdjson/pysimdjson/errors.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-21.11/cysimdjson/simdjson/simdjson.cpp` & `cysimdjson-21.11b2/cysimdjson/simdjson/simdjson.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-21.11/cysimdjson.egg-info/PKG-INFO` & `cysimdjson-21.11b2/cysimdjson.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cysimdjson
-Version: 21.11
+Version: 21.11b2
 Summary: Cython-based wrapper for SIMDJSON
 Home-page: https://github.com/TeskaLabs/cysimdjson
 Author: TeskaLabs Ltd
 Author-email: info@teskalabs.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/TeskaLabs/cysimdjson
 Project-URL: Tracker, https://github.com/TeskaLabs/cysimdjson/issues
@@ -54,25 +54,14 @@
         # Access using JSON Pointer
         print(json_parsed.json_parsed['foo'])
         ```
         
         The `json_parsed` is a read-only dictionary-like object, that provides an access to JSON data.
         
         
-        ## Trade-offs
-        
-        The speed of `cysimdjson` is based on these assumptions:
-        
-        1) The output of the parser is read-only, you cannot modify it
-        2) The output of the parser is not Python dictionary, but lazily evaluated dictionary-like object
-        3) If you convert the parser output into a Python dictionary, you will lose the speed
-        
-        If your design is not aligned with these assumptions, `cysimdjson` is not a good choice.
-        
-        
         ## Documentation
         
         `JSONParser.parse(json_bytes)`
         
         Parse JSON `json_bytes`, represented as `bytes`.
         
         
@@ -89,22 +78,20 @@
         
         `JSONParser.load(path)`
         
         
         ## Installation
         
         ```
+        pip3 install cython
         pip3 install cysimdjson
         ```
         
         Project `cysimdjson` is distributed via PyPI: https://pypi.org/project/cysimdjson/ .
         
-        If you want to install `cysimdjson` from source, you need to install Cython first: `pip3 install cython`.
-        
-        
         ## Performance
         
         ```
         ----------------------------------------------------------------
         # 'jsonexamples/test.json' 2397 bytes
         ----------------------------------------------------------------
         * cysimdjson parse          510291.81 EPS (  1.00)  1223.17 MB/s
@@ -194,15 +181,13 @@
         ## Manual build
         
         ```
         python3 setup.py build_ext --inplace
         ```
         
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `cysimdjson-21.11/setup.py` & `cysimdjson-21.11b2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, Extension
+from setuptools.command.build_py import build_py
 from os import path
 
 from Cython.Build import cythonize
 
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 	long_description = f.read()
 
 extensions = [
 	Extension(
-		"cysimdjson.cysimdjson",
+		"cysimdjson",
 		[			
 			'cysimdjson/cysimdjson.pyx',
 			'cysimdjson/simdjson/simdjson.cpp',
 			'cysimdjson/pysimdjson/errors.cpp',
 			'cysimdjson/cysimdjsonc.cpp',
 		],
 		language="c++",
@@ -23,48 +24,33 @@
 			"-Wno-deprecated",
 		],
 	)
 ]
 
 setup(
 	name='cysimdjson',
-	version="21.11",
+	version="21.11b2",
 	description='Cython-based wrapper for SIMDJSON',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='TeskaLabs Ltd',
 	author_email='info@teskalabs.com',
 	platforms='any',
 	classifiers=[
-		'Development Status :: 5 - Production/Stable',
+		'Development Status :: 4 - Beta',
 		'License :: OSI Approved :: Apache Software License',
-		'Programming Language :: Python :: 3.6',
 		'Programming Language :: Python :: 3.7',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
-		'Programming Language :: Python :: 3.10',
 	],
 	packages=[
 		"cysimdjson",
 	],
 	url='https://github.com/TeskaLabs/cysimdjson',
 	project_urls={
 		"Source": "https://github.com/TeskaLabs/cysimdjson",
 		'Tracker': 'https://github.com/TeskaLabs/cysimdjson/issues',
 	},
 	install_requires=[
 	],
-	setup_requires=[
-		"cython"
-	],
-	package_data={
-		"cysimdjson": [
-			"cysimdjson.pyx",
-			"cysimdjson.h",
-			"cysimdjsonc.h",
-			"jsoninter.h",
-			"pysimdjson/errors.h",
-			"simdjson/simdjson.h",
-		]
-	},
 	ext_modules=cythonize(extensions),
 )
```

