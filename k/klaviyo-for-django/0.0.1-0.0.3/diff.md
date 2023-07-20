# Comparing `tmp/klaviyo-for-django-0.0.1.tar.gz` & `tmp/klaviyo-for-django-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-for-django-0.0.1.tar", last modified: Thu Jul 20 16:03:34 2023, max compression
+gzip compressed data, was "klaviyo-for-django-0.0.3.tar", last modified: Thu Jul 20 18:32:29 2023, max compression
```

## Comparing `klaviyo-for-django-0.0.1.tar` & `klaviyo-for-django-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:34.286201 klaviyo-for-django-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 16:03:21.000000 klaviyo-for-django-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 16:03:34.286201 klaviyo-for-django-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 16:03:21.000000 klaviyo-for-django-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:34.282200 klaviyo-for-django-0.0.1/klaviyo_for_django/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 16:03:21.000000 klaviyo-for-django-0.0.1/klaviyo_for_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:03:34.282200 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 16:03:34.000000 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 16:03:34.000000 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:03:34.000000 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 16:03:34.000000 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 16:03:34.000000 klaviyo-for-django-0.0.1/klaviyo_for_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:03:34.286201 klaviyo-for-django-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-20 16:03:21.000000 klaviyo-for-django-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/klaviyo_for_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/klaviyo_for_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/setup.py
```

### Comparing `klaviyo-for-django-0.0.1/LICENSE` & `klaviyo-for-django-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-for-django-0.0.1/setup.py` & `klaviyo-for-django-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="klaviyo-for-django",
-    version="0.0.1",
+    version="0.0.3",
     author="Santiago Fernandez",
     author_email="",
     packages=find_packages(),
     scripts=[],
     url="http://pypi.python.org/pypi/klaviyo-for-django/",
     license="MIT",
     description="",
```

