# Comparing `tmp/mkdocs-swangallery-0.0.5.tar.gz` & `tmp/mkdocs-swangallery-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-swangallery-0.0.5.tar", last modified: Mon Nov 21 19:02:56 2022, max compression
+gzip compressed data, was "mkdocs-swangallery-0.0.6.tar", last modified: Thu Jul 20 13:43:11 2023, max compression
```

## Comparing `mkdocs-swangallery-0.0.5.tar` & `mkdocs-swangallery-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 19:02:56.570666 mkdocs-swangallery-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-21 19:02:56.570666 mkdocs-swangallery-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 19:02:56.566666 mkdocs-swangallery-0.0.5/mkdocs_swangallery/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7865 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery/swangallery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 19:02:56.566666 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-21 19:02:56.000000 mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 19:02:56.570666 mkdocs-swangallery-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-11-21 19:02:52.000000 mkdocs-swangallery-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:43:11.582033 mkdocs-swangallery-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-20 13:43:11.582033 mkdocs-swangallery-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:43:11.582033 mkdocs-swangallery-0.0.6/mkdocs_swangallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery/swangallery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:43:11.582033 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 13:43:11.000000 mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:43:11.582033 mkdocs-swangallery-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-20 13:43:08.000000 mkdocs-swangallery-0.0.6/setup.py
```

### Comparing `mkdocs-swangallery-0.0.5/LICENSE` & `mkdocs-swangallery-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-swangallery-0.0.5/PKG-INFO` & `mkdocs-swangallery-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swangallery
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plugin for MkDocs to genereate a SWAN Gallery
 Home-page: https://github.com/swan-cern/mkdocs-swangallery
 Author: Diogo Castro
 Author-email: diogo.castro@cern.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `mkdocs-swangallery-0.0.5/mkdocs_swangallery/swangallery.py` & `mkdocs-swangallery-0.0.6/mkdocs_swangallery/swangallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,21 +160,20 @@
 
         os.makedirs(destinationFolder, exist_ok=True)
 
         with open(originalFile) as nb:
             raw_content = nb.read()
             notebook_content = nbformat.reads(raw_content, as_version=4)
 
-            html_exporter = HTMLExporter()
-            html_exporter.template_file = 'basic'
+            html_exporter = HTMLExporter(template_name='basic')
 
             (body, resources) = html_exporter.from_notebook_node(notebook_content)
 
             full_content = "<style>\n"
-            for style in resources['inlining']['css'][1:]:
+            for style in resources['inlining']['css']:
                 full_content += style
             full_content += "</style>\n"
             full_content += body
 
             # Add a special marker in this tag to be able to identify in the next stage
             full_content += "<div id='rendered_gallery_notebook'></div>"
 
@@ -184,14 +183,15 @@
                 if isZip:
                     path = path.replace('.ipynb', '.zip')
 
                 output.write("---\n")
                 output.write("template: notebook.html\n")
                 output.write("notebook_name: %s\n" % notebook)
                 output.write("notebook_url: %s\n" % path)
+                output.write("hide:\n  - navigation\n  - toc\n")
                 output.write("---\n")
                 output.write(full_content)
 
         return destinationFile
 
     def _zip_folder(self, folder, destination):
         zipf = zipfile.ZipFile(destination, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `mkdocs-swangallery-0.0.5/mkdocs_swangallery.egg-info/PKG-INFO` & `mkdocs-swangallery-0.0.6/mkdocs_swangallery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swangallery
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plugin for MkDocs to genereate a SWAN Gallery
 Home-page: https://github.com/swan-cern/mkdocs-swangallery
 Author: Diogo Castro
 Author-email: diogo.castro@cern.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `mkdocs-swangallery-0.0.5/setup.py` & `mkdocs-swangallery-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load README contents
 with open("README.md", encoding = "utf-8") as data:
     long_description = data.read()
 
 setup(
     name="mkdocs-swangallery",
-    version='0.0.5',
+    version='0.0.6',
     url='https://github.com/swan-cern/mkdocs-swangallery',
     license='BSD',
     description='Plugin for MkDocs to genereate a SWAN Gallery',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author='Diogo Castro',
     author_email='diogo.castro@cern.ch',
@@ -23,17 +23,15 @@
         "Topic :: Software Development :: Documentation",
         "Topic :: Text Processing :: Markup :: HTML"
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'mkdocs',
-        'nbconvert==5.*',
-        'jinja2==2.*',
-        'markupsafe==1.*',
+        'nbconvert>=7',
         'ipython_genutils',
         'nbformat',
         'bs4'
         ],
     entry_points={
         'mkdocs.plugins': [
             'swangallery = mkdocs_swangallery:SwanGallery',
```

