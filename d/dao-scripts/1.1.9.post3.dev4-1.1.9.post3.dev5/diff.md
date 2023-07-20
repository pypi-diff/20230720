# Comparing `tmp/dao-scripts-1.1.9.post3.dev4.tar.gz` & `tmp/dao-scripts-1.1.9.post3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao-scripts-1.1.9.post3.dev4.tar", last modified: Fri Jul 14 19:18:53 2023, max compression
+gzip compressed data, was "dao-scripts-1.1.9.post3.dev5.tar", last modified: Fri Jul 14 19:26:18 2023, max compression
```

## Comparing `dao-scripts-1.1.9.post3.dev4.tar` & `dao-scripts-1.1.9.post3.dev5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.578251 dao-scripts-1.1.9.post3.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.566250 dao-scripts-1.1.9.post3.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.570251 dao-scripts-1.1.9.post3.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-14 19:18:53.578251 dao-scripts-1.1.9.post3.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.570251 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-14 19:18:53.578251 dao-scripts-1.1.9.post3.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.574251 dao-scripts-1.1.9.post3.dev4/src/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-14 19:18:53.000000 dao-scripts-1.1.9.post3.dev4/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.574251 dao-scripts-1.1.9.post3.dev4/src/aragon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.574251 dao-scripts-1.1.9.post3.dev4/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/common/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.574251 dao-scripts-1.1.9.post3.dev4/src/daohaus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.574251 dao-scripts-1.1.9.post3.dev4/src/daostack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/endpoints.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5042 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/src/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:18:53.578251 dao-scripts-1.1.9.post3.dev4/test/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 19:18:36.000000 dao-scripts-1.1.9.post3.dev4/test/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.242704 dao-scripts-1.1.9.post3.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.226703 dao-scripts-1.1.9.post3.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.230703 dao-scripts-1.1.9.post3.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-14 19:26:18.242704 dao-scripts-1.1.9.post3.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.234704 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 19:26:18.242704 dao-scripts-1.1.9.post3.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.234704 dao-scripts-1.1.9.post3.dev5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-14 19:26:18.000000 dao-scripts-1.1.9.post3.dev5/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.238704 dao-scripts-1.1.9.post3.dev5/src/aragon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/aragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/aragon/dao_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/aragon/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.238704 dao-scripts-1.1.9.post3.dev5/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/common/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.238704 dao-scripts-1.1.9.post3.dev5/src/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/daohaus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/daohaus/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.238704 dao-scripts-1.1.9.post3.dev5/src/daostack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/daostack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/daostack/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/endpoints.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5042 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/src/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:26:18.238704 dao-scripts-1.1.9.post3.dev5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 19:25:57.000000 dao-scripts-1.1.9.post3.dev5/test/test_placeholder.py
```

### Comparing `dao-scripts-1.1.9.post3.dev4/.github/workflows/ci.yml` & `dao-scripts-1.1.9.post3.dev5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/.gitignore` & `dao-scripts-1.1.9.post3.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/CHANGELOG.md` & `dao-scripts-1.1.9.post3.dev5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/PKG-INFO` & `dao-scripts-1.1.9.post3.dev5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.1.9.post3.dev4
-Summary: "A tool to monitor DAO activity"
+Version: 1.1.9.post3.dev5
+Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,34 +28,34 @@
 # DAO-Analyzer's cache-scripts
 
 ## Set-up & Running
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
-pip install dao-analyzer
+pip install dao-scripts
 ```
 
-Then, you can use this script using the command `daoa-cache-scripts`
+Then, you can use this script using the command `daoa-cache-scripts` or `dao-scripts`
 
 ### Download
 Enter in your terminal (git must be installed) and write down:
 
 ```
-git clone https://github.com/Grasia/dao-analyzer
+git clone https://github.com/Grasia/dao-scripts
 ```
 
-After that, move to repository root directory with:
+After that, move to the repository root directory with:
 
 ```
-cd dao-analyzer
+cd dao-scripts
 ```
 
 ### Installation
-All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the python environment.
+All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the Python environment.
 
 So, you must install the following dependencies to run the tool:
 
 * python3 (3.10 or later)
 * python3-pip
 
 Now, install the Python dependencies:
@@ -64,32 +64,32 @@
 
 If you don't want to share Python dependencies among other projects, you should use a virtual environment, such as [virtualenv](https://docs.python-guide.org/dev/virtualenvs/).
 
 ### How to run it?
 If you want all the data used in the app, you can just use:
 
 ```
-python3 -m cache_scripts
+dao-scripts
 ```
 
-this will create a folder called `datawarehouse` with a lot of files in apache's arrow format.
+this will create a folder called `datawarehouse` with a lot of files in Apache's arrow format.
 
 You can import those files to `pandas` with `read_feather`. For example:
 
 ```python
 pd.read_feather('datawarehouse/aragon/apps.arr')
 ```
 
 ## Usage guide
 If you don't want all the data (and it can take a lot of time), you have a lot of options available to select whichever data you want. The full `--help` output is
 
 ```
 usage: daoa-cache-scripts [-h] [-V] [-p [{aragon,daohaus,daostack} ...]]
                           [--ignore-errors | --no-ignore-errors] [-d] [-f] [-F] [--skip-daohaus-names]
-                          [-n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]]
+                          [-n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]]
                           [-c COLLECTORS [COLLECTORS ...]] [--block-datetime BLOCK_DATETIME]
                           [-D DATAWAREHOUSE] [--cc-api-key CC_API_KEY]
 
 Main script to populate dao-analyzer cache
 
 options:
   -h, --help            show this help message and exit
@@ -98,15 +98,15 @@
                         The platforms to update. Every platform is updated by default.
   --ignore-errors, --no-ignore-errors
                         Whether to ignore errors and continue (default: True)
   -d, --debug           Shows debug info
   -f, --force           Removes the cache before updating
   -F, --delete-force    Removes the datawarehouse folder before doing anything
   --skip-daohaus-names  Skips the step of getting Daohaus Moloch's names, which takes some time
-  -n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...], --networks {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]
+    -n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...], --networks {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]
                         Networks to update. Every network is updated by default
   -c COLLECTORS [COLLECTORS ...], --collectors COLLECTORS [COLLECTORS ...]
                         Collectors to run. For example: aragon/casts
   --block-datetime BLOCK_DATETIME
                         Get data up to a block datetime (input in ISO format)
   -D DATAWAREHOUSE, --datawarehouse DATAWAREHOUSE
                         Specifies the destination folder of the datawarehouse
```

### Comparing `dao-scripts-1.1.9.post3.dev4/README.md` & `dao-scripts-1.1.9.post3.dev5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # DAO-Analyzer's cache-scripts
 
 ## Set-up & Running
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
-pip install dao-analyzer
+pip install dao-scripts
 ```
 
-Then, you can use this script using the command `daoa-cache-scripts`
+Then, you can use this script using the command `daoa-cache-scripts` or `dao-scripts`
 
 ### Download
 Enter in your terminal (git must be installed) and write down:
 
 ```
-git clone https://github.com/Grasia/dao-analyzer
+git clone https://github.com/Grasia/dao-scripts
 ```
 
-After that, move to repository root directory with:
+After that, move to the repository root directory with:
 
 ```
-cd dao-analyzer
+cd dao-scripts
 ```
 
 ### Installation
-All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the python environment.
+All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the Python environment.
 
 So, you must install the following dependencies to run the tool:
 
 * python3 (3.10 or later)
 * python3-pip
 
 Now, install the Python dependencies:
@@ -37,32 +37,32 @@
 
 If you don't want to share Python dependencies among other projects, you should use a virtual environment, such as [virtualenv](https://docs.python-guide.org/dev/virtualenvs/).
 
 ### How to run it?
 If you want all the data used in the app, you can just use:
 
 ```
-python3 -m cache_scripts
+dao-scripts
 ```
 
-this will create a folder called `datawarehouse` with a lot of files in apache's arrow format.
+this will create a folder called `datawarehouse` with a lot of files in Apache's arrow format.
 
 You can import those files to `pandas` with `read_feather`. For example:
 
 ```python
 pd.read_feather('datawarehouse/aragon/apps.arr')
 ```
 
 ## Usage guide
 If you don't want all the data (and it can take a lot of time), you have a lot of options available to select whichever data you want. The full `--help` output is
 
 ```
 usage: daoa-cache-scripts [-h] [-V] [-p [{aragon,daohaus,daostack} ...]]
                           [--ignore-errors | --no-ignore-errors] [-d] [-f] [-F] [--skip-daohaus-names]
-                          [-n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]]
+                          [-n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]]
                           [-c COLLECTORS [COLLECTORS ...]] [--block-datetime BLOCK_DATETIME]
                           [-D DATAWAREHOUSE] [--cc-api-key CC_API_KEY]
 
 Main script to populate dao-analyzer cache
 
 options:
   -h, --help            show this help message and exit
@@ -71,15 +71,15 @@
                         The platforms to update. Every platform is updated by default.
   --ignore-errors, --no-ignore-errors
                         Whether to ignore errors and continue (default: True)
   -d, --debug           Shows debug info
   -f, --force           Removes the cache before updating
   -F, --delete-force    Removes the datawarehouse folder before doing anything
   --skip-daohaus-names  Skips the step of getting Daohaus Moloch's names, which takes some time
-  -n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...], --networks {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]
+    -n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...], --networks {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]
                         Networks to update. Every network is updated by default
   -c COLLECTORS [COLLECTORS ...], --collectors COLLECTORS [COLLECTORS ...]
                         Collectors to run. For example: aragon/casts
   --block-datetime BLOCK_DATETIME
                         Get data up to a block datetime (input in ISO format)
   -D DATAWAREHOUSE, --datawarehouse DATAWAREHOUSE
                         Specifies the destination folder of the datawarehouse
```

### Comparing `dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/PKG-INFO` & `dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dao-scripts
-Version: 1.1.9.post3.dev4
-Summary: "A tool to monitor DAO activity"
+Version: 1.1.9.post3.dev5
+Summary: "A tool to download data to monitor DAO activity"
 Home-page: https://github.com/Grasia/dao-scripts
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-scripts
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-scripts/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,34 +28,34 @@
 # DAO-Analyzer's cache-scripts
 
 ## Set-up & Running
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
-pip install dao-analyzer
+pip install dao-scripts
 ```
 
-Then, you can use this script using the command `daoa-cache-scripts`
+Then, you can use this script using the command `daoa-cache-scripts` or `dao-scripts`
 
 ### Download
 Enter in your terminal (git must be installed) and write down:
 
 ```
-git clone https://github.com/Grasia/dao-analyzer
+git clone https://github.com/Grasia/dao-scripts
 ```
 
-After that, move to repository root directory with:
+After that, move to the repository root directory with:
 
 ```
-cd dao-analyzer
+cd dao-scripts
 ```
 
 ### Installation
-All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the python environment.
+All code has been tested on Linux, but it should work on Windows and macOS, 'cause it just uses the Python environment.
 
 So, you must install the following dependencies to run the tool:
 
 * python3 (3.10 or later)
 * python3-pip
 
 Now, install the Python dependencies:
@@ -64,32 +64,32 @@
 
 If you don't want to share Python dependencies among other projects, you should use a virtual environment, such as [virtualenv](https://docs.python-guide.org/dev/virtualenvs/).
 
 ### How to run it?
 If you want all the data used in the app, you can just use:
 
 ```
-python3 -m cache_scripts
+dao-scripts
 ```
 
-this will create a folder called `datawarehouse` with a lot of files in apache's arrow format.
+this will create a folder called `datawarehouse` with a lot of files in Apache's arrow format.
 
 You can import those files to `pandas` with `read_feather`. For example:
 
 ```python
 pd.read_feather('datawarehouse/aragon/apps.arr')
 ```
 
 ## Usage guide
 If you don't want all the data (and it can take a lot of time), you have a lot of options available to select whichever data you want. The full `--help` output is
 
 ```
 usage: daoa-cache-scripts [-h] [-V] [-p [{aragon,daohaus,daostack} ...]]
                           [--ignore-errors | --no-ignore-errors] [-d] [-f] [-F] [--skip-daohaus-names]
-                          [-n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]]
+                          [-n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]]
                           [-c COLLECTORS [COLLECTORS ...]] [--block-datetime BLOCK_DATETIME]
                           [-D DATAWAREHOUSE] [--cc-api-key CC_API_KEY]
 
 Main script to populate dao-analyzer cache
 
 options:
   -h, --help            show this help message and exit
@@ -98,15 +98,15 @@
                         The platforms to update. Every platform is updated by default.
   --ignore-errors, --no-ignore-errors
                         Whether to ignore errors and continue (default: True)
   -d, --debug           Shows debug info
   -f, --force           Removes the cache before updating
   -F, --delete-force    Removes the datawarehouse folder before doing anything
   --skip-daohaus-names  Skips the step of getting Daohaus Moloch's names, which takes some time
-  -n {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...], --networks {mainnet,_theGraph,arbitrum,xdai,polygon} [{mainnet,_theGraph,arbitrum,xdai,polygon} ...]
+    -n {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...], --networks {mainnet,arbitrum,xdai,polygon} [{mainnet,arbitrum,xdai,polygon} ...]
                         Networks to update. Every network is updated by default
   -c COLLECTORS [COLLECTORS ...], --collectors COLLECTORS [COLLECTORS ...]
                         Collectors to run. For example: aragon/casts
   --block-datetime BLOCK_DATETIME
                         Get data up to a block datetime (input in ISO format)
   -D DATAWAREHOUSE, --datawarehouse DATAWAREHOUSE
                         Specifies the destination folder of the datawarehouse
```

### Comparing `dao-scripts-1.1.9.post3.dev4/dao_scripts.egg-info/SOURCES.txt` & `dao-scripts-1.1.9.post3.dev5/dao_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/setup.cfg` & `dao-scripts-1.1.9.post3.dev5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = dao-scripts
 author = David Davó
 author_email = ddavo@ucm.es
-description = "A tool to monitor DAO activity"
+description = "A tool to download data to monitor DAO activity"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Grasia/dao-scripts
 project_urls = 
 	Source = https://github.com/Grasia/dao-scripts
 	Bug Tracker = https://github.com/Grasia/dao-scripts/issues
 	Changelog = https://github.com/Grasia/dao-scripts/blob/main/CHANGELOG.md
@@ -56,15 +56,14 @@
 dev = 
 	build
 	pytest
 	hypothesis
 	flake8
 	pandas-vet
 	twine
-	pytest
 	hypothesis
 	pandas-vet
 
 [flake8]
 ignore = 
 	E1,
 	E2,
```

### Comparing `dao-scripts-1.1.9.post3.dev4/setup.py` & `dao-scripts-1.1.9.post3.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/aragon/dao_names.json` & `dao-scripts-1.1.9.post3.dev5/src/aragon/dao_names.json`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/aragon/runner.py` & `dao-scripts-1.1.9.post3.dev5/src/aragon/runner.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/argparser.py` & `dao-scripts-1.1.9.post3.dev5/src/argparser.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/common/api_requester.py` & `dao-scripts-1.1.9.post3.dev5/src/common/api_requester.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/common/blockscout.py` & `dao-scripts-1.1.9.post3.dev5/src/common/blockscout.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/common/common.py` & `dao-scripts-1.1.9.post3.dev5/src/common/common.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/common/cryptocompare.py` & `dao-scripts-1.1.9.post3.dev5/src/common/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/common/graphql.py` & `dao-scripts-1.1.9.post3.dev5/src/common/graphql.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/config.py` & `dao-scripts-1.1.9.post3.dev5/src/config.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/daohaus/runner.py` & `dao-scripts-1.1.9.post3.dev5/src/daohaus/runner.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/daostack/runner.py` & `dao-scripts-1.1.9.post3.dev5/src/daostack/runner.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/endpoints.json` & `dao-scripts-1.1.9.post3.dev5/src/endpoints.json`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/main.py` & `dao-scripts-1.1.9.post3.dev5/src/main.py`

 * *Files identical despite different names*

### Comparing `dao-scripts-1.1.9.post3.dev4/src/metadata.py` & `dao-scripts-1.1.9.post3.dev5/src/metadata.py`

 * *Files identical despite different names*

