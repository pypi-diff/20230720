# Comparing `tmp/rayvision_utils-1.2.1.tar.gz` & `tmp/rayvision_utils-1.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_utils-1.2.1.tar", last modified: Wed Aug 18 06:49:00 2021, max compression
+gzip compressed data, was "dist/rayvision_utils-1.2.2.1.tar", last modified: Thu Jul 20 08:47:46 2023, max compression
```

## Comparing `rayvision_utils-1.2.1.tar` & `rayvision_utils-1.2.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      243 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      259 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)      216 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)      454 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      658 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       44 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5344 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/docs/rayvision_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/docs/rayvision_utils/core/
--rw-rw-rw-   0 root         (0) root         (0)      163 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/core/analyse_handle.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/core/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)      744 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/core/exception.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/core/json_handle.rst
--rw-rw-rw-   0 root         (0) root         (0)     3025 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/first_look.rst
--rw-rw-rw-   0 root         (0) root         (0)      853 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/installation_guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      184 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/docs/rayvision_utils/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      452 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils/
--rw-rw-rw-   0 root         (0) root         (0)      343 2021-03-09 11:11:40.000000 rayvision_utils-1.2.1/rayvision_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2729 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/cmd.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2021-08-18 06:29:10.000000 rayvision_utils-1.2.1/rayvision_utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils/exception/
--rw-rw-rw-   0 root         (0) root         (0)       17 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/exception/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/exception/error_msg.py
--rw-rw-rw-   0 root         (0) root         (0)     4431 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/exception/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     2105 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/exception/tips.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/exception/tips_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)       13 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2226 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/test_cmd.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/test_exception.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/test_tips.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3939 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/rayvision_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      454 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1742 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/rayvision_utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       89 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2021-08-18 06:49:00.000000 rayvision_utils-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      979 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2020-05-25 02:35:50.000000 rayvision_utils-1.2.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5344 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/core/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/core/analyse_handle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/core/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/core/exception.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/core/json_handle.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/first_look.rst
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/installation_guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/docs/rayvision_utils/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils/
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2729 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/error_msg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4431 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/tips.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/exception/tips_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/test_cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/test_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/test_tips.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/rayvision_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/rayvision_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-20 08:47:46.000000 rayvision_utils-1.2.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-05 11:45:23.000000 rayvision_utils-1.2.2.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2023-07-20 08:35:02.000000 rayvision_utils-1.2.2.1/tox.ini
```

### Comparing `rayvision_utils-1.2.1/.pre-commit-config.yaml` & `rayvision_utils-1.2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/README.md` & `rayvision_utils-1.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/Makefile` & `rayvision_utils-1.2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/conf.py` & `rayvision_utils-1.2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/index.rst` & `rayvision_utils-1.2.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/make.bat` & `rayvision_utils-1.2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/rayvision_utils/core/exception.rst` & `rayvision_utils-1.2.2.1/docs/rayvision_utils/core/exception.rst`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/rayvision_utils/first_look.rst` & `rayvision_utils-1.2.2.1/docs/rayvision_utils/first_look.rst`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/docs/rayvision_utils/installation_guide.rst` & `rayvision_utils-1.2.2.1/docs/rayvision_utils/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/cmd.py` & `rayvision_utils-1.2.2.1/rayvision_utils/cmd.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/constants.py` & `rayvision_utils-1.2.2.1/rayvision_utils/constants.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/exception/error_msg.py` & `rayvision_utils-1.2.2.1/rayvision_utils/exception/error_msg.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/exception/exception.py` & `rayvision_utils-1.2.2.1/rayvision_utils/exception/exception.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/exception/tips.py` & `rayvision_utils-1.2.2.1/rayvision_utils/exception/tips.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/exception/tips_code.py` & `rayvision_utils-1.2.2.1/rayvision_utils/exception/tips_code.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/tests/conftest.py` & `rayvision_utils-1.2.2.1/rayvision_utils/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/tests/test_exception.py` & `rayvision_utils-1.2.2.1/rayvision_utils/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/tests/test_tips.py` & `rayvision_utils-1.2.2.1/rayvision_utils/tests/test_tips.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/tests/test_utils.py` & `rayvision_utils-1.2.2.1/rayvision_utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils/utils.py` & `rayvision_utils-1.2.2.1/rayvision_utils/utils.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/rayvision_utils.egg-info/SOURCES.txt` & `rayvision_utils-1.2.2.1/rayvision_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/setup.py` & `rayvision_utils-1.2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_utils-1.2.1/tox.ini` & `rayvision_utils-1.2.2.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 commands =
   pytest --cov={env:CI_PROJECT_NAME} --cov-append {posargs}
 
 [testenv:deploy]
 deps =
     twine
 commands =
+    pip install requests==2.28.2
     python setup.py bdist_wheel register -r rayvision_pip upload -r rayvision_pip
     python setup.py sdist
     twine upload --repository pypi dist/*
 
 [testenv:pre-commit]
 skip_install = true
 deps =  pre-commit
```

