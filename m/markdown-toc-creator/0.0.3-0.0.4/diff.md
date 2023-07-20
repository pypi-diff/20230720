# Comparing `tmp/markdown_toc_creator-0.0.3.tar.gz` & `tmp/markdown_toc_creator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_toc_creator-0.0.3.tar", last modified: Wed Jul 19 10:03:10 2023, max compression
+gzip compressed data, was "markdown_toc_creator-0.0.4.tar", last modified: Thu Jul 20 08:09:11 2023, max compression
```

## Comparing `markdown_toc_creator-0.0.3.tar` & `markdown_toc_creator-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/markdown_toc_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/markdown_toc_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/markdown_toc_creator/create_toc.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/markdown_toc_creator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/markdown_toc_creator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/markdown_toc_creator/toc_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 10:03:10.000000 markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:10.402948 markdown_toc_creator-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-19 10:02:59.000000 markdown_toc_creator-0.0.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/markdown_toc_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/markdown_toc_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/markdown_toc_creator/create_toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/markdown_toc_creator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/markdown_toc_creator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/markdown_toc_creator/toc_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 08:09:11.000000 markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:09:11.832854 markdown_toc_creator-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-20 08:09:00.000000 markdown_toc_creator-0.0.4/tests/test_main.py
```

### Comparing `markdown_toc_creator-0.0.3/LICENSE` & `markdown_toc_creator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.3/PKG-INFO` & `markdown_toc_creator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_toc_creator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create table of contents for markdown files
 Home-page: https://github.com/jsh9/markdown-toc-creator
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `markdown_toc_creator-0.0.3/README.md` & `markdown_toc_creator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.3/markdown_toc_creator/create_toc.py` & `markdown_toc_creator-0.0.4/markdown_toc_creator/create_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.3/markdown_toc_creator/main.py` & `markdown_toc_creator-0.0.4/markdown_toc_creator/main.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.3/markdown_toc_creator/toc_entry.py` & `markdown_toc_creator-0.0.4/markdown_toc_creator/toc_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,21 @@
         soup = BeautifulSoup(text, 'html.parser')
         text = soup.get_text()
 
         if self.style == 'gitlab':
             # remove emojis represented as :emoji_name:
             text = re.sub(r':[\w\d_]+:', '', text)
 
-        # convert to lower case, replace spaces with hyphens, remove special characters
-        anchorLink = re.sub(r'[^\w\s-]+', '', text.lower().replace(' ', '-'))
+        # convert to lower case, replace spaces with hyphens,
+        # remove special characters and underscores
+        anchorLink = re.sub(
+            r'[^\w\s-]+',
+            '',
+            text.lower().replace(' ', '-').replace('_', ''),
+        )
 
         if self.style == 'gitlab':
             anchorLink = re.sub(r'-+', '-', anchorLink)
 
         # check last character
         anchorLink = anchorLink[:-1] if anchorLink[-1] == '-' else anchorLink
```

### Comparing `markdown_toc_creator-0.0.3/markdown_toc_creator.egg-info/PKG-INFO` & `markdown_toc_creator-0.0.4/markdown_toc_creator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-toc-creator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create table of contents for markdown files
 Home-page: https://github.com/jsh9/markdown-toc-creator
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `markdown_toc_creator-0.0.3/setup.cfg` & `markdown_toc_creator-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = markdown_toc_creator
-version = 0.0.3
+version = 0.0.4
 description = Create table of contents for markdown files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/markdown-toc-creator
 license = MIT
 license_file = LICENSE
 classifiers =
```

