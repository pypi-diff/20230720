# Comparing `tmp/buscador-0.2.tar.gz` & `tmp/buscador-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.2.tar", last modified: Thu Jul 20 13:34:21 2023, max compression
+gzip compressed data, was "buscador-0.3.tar", last modified: Thu Jul 20 13:41:44 2023, max compression
```

## Comparing `buscador-0.2.tar` & `buscador-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.533546 buscador-0.2/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.2/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:34:21.533777 buscador-0.2/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      696 2023-07-20 13:25:10.000000 buscador-0.2/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.528159 buscador-0.2/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.2/buscador/__init__.py
--rw-r--r--   0 samcook    (501) staff       (20)      450 2023-07-19 20:53:58.000000 buscador-0.2/buscador/classFindValue.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:34:21.532905 buscador-0.2/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       23 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 13:34:21.000000 buscador-0.2/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 13:34:21.534563 buscador-0.2/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)     1053 2023-07-20 13:33:23.000000 buscador-0.2/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:41:44.556449 buscador-0.3/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.3/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:41:44.556780 buscador-0.3/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      697 2023-07-20 13:40:09.000000 buscador-0.3/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:41:44.551305 buscador-0.3/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)       46 2023-07-19 20:55:35.000000 buscador-0.3/buscador/__init__.py
+-rw-r--r--   0 samcook    (501) staff       (20)      450 2023-07-19 20:53:58.000000 buscador-0.3/buscador/classFindValue.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 13:41:44.555866 buscador-0.3/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      738 2023-07-20 13:41:44.000000 buscador-0.3/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      247 2023-07-20 13:41:44.000000 buscador-0.3/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 13:41:44.000000 buscador-0.3/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       18 2023-07-20 13:41:44.000000 buscador-0.3/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 13:41:44.000000 buscador-0.3/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 13:41:44.557743 buscador-0.3/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)     1035 2023-07-20 13:41:29.000000 buscador-0.3/setup.py
```

### Comparing `buscador-0.2/LICENSE.txt` & `buscador-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buscador-0.2/PKG-INFO` & `buscador-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.2
+Version: 0.3
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.2.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.3.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.2/README.md` & `buscador-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 
 Every time you want to update your package later on, upload a new version to github, create a new release as we just discussed, specify a new release tag and copy-paste the link to Source into the setup.py file (do not forget to also increment the version number).
 
 https://medium.com/@joel.barmettler/how-to-upload-your-python-package-to-pypi-65edc5fe9c56
 
 https://dillinger.io
 
-New Version
+New Version*
 . Simply upload your new code to github, create a new release, then adapt the setup.py file (new download_url — according to your new release tag, new version), then run the setup.py and the twin command again (navigate to your folder first!)
 
 - python setup.py sdist
 - twine upload dist/*
```

### Comparing `buscador-0.2/buscador.egg-info/PKG-INFO` & `buscador-0.3/buscador.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.2
+Version: 0.3
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.2.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/0.3.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.2/setup.py` & `buscador-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'buscador',         
   packages = ['buscador'],   
-  version = '0.2',      
+  version = '0.3',      
   license='MIT',        
   description = 'Just a collection of helpful tools',   
   author = 'Samuel Cook',                   
   author_email = 'samcook23@hotmail.com',     
   url = 'https://github.com/SamuelBCook',  
-  download_url = 'https://github.com/SamuelBCook/buscador/archive/refs/tags/0.2.tar.gz',    
+  download_url = 'https://github.com/SamuelBCook/buscador/archive/refs/tags/0.3.tar.gz',    
   keywords = ['tools', 'json', 'easy'],   
   install_requires=[           
           'pandas',
-          'json',
           'time',
           'boto3'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" 
     'Intended Audience :: Developers',      
     'Topic :: Software Development :: Build Tools',
```

