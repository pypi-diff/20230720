# Comparing `tmp/ape-polygon-0.6.4.tar.gz` & `tmp/ape-polygon-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.6.4.tar", last modified: Tue Jun 13 14:05:41 2023, max compression
+gzip compressed data, was "ape-polygon-0.6.5.tar", last modified: Thu Jul 20 13:08:57 2023, max compression
```

## Comparing `ape-polygon-0.6.4.tar` & `ape-polygon-0.6.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 13:08:57.000000 ape-polygon-0.6.5/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:08:57.455962 ape-polygon-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 13:07:34.000000 ape-polygon-0.6.5/tests/test_provider.py
```

### Comparing `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/release-drafter.yml` & `ape-polygon-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/workflows/commitlint.yaml` & `ape-polygon-0.6.5/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/workflows/prtitle.yaml` & `ape-polygon-0.6.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/workflows/publish.yaml` & `ape-polygon-0.6.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.github/workflows/test.yaml` & `ape-polygon-0.6.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.gitignore` & `ape-polygon-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/.pre-commit-config.yaml` & `ape-polygon-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/CONTRIBUTING.md` & `ape-polygon-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/LICENSE` & `ape-polygon-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/PKG-INFO` & `ape-polygon-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-polygon-0.6.4/README.md` & `ape-polygon-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/ape_polygon/__init__.py` & `ape-polygon-0.6.5/ape_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/ape_polygon/ecosystem.py` & `ape-polygon-0.6.5/ape_polygon/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.6.5/ape_polygon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-polygon-0.6.4/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.6.5/ape_polygon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/ape_polygon.egg-info/requires.txt` & `ape-polygon-0.6.5/ape_polygon.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 eth-ape<0.7,>=0.6.0
-typing-extensions==4.5.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 black<24,>=23.3.0
```

### Comparing `ape-polygon-0.6.4/pyproject.toml` & `ape-polygon-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.4/setup.py` & `ape-polygon-0.6.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-polygon",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.0,<0.7",
-        "typing-extensions==4.5.0",  # Can remove once Pydantic patched and ape updated.
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_polygon"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `ape-polygon-0.6.4/tests/test_integration.py` & `ape-polygon-0.6.5/tests/test_integration.py`

 * *Files identical despite different names*

