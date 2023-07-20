# Comparing `tmp/ou_container_content-1.1.4.tar.gz` & `tmp/ou_container_content-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_container_content-1.1.4.tar", max compression
+gzip compressed data, was "ou_container_content-1.2.0.tar", max compression
```

## Comparing `ou_container_content-1.1.4.tar` & `ou_container_content-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      588 2023-06-28 14:39:18.873439 ou_container_content-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       57 2023-06-28 14:39:18.873439 ou_container_content-1.1.4/src/ou_container_content/__init__.py
--rw-r--r--   0        0        0     2846 2023-06-28 14:39:18.873439 ou_container_content-1.1.4/src/ou_container_content/__main__.py
--rw-r--r--   0        0        0     6505 2023-06-28 14:39:18.874439 ou_container_content-1.1.4/src/ou_container_content/distributor.py
--rw-r--r--   0        0        0       40 2023-06-28 14:39:18.874439 ou_container_content-1.1.4/src/ou_container_content/frontend/__init__.py
--rw-r--r--   0        0        0       40 2023-06-28 14:39:18.874439 ou_container_content-1.1.4/src/ou_container_content/frontend/build/__init__.py
--rw-r--r--   0        0        0     5544 2023-06-28 14:39:18.874439 ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.css
--rw-r--r--   0        0        0     7148 2023-06-28 14:39:18.874439 ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.js
--rw-r--r--   0        0        0    68795 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.js.map
--rw-r--r--   0        0        0      890 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/global.css
--rw-r--r--   0        0        0      642 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/index.html
--rw-r--r--   0        0        0      503 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-1.png
--rw-r--r--   0        0        0      703 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-2.png
--rw-r--r--   0        0        0      897 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-3.png
--rw-r--r--   0        0        0     1601 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-4.png
--rw-r--r--   0        0        0     2946 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/handlers.py
--rw-r--r--   0        0        0     1594 2023-06-28 14:39:18.875439 ou_container_content-1.1.4/src/ou_container_content/process.py
--rw-r--r--   0        0        0     1499 2023-06-28 14:39:18.876439 ou_container_content-1.1.4/src/ou_container_content/scripts.py
--rw-r--r--   0        0        0     1345 2023-06-28 14:39:18.876439 ou_container_content-1.1.4/src/ou_container_content/services.py
--rw-r--r--   0        0        0     3180 2023-06-28 14:39:18.876439 ou_container_content-1.1.4/src/ou_container_content/validator.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 ou_container_content-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-07-20 11:35:28.799952 ou_container_content-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-07-20 11:35:28.799952 ou_container_content-1.2.0/src/ou_container_content/__init__.py
+-rw-r--r--   0        0        0     2846 2023-07-20 11:35:28.812953 ou_container_content-1.2.0/src/ou_container_content/__main__.py
+-rw-r--r--   0        0        0     6505 2023-07-20 11:35:28.812953 ou_container_content-1.2.0/src/ou_container_content/distributor.py
+-rw-r--r--   0        0        0       40 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/build/__init__.py
+-rw-r--r--   0        0        0     5544 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.css
+-rw-r--r--   0        0        0     7148 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.js
+-rw-r--r--   0        0        0    68795 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.js.map
+-rw-r--r--   0        0        0      890 2023-07-20 11:35:28.813953 ou_container_content-1.2.0/src/ou_container_content/frontend/global.css
+-rw-r--r--   0        0        0      642 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/frontend/index.html
+-rw-r--r--   0        0        0      503 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-1.png
+-rw-r--r--   0        0        0      703 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-2.png
+-rw-r--r--   0        0        0      897 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-3.png
+-rw-r--r--   0        0        0     1601 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-4.png
+-rw-r--r--   0        0        0     2946 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/handlers.py
+-rw-r--r--   0        0        0     1594 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/process.py
+-rw-r--r--   0        0        0     1499 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/scripts.py
+-rw-r--r--   0        0        0     1345 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/services.py
+-rw-r--r--   0        0        0     3180 2023-07-20 11:35:28.814953 ou_container_content-1.2.0/src/ou_container_content/validator.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 ou_container_content-1.2.0/PKG-INFO
```

### Comparing `ou_container_content-1.1.4/pyproject.toml` & `ou_container_content-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ou-container-content"
-version = "1.1.4"
+version = "1.2.0"
 description = ""
 authors = ["Mark Hall <mark.hall@open.ac.uk>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.0"
 Cerberus = "^1.3.3"
 tornado = "^6.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.3"
 flake8 = "^3.9.1"
 flake8-docstrings = "^1.6.0"
```

### Comparing `ou_container_content-1.1.4/src/ou_container_content/__main__.py` & `ou_container_content-1.2.0/src/ou_container_content/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/distributor.py` & `ou_container_content-1.2.0/src/ou_container_content/distributor.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.css` & `ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.css`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.js` & `ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.js`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/build/bundle.js.map` & `ou_container_content-1.2.0/src/ou_container_content/frontend/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/global.css` & `ou_container_content-1.2.0/src/ou_container_content/frontend/global.css`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/index.html` & `ou_container_content-1.2.0/src/ou_container_content/frontend/index.html`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-2.png` & `ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-2.png`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-3.png` & `ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-3.png`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/frontend/ou-favicon-4.png` & `ou_container_content-1.2.0/src/ou_container_content/frontend/ou-favicon-4.png`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/handlers.py` & `ou_container_content-1.2.0/src/ou_container_content/handlers.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/process.py` & `ou_container_content-1.2.0/src/ou_container_content/process.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/scripts.py` & `ou_container_content-1.2.0/src/ou_container_content/scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/services.py` & `ou_container_content-1.2.0/src/ou_container_content/services.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/src/ou_container_content/validator.py` & `ou_container_content-1.2.0/src/ou_container_content/validator.py`

 * *Files identical despite different names*

### Comparing `ou_container_content-1.1.4/PKG-INFO` & `ou_container_content-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ou-container-content
-Version: 1.1.4
+Version: 1.2.0
 Summary: 
 Author: Mark Hall
 Author-email: mark.hall@open.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Cerberus (>=1.3.3,<2.0.0)
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: tornado (>=6.1,<7.0)
```

