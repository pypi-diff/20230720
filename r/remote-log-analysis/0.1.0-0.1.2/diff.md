# Comparing `tmp/remote_log_analysis-0.1.0.tar.gz` & `tmp/remote_log_analysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_log_analysis-0.1.0.tar", max compression
+gzip compressed data, was "remote_log_analysis-0.1.2.tar", max compression
```

## Comparing `remote_log_analysis-0.1.0.tar` & `remote_log_analysis-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-17 00:53:07.016209 remote_log_analysis-0.1.0/LICENSE
--rw-r--r--   0        0        0     1372 2023-07-17 00:53:07.128211 remote_log_analysis-0.1.0/README.md
--rw-r--r--   0        0        0      474 2023-07-19 12:53:48.286233 remote_log_analysis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      923 2023-07-20 02:12:49.923450 remote_log_analysis-0.1.0/remote_log_analysis/__init__.py
--rw-r--r--   0        0        0     2390 2023-07-17 00:53:07.132211 remote_log_analysis-0.1.0/remote_log_analysis/remote_executor_interface.py
--rw-r--r--   0        0        0     6640 2023-07-20 03:37:46.336264 remote_log_analysis-0.1.0/remote_log_analysis/remote_file_base.py
--rw-r--r--   0        0        0     6355 2023-07-17 00:53:07.116211 remote_log_analysis-0.1.0/remote_log_analysis/remote_linux_executor.py
--rw-r--r--   0        0        0     3708 2023-07-20 14:27:09.134131 remote_log_analysis-0.1.0/remote_log_analysis/remote_log_search.py
--rw-r--r--   0        0        0    11624 2023-07-20 03:02:39.187358 remote_log_analysis-0.1.0/remote_log_analysis/remote_log_utils.py
--rw-r--r--   0        0        0      394 2023-07-17 00:53:07.116211 remote_log_analysis-0.1.0/remote_log_analysis/remote_path_info.py
--rw-r--r--   0        0        0     3854 2023-07-20 03:38:16.344548 remote_log_analysis-0.1.0/remote_log_analysis/remote_text_log.py
--rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 remote_log_analysis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-17 00:53:07.016209 remote_log_analysis-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1372 2023-07-17 00:53:07.128211 remote_log_analysis-0.1.2/README.md
+-rw-r--r--   0        0        0      612 2023-07-20 16:51:23.932417 remote_log_analysis-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      923 2023-07-20 02:12:49.923450 remote_log_analysis-0.1.2/remote_log_analysis/__init__.py
+-rw-r--r--   0        0        0     2390 2023-07-17 00:53:07.132211 remote_log_analysis-0.1.2/remote_log_analysis/remote_executor_interface.py
+-rw-r--r--   0        0        0     6640 2023-07-20 03:37:46.336264 remote_log_analysis-0.1.2/remote_log_analysis/remote_file_base.py
+-rw-r--r--   0        0        0     6355 2023-07-17 00:53:07.116211 remote_log_analysis-0.1.2/remote_log_analysis/remote_linux_executor.py
+-rw-r--r--   0        0        0     3708 2023-07-20 14:27:09.134131 remote_log_analysis-0.1.2/remote_log_analysis/remote_log_search.py
+-rw-r--r--   0        0        0    11624 2023-07-20 03:02:39.187358 remote_log_analysis-0.1.2/remote_log_analysis/remote_log_utils.py
+-rw-r--r--   0        0        0      394 2023-07-17 00:53:07.116211 remote_log_analysis-0.1.2/remote_log_analysis/remote_path_info.py
+-rw-r--r--   0        0        0     3854 2023-07-20 03:38:16.344548 remote_log_analysis-0.1.2/remote_log_analysis/remote_text_log.py
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 remote_log_analysis-0.1.2/PKG-INFO
```

### Comparing `remote_log_analysis-0.1.0/LICENSE` & `remote_log_analysis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/README.md` & `remote_log_analysis-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/__init__.py` & `remote_log_analysis-0.1.2/remote_log_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_executor_interface.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_executor_interface.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_file_base.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_file_base.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_linux_executor.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_linux_executor.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_log_search.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_log_search.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_log_utils.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_log_utils.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/remote_log_analysis/remote_text_log.py` & `remote_log_analysis-0.1.2/remote_log_analysis/remote_text_log.py`

 * *Files identical despite different names*

### Comparing `remote_log_analysis-0.1.0/PKG-INFO` & `remote_log_analysis-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: remote-log-analysis
-Version: 0.1.0
+Version: 0.1.2
 Summary: Analyze log files on remote hosts locally
+Home-page: https://github.com/kubiyak/remote_log_analysis
+License: MIT
 Author: Kuberan Naganathan
 Author-email: python_cpp_developer@protonmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fabric (>=3.1.0,<4.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Project-URL: Repository, https://github.com/kubiyak/remote_log_analysis
 Description-Content-Type: text/markdown
 
 <H1> Remote Log Analysis </H1>
 <H2>Overview</H2>
 <p>
 A log file is a sequence of bytes where some immutability guarantee exists for
 already written data. New data can be appended to the end of a log file but bytes
```

