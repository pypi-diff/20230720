# Comparing `tmp/claude2-1.0.0.tar.gz` & `tmp/claude2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude2-1.0.0.tar", last modified: Thu Jul 20 11:19:49 2023, max compression
+gzip compressed data, was "claude2-1.0.1.tar", last modified: Thu Jul 20 11:23:39 2023, max compression
```

## Comparing `claude2-1.0.0.tar` & `claude2-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:19:49.298545 claude2-1.0.0/
-drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:19:49.294997 claude2-1.0.0/Claude/
--rw-r--r--   0 nipunbhatia   (501) staff       (20)       22 2023-07-20 11:18:34.000000 claude2-1.0.0/Claude/__init__.py
--rw-------   0 nipunbhatia   (501) staff       (20)     6316 2023-07-20 10:11:49.000000 claude2-1.0.0/Claude/claude.py
--rw-r--r--   0 nipunbhatia   (501) staff       (20)     1069 2023-07-20 08:07:48.000000 claude2-1.0.0/LICENSE
--rw-r--r--   0 nipunbhatia   (501) staff       (20)      890 2023-07-20 11:19:49.298109 claude2-1.0.0/PKG-INFO
--rw-r--r--   0 nipunbhatia   (501) staff       (20)      197 2023-07-20 10:22:16.000000 claude2-1.0.0/README.md
-drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:19:49.297541 claude2-1.0.0/claude2.egg-info/
--rw-r--r--   0 nipunbhatia   (501) staff       (20)      890 2023-07-20 11:19:49.000000 claude2-1.0.0/claude2.egg-info/PKG-INFO
--rw-r--r--   0 nipunbhatia   (501) staff       (20)      216 2023-07-20 11:19:49.000000 claude2-1.0.0/claude2.egg-info/SOURCES.txt
--rw-r--r--   0 nipunbhatia   (501) staff       (20)        1 2023-07-20 11:19:49.000000 claude2-1.0.0/claude2.egg-info/dependency_links.txt
--rw-r--r--   0 nipunbhatia   (501) staff       (20)        9 2023-07-20 11:19:49.000000 claude2-1.0.0/claude2.egg-info/requires.txt
--rw-r--r--   0 nipunbhatia   (501) staff       (20)        7 2023-07-20 11:19:49.000000 claude2-1.0.0/claude2.egg-info/top_level.txt
--rw-r--r--   0 nipunbhatia   (501) staff       (20)       38 2023-07-20 11:19:49.298692 claude2-1.0.0/setup.cfg
--rw-r--r--   0 nipunbhatia   (501) staff       (20)     1127 2023-07-20 11:19:42.000000 claude2-1.0.0/setup.py
+drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:23:39.815715 claude2-1.0.1/
+drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:23:39.811876 claude2-1.0.1/Claude/
+-rw-------   0 nipunbhatia   (501) staff       (20)     6316 2023-07-20 10:11:49.000000 claude2-1.0.1/Claude/claude.py
+drwxr-xr-x   0 nipunbhatia   (501) staff       (20)        0 2023-07-20 11:23:39.814692 claude2-1.0.1/Claude/claude2.egg-info/
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)      890 2023-07-20 11:23:39.000000 claude2-1.0.1/Claude/claude2.egg-info/PKG-INFO
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)      232 2023-07-20 11:23:39.000000 claude2-1.0.1/Claude/claude2.egg-info/SOURCES.txt
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)        1 2023-07-20 11:23:39.000000 claude2-1.0.1/Claude/claude2.egg-info/dependency_links.txt
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)        9 2023-07-20 11:23:39.000000 claude2-1.0.1/Claude/claude2.egg-info/requires.txt
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)        7 2023-07-20 11:23:39.000000 claude2-1.0.1/Claude/claude2.egg-info/top_level.txt
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)     1069 2023-07-20 08:07:48.000000 claude2-1.0.1/LICENSE
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)      890 2023-07-20 11:23:39.815385 claude2-1.0.1/PKG-INFO
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)      197 2023-07-20 10:22:16.000000 claude2-1.0.1/README.md
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)       38 2023-07-20 11:23:39.815833 claude2-1.0.1/setup.cfg
+-rw-r--r--   0 nipunbhatia   (501) staff       (20)     1196 2023-07-20 11:23:10.000000 claude2-1.0.1/setup.py
```

### Comparing `claude2-1.0.0/Claude/claude.py` & `claude2-1.0.1/Claude/claude.py`

 * *Files identical despite different names*

### Comparing `claude2-1.0.0/LICENSE` & `claude2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `claude2-1.0.0/PKG-INFO` & `claude2-1.0.1/Claude/claude2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude2
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package provides an unofficial api for interacting with the Claude from Anthropic
 Home-page: https://github.com/Nipun1212/Claude_api
 Author: Nipun
 Author-email: nipunbhatia06@gmail.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `claude2-1.0.0/claude2.egg-info/PKG-INFO` & `claude2-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude2
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package provides an unofficial api for interacting with the Claude from Anthropic
 Home-page: https://github.com/Nipun1212/Claude_api
 Author: Nipun
 Author-email: nipunbhatia06@gmail.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `claude2-1.0.0/setup.py` & `claude2-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 setup(
     name='claude2', 
-    version='1.0.0',  
+    version='1.0.1',  
     author='Nipun',
     license="MIT",
     author_email='nipunbhatia06@gmail.com',
     description='A Python package provides an unofficial api for interacting with the Claude from Anthropic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Nipun1212/Claude_api',  # Replace with your GitHub repository URL
@@ -20,12 +20,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords=['claude', 'ai', 'claude-ai', 'API', 'requests', 'chatbot'],
+    package_dir={
+    "": "Claude"
+    },
+    py_modules=["claude"],
     install_requires=[
         'requests',  # List any dependencies your package needs
     ],
     python_requires=">=3.7",
 )
```

