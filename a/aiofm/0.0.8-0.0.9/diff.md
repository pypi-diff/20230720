# Comparing `tmp/aiofm-0.0.8.tar.gz` & `tmp/aiofm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofm-0.0.8.tar", last modified: Sun Mar  5 18:54:25 2023, max compression
+gzip compressed data, was "aiofm-0.0.9.tar", last modified: Sun Mar  5 23:23:13 2023, max compression
```

## Comparing `aiofm-0.0.8.tar` & `aiofm-0.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.900180 aiofm-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-05 18:54:15.000000 aiofm-0.0.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-05 18:54:15.000000 aiofm-0.0.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.892180 aiofm-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.896180 aiofm-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-05 18:54:15.000000 aiofm-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-05 18:54:15.000000 aiofm-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-05 18:54:15.000000 aiofm-0.0.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-05 18:54:15.000000 aiofm-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-05 18:54:15.000000 aiofm-0.0.8/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-05 18:54:15.000000 aiofm-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-05 18:54:15.000000 aiofm-0.0.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-05 18:54:15.000000 aiofm-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-05 18:54:15.000000 aiofm-0.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-05 18:54:15.000000 aiofm-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-05 18:54:15.000000 aiofm-0.0.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-05 18:54:15.000000 aiofm-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-03-05 18:54:15.000000 aiofm-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-05 18:54:15.000000 aiofm-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-05 18:54:15.000000 aiofm-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-05 18:54:25.900180 aiofm-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-05 18:54:15.000000 aiofm-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.896180 aiofm-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.896180 aiofm-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-05 18:54:15.000000 aiofm-0.0.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-05 18:54:15.000000 aiofm-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-05 18:54:15.000000 aiofm-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-05 18:54:15.000000 aiofm-0.0.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-05 18:54:25.900180 aiofm-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-05 18:54:15.000000 aiofm-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.892180 aiofm-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.896180 aiofm-0.0.8/src/aiofm/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.900180 aiofm-0.0.8/src/aiofm/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/protocols/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/protocols/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-05 18:54:15.000000 aiofm-0.0.8/src/aiofm/tst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.896180 aiofm-0.0.8/src/aiofm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-05 18:54:25.000000 aiofm-0.0.8/src/aiofm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.900180 aiofm-0.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:54:25.900180 aiofm-0.0.8/tests/aiofm/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-05 18:54:15.000000 aiofm-0.0.8/tests/aiofm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-03-05 18:54:15.000000 aiofm-0.0.8/tests/aiofm/test_memory_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-03-05 18:54:15.000000 aiofm-0.0.8/tests/aiofm/test_s3_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-05 18:54:15.000000 aiofm-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-05 18:54:15.000000 aiofm-0.0.8/tests/travis_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-05 18:54:15.000000 aiofm-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.587821 aiofm-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-05 23:23:02.000000 aiofm-0.0.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-05 23:23:02.000000 aiofm-0.0.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.579820 aiofm-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.583821 aiofm-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-05 23:23:02.000000 aiofm-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-05 23:23:02.000000 aiofm-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-05 23:23:02.000000 aiofm-0.0.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-05 23:23:02.000000 aiofm-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-05 23:23:02.000000 aiofm-0.0.9/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-05 23:23:02.000000 aiofm-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-05 23:23:02.000000 aiofm-0.0.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-05 23:23:02.000000 aiofm-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-05 23:23:02.000000 aiofm-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-05 23:23:02.000000 aiofm-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-05 23:23:02.000000 aiofm-0.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-05 23:23:02.000000 aiofm-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-03-05 23:23:02.000000 aiofm-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-05 23:23:02.000000 aiofm-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-05 23:23:02.000000 aiofm-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-05 23:23:13.587821 aiofm-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-05 23:23:02.000000 aiofm-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.583821 aiofm-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.583821 aiofm-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-05 23:23:02.000000 aiofm-0.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-05 23:23:02.000000 aiofm-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-05 23:23:02.000000 aiofm-0.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-05 23:23:02.000000 aiofm-0.0.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-05 23:23:13.587821 aiofm-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-05 23:23:02.000000 aiofm-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.579820 aiofm-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.583821 aiofm-0.0.9/src/aiofm/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.587821 aiofm-0.0.9/src/aiofm/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/protocols/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/protocols/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-05 23:23:02.000000 aiofm-0.0.9/src/aiofm/tst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.583821 aiofm-0.0.9/src/aiofm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-05 23:23:13.000000 aiofm-0.0.9/src/aiofm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.587821 aiofm-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 23:23:13.587821 aiofm-0.0.9/tests/aiofm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-05 23:23:02.000000 aiofm-0.0.9/tests/aiofm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-03-05 23:23:02.000000 aiofm-0.0.9/tests/aiofm/test_memory_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-03-05 23:23:02.000000 aiofm-0.0.9/tests/aiofm/test_s3_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-05 23:23:02.000000 aiofm-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-05 23:23:02.000000 aiofm-0.0.9/tests/travis_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-05 23:23:02.000000 aiofm-0.0.9/tox.ini
```

### Comparing `aiofm-0.0.8/.coveragerc` & `aiofm-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/.github/workflows/python-publish.yml` & `aiofm-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/.pre-commit-config.yaml` & `aiofm-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/.travis.yml` & `aiofm-0.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/CONTRIBUTING.rst` & `aiofm-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/LICENSE` & `aiofm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/LICENSE.txt` & `aiofm-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/Makefile` & `aiofm-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/PKG-INFO` & `aiofm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Async file manager for Python
 Home-page: https://github.com/kamikaze/aiofm
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl3
 Project-URL: Documentation, https://github.com/kamikaze/aiofm/wiki
 Platform: any
```

### Comparing `aiofm-0.0.8/README.rst` & `aiofm-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/docs/Makefile` & `aiofm-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/docs/conf.py` & `aiofm-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/docs/index.rst` & `aiofm-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/docs/installation.rst` & `aiofm-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/requirements.txt` & `aiofm-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/setup.cfg` & `aiofm-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/setup.py` & `aiofm-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/src/aiofm/protocols/__init__.py` & `aiofm-0.0.9/src/aiofm/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/src/aiofm/protocols/memory.py` & `aiofm-0.0.9/src/aiofm/protocols/memory.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/src/aiofm/protocols/s3.py` & `aiofm-0.0.9/src/aiofm/protocols/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,46 +38,66 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 class S3WritableFile(BytesIO):
-    def __init__(self, bucket_name, object_key, s3_client):
+    def __init__(self, bucket_name: str, object_key: str, s3_client, part_size: int = 16 * 1024 * 1024):
         super().__init__()
         self.bucket_name = bucket_name
         self.object_key = object_key
         self.s3_client = s3_client
         self.upload_id = None
         self.parts = []
         self.part_number = 1
+        self.part_size = part_size
 
     def write(self, data):
         if isinstance(data, StreamingBody):
             self.s3_client.upload_fileobj(data, self.bucket_name, self.object_key)
         elif isinstance(data, S3ReadableFile):
             self.s3_client.upload_fileobj(data.stream, self.bucket_name, self.object_key)
         elif isinstance(data, bytes):
+            super().write(data)
+
             if not self.upload_id:
                 create_mpu_result = self.s3_client.create_multipart_upload(
                     Bucket=self.bucket_name, Key=self.object_key
                 )
                 self.upload_id = create_mpu_result['UploadId']
 
+            if self.tell() >= self.part_size:
+                self.seek(0)
+                part = self.s3_client.upload_part(
+                    Body=self.read(self.part_size), Bucket=self.bucket_name, Key=self.object_key,
+                    PartNumber=self.part_number, UploadId=self.upload_id
+                )
+                self.seek(0)
+                self.truncate(self.part_size)
+                self.parts.append({'ETag': part['ETag'], 'PartNumber': self.part_number})
+                self.part_number += 1
+        else:
+            raise ValueError(f'Unsupported data type: {type(data)}')
+
+    def flush(self):
+        if self.tell() > 0:
+            self.seek(0)
             part = self.s3_client.upload_part(
-                Body=data, Bucket=self.bucket_name, Key=self.object_key, PartNumber=self.part_number,
-                UploadId=self.upload_id
+                Body=self.read(), Bucket=self.bucket_name, Key=self.object_key,
+                PartNumber=self.part_number, UploadId=self.upload_id
             )
+            self.seek(0)
+            self.truncate()
             self.parts.append({'ETag': part['ETag'], 'PartNumber': self.part_number})
             self.part_number += 1
-        else:
-            raise ValueError(f'Unsupported data type: {type(data)}')
 
     def close(self):
         if self.upload_id and self.parts:
+            self.flush()
             self.s3_client.complete_multipart_upload(
                 Bucket=self.bucket_name, Key=self.object_key, UploadId=self.upload_id,
                 MultipartUpload={'Parts': self.parts}
             )
 
     def __enter__(self):
         return self
```

### Comparing `aiofm-0.0.8/src/aiofm/tst.py` & `aiofm-0.0.9/src/aiofm/tst.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/src/aiofm.egg-info/PKG-INFO` & `aiofm-0.0.9/src/aiofm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Async file manager for Python
 Home-page: https://github.com/kamikaze/aiofm
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl3
 Project-URL: Documentation, https://github.com/kamikaze/aiofm/wiki
 Platform: any
```

### Comparing `aiofm-0.0.8/src/aiofm.egg-info/SOURCES.txt` & `aiofm-0.0.9/src/aiofm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/tests/aiofm/conftest.py` & `aiofm-0.0.9/tests/aiofm/conftest.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/tests/aiofm/test_memory_protocol.py` & `aiofm-0.0.9/tests/aiofm/test_memory_protocol.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/tests/aiofm/test_s3_protocol.py` & `aiofm-0.0.9/tests/aiofm/test_s3_protocol.py`

 * *Files identical despite different names*

### Comparing `aiofm-0.0.8/tests/travis_install.sh` & `aiofm-0.0.9/tests/travis_install.sh`

 * *Files identical despite different names*

