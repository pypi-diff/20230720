# Comparing `tmp/djangoldp_babelfish-0.0.2.tar.gz` & `tmp/djangoldp_babelfish-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_babelfish-0.0.2.tar", last modified: Thu Jul 20 17:41:50 2023, max compression
+gzip compressed data, was "dist/djangoldp_babelfish-0.0.3.tar", last modified: Thu Jul 20 17:44:38 2023, max compression
```

## Comparing `djangoldp_babelfish-0.0.2.tar` & `djangoldp_babelfish-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-20 17:41:47.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-20 17:41:28.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 17:41:50.000000 djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-20 17:44:35.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-20 17:44:16.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 17:44:38.000000 djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/requires.txt
```

### Comparing `djangoldp_babelfish-0.0.2/README.md` & `djangoldp_babelfish-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 
 If, no error, it's working.
 
 ## Specific settings
 
 AS for all the other djangoLDP packages, there are some settings which you can customize:
 
-Settings        | Example values     | Usage   
-----------------|--------------------|
-`BABELFISH_CLIENT_ID`      | `iYxxxMu-dGssslaIaSxxxxxxxx` | Provided by Babelfish upon organization registration
-`BABELFISH_CLIENT_SECRET` | `e6ssslvl_WII9qP7E1rxxxxxx` | Provided by Babelfish upon organization registration   
-`BABELFISH_BASE_URL` | https://babelfish.data-container.net | The Babelfish server you would like to use         
-`BABELFISH_ORGANISATION_ID` | 811 | Provided by Babelfish upon organisation registration
+Settings                    | Example values                       | Usage   
+----------------------------|--------------------------------------|-----------------------------------------------------
+`BABELFISH_CLIENT_ID`       | `iYxxxMu-dGssslaIaSxxxxxxxx`         | Provided by Babelfish upon organization registration
+`BABELFISH_CLIENT_SECRET`   | `e6ssslvl_WII9qP7E1rxxxxxx`          | Provided by Babelfish upon organization registration   
+`BABELFISH_BASE_URL`        | https://babelfish.data-container.net | The Babelfish server you would like to use         
+`BABELFISH_ORGANISATION_ID` | 811                                  | Provided by Babelfish upon organisation registration
```

### Comparing `djangoldp_babelfish-0.0.2/setup.cfg` & `djangoldp_babelfish-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.2/djangoldp_babelfish/views.py` & `djangoldp_babelfish-0.0.3/djangoldp_babelfish/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.2/djangoldp_babelfish/models.py` & `djangoldp_babelfish-0.0.3/djangoldp_babelfish/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-0.0.3/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-0.0.2/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-0.0.3/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

