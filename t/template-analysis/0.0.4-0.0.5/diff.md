# Comparing `tmp/template_analysis-0.0.4.tar.gz` & `tmp/template_analysis-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template_analysis-0.0.4.tar", last modified: Tue Mar 21 13:12:04 2023, max compression
+gzip compressed data, was "template_analysis-0.0.5.tar", last modified: Thu Jul 20 14:41:45 2023, max compression
```

## Comparing `template_analysis-0.0.4.tar` & `template_analysis-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.685753 template_analysis-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.681753 template_analysis-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.685753 template_analysis-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-03-21 13:11:39.000000 template_analysis-0.0.4/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-21 13:11:39.000000 template_analysis-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-21 13:12:04.685753 template_analysis-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-21 13:11:39.000000 template_analysis-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    33361 2023-03-21 13:11:39.000000 template_analysis-0.0.4/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-21 13:11:39.000000 template_analysis-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-21 13:11:39.000000 template_analysis-0.0.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-21 13:12:04.689753 template_analysis-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.685753 template_analysis-0.0.4/template_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-21 13:11:39.000000 template_analysis-0.0.4/template_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-21 13:12:04.000000 template_analysis-0.0.4/template_analysis/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-21 13:11:39.000000 template_analysis-0.0.4/template_analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-21 13:11:39.000000 template_analysis-0.0.4/template_analysis/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-21 13:11:39.000000 template_analysis-0.0.4/template_analysis/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.685753 template_analysis-0.0.4/template_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-21 13:12:04.000000 template_analysis-0.0.4/template_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-21 13:12:04.000000 template_analysis-0.0.4/template_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:12:04.000000 template_analysis-0.0.4/template_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-21 13:12:04.000000 template_analysis-0.0.4/template_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:12:04.685753 template_analysis-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:11:39.000000 template_analysis-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-21 13:11:39.000000 template_analysis-0.0.4/tests/test_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-21 13:11:39.000000 template_analysis-0.0.4/tests/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-21 13:11:39.000000 template_analysis-0.0.4/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-20 14:41:14.000000 template_analysis-0.0.5/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 14:41:14.000000 template_analysis-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 14:41:45.422818 template_analysis-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 14:41:14.000000 template_analysis-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    31937 2023-07-20 14:41:14.000000 template_analysis-0.0.5/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-20 14:41:14.000000 template_analysis-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-20 14:41:45.422818 template_analysis-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/template_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 14:41:14.000000 template_analysis-0.0.5/template_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:41:45.000000 template_analysis-0.0.5/template_analysis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 14:41:14.000000 template_analysis-0.0.5/template_analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 14:41:14.000000 template_analysis-0.0.5/template_analysis/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-20 14:41:14.000000 template_analysis-0.0.5/template_analysis/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/template_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 14:41:45.000000 template_analysis-0.0.5/template_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-20 14:41:45.000000 template_analysis-0.0.5/template_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:41:45.000000 template_analysis-0.0.5/template_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 14:41:45.000000 template_analysis-0.0.5/template_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:45.418818 template_analysis-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:41:14.000000 template_analysis-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-20 14:41:14.000000 template_analysis-0.0.5/tests/test_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-20 14:41:14.000000 template_analysis-0.0.5/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 14:41:14.000000 template_analysis-0.0.5/tests/test_template.py
```

### Comparing `template_analysis-0.0.4/.github/workflows/pypi-publish.yml` & `template_analysis-0.0.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/.github/workflows/python-test.yml` & `template_analysis-0.0.5/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/.gitignore` & `template_analysis-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/LICENSE` & `template_analysis-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/PKG-INFO` & `template_analysis-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template_analysis
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create template from strings (reverse formatter)
 Home-page: https://github.com/kitsuyui/python-template-analysis
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `template_analysis-0.0.4/README.md` & `template_analysis-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/poetry.lock` & `template_analysis-0.0.5/poetry.lock`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,39 @@
-# This file is automatically @generated by Poetry 1.4.1 and should not be changed by hand.
-
-[[package]]
-name = "attrs"
-version = "22.2.0"
-description = "Classes Without Boilerplate"
-category = "dev"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
-    {file = "attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
-]
-
-[package.extras]
-cov = ["attrs[tests]", "coverage-enable-subprocess", "coverage[toml] (>=5.3)"]
-dev = ["attrs[docs,tests]"]
-docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope.interface"]
-tests = ["attrs[tests-no-zope]", "zope.interface"]
-tests-no-zope = ["cloudpickle", "cloudpickle", "hypothesis", "hypothesis", "mypy (>=0.971,<0.990)", "mypy (>=0.971,<0.990)", "pympler", "pympler", "pytest (>=4.3.0)", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-mypy-plugins", "pytest-xdist[psutil]", "pytest-xdist[psutil]"]
+# This file is automatically @generated by Poetry 1.4.2 and should not be changed by hand.
 
 [[package]]
 name = "black"
-version = "23.1.0"
+version = "23.7.0"
 description = "The uncompromising code formatter."
 category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221"},
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26"},
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b"},
-    {file = "black-23.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"},
-    {file = "black-23.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958"},
-    {file = "black-23.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a"},
-    {file = "black-23.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481"},
-    {file = "black-23.1.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad"},
-    {file = "black-23.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8"},
-    {file = "black-23.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580"},
-    {file = "black-23.1.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468"},
-    {file = "black-23.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739"},
-    {file = "black-23.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9"},
-    {file = "black-23.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555"},
-    {file = "black-23.1.0-py3-none-any.whl", hash = "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32"},
-    {file = "black-23.1.0.tar.gz", hash = "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be"},
+    {file = "black-23.7.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc"},
+    {file = "black-23.7.0-cp310-cp310-win_amd64.whl", hash = "sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a"},
+    {file = "black-23.7.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926"},
+    {file = "black-23.7.0-cp311-cp311-win_amd64.whl", hash = "sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6"},
+    {file = "black-23.7.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a"},
+    {file = "black-23.7.0-cp38-cp38-win_amd64.whl", hash = "sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087"},
+    {file = "black-23.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91"},
+    {file = "black-23.7.0-cp39-cp39-win_amd64.whl", hash = "sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491"},
+    {file = "black-23.7.0-py3-none-any.whl", hash = "sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96"},
+    {file = "black-23.7.0.tar.gz", hash = "sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
 packaging = ">=22.0"
 pathspec = ">=0.9.0"
@@ -118,71 +96,71 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.2.2"
+version = "7.2.3"
 description = "Code coverage measurement for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "coverage-7.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7"},
-    {file = "coverage-7.2.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2"},
-    {file = "coverage-7.2.2-cp310-cp310-win32.whl", hash = "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292"},
-    {file = "coverage-7.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab"},
-    {file = "coverage-7.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b"},
-    {file = "coverage-7.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57"},
-    {file = "coverage-7.2.2-cp311-cp311-win32.whl", hash = "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d"},
-    {file = "coverage-7.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512"},
-    {file = "coverage-7.2.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9"},
-    {file = "coverage-7.2.2-cp37-cp37m-win32.whl", hash = "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8"},
-    {file = "coverage-7.2.2-cp37-cp37m-win_amd64.whl", hash = "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25"},
-    {file = "coverage-7.2.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6"},
-    {file = "coverage-7.2.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2"},
-    {file = "coverage-7.2.2-cp38-cp38-win32.whl", hash = "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3"},
-    {file = "coverage-7.2.2-cp38-cp38-win_amd64.whl", hash = "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8"},
-    {file = "coverage-7.2.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d"},
-    {file = "coverage-7.2.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be"},
-    {file = "coverage-7.2.2-cp39-cp39-win32.whl", hash = "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc"},
-    {file = "coverage-7.2.2-cp39-cp39-win_amd64.whl", hash = "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef"},
-    {file = "coverage-7.2.2-pp37.pp38.pp39-none-any.whl", hash = "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968"},
-    {file = "coverage-7.2.2.tar.gz", hash = "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2"},
+    {file = "coverage-7.2.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5"},
+    {file = "coverage-7.2.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535"},
+    {file = "coverage-7.2.3-cp310-cp310-win32.whl", hash = "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91"},
+    {file = "coverage-7.2.3-cp310-cp310-win_amd64.whl", hash = "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e"},
+    {file = "coverage-7.2.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79"},
+    {file = "coverage-7.2.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4"},
+    {file = "coverage-7.2.3-cp311-cp311-win32.whl", hash = "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925"},
+    {file = "coverage-7.2.3-cp311-cp311-win_amd64.whl", hash = "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910"},
+    {file = "coverage-7.2.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48"},
+    {file = "coverage-7.2.3-cp37-cp37m-win32.whl", hash = "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1"},
+    {file = "coverage-7.2.3-cp37-cp37m-win_amd64.whl", hash = "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f"},
+    {file = "coverage-7.2.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab"},
+    {file = "coverage-7.2.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152"},
+    {file = "coverage-7.2.3-cp38-cp38-win32.whl", hash = "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22"},
+    {file = "coverage-7.2.3-cp38-cp38-win_amd64.whl", hash = "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367"},
+    {file = "coverage-7.2.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235"},
+    {file = "coverage-7.2.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4"},
+    {file = "coverage-7.2.3-cp39-cp39-win32.whl", hash = "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30"},
+    {file = "coverage-7.2.3-cp39-cp39-win_amd64.whl", hash = "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a"},
+    {file = "coverage-7.2.3-pp37.pp38.pp39-none-any.whl", hash = "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0"},
+    {file = "coverage-7.2.3.tar.gz", hash = "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259"},
 ]
 
 [package.dependencies]
 tomli = {version = "*", optional = true, markers = "python_full_version <= \"3.11.0a6\" and extra == \"toml\""}
 
 [package.extras]
 toml = ["tomli"]
@@ -259,52 +237,52 @@
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "mypy"
-version = "1.1.1"
+version = "1.4.1"
 description = "Optional static typing for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "mypy-1.1.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af"},
-    {file = "mypy-1.1.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1"},
-    {file = "mypy-1.1.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799"},
-    {file = "mypy-1.1.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78"},
-    {file = "mypy-1.1.1-cp310-cp310-win_amd64.whl", hash = "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e"},
-    {file = "mypy-1.1.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389"},
-    {file = "mypy-1.1.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2"},
-    {file = "mypy-1.1.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5"},
-    {file = "mypy-1.1.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c"},
-    {file = "mypy-1.1.1-cp311-cp311-win_amd64.whl", hash = "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54"},
-    {file = "mypy-1.1.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5"},
-    {file = "mypy-1.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707"},
-    {file = "mypy-1.1.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5"},
-    {file = "mypy-1.1.1-cp37-cp37m-win_amd64.whl", hash = "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"},
-    {file = "mypy-1.1.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b"},
-    {file = "mypy-1.1.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51"},
-    {file = "mypy-1.1.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b"},
-    {file = "mypy-1.1.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9"},
-    {file = "mypy-1.1.1-cp38-cp38-win_amd64.whl", hash = "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a"},
-    {file = "mypy-1.1.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598"},
-    {file = "mypy-1.1.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c"},
-    {file = "mypy-1.1.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a"},
-    {file = "mypy-1.1.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f"},
-    {file = "mypy-1.1.1-cp39-cp39-win_amd64.whl", hash = "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f"},
-    {file = "mypy-1.1.1-py3-none-any.whl", hash = "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4"},
-    {file = "mypy-1.1.1.tar.gz", hash = "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f"},
+    {file = "mypy-1.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8"},
+    {file = "mypy-1.4.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878"},
+    {file = "mypy-1.4.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd"},
+    {file = "mypy-1.4.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc"},
+    {file = "mypy-1.4.1-cp310-cp310-win_amd64.whl", hash = "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258"},
+    {file = "mypy-1.4.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2"},
+    {file = "mypy-1.4.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7"},
+    {file = "mypy-1.4.1-cp311-cp311-win_amd64.whl", hash = "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01"},
+    {file = "mypy-1.4.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b"},
+    {file = "mypy-1.4.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"},
+    {file = "mypy-1.4.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7"},
+    {file = "mypy-1.4.1-cp37-cp37m-win_amd64.whl", hash = "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3"},
+    {file = "mypy-1.4.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6"},
+    {file = "mypy-1.4.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f"},
+    {file = "mypy-1.4.1-cp38-cp38-win_amd64.whl", hash = "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3"},
+    {file = "mypy-1.4.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816"},
+    {file = "mypy-1.4.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c"},
+    {file = "mypy-1.4.1-cp39-cp39-win_amd64.whl", hash = "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f"},
+    {file = "mypy-1.4.1-py3-none-any.whl", hash = "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4"},
+    {file = "mypy-1.4.1.tar.gz", hash = "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b"},
 ]
 
 [package.dependencies]
 mypy-extensions = ">=1.0.0"
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
-typing-extensions = ">=3.10"
+typing-extensions = ">=4.1.0"
 
 [package.extras]
 dmypy = ["psutil (>=4.0)"]
 install-types = ["pip"]
 python2 = ["typed-ast (>=1.4.0,<2)"]
 reports = ["lxml"]
 
@@ -354,27 +332,27 @@
 files = [
     {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
     {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.1.1"
+version = "3.2.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.1.1-py3-none-any.whl", hash = "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"},
-    {file = "platformdirs-3.1.1.tar.gz", hash = "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa"},
+    {file = "platformdirs-3.2.0-py3-none-any.whl", hash = "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"},
+    {file = "platformdirs-3.2.0.tar.gz", hash = "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08"},
 ]
 
 [package.extras]
 docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 description = "plugin and hook calling mechanisms for python"
 category = "dev"
 optional = false
@@ -386,22 +364,22 @@
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "poethepoet"
-version = "0.18.1"
+version = "0.21.1"
 description = "A task runner that works well with poetry."
 category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "poethepoet-0.18.1-py3-none-any.whl", hash = "sha256:e85727bf6f4a10bf6c1a43026bdeb40df689bea3c4682d03cbe531cabc8f2ba6"},
-    {file = "poethepoet-0.18.1.tar.gz", hash = "sha256:5f3566b14c2f5dccdfbc3bb26f0096006b38dc0b9c74bd4f8dd1eba7b0e29f6a"},
+    {file = "poethepoet-0.21.1-py3-none-any.whl", hash = "sha256:c79b2aefc889c4490db9d64ecc1896db78700aa212b8c5f0bca4aee0395e7714"},
+    {file = "poethepoet-0.21.1.tar.gz", hash = "sha256:39d754f53714545a23cfc94b122deaf3548218b6e35b453c30973c5598719e9f"},
 ]
 
 [package.dependencies]
 pastel = ">=0.2.1,<0.3.0"
 tomli = ">=1.2.2"
 
 [package.extras]
@@ -444,80 +422,79 @@
 ]
 
 [package.dependencies]
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 
 [[package]]
 name = "pytest"
-version = "7.2.2"
+version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.2.2-py3-none-any.whl", hash = "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e"},
-    {file = "pytest-7.2.2.tar.gz", hash = "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"},
+    {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [package.dependencies]
-attrs = ">=19.2.0"
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 iniconfig = "*"
 packaging = "*"
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "pytest-cov"
-version = "4.0.0"
+version = "4.1.0"
 description = "Pytest plugin for measuring coverage."
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "pytest-cov-4.0.0.tar.gz", hash = "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"},
-    {file = "pytest_cov-4.0.0-py3-none-any.whl", hash = "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b"},
+    {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
+    {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
 ]
 
 [package.dependencies]
 coverage = {version = ">=5.2.1", extras = ["toml"]}
 pytest = ">=4.6"
 
 [package.extras]
 testing = ["fields", "hunter", "process-tests", "pytest-xdist", "six", "virtualenv"]
 
 [[package]]
 name = "pyupgrade"
-version = "3.3.1"
+version = "3.9.0"
 description = "A tool to automatically upgrade syntax for newer versions."
 category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8.1"
 files = [
-    {file = "pyupgrade-3.3.1-py2.py3-none-any.whl", hash = "sha256:3b93641963df022d605c78aeae4b5956a5296ea24701eafaef9c487527b77e60"},
-    {file = "pyupgrade-3.3.1.tar.gz", hash = "sha256:f88bce38b0ba92c2a9a5063c8629e456e8d919b67d2d42c7ecab82ff196f9813"},
+    {file = "pyupgrade-3.9.0-py2.py3-none-any.whl", hash = "sha256:1807e324a1432f05a830bc1847095c90b604c91de66237fff55cb98b99d4da10"},
+    {file = "pyupgrade-3.9.0.tar.gz", hash = "sha256:a4c7132f4614f7acbacb756275c8a7881ad418f8a1c6ff6512c30dcf4c98f500"},
 ]
 
 [package.dependencies]
 tokenize-rt = ">=3.2.0"
 
 [[package]]
 name = "setuptools"
-version = "67.6.0"
+version = "67.6.1"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "setuptools-67.6.0-py3-none-any.whl", hash = "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"},
-    {file = "setuptools-67.6.0.tar.gz", hash = "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077"},
+    {file = "setuptools-67.6.1-py3-none-any.whl", hash = "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"},
+    {file = "setuptools-67.6.1.tar.gz", hash = "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
 testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
```

### Comparing `template_analysis-0.0.4/pyproject.toml` & `template_analysis-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/setup.cfg` & `template_analysis-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/template_analysis/analyzer.py` & `template_analysis-0.0.5/template_analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/template_analysis/symbol.py` & `template_analysis-0.0.5/template_analysis/symbol.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 Character = str
 Chunk = str
 
 
 @dataclass(frozen=True)
 class Symbol:
+    """A symbol in a template."""
+
     value: object
 
     @classmethod
     def create(cls) -> Symbol:
         return cls(object())
 
 
 @dataclass
 class SymbolTable:
+    """A table of symbols."""
+
     table: dict[Symbol, SymbolChunk]
 
     @classmethod
     def create(cls) -> SymbolTable:
         return cls({})
 
     def add(self, symbol: Symbol, chunk: SymbolChunk) -> None:
```

### Comparing `template_analysis-0.0.4/template_analysis/template.py` & `template_analysis-0.0.5/template_analysis/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,44 @@
 from typing import Union
 
 from .symbol import Symbol, SymbolTemplate
 
 
 @dataclass(frozen=True)
 class Variable:
+    """A extracted variable in a template."""
+
     id: int
 
     def to_format_string(self) -> str:
         return "{}"
 
 
 @dataclass(frozen=True)
 class PlainText:
+    """A plain text chunk in a template."""
+
     value: str
 
     def to_format_string(self) -> str:
         return self.value
 
 
+# A part of a template is either a plain text chunk or a variable.
 TemplatePart = Union[PlainText, Variable]
 
 
 @dataclass(frozen=True)
 class Template:
+    """A template extracted from a formatted string.
+
+    A template is a list of parts,
+    where each part is either a plain text chunk or a variable.
+    """
+
     parts: list[TemplatePart]
 
     @classmethod
     def from_symbol_template(cls, st: SymbolTemplate) -> Template:
         parts: list[TemplatePart] = []
         variables = 0
         for chunk in st.text:
```

### Comparing `template_analysis-0.0.4/template_analysis.egg-info/PKG-INFO` & `template_analysis-0.0.5/template_analysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-analysis
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create template from strings (reverse formatter)
 Home-page: https://github.com/kitsuyui/python-template-analysis
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `template_analysis-0.0.4/template_analysis.egg-info/SOURCES.txt` & `template_analysis-0.0.5/template_analysis.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 .editorconfig
 .gitignore
 .gitignore.in
 LICENSE
 README.md
 poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
+.github/renovate.json5
 .github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 template_analysis/__init__.py
 template_analysis/_version.py
 template_analysis/analyzer.py
 template_analysis/symbol.py
 template_analysis/template.py
 template_analysis.egg-info/PKG-INFO
 template_analysis.egg-info/SOURCES.txt
```

### Comparing `template_analysis-0.0.4/tests/test_analyzer.py` & `template_analysis-0.0.5/tests/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `template_analysis-0.0.4/tests/test_symbol.py` & `template_analysis-0.0.5/tests/test_symbol.py`

 * *Files identical despite different names*

