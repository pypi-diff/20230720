# Comparing `tmp/zq-tools-0.9.9.tar.gz` & `tmp/zq-tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-tools-0.9.9.tar", last modified: Wed Dec 21 11:12:03 2022, max compression
+gzip compressed data, was "zq-tools-1.0.0.tar", last modified: Thu Jul 20 10:11:49 2023, max compression
```

## Comparing `zq-tools-0.9.9.tar` & `zq-tools-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2022-12-21 11:12:03.299977 zq-tools-0.9.9/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3470 2022-12-21 11:12:03.299977 zq-tools-0.9.9/PKG-INFO
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     2655 2022-12-21 11:10:34.000000 zq-tools-0.9.9/README.md
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       38 2022-12-21 11:12:03.303977 zq-tools-0.9.9/setup.cfg
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      622 2022-12-21 11:10:49.000000 zq-tools-0.9.9/setup.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2022-12-21 11:12:03.199978 zq-tools-0.9.9/test/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       91 2022-11-19 05:19:08.000000 zq-tools-0.9.9/test/test_zq_logger.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     1051 2022-09-25 08:06:36.000000 zq-tools-0.9.9/test/test_zq_tracing.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2022-12-21 11:12:03.247978 zq-tools-0.9.9/zq_tools/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      187 2022-11-19 05:17:23.000000 zq-tools-0.9.9/zq_tools/__init__.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      830 2022-12-21 11:09:55.000000 zq-tools-0.9.9/zq_tools/zq_cycle.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     4596 2022-10-25 03:53:08.000000 zq-tools-0.9.9/zq_tools/zq_decorator.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      520 2022-09-25 08:26:17.000000 zq-tools-0.9.9/zq_tools/zq_files.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     8521 2022-11-19 05:11:46.000000 zq-tools-0.9.9/zq_tools/zq_logger.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     5227 2022-10-20 06:14:14.000000 zq-tools-0.9.9/zq_tools/zq_tracing.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2022-12-21 11:12:03.291978 zq-tools-0.9.9/zq_tools.egg-info/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3470 2022-12-21 11:12:02.000000 zq-tools-0.9.9/zq_tools.egg-info/PKG-INFO
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      357 2022-12-21 11:12:03.000000 zq-tools-0.9.9/zq_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        1 2022-12-21 11:12:02.000000 zq-tools-0.9.9/zq_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       23 2022-12-21 11:12:02.000000 zq-tools-0.9.9/zq_tools.egg-info/requires.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        9 2022-12-21 11:12:02.000000 zq-tools-0.9.9/zq_tools.egg-info/top_level.txt
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:11:49.611075 zq-tools-1.0.0/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)     2736 2023-07-20 10:10:25.000000 zq-tools-1.0.0/README.md
+-rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-07-20 10:11:49.611075 zq-tools-1.0.0/setup.cfg
+-rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-07-20 10:11:00.000000 zq-tools-1.0.0/setup.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.601075 zq-tools-1.0.0/test/
+-rw-r--r--   0 togo      (1000) togo      (1000)      256 2023-07-20 10:09:20.000000 zq-tools-1.0.0/test/test_zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-07-20 09:54:35.000000 zq-tools-1.0.0/test/test_zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/zq_tools/
+-rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/__init__.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_cycle.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_decorator.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_files.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     8482 2023-07-20 10:09:08.000000 zq-tools-1.0.0/zq_tools/zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-07-20 09:54:35.000000 zq-tools-1.0.0/zq_tools/zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:11:49.611075 zq-tools-1.0.0/zq_tools.egg-info/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/requires.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-07-20 10:11:49.000000 zq-tools-1.0.0/zq_tools.egg-info/top_level.txt
```

### Comparing `zq-tools-0.9.9/PKG-INFO` & `zq-tools-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,54 @@
-Metadata-Version: 2.1
-Name: zq-tools
-Version: 0.9.9
-Summary: A collection of tools for zzqq2199
-Home-page: UNKNOWN
-Author: zzqq2199
-Author-email: zhouquanjs@qq.com
-License: UNKNOWN
-Description: # zq_logger
-        generates a logger, preformatted with the file name, line number information, differrent levels of color, and can be output in the console and written to a file at the same time.
-        
-        ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220701162735.png)
-        
-        If you use vscode to view the output log in the editor, `ANSI Colors` extension is recommended to install.
-        
-        # zq_tracing
-        help generate json file used in `chrome://tracing`
-        
-        ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
-        
-        
-        # Release Notes
-        - 0.9.9: add `__repr__` for zq_cycle
-        - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
-        - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
-        - 0.9.6: increase version due to keep failing on uploading
-        - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
-        - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
-        - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
-        - 0.9.1: use `default_logger` instead of `print`
-        - 0.9.0: add decorator and manager: `zq_decorator.timeit`
-        - 0.8.8: add decorator: `zq_decorator.do_nothing`
-        - 0.8.7: add api: `zq_tracing.enable_trace`, `zq_tracing.disable_trace`
-        - 0.8.6: add api: `zq_tracing.record_init`, `zq_tracing.record_append`
-        - 0.8.5: add api: `zq_tracing.set_start_timestamp`
-        - 0.8.4: fix bug, add `colorful` to dependency
-        - 0.8.3: add `zq_files`
-        - 0.8.2: support `from zq_tools.zq_logger import default_logger as logger`
-        - 0.8.0: use `add_log_file` to add a log file to the logger.
-        - 0.7.0: re-think the color print logic
-        - 0.6.0: rename function: logger.print* --> logger.prank*
-        - 0.5.9: set level of print bewteen DEBUG and INFO, add `*_root` functions
-        - 0.5.8: implement `__len__` and `__iter__` for zq_cycle
-        - 0.5.6: add colors for different rank. add filter for zq_logger
-        - 0.5.5: disable color by default for `print` and `print_all`
-        - 0.5.3: zq_logger supports `print`, `print_all`, `set_rank`
-        - 0.5.1: move tag to ahead of msg
-        - 0.5.0: zq_logger supports color API, add tag
-        - 0.4.1: fix bug of zq_cycle
-        - 0.4.0: add zq_cycle
-        - 0.3.6: default unit of timestamp: us
-        - 0.3.5: support manually specifiying tid/pid when calling `zq_tracing.record_*`
-        - 0.3.4: fix bug
-        - 0.3.3: add default logger, call `zq_logger.get_logger()`, return a pre-defined logger
-        - 0.3.2: add async record, support nested and ordered tracing events
-        - 0.3.1: add install dependencies
-        - 0.3.0: output `pathname` instead of `filename`, better support for IDE's jumping function
-        
-        
-        # TODO:
-        - add setLogPath()
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# zq_logger
+generates a logger, preformatted with the file name, line number information, differrent levels of color, and can be output in the console and written to a file at the same time.
+
+![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220701162735.png)
+
+If you use vscode to view the output log in the editor, `ANSI Colors` extension is recommended to install.
+
+# zq_tracing
+help generate json file used in `chrome://tracing`
+
+![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
+
+
+# Release Notes
+- 1.0.0: make `zq_logger` support print to screen and file with different levels
+- 0.9.9: add `__repr__` for zq_cycle
+- 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
+- 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
+- 0.9.6: increase version due to keep failing on uploading
+- 0.9.4: fix bug: `zq_decorator.time_it(sync)`
+- 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
+- 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
+- 0.9.1: use `default_logger` instead of `print`
+- 0.9.0: add decorator and manager: `zq_decorator.timeit`
+- 0.8.8: add decorator: `zq_decorator.do_nothing`
+- 0.8.7: add api: `zq_tracing.enable_trace`, `zq_tracing.disable_trace`
+- 0.8.6: add api: `zq_tracing.record_init`, `zq_tracing.record_append`
+- 0.8.5: add api: `zq_tracing.set_start_timestamp`
+- 0.8.4: fix bug, add `colorful` to dependency
+- 0.8.3: add `zq_files`
+- 0.8.2: support `from zq_tools.zq_logger import default_logger as logger`
+- 0.8.0: use `add_log_file` to add a log file to the logger.
+- 0.7.0: re-think the color print logic
+- 0.6.0: rename function: logger.print* --> logger.prank*
+- 0.5.9: set level of print bewteen DEBUG and INFO, add `*_root` functions
+- 0.5.8: implement `__len__` and `__iter__` for zq_cycle
+- 0.5.6: add colors for different rank. add filter for zq_logger
+- 0.5.5: disable color by default for `print` and `print_all`
+- 0.5.3: zq_logger supports `print`, `print_all`, `set_rank`
+- 0.5.1: move tag to ahead of msg
+- 0.5.0: zq_logger supports color API, add tag
+- 0.4.1: fix bug of zq_cycle
+- 0.4.0: add zq_cycle
+- 0.3.6: default unit of timestamp: us
+- 0.3.5: support manually specifiying tid/pid when calling `zq_tracing.record_*`
+- 0.3.4: fix bug
+- 0.3.3: add default logger, call `zq_logger.get_logger()`, return a pre-defined logger
+- 0.3.2: add async record, support nested and ordered tracing events
+- 0.3.1: add install dependencies
+- 0.3.0: output `pathname` instead of `filename`, better support for IDE's jumping function
+
+
+# TODO:
+- add setLogPath()
```

### Comparing `zq-tools-0.9.9/README.md` & `zq-tools-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,33 @@
+Metadata-Version: 2.1
+Name: zq-tools
+Version: 1.0.0
+Summary: A collection of tools for zzqq2199
+Author: zzqq2199
+Author-email: zhouquanjs@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # zq_logger
 generates a logger, preformatted with the file name, line number information, differrent levels of color, and can be output in the console and written to a file at the same time.
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220701162735.png)
 
 If you use vscode to view the output log in the editor, `ANSI Colors` extension is recommended to install.
 
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
+- 1.0.0: make `zq_logger` support print to screen and file with different levels
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
@@ -46,8 +58,8 @@
 - 0.3.3: add default logger, call `zq_logger.get_logger()`, return a pre-defined logger
 - 0.3.2: add async record, support nested and ordered tracing events
 - 0.3.1: add install dependencies
 - 0.3.0: output `pathname` instead of `filename`, better support for IDE's jumping function
 
 
 # TODO:
-- add setLogPath()
+- add setLogPath()
```

### Comparing `zq-tools-0.9.9/setup.py` & `zq-tools-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="zq-tools",
-    version="0.9.9",
+    version="1.0.0",
     author="zzqq2199",
     author_email="zhouquanjs@qq.com",
     description="A collection of tools for zzqq2199",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["zq_tools"],
     classifiers=[
```

### Comparing `zq-tools-0.9.9/test/test_zq_tracing.py` & `zq-tools-1.0.0/test/test_zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-0.9.9/zq_tools/zq_cycle.py` & `zq-tools-1.0.0/zq_tools/zq_cycle.py`

 * *Files identical despite different names*

### Comparing `zq-tools-0.9.9/zq_tools/zq_decorator.py` & `zq-tools-1.0.0/zq_tools/zq_decorator.py`

 * *Files identical despite different names*

### Comparing `zq-tools-0.9.9/zq_tools/zq_files.py` & `zq-tools-1.0.0/zq_tools/zq_files.py`

 * *Files identical despite different names*

### Comparing `zq-tools-0.9.9/zq_tools/zq_logger.py` & `zq-tools-1.0.0/zq_tools/zq_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,18 +29,23 @@
         super(ZQ_Logger, self).__init__(name)
         self.tag = ""
         self.print_thread = False
         self.print_level = True
         self.rank = 0
         self.log_files = dict()
         
-    def add_log_file(self, log_file:str):
+    def add_log_file(self, log_file:str, level:int=logging.DEBUG):
         # file handler follows same level control behavior as console handler
         if log_file in self.log_files: return
+        if log_file in self.log_files:
+            handler = self.log_files[log_file]
+            handler.setLevel(level)
+            return
         handler = logging.FileHandler(log_file)
+        handler.setLevel(level)
         self.log_files[log_file] = handler
         self.addHandler(handler)
         self.reset_format()
         
         
     def generate_fmt(self)->logging.StreamHandler:
         thread_fmt = "" if not self.print_thread else "[%(threadName)s] "
@@ -82,21 +87,21 @@
         self._log(self.PRANK, color(msg), args, **kwargs)
     def debug(self, msg:str, color:str='',*args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if not self.isEnabledFor(self.DEBUG): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.DEBUG, color(msg), args, **kwargs)
     def info(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
+        self._log(logging.INFO, cf.green(msg), args, kwargs)
     def warn(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        self._log(logging.WARN, cf.yellow(msg), args, kwargs)
     def error(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        self._log(logging.ERROR, cf.red(msg), args, kwargs)
     def fatal(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
 
     def prank_root(self, msg:str, color:str='', root=0, *args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.PRANK): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.PRANK, color(msg), args, **kwargs)
@@ -104,24 +109,24 @@
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.DEBUG): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.DEBUG, color(msg), args, **kwargs)
     def info_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
+        self._log(logging.INFO, cf.green(msg), args, kwargs)
     def warn_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        self._log(logging.WARN, cf.yellow(msg), args, kwargs)
     def error_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        self._log(logging.ERROR, cf.red(msg), args, kwargs)
     def fatal_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
         
     warning = warn
     critical = fatal
     warning_root = warn_root
     critical_root = fatal_root
     
 def get_level_from_env(logger_name:str, default_level="info"):
@@ -146,17 +151,18 @@
                enable_console = True)->ZQ_Logger:
     if logger_name in allocated_loggers: return allocated_loggers[logger_name]
     # why need to call `setLoggerClass` twice? refer to the issue: https://bugs.python.org/issue37258
     logging.setLoggerClass(ZQ_Logger)
     logger = logging.getLogger(logger_name)
     logging.setLoggerClass(logging.Logger)
     # Initilize level from environment. If not specified, use INFO
-    logger.setLevel(get_level_from_env(logger_name))
     if enable_console:
-        logger.addHandler(logging.StreamHandler())
+        console_handler = logging.StreamHandler()
+        console_handler.setLevel(get_level_from_env(logger_name))
+        logger.addHandler(console_handler)
     logger.reset_format()
     allocated_loggers[logger_name] = logger
     return logger
 
 default_logger = get_logger()
```

### Comparing `zq-tools-0.9.9/zq_tools/zq_tracing.py` & `zq-tools-1.0.0/zq_tools/zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-0.9.9/zq_tools.egg-info/PKG-INFO` & `zq-tools-1.0.0/zq_tools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 0.9.9
+Version: 1.0.0
 Summary: A collection of tools for zzqq2199
-Home-page: UNKNOWN
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
-License: UNKNOWN
-Description: # zq_logger
-        generates a logger, preformatted with the file name, line number information, differrent levels of color, and can be output in the console and written to a file at the same time.
-        
-        ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220701162735.png)
-        
-        If you use vscode to view the output log in the editor, `ANSI Colors` extension is recommended to install.
-        
-        # zq_tracing
-        help generate json file used in `chrome://tracing`
-        
-        ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
-        
-        
-        # Release Notes
-        - 0.9.9: add `__repr__` for zq_cycle
-        - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
-        - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
-        - 0.9.6: increase version due to keep failing on uploading
-        - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
-        - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
-        - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
-        - 0.9.1: use `default_logger` instead of `print`
-        - 0.9.0: add decorator and manager: `zq_decorator.timeit`
-        - 0.8.8: add decorator: `zq_decorator.do_nothing`
-        - 0.8.7: add api: `zq_tracing.enable_trace`, `zq_tracing.disable_trace`
-        - 0.8.6: add api: `zq_tracing.record_init`, `zq_tracing.record_append`
-        - 0.8.5: add api: `zq_tracing.set_start_timestamp`
-        - 0.8.4: fix bug, add `colorful` to dependency
-        - 0.8.3: add `zq_files`
-        - 0.8.2: support `from zq_tools.zq_logger import default_logger as logger`
-        - 0.8.0: use `add_log_file` to add a log file to the logger.
-        - 0.7.0: re-think the color print logic
-        - 0.6.0: rename function: logger.print* --> logger.prank*
-        - 0.5.9: set level of print bewteen DEBUG and INFO, add `*_root` functions
-        - 0.5.8: implement `__len__` and `__iter__` for zq_cycle
-        - 0.5.6: add colors for different rank. add filter for zq_logger
-        - 0.5.5: disable color by default for `print` and `print_all`
-        - 0.5.3: zq_logger supports `print`, `print_all`, `set_rank`
-        - 0.5.1: move tag to ahead of msg
-        - 0.5.0: zq_logger supports color API, add tag
-        - 0.4.1: fix bug of zq_cycle
-        - 0.4.0: add zq_cycle
-        - 0.3.6: default unit of timestamp: us
-        - 0.3.5: support manually specifiying tid/pid when calling `zq_tracing.record_*`
-        - 0.3.4: fix bug
-        - 0.3.3: add default logger, call `zq_logger.get_logger()`, return a pre-defined logger
-        - 0.3.2: add async record, support nested and ordered tracing events
-        - 0.3.1: add install dependencies
-        - 0.3.0: output `pathname` instead of `filename`, better support for IDE's jumping function
-        
-        
-        # TODO:
-        - add setLogPath()
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+
+# zq_logger
+generates a logger, preformatted with the file name, line number information, differrent levels of color, and can be output in the console and written to a file at the same time.
+
+![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220701162735.png)
+
+If you use vscode to view the output log in the editor, `ANSI Colors` extension is recommended to install.
+
+# zq_tracing
+help generate json file used in `chrome://tracing`
+
+![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
+
+
+# Release Notes
+- 1.0.0: make `zq_logger` support print to screen and file with different levels
+- 0.9.9: add `__repr__` for zq_cycle
+- 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
+- 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
+- 0.9.6: increase version due to keep failing on uploading
+- 0.9.4: fix bug: `zq_decorator.time_it(sync)`
+- 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
+- 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
+- 0.9.1: use `default_logger` instead of `print`
+- 0.9.0: add decorator and manager: `zq_decorator.timeit`
+- 0.8.8: add decorator: `zq_decorator.do_nothing`
+- 0.8.7: add api: `zq_tracing.enable_trace`, `zq_tracing.disable_trace`
+- 0.8.6: add api: `zq_tracing.record_init`, `zq_tracing.record_append`
+- 0.8.5: add api: `zq_tracing.set_start_timestamp`
+- 0.8.4: fix bug, add `colorful` to dependency
+- 0.8.3: add `zq_files`
+- 0.8.2: support `from zq_tools.zq_logger import default_logger as logger`
+- 0.8.0: use `add_log_file` to add a log file to the logger.
+- 0.7.0: re-think the color print logic
+- 0.6.0: rename function: logger.print* --> logger.prank*
+- 0.5.9: set level of print bewteen DEBUG and INFO, add `*_root` functions
+- 0.5.8: implement `__len__` and `__iter__` for zq_cycle
+- 0.5.6: add colors for different rank. add filter for zq_logger
+- 0.5.5: disable color by default for `print` and `print_all`
+- 0.5.3: zq_logger supports `print`, `print_all`, `set_rank`
+- 0.5.1: move tag to ahead of msg
+- 0.5.0: zq_logger supports color API, add tag
+- 0.4.1: fix bug of zq_cycle
+- 0.4.0: add zq_cycle
+- 0.3.6: default unit of timestamp: us
+- 0.3.5: support manually specifiying tid/pid when calling `zq_tracing.record_*`
+- 0.3.4: fix bug
+- 0.3.3: add default logger, call `zq_logger.get_logger()`, return a pre-defined logger
+- 0.3.2: add async record, support nested and ordered tracing events
+- 0.3.1: add install dependencies
+- 0.3.0: output `pathname` instead of `filename`, better support for IDE's jumping function
+
+
+# TODO:
+- add setLogPath()
```

