# Comparing `tmp/bagit-create-0.1.8.tar.gz` & `tmp/bagit-create-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagit-create-0.1.8.tar", last modified: Tue May 24 10:13:25 2022, max compression
+gzip compressed data, was "bagit-create-0.1.9.tar", last modified: Tue May 24 14:00:33 2022, max compression
```

## Comparing `bagit-create-0.1.8.tar` & `bagit-create-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 10:13:25.316000 bagit-create-0.1.8/
--rw-r--r--   0 root         (0) root         (0)      142 2022-05-24 10:13:18.000000 bagit-create-0.1.8/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    35171 2022-05-24 10:13:18.000000 bagit-create-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2022-05-24 10:13:18.000000 bagit-create-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    16593 2022-05-24 10:13:25.316000 bagit-create-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15901 2022-05-24 10:13:18.000000 bagit-create-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 10:13:25.312000 bagit-create-0.1.8/bagit_create/
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/bibdocfile.py
--rw-r--r--   0 root         (0) root         (0)     3258 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/cds.py
--rwxr-xr-x   0 root         (0) root         (0)     4815 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/cli.py
--rw-r--r--   0 root         (0) root         (0)     1685 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/cod.py
--rw-r--r--   0 root         (0) root         (0)     9604 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 10:13:25.316000 bagit-create-0.1.8/bagit_create/pipelines/
--rw-r--r--   0 root         (0) root         (0)    16453 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/base.py
--rw-r--r--   0 root         (0) root         (0)     2923 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/codimd.py
--rw-r--r--   0 root         (0) root         (0)     8615 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/indico.py
--rw-r--r--   0 root         (0) root         (0)     7498 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/invenio_v1.py
--rw-r--r--   0 root         (0) root         (0)     5766 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/invenio_v3.py
--rw-r--r--   0 root         (0) root         (0)     4802 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/local.py
--rw-r--r--   0 root         (0) root         (0)     6028 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/pipelines/opendata.py
--rw-r--r--   0 root         (0) root         (0)      109 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 10:13:25.316000 bagit-create-0.1.8/bagit_create/test/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3412 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/bdf_test.py
--rw-r--r--   0 root         (0) root         (0)     1753 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/local_test.py
--rw-r--r--   0 root         (0) root         (0)     2546 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/main_test.py
--rw-r--r--   0 root         (0) root         (0)     3347 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/upstream_pipeline_test.py
--rw-r--r--   0 root         (0) root         (0)      811 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/test/urlparse_test.py
--rw-r--r--   0 root         (0) root         (0)     1076 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-05-24 10:13:18.000000 bagit-create-0.1.8/bagit_create/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 10:13:25.316000 bagit-create-0.1.8/bagit_create.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16593 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      930 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      337 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-05-24 10:13:25.000000 bagit-create-0.1.8/bagit_create.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-05-24 10:13:18.000000 bagit-create-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      166 2022-05-24 10:13:25.316000 bagit-create-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2017 2022-05-24 10:13:18.000000 bagit-create-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 14:00:33.032000 bagit-create-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)      142 2022-05-24 14:00:26.000000 bagit-create-0.1.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    35171 2022-05-24 14:00:26.000000 bagit-create-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       92 2022-05-24 14:00:26.000000 bagit-create-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16593 2022-05-24 14:00:33.032000 bagit-create-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15901 2022-05-24 14:00:26.000000 bagit-create-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 14:00:33.028000 bagit-create-0.1.9/bagit_create/
+-rw-r--r--   0 root         (0) root         (0)       25 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/bibdocfile.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/cds.py
+-rwxr-xr-x   0 root         (0) root         (0)     4815 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/cod.py
+-rw-r--r--   0 root         (0) root         (0)     9604 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 14:00:33.028000 bagit-create-0.1.9/bagit_create/pipelines/
+-rw-r--r--   0 root         (0) root         (0)    16453 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/base.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/codimd.py
+-rw-r--r--   0 root         (0) root         (0)     8615 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/indico.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/invenio.ini
+-rw-r--r--   0 root         (0) root         (0)     7498 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/invenio_v1.py
+-rw-r--r--   0 root         (0) root         (0)     5766 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/invenio_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/local.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/pipelines/opendata.py
+-rw-r--r--   0 root         (0) root         (0)      109 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 14:00:33.028000 bagit-create-0.1.9/bagit_create/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/bdf_test.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/local_test.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/main_test.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/upstream_pipeline_test.py
+-rw-r--r--   0 root         (0) root         (0)      811 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/test/urlparse_test.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-05-24 14:00:26.000000 bagit-create-0.1.9/bagit_create/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-24 14:00:33.028000 bagit-create-0.1.9/bagit_create.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16593 2022-05-24 14:00:32.000000 bagit-create-0.1.9/bagit_create.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      965 2022-05-24 14:00:33.000000 bagit-create-0.1.9/bagit_create.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-24 14:00:32.000000 bagit-create-0.1.9/bagit_create.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2022-05-24 14:00:32.000000 bagit-create-0.1.9/bagit_create.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2022-05-24 14:00:32.000000 bagit-create-0.1.9/bagit_create.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-05-24 14:00:32.000000 bagit-create-0.1.9/bagit_create.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-05-24 14:00:26.000000 bagit-create-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      166 2022-05-24 14:00:33.032000 bagit-create-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2017 2022-05-24 14:00:26.000000 bagit-create-0.1.9/setup.py
```

### Comparing `bagit-create-0.1.8/LICENSE` & `bagit-create-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/PKG-INFO` & `bagit-create-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagit-create
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create BagIt packages harvesting data from upstream sources
 Home-page: https://gitlab.cern.ch/digitalmemory/bagit-create
 Author: Antonio Vivace
 Author-email: antonio.vivace@cern.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bagit-create-0.1.8/README.md` & `bagit-create-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/bibdocfile.py` & `bagit-create-0.1.9/bagit_create/bibdocfile.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/cds.py` & `bagit-create-0.1.9/bagit_create/cds.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/cli.py` & `bagit-create-0.1.9/bagit_create/cli.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/cod.py` & `bagit-create-0.1.9/bagit_create/cod.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/main.py` & `bagit-create-0.1.9/bagit_create/main.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/base.py` & `bagit-create-0.1.9/bagit_create/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/codimd.py` & `bagit-create-0.1.9/bagit_create/pipelines/codimd.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/indico.py` & `bagit-create-0.1.9/bagit_create/pipelines/indico.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/invenio_v1.py` & `bagit-create-0.1.9/bagit_create/pipelines/invenio_v1.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/invenio_v3.py` & `bagit-create-0.1.9/bagit_create/pipelines/invenio_v3.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/local.py` & `bagit-create-0.1.9/bagit_create/pipelines/local.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/pipelines/opendata.py` & `bagit-create-0.1.9/bagit_create/pipelines/opendata.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/test/bdf_test.py` & `bagit-create-0.1.9/bagit_create/test/bdf_test.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/test/local_test.py` & `bagit-create-0.1.9/bagit_create/test/local_test.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/test/main_test.py` & `bagit-create-0.1.9/bagit_create/test/main_test.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/test/upstream_pipeline_test.py` & `bagit-create-0.1.9/bagit_create/test/upstream_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/test/urlparse_test.py` & `bagit-create-0.1.9/bagit_create/test/urlparse_test.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create/utils.py` & `bagit-create-0.1.9/bagit_create/utils.py`

 * *Files identical despite different names*

### Comparing `bagit-create-0.1.8/bagit_create.egg-info/PKG-INFO` & `bagit-create-0.1.9/bagit_create.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagit-create
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create BagIt packages harvesting data from upstream sources
 Home-page: https://gitlab.cern.ch/digitalmemory/bagit-create
 Author: Antonio Vivace
 Author-email: antonio.vivace@cern.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bagit-create-0.1.8/bagit_create.egg-info/SOURCES.txt` & `bagit-create-0.1.9/bagit_create.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 bagit_create.egg-info/dependency_links.txt
 bagit_create.egg-info/entry_points.txt
 bagit_create.egg-info/requires.txt
 bagit_create.egg-info/top_level.txt
 bagit_create/pipelines/base.py
 bagit_create/pipelines/codimd.py
 bagit_create/pipelines/indico.py
+bagit_create/pipelines/invenio.ini
 bagit_create/pipelines/invenio_v1.py
 bagit_create/pipelines/invenio_v3.py
 bagit_create/pipelines/local.py
 bagit_create/pipelines/opendata.py
 bagit_create/test/__init__.py
 bagit_create/test/bdf_test.py
 bagit_create/test/local_test.py
```

### Comparing `bagit-create-0.1.8/setup.py` & `bagit-create-0.1.9/setup.py`

 * *Files identical despite different names*

