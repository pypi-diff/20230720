# Comparing `tmp/thermoblock-23.7.0.dev0.tar.gz` & `tmp/thermoblock-23.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoblock-23.7.0.dev0.tar", last modified: Thu Jul 20 10:33:53 2023, max compression
+gzip compressed data, was "thermoblock-23.7.0.dev1.tar", last modified: Thu Jul 20 13:50:23 2023, max compression
```

## Comparing `thermoblock-23.7.0.dev0.tar` & `thermoblock-23.7.0.dev1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     5672 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.482183 thermoblock-23.7.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.486184 thermoblock-23.7.0.dev0/src/thermoblock/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/src/thermoblock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/src/thermoblock/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    39823 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/src/thermoblock/resources/colorspectrum.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    28100 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/src/thermoblock/resources/colorspectrum.pck
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/src/thermoblock/resources/materiallist.pck
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/src/thermoblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 10:33:53.000000 thermoblock-23.7.0.dev0/src/thermoblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-20 10:33:53.000000 thermoblock-23.7.0.dev0/src/thermoblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:33:53.000000 thermoblock-23.7.0.dev0/src/thermoblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-20 10:33:53.000000 thermoblock-23.7.0.dev0/src/thermoblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:33:53.490183 thermoblock-23.7.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-20 10:33:32.000000 thermoblock-23.7.0.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.212284 thermoblock-23.7.0.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5672 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.208284 thermoblock-23.7.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.216284 thermoblock-23.7.0.dev1/src/thermoblock/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/src/thermoblock/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    39823 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    28100 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.pck
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/src/thermoblock/resources/materiallist.pck
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5901 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-20 13:50:23.000000 thermoblock-23.7.0.dev1/src/thermoblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:50:23.220284 thermoblock-23.7.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-20 13:50:08.000000 thermoblock-23.7.0.dev1/tox.ini
```

### Comparing `thermoblock-23.7.0.dev0/.github/workflows/ci.yml` & `thermoblock-23.7.0.dev1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/.github/workflows/docs.yml` & `thermoblock-23.7.0.dev1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/.github/workflows/release.yml` & `thermoblock-23.7.0.dev1/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     steps:
       - uses: actions/download-artifact@v3
       - uses: conda-incubator/setup-miniconda@v2
         with:
           python-version: '3.10'
 
       - run: conda install -c conda-forge --yes anaconda-client
-      - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
+      - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user physicscore --label main $(ls conda-package-*/*/*.tar.bz2)
   manage-versions:
     name: Manage Versions
 
     runs-on: 'ubuntu-20.04'
 
     outputs:
       version-new: ${{ steps.version.outputs.new }}
```

### Comparing `thermoblock-23.7.0.dev0/.github/workflows/test.yml` & `thermoblock-23.7.0.dev1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/.pre-commit-config.yaml` & `thermoblock-23.7.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/CONTRIBUTING.md` & `thermoblock-23.7.0.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/LICENSE` & `thermoblock-23.7.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/PKG-INFO` & `thermoblock-23.7.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermoblock
-Version: 23.7.0.dev0
+Version: 23.7.0.dev1
 Summary: Flux simulation toy building library.
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Physicscore contributors (https://github.com/physicscore)
         All rights reserved.
```

### Comparing `thermoblock-23.7.0.dev0/README.md` & `thermoblock-23.7.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/conda/meta.yaml` & `thermoblock-23.7.0.dev1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/docs/conf.py` & `thermoblock-23.7.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/docs/developer/coding-conventions.md` & `thermoblock-23.7.0.dev1/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/docs/developer/dependency-management.md` & `thermoblock-23.7.0.dev1/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/docs/developer/getting-started.md` & `thermoblock-23.7.0.dev1/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/pyproject.toml` & `thermoblock-23.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/requirements/ci.txt` & `thermoblock-23.7.0.dev1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/requirements/dev.txt` & `thermoblock-23.7.0.dev1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/requirements/docs.txt` & `thermoblock-23.7.0.dev1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/requirements/static.txt` & `thermoblock-23.7.0.dev1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/src/thermoblock/resources/colorspectrum.jpg` & `thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.jpg`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/src/thermoblock/resources/colorspectrum.pck` & `thermoblock-23.7.0.dev1/src/thermoblock/resources/colorspectrum.pck`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/src/thermoblock.egg-info/PKG-INFO` & `thermoblock-23.7.0.dev1/src/thermoblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermoblock
-Version: 23.7.0.dev0
+Version: 23.7.0.dev1
 Summary: Flux simulation toy building library.
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Physicscore contributors (https://github.com/physicscore)
         All rights reserved.
```

### Comparing `thermoblock-23.7.0.dev0/src/thermoblock.egg-info/SOURCES.txt` & `thermoblock-23.7.0.dev1/src/thermoblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thermoblock-23.7.0.dev0/tox.ini` & `thermoblock-23.7.0.dev1/tox.ini`

 * *Files identical despite different names*

