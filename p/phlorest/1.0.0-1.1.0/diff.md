# Comparing `tmp/phlorest-1.0.0.tar.gz` & `tmp/phlorest-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlorest-1.0.0.tar", last modified: Tue Jul 18 13:00:07 2023, max compression
+gzip compressed data, was "phlorest-1.1.0.tar", last modified: Thu Jul 20 09:56:17 2023, max compression
```

## Comparing `phlorest-1.0.0.tar` & `phlorest-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 10:52:09.000000 phlorest-1.0.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-23 10:52:09.000000 phlorest-1.0.0/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-18 13:00:07.177544 phlorest-1.0.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1934 2023-07-17 08:36:51.000000 phlorest-1.0.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-23 10:52:09.000000 phlorest-1.0.0/pyproject.toml
--rw-rw-r--   0 robert    (1000) robert    (1000)     2242 2023-07-18 13:00:07.177544 phlorest-1.0.0/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-23 10:52:08.000000 phlorest-1.0.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/
--rw-rw-r--   0 robert    (1000) robert    (1000)      293 2023-07-18 12:59:16.000000 phlorest-1.0.0/src/phlorest/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3945 2022-12-23 10:52:07.000000 phlorest-1.0.0/src/phlorest/__main__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3307 2023-07-12 10:55:15.000000 phlorest-1.0.0/src/phlorest/beast.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    10020 2023-07-17 10:08:16.000000 phlorest-1.0.0/src/phlorest/cldfwriter.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/commands/
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2429 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/check.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1734 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/merge_characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8676 2023-07-18 11:31:01.000000 phlorest-1.0.0/src/phlorest/dataset.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2192 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/metadata.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3700 2023-07-17 11:04:32.000000 phlorest-1.0.0/src/phlorest/nexuslib.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/.github/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/
--rw-rw-r--   0 robert    (1000) robert    (1000)      629 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
--rw-rw-r--   0 robert    (1000) robert    (1000)      796 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/etc/
--rw-rw-r--   0 robert    (1000) robert    (1000)       10 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/etc/characters.csv
--rw-rw-r--   0 robert    (1000) robert    (1000)       16 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/etc/taxa.csv
--rw-rw-r--   0 robert    (1000) robert    (1000)       89 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)      605 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/setup.py_tmpl
--rw-rw-r--   0 robert    (1000) robert    (1000)      258 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/scaffold.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1078 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)      171 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/entry_points.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 10:52:07.000000 phlorest-1.0.0/src/phlorest.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      245 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        9 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/top_level.txt
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/tests/
--rw-rw-r--   0 robert    (1000) robert    (1000)      663 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_beast.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2232 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_cldfwriter.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      681 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_cli.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3484 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_dataset.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      409 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_metadata.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      814 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_nexuslib.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      261 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_scaffold.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 10:52:09.000000 phlorest-1.1.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-23 10:52:09.000000 phlorest-1.1.0/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-20 09:56:17.119885 phlorest-1.1.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1934 2023-07-17 08:36:51.000000 phlorest-1.1.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-23 10:52:09.000000 phlorest-1.1.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2242 2023-07-20 09:56:17.119885 phlorest-1.1.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-23 10:52:08.000000 phlorest-1.1.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      293 2023-07-20 09:55:39.000000 phlorest-1.1.0/src/phlorest/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3945 2022-12-23 10:52:07.000000 phlorest-1.1.0/src/phlorest/__main__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3307 2023-07-12 10:55:15.000000 phlorest-1.1.0/src/phlorest/beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11035 2023-07-20 06:21:20.000000 phlorest-1.1.0/src/phlorest/cldfwriter.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2429 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/check.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1734 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/merge_characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8676 2023-07-18 11:31:01.000000 phlorest-1.1.0/src/phlorest/dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2192 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3700 2023-07-17 11:04:32.000000 phlorest-1.1.0/src/phlorest/nexuslib.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/.github/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      632 2023-07-18 13:29:33.000000 phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
+-rw-rw-r--   0 robert    (1000) robert    (1000)      796 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/etc/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       10 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/etc/characters.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       16 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/etc/taxa.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       89 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      605 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/setup.py_tmpl
+-rw-rw-r--   0 robert    (1000) robert    (1000)      258 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/scaffold.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1078 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)      171 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 10:52:07.000000 phlorest-1.1.0/src/phlorest.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      245 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        9 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      663 2023-07-12 10:55:15.000000 phlorest-1.1.0/tests/test_beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2730 2023-07-20 06:32:03.000000 phlorest-1.1.0/tests/test_cldfwriter.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      681 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_cli.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3552 2023-07-20 06:25:32.000000 phlorest-1.1.0/tests/test_dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      409 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      917 2023-07-20 06:22:43.000000 phlorest-1.1.0/tests/test_nexuslib.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      261 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_scaffold.py
```

### Comparing `phlorest-1.0.0/LICENSE` & `phlorest-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/PKG-INFO` & `phlorest-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 1.0.0
+Version: 1.1.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
 Keywords: cldf
```

### Comparing `phlorest-1.0.0/README.md` & `phlorest-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/setup.cfg` & `phlorest-1.1.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phlorest
-version = 1.0.0
+version = 1.1.0
 author = Simon Greenhill and Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 description = A cldfbench plugin to curate language phylogenies
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cldf
 license = Apache 2.0
@@ -29,15 +29,15 @@
 zip_safe = False
 packages = find:
 package_dir = 
 	= src
 python_requires = >=3.8
 install_requires = 
 	newick>=1.9
-	commonnexus>=1.4
+	commonnexus>=1.5
 	cldfviz>=0.10
 	pycldf>=1.33.0
 	clldutils
 	cldfbench>=1.10.0
 	cldfcatalog
 	attrs
 	pyglottolog>=3.9.0
```

### Comparing `phlorest-1.0.0/src/phlorest/__main__.py` & `phlorest-1.1.0/src/phlorest/__main__.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/beast.py` & `phlorest-1.1.0/src/phlorest/beast.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/cldfwriter.py` & `phlorest-1.1.0/src/phlorest/cldfwriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,35 @@
         self.posterior = NexusFile(self.cldf_spec.dir / 'posterior.trees', zipped=True)
         self.posterior.__enter__()
         res = cldfbench.CLDFWriter.__enter__(self)
         self.add_schema()
         return res
 
     def __exit__(self, *args):
+        if self.dataset:
+            if self.dataset.metadata.cldf:
+                self.cldf.add_provenance(
+                    wasDerivedFrom={
+                        "rdf:about": self.dataset.metadata.cldf,
+                        "rdf:type": "prov:Entity",
+                        'dc:description': 'The CLDF dataset from which the data underlying the '
+                                          'analysis was derived',
+                        'dc:format': 'https://cldf.clld.org',
+                    }
+                )
+            if self.dataset.metadata.data and self.dataset.metadata.data.startswith('http'):
+                self.cldf.add_provenance(
+                    wasDerivedFrom={
+                        "rdf:about": self.dataset.metadata.data,
+                        "rdf:type": "prov:Entity",
+                        'dc:description': 'The dataset from which the data underlying the '
+                                          'analysis was derived',
+                    }
+                )
+
         self.summary.__exit__(*args)
         self.posterior.__exit__(*args)
         return cldfbench.CLDFWriter.__exit__(self, *args)
 
     def add_schema(self):
         t = self.cldf.add_component('LanguageTable')
         t.common_props['dc:description'] = \
```

### Comparing `phlorest-1.0.0/src/phlorest/commands/check.py` & `phlorest-1.1.0/src/phlorest/commands/check.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/commands/merge_characters.py` & `phlorest-1.1.0/src/phlorest/commands/merge_characters.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/dataset.py` & `phlorest-1.1.0/src/phlorest/dataset.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/metadata.py` & `phlorest-1.1.0/src/phlorest/metadata.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/nexuslib.py` & `phlorest-1.1.0/src/phlorest/nexuslib.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml` & `phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml`

 * *Files 25% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6]
+        python-version: ["3.10"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pytest-cldf
     - name: Test with pytest
```

### Comparing `phlorest-1.0.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl` & `phlorest-1.1.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest/phlorest_template/setup.py_tmpl` & `phlorest-1.1.0/src/phlorest/phlorest_template/setup.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/src/phlorest.egg-info/PKG-INFO` & `phlorest-1.1.0/src/phlorest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 1.0.0
+Version: 1.1.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
 Keywords: cldf
```

### Comparing `phlorest-1.0.0/src/phlorest.egg-info/SOURCES.txt` & `phlorest-1.1.0/src/phlorest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/tests/test_beast.py` & `phlorest-1.1.0/tests/test_beast.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/tests/test_cldfwriter.py` & `phlorest-1.1.0/tests/test_cldfwriter.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,34 @@
     with CLDFWriter(cldf_spec=cldfbench.CLDFSpec(dir=tmp_path)) as writer:
         writer.add_taxa(dataset.taxa, glottolog, mocker.Mock())
         writer.add_data(
             (repos / 'raw' / 'data.nex').read_text(encoding='utf8'),
             [{'Site': '0', 'Gloss': 'abc'}], mocker.Mock())
         assert writer.cldf['ParameterTable', 'Gloss']
 
+    with CLDFWriter(cldf_spec=cldfbench.CLDFSpec(dir=tmp_path)) as writer:
+        writer.add_taxa(dataset.taxa, glottolog, mocker.Mock())
+        writer.add_data(
+            """\
+#NEXUS
+
+BEGIN DATA;
+	dimensions ntax=3 nchar=1;
+	format datatype=STANDARD gap=- missing=? symbols="ABC";
+	MATRIX
+	Jeju A
+	SouthJeolla B
+	NorthJeolla C
+	;
+END;""",
+            [{'Site': '0', 'Gloss': 'abc'}],
+            mocker.Mock(),
+            binarise=True)
+        assert writer.cldf['ParameterTable', 'Gloss']
+
 
 def test_CLDFWriter_nexus_data_3(repos, tmp_path, mocker, nexus_tree, dataset, glottolog):
     from commonnexus import Nexus
 
     with CLDFWriter(cldf_spec=cldfbench.CLDFSpec(dir=tmp_path)) as writer:
         writer.add_taxa(dataset.taxa, glottolog, mocker.Mock())
         writer.add_data(
```

### Comparing `phlorest-1.0.0/tests/test_cli.py` & `phlorest-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.0.0/tests/test_dataset.py` & `phlorest-1.1.0/tests/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 
 def test_PhlorestDir(repos):
     d = PhlorestDir(repos / 'raw')
     nex = d.read_nexus('nexus.trees', preprocessor=lambda s: s.replace('Cojubim', 'abcdefg'))
     assert 'abcdefg' in str(nex)
 
+    nex = d.read_nexus('nexus.trees.gz')
+    assert nex.TREES.TREE
+
 
 def test_PhlorestDir_with_rates(repos):
     d = PhlorestDir(repos / 'raw')
     nex = d.read_nexus('trees_with_rate.trees')
     for node in nex.TREES.TREE.newick.walk():
         if node.name == '1':
             assert ('height' in node.properties) and ('rate' in node.properties)
```

### Comparing `phlorest-1.0.0/tests/test_nexuslib.py` & `phlorest-1.1.0/tests/test_nexuslib.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,7 +20,12 @@
 def test_NexusFile(tmp_path, mocker):
     with NexusFile(tmp_path / 'test.nex') as nex:
         nex.append(Tree('n', '(A:1,B:2)root:3;', None), 'a', {'A', 'B'}, 'years', mocker.Mock())
         with pytest.raises(ValueError):
             nex.append(Tree('n', '(A:1,B:2)root:3;', None), 'c', {'A', 'B'}, 'change', mocker.Mock())
     res = Nexus.from_file(tmp_path / 'test.nex')
     assert len(res.TREES.trees) == 1
+
+
+def test_Tree():
+    t = Tree('n', '(A:1,B:2)root:3;', None)
+    assert str(t) == '(A:1,B:2)root:3;'
```

