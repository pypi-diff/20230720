# Comparing `tmp/gitlab-ci-generator-1.0.8.tar.gz` & `tmp/gitlab-ci-generator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.8.tar", last modified: Sat Jun  3 18:40:38 2023, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.9.tar", last modified: Thu Jul 20 13:31:43 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.8.tar` & `gitlab-ci-generator-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     9632 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.8/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.949511 gitlab-ci-generator-1.0.8/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     2220 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-07-20 13:31:43.714470 gitlab-ci-generator-1.0.9/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.9/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-07-20 13:31:43.714470 gitlab-ci-generator-1.0.9/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     9632 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.9/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-07-20 13:31:43.714470 gitlab-ci-generator-1.0.9/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1142 2023-07-20 13:31:27.000000 gitlab-ci-generator-1.0.9/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-07-20 13:31:43.710471 gitlab-ci-generator-1.0.9/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-07-20 13:31:43.710471 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-07-20 13:31:43.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-07-20 13:31:43.714470 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-07-20 13:31:43.714470 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     2220 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.8/PKG-INFO` & `gitlab-ci-generator-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
```

### Comparing `gitlab-ci-generator-1.0.8/README.md` & `gitlab-ci-generator-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.8/setup.py` & `gitlab-ci-generator-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
-from packaging.version import Version
+# from packaging.version import Version
 from os.path import exists
 
 if exists("VERSION.txt"):
     with open("VERSION.txt", "r") as fh:
         version_string = fh.read()
 else:
     version_string = "0.0.0"
-version = Version(version_string)
+# version = Version(version_string)
+version = version_string
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gitlab-ci-generator',
     description='Generates a mono-repo ci file.',
```

### Comparing `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.9/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
```

### Comparing `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.9/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files identical despite different names*

