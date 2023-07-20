# Comparing `tmp/emark-1.1rc1.tar.gz` & `tmp/emark-1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emark-1.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "emark-1.1rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `emark-1.1rc1.tar` & `emark-1.1rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1518 2023-07-20 14:33:00.770370 emark-1.1rc1/LICENSE
--rw-r--r--   0        0        0     5944 2023-07-20 14:33:00.770370 emark-1.1rc1/README.md
--rw-r--r--   0        0        0      152 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/__init__.py
--rw-r--r--   0        0        0      158 2023-07-20 14:33:46.338776 emark-1.1rc1/emark/_version.py
--rw-r--r--   0        0        0     2244 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/backends.py
--rw-r--r--   0        0        0     1030 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/buildapi.py
--rw-r--r--   0        0        0      309 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/conf.py
--rw-r--r--   0        0        0      535 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9005 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/message.py
--rw-r--r--   0        0        0     3474 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/migrations/__init__.py
--rw-r--r--   0        0        0     2238 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/models.py
--rw-r--r--   0        0        0     3259 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/base.html
--rw-r--r--   0        0        0     1081 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/license.txt
--rw-r--r--   0        0        0     5945 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/styles.css
--rw-r--r--   0        0        0      325 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/urls.py
--rw-r--r--   0        0        0     3796 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/utils.py
--rw-r--r--   0        0        0     2343 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/views.py
--rw-r--r--   0        0        0     2302 2023-07-20 14:33:00.770370 emark-1.1rc1/pyproject.toml
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-07-20 16:18:52.533908 emark-1.1rc2/LICENSE
+-rw-r--r--   0        0        0     5944 2023-07-20 16:18:52.533908 emark-1.1rc2/README.md
+-rw-r--r--   0        0        0      152 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-20 16:19:13.853742 emark-1.1rc2/emark/_version.py
+-rw-r--r--   0        0        0     2736 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/backends.py
+-rw-r--r--   0        0        0     1030 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/buildapi.py
+-rw-r--r--   0        0        0      309 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/conf.py
+-rw-r--r--   0        0        0      535 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9005 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/message.py
+-rw-r--r--   0        0        0     3474 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/migrations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/models.py
+-rw-r--r--   0        0        0     3259 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/templates/emark/base.html
+-rw-r--r--   0        0        0     1081 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/templates/emark/license.txt
+-rw-r--r--   0        0        0     5945 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/templates/emark/styles.css
+-rw-r--r--   0        0        0      325 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/urls.py
+-rw-r--r--   0        0        0     3796 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/utils.py
+-rw-r--r--   0        0        0     2343 2023-07-20 16:18:52.533908 emark-1.1rc2/emark/views.py
+-rw-r--r--   0        0        0     2302 2023-07-20 16:18:52.533908 emark-1.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc2/PKG-INFO
```

### Comparing `emark-1.1rc1/LICENSE` & `emark-1.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/README.md` & `emark-1.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/buildapi.py` & `emark-1.1rc2/emark/buildapi.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/locale/de/LC_MESSAGES/django.po` & `emark-1.1rc2/emark/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/message.py` & `emark-1.1rc2/emark/message.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/migrations/0001_initial.py` & `emark-1.1rc2/emark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/models.py` & `emark-1.1rc2/emark/models.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/templates/emark/base.html` & `emark-1.1rc2/emark/templates/emark/base.html`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/templates/emark/license.txt` & `emark-1.1rc2/emark/templates/emark/license.txt`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/templates/emark/styles.css` & `emark-1.1rc2/emark/templates/emark/styles.css`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/utils.py` & `emark-1.1rc2/emark/utils.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/emark/views.py` & `emark-1.1rc2/emark/views.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/pyproject.toml` & `emark-1.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emark-1.1rc1/PKG-INFO` & `emark-1.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emark
-Version: 1.1rc1
+Version: 1.1rc2
 Summary: Markdown template based HTML and text emails for Django.
 Keywords: Markdown,Django,email,templates,HTML
 Author-email: Rust Saiargaliev <fly.amureki@gmail.com>, Johannes Maron <johannes@maron.family>, Mostafa Mohamed <mostafa.anm91@gmail.com>, Jacqueline Kraus <jacquelinekraus1992@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

