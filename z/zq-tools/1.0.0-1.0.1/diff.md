# Comparing `tmp/zq-tools-1.0.0.tar.gz` & `tmp/zq-tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-tools-1.0.0.tar", last modified: Thu Jul 20 10:11:49 2023, max compression
+gzip compressed data, was "zq-tools-1.0.1.tar", last modified: Thu Jul 20 10:30:19 2023, max compression
```

## Comparing `zq-tools-1.0.0.tar` & `zq-tools-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/
--rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:11:49.611075 zq-tools-1.0.0/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)     2736 2023-07-20 10:10:25.000000 zq-tools-1.0.0/README.md
--rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-07-20 10:11:49.611075 zq-tools-1.0.0/setup.cfg
--rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-07-20 10:11:00.000000 zq-tools-1.0.0/setup.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.601075 zq-tools-1.0.0/test/
--rw-r--r--   0 togo      (1000) togo      (1000)      256 2023-07-20 10:09:20.000000 zq-tools-1.0.0/test/test_zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-07-20 09:54:35.000000 zq-tools-1.0.0/test/test_zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/zq_tools/
--rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/__init__.py
--rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_cycle.py
--rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_decorator.py
--rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_files.py
--rw-r--r--   0 togo      (1000) togo      (1000)     8482 2023-07-20 10:09:08.000000 zq-tools-1.0.0/zq_tools/zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/zq_tools.egg-info/
--rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/SOURCES.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/dependency_links.txt
--rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/requires.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/top_level.txt
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:30:19.260483 zq-tools-1.0.1/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)     2736 2023-07-20 10:30:08.000000 zq-tools-1.0.1/README.md
+-rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-07-20 10:30:19.260483 zq-tools-1.0.1/setup.cfg
+-rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-07-20 10:30:12.000000 zq-tools-1.0.1/setup.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.250483 zq-tools-1.0.1/test/
+-rw-r--r--   0 togo      (1000) togo      (1000)      256 2023-07-20 10:09:20.000000 zq-tools-1.0.1/test/test_zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-07-20 09:54:35.000000 zq-tools-1.0.1/test/test_zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/zq_tools/
+-rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/__init__.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_cycle.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_decorator.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_files.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     8517 2023-07-20 10:29:03.000000 zq-tools-1.0.1/zq_tools/zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/zq_tools.egg-info/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/requires.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/top_level.txt
```

### Comparing `zq-tools-1.0.0/PKG-INFO` & `zq-tools-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.0: make `zq_logger` support print to screen and file with different levels
+- 1.0.1: make `zq_logger` support print to screen and file with different levels
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.0/README.md` & `zq-tools-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.0: make `zq_logger` support print to screen and file with different levels
+- 1.0.1: make `zq_logger` support print to screen and file with different levels
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.0/setup.py` & `zq-tools-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="zq-tools",
-    version="1.0.0",
+    version="1.0.1",
     author="zzqq2199",
     author_email="zhouquanjs@qq.com",
     description="A collection of tools for zzqq2199",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["zq_tools"],
     classifiers=[
```

### Comparing `zq-tools-1.0.0/test/test_zq_tracing.py` & `zq-tools-1.0.1/test/test_zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.0/zq_tools/zq_cycle.py` & `zq-tools-1.0.1/zq_tools/zq_cycle.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.0/zq_tools/zq_decorator.py` & `zq-tools-1.0.1/zq_tools/zq_decorator.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.0/zq_tools/zq_files.py` & `zq-tools-1.0.1/zq_tools/zq_files.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.0/zq_tools/zq_logger.py` & `zq-tools-1.0.1/zq_tools/zq_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 def get_logger(logger_name="Z_LEVEL",
                enable_console = True)->ZQ_Logger:
     if logger_name in allocated_loggers: return allocated_loggers[logger_name]
     # why need to call `setLoggerClass` twice? refer to the issue: https://bugs.python.org/issue37258
     logging.setLoggerClass(ZQ_Logger)
     logger = logging.getLogger(logger_name)
     logging.setLoggerClass(logging.Logger)
+    logger.setLevel(logging.DEBUG)
     # Initilize level from environment. If not specified, use INFO
     if enable_console:
         console_handler = logging.StreamHandler()
         console_handler.setLevel(get_level_from_env(logger_name))
         logger.addHandler(console_handler)
     logger.reset_format()
     allocated_loggers[logger_name] = logger
```

### Comparing `zq-tools-1.0.0/zq_tools/zq_tracing.py` & `zq-tools-1.0.1/zq_tools/zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.0/zq_tools.egg-info/PKG-INFO` & `zq-tools-1.0.1/zq_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.0: make `zq_logger` support print to screen and file with different levels
+- 1.0.1: make `zq_logger` support print to screen and file with different levels
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

