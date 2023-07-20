# Comparing `tmp/hyfi_template-0.4.7.tar.gz` & `tmp/hyfi_template-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.4.7.tar", max compression
+gzip compressed data, was "hyfi_template-0.4.8.tar", max compression
```

## Comparing `hyfi_template-0.4.7.tar` & `hyfi_template-0.4.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-18 09:11:25.541863 hyfi_template-0.4.7/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-18 09:11:25.541863 hyfi_template-0.4.7/README.md
--rw-r--r--   0        0        0     3013 2023-07-18 09:12:04.078076 hyfi_template-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      286 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/__cli__.py
--rw-r--r--   0        0        0      438 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/__init__.py
--rw-r--r--   0        0        0       22 2023-07-18 09:12:04.006076 hyfi_template-0.4.7/src/hyfit/_version.py
--rw-r--r--   0        0        0        0 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/__init__.py
--rw-r--r--   0        0        0      249 2023-07-18 09:12:04.006076 hyfi_template-0.4.7/src/hyfit/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/about.yaml
--rw-r--r--   0        0        0      159 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/task/__init__.yaml
--rw-r--r--   0        0        0      124 2023-07-18 09:11:25.549863 hyfi_template-0.4.7/src/hyfit/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-18 09:11:25.549863 hyfi_template-0.4.7/src/hyfit/py.typed
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 hyfi_template-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 18:40:37.515248 hyfi_template-0.4.8/LICENSE
+-rw-r--r--   0        0        0     2215 2023-07-20 18:40:37.515248 hyfi_template-0.4.8/README.md
+-rw-r--r--   0        0        0     3012 2023-07-20 18:41:08.340112 hyfi_template-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-20 18:40:37.515248 hyfi_template-0.4.8/src/hyfit/__cli__.py
+-rw-r--r--   0        0        0      438 2023-07-20 18:40:37.515248 hyfi_template-0.4.8/src/hyfit/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-20 18:41:08.276104 hyfi_template-0.4.8/src/hyfit/_version.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:40:37.515248 hyfi_template-0.4.8/src/hyfit/conf/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-20 18:41:08.280104 hyfi_template-0.4.8/src/hyfit/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      159 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      213 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      124 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-20 18:40:37.519248 hyfi_template-0.4.8/src/hyfit/py.typed
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.4.8/PKG-INFO
```

### Comparing `hyfi_template-0.4.7/LICENSE` & `hyfi_template-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/README.md` & `hyfi_template-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/pyproject.toml` & `hyfi_template-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.4.7"
+version = "0.4.8"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfit", from = "src" }]
 
 [tool.poetry.scripts]
 hyfit = 'hyfit.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.14"
+hyfi = "^1.3.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/batch/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/copier/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/dotenv/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/hydra/help/help.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/mode/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/path/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/src/hyfit/conf/project/__init__.yaml` & `hyfi_template-0.4.8/src/hyfit/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.7/PKG-INFO` & `hyfi_template-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.4.7
+Version: 0.4.8
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.2.14,<2.0.0)
+Requires-Dist: hyfi (>=1.3.1,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

