# Comparing `tmp/zuicorn-1.0.5.tar.gz` & `tmp/zuicorn-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuicorn-1.0.5.tar", last modified: Thu Jul 20 08:11:22 2023, max compression
+gzip compressed data, was "zuicorn-1.0.6.tar", last modified: Thu Jul 20 08:31:19 2023, max compression
```

## Comparing `zuicorn-1.0.5.tar` & `zuicorn-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:11:22.162485 zuicorn-1.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-20 08:11:22.162485 zuicorn-1.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-20 08:11:22.162485 zuicorn-1.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      913 2023-07-20 08:09:50.000000 zuicorn-1.0.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:11:22.162485 zuicorn-1.0.5/zuicorn/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-20 08:09:15.000000 zuicorn-1.0.5/zuicorn/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8539 2023-07-20 08:05:32.000000 zuicorn-1.0.5/zuicorn/wsgi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:11:22.162485 zuicorn-1.0.5/zuicorn.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-20 08:11:22.000000 zuicorn-1.0.5/zuicorn.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:31:19.857687 zuicorn-1.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-20 08:31:19.857687 zuicorn-1.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-20 08:31:19.857687 zuicorn-1.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      913 2023-07-20 08:31:14.000000 zuicorn-1.0.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:31:19.853686 zuicorn-1.0.6/zuicorn/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-20 08:09:15.000000 zuicorn-1.0.6/zuicorn/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8530 2023-07-20 08:30:56.000000 zuicorn-1.0.6/zuicorn/wsgi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:31:19.857687 zuicorn-1.0.6/zuicorn.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-20 08:31:19.000000 zuicorn-1.0.6/zuicorn.egg-info/top_level.txt
```

### Comparing `zuicorn-1.0.5/setup.py` & `zuicorn-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zuicorn',
-    version='1.0.5',
+    version='1.0.6',
     description='A WSGI server designed & developed for ZYLO Python web Framework.',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zuicorn',
     packages=find_packages(),
     install_requires=['gevent', 'colorama', 'python-daemon', 'zylo-admin', 'zylo'],  
     classifiers=[
```

### Comparing `zuicorn-1.0.5/zuicorn/wsgi.py` & `zuicorn-1.0.6/zuicorn/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     else:
         server.run()
 
     # Save logs
     if platform.system() == 'Windows':
         log_dir = os.path.join(os.getenv('APPDATA'), 'zyloWSGI', 'logs')
     else:
-        log_dir = os.path.join(Path.home(), 'zyloWSGI', 'logs')
+        log_dir = os.path.expanduser('~/zuicorn/logs')
 
     os.makedirs(log_dir, exist_ok=True)
     log_path = os.path.join(log_dir, 'wsgi.json')
 
     server.save_logs(log_path)
```

