# Comparing `tmp/simple_plugin_manager_zimolab1995-0.0.3.tar.gz` & `tmp/simple_plugin_manager_zimolab1995-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_plugin_manager_zimolab1995-0.0.3.tar", last modified: Thu Jul 13 12:08:34 2023, max compression
+gzip compressed data, was "simple_plugin_manager_zimolab1995-0.0.4.tar", last modified: Thu Jul 20 14:03:51 2023, max compression
```

## Comparing `simple_plugin_manager_zimolab1995-0.0.3.tar` & `simple_plugin_manager_zimolab1995-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-12 14:17:41.000000 simple_plugin_manager_zimolab1995-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      653 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-12 14:16:25.000000 simple_plugin_manager_zimolab1995-0.0.3/README.md
--rw-rw-rw-   0        0        0      660 2023-07-13 12:08:09.000000 simple_plugin_manager_zimolab1995-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.074505 simple_plugin_manager_zimolab1995-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.085034 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/
--rw-rw-rw-   0        0        0        0 2023-07-12 14:18:01.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/__init__.py
--rw-rw-rw-   0        0        0      212 2023-07-13 11:05:22.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/exceptions.py
--rw-rw-rw-   0        0        0    13468 2023-07-13 11:21:51.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/manager.py
--rw-rw-rw-   0        0        0      865 2023-07-13 09:13:06.000000 simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/plugin.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:08:34.094561 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/
--rw-rw-rw-   0        0        0      653 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-13 12:08:34.000000 simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 14:03:51.883130 simple_plugin_manager_zimolab1995-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 14:17:41.000000 simple_plugin_manager_zimolab1995-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      653 2023-07-20 14:03:51.883130 simple_plugin_manager_zimolab1995-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-12 14:16:25.000000 simple_plugin_manager_zimolab1995-0.0.4/README.md
+-rw-rw-rw-   0        0        0      660 2023-07-20 14:00:18.000000 simple_plugin_manager_zimolab1995-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-20 14:03:51.884125 simple_plugin_manager_zimolab1995-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 14:03:51.864825 simple_plugin_manager_zimolab1995-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 14:03:51.874129 simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/
+-rw-rw-rw-   0        0        0        0 2023-07-12 14:18:01.000000 simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-07-13 11:05:22.000000 simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/exceptions.py
+-rw-rw-rw-   0        0        0    13476 2023-07-20 13:56:33.000000 simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/manager.py
+-rw-rw-rw-   0        0        0      865 2023-07-13 09:13:06.000000 simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:03:51.882126 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-07-20 14:03:51.000000 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-20 14:03:51.000000 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:03:51.000000 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-20 14:03:51.000000 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-20 14:03:51.000000 simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/top_level.txt
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/LICENSE` & `simple_plugin_manager_zimolab1995-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/PKG-INFO` & `simple_plugin_manager_zimolab1995-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_plugin_manager_zimolab1995
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple plugin manager for python project
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/simple_plugin_manager
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/simple_plugin_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/pyproject.toml` & `simple_plugin_manager_zimolab1995-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_plugin_manager_zimolab1995"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="zimolab1995", email="zimolab@aliyun.com" },
 ]
 description = "A simple plugin manager for python project"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/manager.py` & `simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,24 +241,24 @@
     def _load_plugin(self, plugin_file: str, encoding: str) -> PluginInfo:
         try:
             source = self._readfile(plugin_file, encoding)
         except BaseException as e:
             raise e
         plugin_dir = self._normpath(os.path.dirname(plugin_file))
         plugin_name = self._get_plugin_name(plugin_dir)
-        sys.path.append(plugin_dir)
+        # sys.path.append(plugin_dir)
         try:
             locals_ = {}
             self._executor.exec(source=source, filename=plugin_file, globals_=self._exec_globals, locals_=locals_)
             return PluginInfo.from_exec_result(plugin_name, locals_)
         except BaseException as e:
             raise InvalidPlugin(e)
-        finally:
-            if plugin_dir in sys.path:
-                sys.path.remove(plugin_dir)
+        # finally:
+        #     if plugin_dir in sys.path:
+        #         sys.path.remove(plugin_dir)
 
     @staticmethod
     def _get_plugin_name(path: str):
         if os.path.isfile(path):
             return path.split(".")[0]
         elif os.path.isdir(path):
             return os.path.basename(path)
```

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/src/plugin_manager/plugin.py` & `simple_plugin_manager_zimolab1995-0.0.4/src/plugin_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `simple_plugin_manager_zimolab1995-0.0.3/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO` & `simple_plugin_manager_zimolab1995-0.0.4/src/simple_plugin_manager_zimolab1995.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-plugin-manager-zimolab1995
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple plugin manager for python project
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/simple_plugin_manager
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/simple_plugin_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

