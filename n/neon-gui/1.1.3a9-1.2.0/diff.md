# Comparing `tmp/neon_gui-1.1.3a9.tar.gz` & `tmp/neon_gui-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_gui-1.1.3a9.tar", last modified: Thu Jun 29 22:17:32 2023, max compression
+gzip compressed data, was "neon_gui-1.2.0.tar", last modified: Thu Jul 20 16:38:24 2023, max compression
```

## Comparing `neon_gui-1.1.3a9.tar` & `neon_gui-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/neon_gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/neon_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-20 16:38:18.000000 neon_gui-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-20 16:38:24.785737 neon_gui-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 16:38:18.000000 neon_gui-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/neon_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-20 16:38:18.000000 neon_gui-1.2.0/neon_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:38:24.785737 neon_gui-1.2.0/neon_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 16:38:24.000000 neon_gui-1.2.0/neon_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:38:24.785737 neon_gui-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-20 16:38:18.000000 neon_gui-1.2.0/setup.py
```

### Comparing `neon_gui-1.1.3a9/LICENSE.md` & `neon_gui-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/PKG-INFO` & `neon_gui-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_gui
-Version: 1.1.3a9
+Version: 1.2.0
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a9/README.md` & `neon_gui-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/neon_gui/__init__.py` & `neon_gui-1.2.0/neon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/neon_gui/__main__.py` & `neon_gui-1.2.0/neon_gui/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,9 +47,16 @@
         try:
             print_malloc(snapshot_malloc())
         except Exception as e:
             LOG.error(e)
     gui.shutdown()
 
 
+def deprecated_entrypoint():
+    from ovos_utils.log import log_deprecation
+    log_deprecation("Use `neon-gui run` in place of "
+                    "`neon_gui_service`", "2.0.0")
+    main()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `neon_gui-1.1.3a9/neon_gui/cli.py` & `neon_gui-1.2.0/neon_gui/cli.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/neon_gui/service.py` & `neon_gui-1.2.0/neon_gui/service.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/neon_gui/utils.py` & `neon_gui-1.2.0/neon_gui/utils.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a9/neon_gui.egg-info/PKG-INFO` & `neon_gui-1.2.0/neon_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.3a9
+Version: 1.2.0
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a9/setup.py` & `neon_gui-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,12 +75,12 @@
     author_email='developers@neon.ai',
     description="Neon GUI Module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
             # TODO: Deprecate `neon_gui_service` entrypoint
-            'neon_gui_service=neon_gui.__main__:main',
+            'neon_gui_service=neon_gui.__main__:deprecated_entrypoint',
             'neon-gui=neon_gui.cli:neon_gui_cli'
         ]
     }
 )
```

