# Comparing `tmp/ai-aside-3.0.0.tar.gz` & `tmp/ai-aside-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-aside-3.0.0.tar", last modified: Mon Jul 17 15:04:42 2023, max compression
+gzip compressed data, was "ai-aside-3.0.1.tar", last modified: Thu Jul 20 14:10:32 2023, max compression
```

## Comparing `ai-aside-3.0.0.tar` & `ai-aside-3.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-17 15:04:38.000000 ai-aside-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-17 15:04:38.000000 ai-aside-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-17 15:04:38.000000 ai-aside-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8385 2023-07-17 15:04:42.959770 ai-aside-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-17 15:04:38.000000 ai-aside-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/platform_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/ai_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8385 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-17 15:04:38.000000 ai-aside-3.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-17 15:04:38.000000 ai-aside-3.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-17 15:04:42.959770 ai-aside-3.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5302 2023-07-17 15:04:38.000000 ai-aside-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_block.py
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-20 14:10:26.000000 ai-aside-3.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-20 14:10:26.000000 ai-aside-3.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-20 14:10:26.000000 ai-aside-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8514 2023-07-20 14:10:32.349169 ai-aside-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-20 14:10:26.000000 ai-aside-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.345168 ai-aside-3.0.1/ai_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8561 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/ai_aside/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/platform_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/ai_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.345168 ai-aside-3.0.1/ai_aside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8514 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-20 14:10:26.000000 ai-aside-3.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-20 14:10:26.000000 ai-aside-3.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-20 14:10:32.349169 ai-aside-3.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5302 2023-07-20 14:10:26.000000 ai-aside-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_text_utils.py
```

### Comparing `ai-aside-3.0.0/CHANGELOG.rst` & `ai-aside-3.0.1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+3.0.1 – 2023-07-20
+**********************************************
+
+* Add positive log when summary fragement decides to inject
 
 3.0.0 – 2023-07-16
 **********************************************
 
 Features
 =========
 * Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_70c84ud4_/tmpk27_s4za_TarContainer/0/1.rst", line 70, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_70c84ud4_/tmpk27_s4za_TarContainer/0/1.rst", line 70, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,14 @@
 Change Log ########## .. All enhancements and patches to ai_aside will be
 documented in this file. It adheres to the structure of https://
 keepachangelog.com/ , but in reStructuredText instead of Markdown (for ease of
 incorporation into Sphinx documentation and the PyPI description). This project
 adheres to Semantic Versioning (https://semver.org/). .. There should always be
 an "Unreleased" section for changes pending release. Unreleased **********
-3.0.0 â 2023-07-16 ********************************************** Features
-========= * Summary content handler now requires a staff user identity,
-otherwise returns 403. This is a breaking change. * Added models to
-summaryhook_aside (Has migrations) * Catch exceptions in a couple of locations
-so the aside cannot crash content. 2.0.2 â 2023-07-05
-********************************************** Fix ===== * Updated HTML parser
-to remove tags with their content for specific cases like `
+3.0.1 â 2023-07-20 ********************************************** * Add
+positive log when summary fragement decides to inject 3.0.0 â 2023-07-16
+********************************************** Features ========= * Summary
+content handler now requires a staff user identity, otherwise returns 403. This
+is a breaking change. * Added models to summaryhook_aside (Has migrations) *
+Catch exceptions in a couple of locations so the aside cannot crash content.
+2.0.2 â 2023-07-05 ********************************************** Fix ===== *
+Updated HTML parser to remove tags with their content for specific cases like `
```

### Comparing `ai-aside-3.0.0/LICENSE.txt` & `ai-aside-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/PKG-INFO` & `ai-aside-3.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 3.0.0
+Version: 3.0.1
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -207,14 +207,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+3.0.1 – 2023-07-20
+**********************************************
+
+* Add positive log when summary fragement decides to inject
 
 3.0.0 – 2023-07-16
 **********************************************
 
 Features
 =========
 * Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
```

### Comparing `ai-aside-3.0.0/README.rst` & `ai-aside-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/apps.py` & `ai-aside-3.0.1/ai_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/block.py` & `ai-aside-3.0.1/ai_aside/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,22 +205,26 @@
         fragment = Fragment('')
 
         # Check if there is content that worths summarizing
         length, _ = _parse_children_contents(block)
         if length < settings.SUMMARY_HOOK_MIN_SIZE:
             return fragment
 
+        usage_id = block.scope_ids.usage_id
+
+        log.info(f'Summary hook injecting into {usage_id}')
+
         handler_url = self._summary_handler_url()
 
         fragment.add_content(
             _render_summary(
                 {
                     'data_url_api': settings.SUMMARY_HOOK_HOST,
-                    'data_course_id': block.scope_ids.usage_id.course_key,
-                    'data_content_id': block.scope_ids.usage_id,
+                    'data_course_id': usage_id.course_key,
+                    'data_content_id': usage_id,
                     'data_handler_url': handler_url,
                     'js_url': settings.SUMMARY_HOOK_HOST + settings.SUMMARY_HOOK_JS_PATH,
                 }
             )
         )
         return fragment
```

### Comparing `ai-aside-3.0.0/ai_aside/migrations/0001_initial.py` & `ai-aside-3.0.1/ai_aside/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/models.py` & `ai-aside-3.0.1/ai_aside/models.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/platform_imports.py` & `ai-aside-3.0.1/ai_aside/platform_imports.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/settings/devstack.py` & `ai-aside-3.0.1/ai_aside/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/text_utils.py` & `ai-aside-3.0.1/ai_aside/text_utils.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside/waffle.py` & `ai-aside-3.0.1/ai_aside/waffle.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/ai_aside.egg-info/PKG-INFO` & `ai-aside-3.0.1/ai_aside.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 3.0.0
+Version: 3.0.1
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -207,14 +207,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+3.0.1 – 2023-07-20
+**********************************************
+
+* Add positive log when summary fragement decides to inject
 
 3.0.0 – 2023-07-16
 **********************************************
 
 Features
 =========
 * Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
```

### Comparing `ai-aside-3.0.0/ai_aside.egg-info/SOURCES.txt` & `ai-aside-3.0.1/ai_aside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/requirements/constraints.txt` & `ai-aside-3.0.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/setup.py` & `ai-aside-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/tests/test_block.py` & `ai-aside-3.0.1/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/tests/test_models.py` & `ai-aside-3.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.0/tests/test_text_utils.py` & `ai-aside-3.0.1/tests/test_text_utils.py`

 * *Files identical despite different names*

