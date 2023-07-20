# Comparing `tmp/molgenis_emx2_pyclient-8.207.1.tar.gz` & `tmp/molgenis_emx2_pyclient-8.207.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.207.1.tar", last modified: Wed Jul 19 07:03:37 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.207.2.tar", last modified: Thu Jul 20 08:12:17 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.207.1.tar` & `molgenis_emx2_pyclient-8.207.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:03:37.315318 molgenis_emx2_pyclient-8.207.1/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-19 07:03:37.315318 molgenis_emx2_pyclient-8.207.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 07:03:37.319318 molgenis_emx2_pyclient-8.207.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:03:37.315318 molgenis_emx2_pyclient-8.207.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:03:37.315318 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-19 06:53:53.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:03:37.315318 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-19 07:03:37.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-19 07:03:37.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 07:03:37.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-19 07:03:37.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 07:03:37.000000 molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-19 06:59:25.000000 molgenis_emx2_pyclient-8.207.1/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:12:17.711750 molgenis_emx2_pyclient-8.207.2/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-20 08:12:17.711750 molgenis_emx2_pyclient-8.207.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 08:12:17.711750 molgenis_emx2_pyclient-8.207.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:12:17.707750 molgenis_emx2_pyclient-8.207.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:12:17.711750 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-20 08:02:23.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:12:17.711750 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-20 08:12:17.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-20 08:12:17.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:12:17.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-20 08:12:17.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 08:12:17.000000 molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 08:08:12.000000 molgenis_emx2_pyclient-8.207.2/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.207.1/LICENSE` & `molgenis_emx2_pyclient-8.207.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.207.1/PKG-INFO` & `molgenis_emx2_pyclient-8.207.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.207.1
+Version: 8.207.2
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.207.1/README.md` & `molgenis_emx2_pyclient-8.207.2/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.207.1/pyproject.toml` & `molgenis_emx2_pyclient-8.207.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.207.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.207.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.207.1
+Version: 8.207.2
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

