# Comparing `tmp/imgopt-0.1.tar.gz` & `tmp/imgopt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgopt-0.1.tar", last modified: Thu Jul 20 19:21:11 2023, max compression
+gzip compressed data, was "imgopt-0.2.tar", last modified: Thu Jul 20 19:24:47 2023, max compression
```

## Comparing `imgopt-0.1.tar` & `imgopt-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:21:11.226709 imgopt-0.1/
--rw-rw-rw-   0        0        0      224 2023-07-20 19:21:11.224696 imgopt-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-20 19:18:35.000000 imgopt-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 19:21:11.193690 imgopt-0.1/imgopt/
--rw-rw-rw-   0        0        0     2351 2023-07-20 19:14:18.000000 imgopt-0.1/imgopt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:21:11.222709 imgopt-0.1/imgopt.egg-info/
--rw-rw-rw-   0        0        0      224 2023-07-20 19:21:11.000000 imgopt-0.1/imgopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-20 19:21:11.000000 imgopt-0.1/imgopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:21:11.000000 imgopt-0.1/imgopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 19:21:11.000000 imgopt-0.1/imgopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 19:21:11.000000 imgopt-0.1/imgopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 19:21:11.227697 imgopt-0.1/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-07-20 19:19:36.000000 imgopt-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.205194 imgopt-0.2/
+-rw-rw-rw-   0        0        0      224 2023-07-20 19:24:47.204197 imgopt-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:18:35.000000 imgopt-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.186200 imgopt-0.2/imgopt/
+-rw-rw-rw-   0        0        0     2274 2023-07-20 19:24:35.000000 imgopt-0.2/imgopt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.203197 imgopt-0.2/imgopt.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:24:47.206197 imgopt-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-07-20 19:24:42.000000 imgopt-0.2/setup.py
```

### Comparing `imgopt-0.1/imgopt/__init__.py` & `imgopt-0.2/imgopt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import requests
 import urllib
 import os
 
 def OptmizeImage(input_file_path, output_file_path=None):
     file_extension = os.path.splitext(input_file_path)[1].lower()
-    print(file_extension)
     if file_extension == '.png':
         mime = 'image/png'
     elif file_extension == '.jpg':
         mime = 'image/jpeg'
     elif file_extension == '.jpeg':
         mime = 'image/jpeg'
 
@@ -25,15 +24,15 @@
         result = response.json()
 
         dest_url = result['dest']
 
         if not output_file_path:
             output_file_path = os.path.join(os.getcwd(), f"{os.urandom(8).hex()}.jpg")
         urllib.request.urlretrieve(dest_url, output_file_path)
-        print(f"Image downloaded successfully as {output_file_path}")
+        print(True)
     except FileNotFoundError:
         print("File/Folder not found.")
     except Exception as e:
         print(f"Error: {e}")
 
 
 def DynamicCompress(input_file_path, output_file_path=None,qlty=None):
```

