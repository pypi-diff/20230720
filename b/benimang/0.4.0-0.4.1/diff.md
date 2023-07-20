# Comparing `tmp/benimang-0.4.0.tar.gz` & `tmp/benimang-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.0.tar", last modified: Thu Jul 20 07:15:06 2023, max compression
+gzip compressed data, was "benimang-0.4.1.tar", last modified: Thu Jul 20 10:06:22 2023, max compression
```

## Comparing `benimang-0.4.0.tar` & `benimang-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 07:15:06.759571 benimang-0.4.0/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-20 07:15:06.758570 benimang-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 07:15:06.752568 benimang-0.4.0/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.0/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.0/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.0/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.0/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.0/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.0/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.0/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.0/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.0/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/btable.py
--rw-rw-rw-   0        0        0     4890 2023-07-20 03:23:06.000000 benimang-0.4.0/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.0/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.0/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.0/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:15:06.756570 benimang-0.4.0/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-20 07:15:06.000000 benimang-0.4.0/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-20 07:15:06.000000 benimang-0.4.0/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 07:15:06.000000 benimang-0.4.0/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-20 07:15:06.000000 benimang-0.4.0/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-20 07:03:03.000000 benimang-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 07:15:06.759571 benimang-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 07:15:06.757569 benimang-0.4.0/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.0/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.879927 benimang-0.4.1/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-20 10:06:22.879927 benimang-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.873926 benimang-0.4.1/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.1/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.1/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.1/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.1/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.1/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.1/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.1/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/btable.py
+-rw-rw-rw-   0        0        0     4819 2023-07-20 09:58:58.000000 benimang-0.4.1/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.1/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.876926 benimang-0.4.1/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-20 10:05:44.000000 benimang-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 10:06:22.879927 benimang-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.877926 benimang-0.4.1/test/
+-rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.1/test/test_sample.py
```

### Comparing `benimang-0.4.0/beni/bbyte.py` & `benimang-0.4.1/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bcache.py` & `benimang-0.4.1/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bcolor.py` & `benimang-0.4.1/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bexecute.py` & `benimang-0.4.1/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bfile.py` & `benimang-0.4.1/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bfunc.py` & `benimang-0.4.1/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bhttp.py` & `benimang-0.4.1/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/binput.py` & `benimang-0.4.1/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/block.py` & `benimang-0.4.1/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/blog.py` & `benimang-0.4.1/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bpath.py` & `benimang-0.4.1/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bplaywright.py` & `benimang-0.4.1/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bprogress.py` & `benimang-0.4.1/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bqiniu.py` & `benimang-0.4.1/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bsqlite.py` & `benimang-0.4.1/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bstorage.py` & `benimang-0.4.1/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/btable.py` & `benimang-0.4.1/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/btask.py` & `benimang-0.4.1/beni/btask.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import inspect
 import sys
 from contextlib import asynccontextmanager
 from datetime import datetime as Datetime
 from pathlib import Path
 
 import nest_asyncio
-from colorama import Back, Fore
+from colorama import Fore
 from typer import Typer
 
 from beni import bcolor, bfunc, block, blog, bpath, btime
 from beni.btype import Null
 
-_APP = Typer()
+app = Typer()
 _LOGFILE_COUNT = 100
 _TASKS = 'tasks'
 
 nest_asyncio.apply()
 
 _key: str = 'btask'
 _logDir: Path = Null
@@ -48,16 +48,16 @@
                 files = filter(lambda x: not x.name.startswith('_'), files)
                 for moduleName in [x.stem for x in files]:
                     exec(f'import {_TASKS}.{moduleName}')
                     module = eval(f'{_TASKS}.{moduleName}')
                     if hasattr(module, 'app'):
                         sub: Typer = getattr(module, 'app')
                         sub.info.name = moduleName.replace('_', '-')
-                        _APP.add_typer(sub, name=sub.info.name)
-                _APP()
+                        app.add_typer(sub, name=sub.info.name)
+                app()
             except BaseException as ex:
                 if type(ex) is SystemExit and ex.code in (0, 2):
                     # 0 - 正常结束
                     # 2 - Error: Missing command.
                     pass
                 else:
                     raise
@@ -97,36 +97,36 @@
             blog.error('执行失败')
             raise
         finally:
             criticalNum = blog.getCountCritical()
             errorNum = blog.getCountError()
             warningNum = blog.getCountWarning()
             if criticalNum:
-                color = Fore.LIGHTWHITE_EX + Back.LIGHTMAGENTA_EX
+                color = Fore.LIGHTMAGENTA_EX
             elif errorNum:
-                color = Fore.LIGHTWHITE_EX + Back.LIGHTRED_EX
+                color = Fore.LIGHTRED_EX
             elif warningNum:
-                color = Fore.BLACK + Back.YELLOW
+                color = Fore.YELLOW
             else:
-                color = Fore.BLACK + Back.LIGHTGREEN_EX
+                color = Fore.LIGHTGREEN_EX
             bcolor.set(color)
             blog.info('-' * 75)
             msgAry = ['任务结束']
             if criticalNum:
                 msgAry.append(f'critical({criticalNum})')
             if errorNum:
                 msgAry.append(f'error({errorNum})')
             if warningNum:
                 msgAry.append(f'warning({warningNum})')
-            bcolor.set(color)
-            blog.info(' '.join(msgAry))
             duration = str(Datetime.now() - start_time)
             if duration.startswith('0:'):
                 duration = '0' + duration
-            blog.info(f'用时: {duration}')
+            msgAry.append(f'\n用时: {duration}')
+            bcolor.set(color)
+            blog.info(' '.join(msgAry))
 
             # 删除多余的日志
             try:
                 if logFile:
                     logFileAry = list(logFile.parent.glob('*.log'))
                     logFileAry.remove(logFile)
                     logFileAry.sort()
```

### Comparing `benimang-0.4.0/beni/btime.py` & `benimang-0.4.1/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/beni/bzip.py` & `benimang-0.4.1/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/benimang.egg-info/SOURCES.txt` & `benimang-0.4.1/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.4.0/test/test_sample.py` & `benimang-0.4.1/test/test_sample.py`

 * *Files identical despite different names*

