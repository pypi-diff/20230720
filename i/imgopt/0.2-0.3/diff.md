# Comparing `tmp/imgopt-0.2.tar.gz` & `tmp/imgopt-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgopt-0.2.tar", last modified: Thu Jul 20 19:24:47 2023, max compression
+gzip compressed data, was "imgopt-0.3.tar", last modified: Thu Jul 20 19:42:21 2023, max compression
```

## Comparing `imgopt-0.2.tar` & `imgopt-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.205194 imgopt-0.2/
--rw-rw-rw-   0        0        0      224 2023-07-20 19:24:47.204197 imgopt-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-20 19:18:35.000000 imgopt-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.186200 imgopt-0.2/imgopt/
--rw-rw-rw-   0        0        0     2274 2023-07-20 19:24:35.000000 imgopt-0.2/imgopt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:24:47.203197 imgopt-0.2/imgopt.egg-info/
--rw-rw-rw-   0        0        0      224 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 19:24:47.000000 imgopt-0.2/imgopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 19:24:47.206197 imgopt-0.2/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-07-20 19:24:42.000000 imgopt-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:42:21.838570 imgopt-0.3/
+-rw-rw-rw-   0        0        0     2438 2023-07-20 19:42:21.837570 imgopt-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-07-20 19:42:04.000000 imgopt-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:42:21.820380 imgopt-0.3/imgopt/
+-rw-rw-rw-   0        0        0     2247 2023-07-20 19:28:37.000000 imgopt-0.3/imgopt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:42:21.836584 imgopt-0.3/imgopt.egg-info/
+-rw-rw-rw-   0        0        0     2438 2023-07-20 19:42:21.000000 imgopt-0.3/imgopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-20 19:42:21.000000 imgopt-0.3/imgopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:42:21.000000 imgopt-0.3/imgopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 19:42:21.000000 imgopt-0.3/imgopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 19:42:21.000000 imgopt-0.3/imgopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:42:21.839569 imgopt-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-07-20 19:28:43.000000 imgopt-0.3/setup.py
```

### Comparing `imgopt-0.2/imgopt/__init__.py` & `imgopt-0.3/imgopt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         print("File/Folder not found.")
     except Exception as e:
         print(f"Error: {e}")
 
 
 def DynamicCompress(input_file_path, output_file_path=None,qlty=None):
     file_extension = os.path.splitext(input_file_path)[1].lower()
-    print(file_extension)
     if file_extension == '.png':
         mime = 'image/png'
     elif file_extension == '.jpg':
         mime = 'image/jpeg'
     elif file_extension == '.jpeg':
         mime = 'image/jpeg'
```

