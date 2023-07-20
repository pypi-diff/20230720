# Comparing `tmp/types-PyYAML-6.0.8.tar.gz` & `tmp/types-PyYAML-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyYAML-6.0.8.tar", last modified: Wed Jun  1 18:25:30 2022, max compression
+gzip compressed data, was "types-PyYAML-6.0.9.tar", last modified: Sat Jun 25 18:22:10 2022, max compression
```

## Comparing `types-PyYAML-6.0.8.tar` & `types-PyYAML-6.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 18:25:30.810219 types-PyYAML-6.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-06-01 18:25:29.000000 types-PyYAML-6.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-01 18:25:29.000000 types-PyYAML-6.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-06-01 18:25:30.810219 types-PyYAML-6.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 18:25:30.810219 types-PyYAML-6.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-06-01 18:25:29.000000 types-PyYAML-6.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 18:25:30.806219 types-PyYAML-6.0.8/types_PyYAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-06-01 18:25:30.000000 types-PyYAML-6.0.8/types_PyYAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-01 18:25:30.000000 types-PyYAML-6.0.8/types_PyYAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 18:25:30.000000 types-PyYAML-6.0.8/types_PyYAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-01 18:25:30.000000 types-PyYAML-6.0.8/types_PyYAML.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 18:25:30.810219 types-PyYAML-6.0.8/yaml-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-01 18:25:29.000000 types-PyYAML-6.0.8/yaml-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/_yaml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/composer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/constructor.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/cyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/dumper.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/emitter.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/error.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/representer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/scanner.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-06-01 18:25:19.000000 types-PyYAML-6.0.8/yaml-stubs/tokens.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 18:22:10.604620 types-PyYAML-6.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-06-25 18:22:09.000000 types-PyYAML-6.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-25 18:22:09.000000 types-PyYAML-6.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-06-25 18:22:10.600619 types-PyYAML-6.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-25 18:22:10.604620 types-PyYAML-6.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-06-25 18:22:09.000000 types-PyYAML-6.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 18:22:10.600619 types-PyYAML-6.0.9/types_PyYAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-06-25 18:22:10.000000 types-PyYAML-6.0.9/types_PyYAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-25 18:22:10.000000 types-PyYAML-6.0.9/types_PyYAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 18:22:10.000000 types-PyYAML-6.0.9/types_PyYAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-25 18:22:10.000000 types-PyYAML-6.0.9/types_PyYAML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 18:22:10.600619 types-PyYAML-6.0.9/yaml-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-25 18:22:09.000000 types-PyYAML-6.0.9/yaml-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/_yaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/composer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/constructor.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/cyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/dumper.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/emitter.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/representer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      786 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/scanner.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-06-25 18:22:01.000000 types-PyYAML-6.0.9/yaml-stubs/tokens.pyi
```

### Comparing `types-PyYAML-6.0.8/CHANGELOG.md` & `types-PyYAML-6.0.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 6.0.9 (2022-06-25)
+
+PyYAML: check missing defs (#8159)
+
 ## 6.0.8 (2022-06-01)
 
 PyYAML: Add types to `add_constructor` (#7989)
 
 ## 6.0.7 (2022-04-20)
 
 Use `TypeAlias` for type aliases where possible, part II (#7667)
```

### Comparing `types-PyYAML-6.0.8/PKG-INFO` & `types-PyYAML-6.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyYAML
-Version: 6.0.8
+Version: 6.0.9
 Summary: Typing stubs for PyYAML
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyYAML.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `PyYAML` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyYAML`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyYAML. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `461289e18174d765d18382c821053f3e14b8b978`.
+This package was generated from typeshed commit `f5f37fed3a5eeb5b65bc77e401dcd31bd4284722`.
```

### Comparing `types-PyYAML-6.0.8/setup.py` & `types-PyYAML-6.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `PyYAML` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyYAML`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyYAML. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `461289e18174d765d18382c821053f3e14b8b978`.
+This package was generated from typeshed commit `f5f37fed3a5eeb5b65bc77e401dcd31bd4284722`.
 '''.lstrip()
 
 setup(name=name,
-      version="6.0.8",
+      version="6.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyYAML.md",
```

### Comparing `types-PyYAML-6.0.8/types_PyYAML.egg-info/PKG-INFO` & `types-PyYAML-6.0.9/types_PyYAML.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyYAML
-Version: 6.0.8
+Version: 6.0.9
 Summary: Typing stubs for PyYAML
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyYAML.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `PyYAML` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyYAML`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyYAML. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `461289e18174d765d18382c821053f3e14b8b978`.
+This package was generated from typeshed commit `f5f37fed3a5eeb5b65bc77e401dcd31bd4284722`.
```

### Comparing `types-PyYAML-6.0.8/types_PyYAML.egg-info/SOURCES.txt` & `types-PyYAML-6.0.9/types_PyYAML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/__init__.pyi` & `types-PyYAML-6.0.9/yaml-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/_yaml.pyi` & `types-PyYAML-6.0.9/yaml-stubs/_yaml.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/composer.pyi` & `types-PyYAML-6.0.9/yaml-stubs/composer.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/constructor.pyi` & `types-PyYAML-6.0.9/yaml-stubs/constructor.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/cyaml.pyi` & `types-PyYAML-6.0.9/yaml-stubs/cyaml.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/dumper.pyi` & `types-PyYAML-6.0.9/yaml-stubs/dumper.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/emitter.pyi` & `types-PyYAML-6.0.9/yaml-stubs/emitter.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/error.pyi` & `types-PyYAML-6.0.9/yaml-stubs/error.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/events.pyi` & `types-PyYAML-6.0.9/yaml-stubs/events.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/loader.pyi` & `types-PyYAML-6.0.9/yaml-stubs/loader.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/nodes.pyi` & `types-PyYAML-6.0.9/yaml-stubs/nodes.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/parser.pyi` & `types-PyYAML-6.0.9/yaml-stubs/parser.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/reader.pyi` & `types-PyYAML-6.0.9/yaml-stubs/reader.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/representer.pyi` & `types-PyYAML-6.0.9/yaml-stubs/representer.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/resolver.pyi` & `types-PyYAML-6.0.9/yaml-stubs/resolver.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/scanner.pyi` & `types-PyYAML-6.0.9/yaml-stubs/scanner.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/serializer.pyi` & `types-PyYAML-6.0.9/yaml-stubs/serializer.pyi`

 * *Files identical despite different names*

### Comparing `types-PyYAML-6.0.8/yaml-stubs/tokens.pyi` & `types-PyYAML-6.0.9/yaml-stubs/tokens.pyi`

 * *Files identical despite different names*

