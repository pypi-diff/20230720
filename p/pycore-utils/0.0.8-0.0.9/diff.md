# Comparing `tmp/pycore-utils-0.0.8.tar.gz` & `tmp/pycore-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycore-utils-0.0.8.tar", last modified: Fri Nov 15 02:46:28 2019, max compression
+gzip compressed data, was "dist\pycore-utils-0.0.9.tar", last modified: Fri Nov 15 02:51:36 2019, max compression
```

## Comparing `pycore-utils-0.0.8.tar` & `pycore-utils-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/
--rw-rw-rw-   0        0        0      213 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/data/
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/data/database/
--rw-rw-rw-   0        0        0      545 2019-11-12 06:32:08.000000 pycore-utils-0.0.8/pycore/data/database/mysql_connection.py
--rw-rw-rw-   0        0        0        0 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/data/database/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/data/entity/
--rw-rw-rw-   0        0        0      175 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/data/entity/config.py
--rw-rw-rw-   0        0        0      403 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/data/entity/globalvar.py
--rw-rw-rw-   0        0        0        0 2019-11-12 05:32:42.000000 pycore-utils-0.0.8/pycore/data/entity/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-12 05:31:42.000000 pycore-utils-0.0.8/pycore/data/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/http/
--rw-rw-rw-   0        0        0       70 2019-11-14 09:38:26.000000 pycore-utils-0.0.8/pycore/http/ErrorCode.py
--rw-rw-rw-   0        0        0     2791 2019-11-15 02:46:22.000000 pycore-utils-0.0.8/pycore/http/handle.py
--rw-rw-rw-   0        0        0     1633 2019-11-15 02:34:42.000000 pycore-utils-0.0.8/pycore/http/http_server.py
--rw-rw-rw-   0        0        0        0 2019-11-12 06:27:45.000000 pycore-utils-0.0.8/pycore/http/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore/utils/
--rw-rw-rw-   0        0        0     1253 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/utils/http_utils.py
--rw-rw-rw-   0        0        0     2377 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/utils/logger_utils.py
--rw-rw-rw-   0        0        0     3157 2019-11-12 05:36:11.000000 pycore-utils-0.0.8/pycore/utils/multi_queue.py
--rw-rw-rw-   0        0        0     3970 2019-11-12 06:32:08.000000 pycore-utils-0.0.8/pycore/utils/redis_utils.py
--rw-rw-rw-   0        0        0      963 2019-11-14 09:22:19.000000 pycore-utils-0.0.8/pycore/utils/stringutils.py
--rw-rw-rw-   0        0        0     2233 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/utils/tcp_count.py
--rw-rw-rw-   0        0        0        0 2019-11-12 03:45:07.000000 pycore-utils-0.0.8/pycore/utils/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-12 05:30:36.000000 pycore-utils-0.0.8/pycore/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore_utils.egg-info/
--rw-rw-rw-   0        0        0        1 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      660 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/pycore_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2019-11-12 05:38:20.000000 pycore-utils-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2019-11-15 02:46:28.000000 pycore-utils-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      273 2019-11-15 02:46:22.000000 pycore-utils-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/
+-rw-rw-rw-   0        0        0      213 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/data/
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/data/database/
+-rw-rw-rw-   0        0        0      545 2019-11-12 06:32:08.000000 pycore-utils-0.0.9/pycore/data/database/mysql_connection.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/data/database/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/data/entity/
+-rw-rw-rw-   0        0        0      175 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/data/entity/config.py
+-rw-rw-rw-   0        0        0      403 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/data/entity/globalvar.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 05:32:42.000000 pycore-utils-0.0.9/pycore/data/entity/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 05:31:42.000000 pycore-utils-0.0.9/pycore/data/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/http/
+-rw-rw-rw-   0        0        0       70 2019-11-14 09:38:26.000000 pycore-utils-0.0.9/pycore/http/ErrorCode.py
+-rw-rw-rw-   0        0        0     2789 2019-11-15 02:51:05.000000 pycore-utils-0.0.9/pycore/http/handle.py
+-rw-rw-rw-   0        0        0     1633 2019-11-15 02:34:42.000000 pycore-utils-0.0.9/pycore/http/http_server.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 06:27:45.000000 pycore-utils-0.0.9/pycore/http/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore/utils/
+-rw-rw-rw-   0        0        0     1253 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/utils/http_utils.py
+-rw-rw-rw-   0        0        0     2377 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/utils/logger_utils.py
+-rw-rw-rw-   0        0        0     3157 2019-11-12 05:36:11.000000 pycore-utils-0.0.9/pycore/utils/multi_queue.py
+-rw-rw-rw-   0        0        0     3970 2019-11-12 06:32:08.000000 pycore-utils-0.0.9/pycore/utils/redis_utils.py
+-rw-rw-rw-   0        0        0      963 2019-11-14 09:22:19.000000 pycore-utils-0.0.9/pycore/utils/stringutils.py
+-rw-rw-rw-   0        0        0     2233 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/utils/tcp_count.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 03:45:07.000000 pycore-utils-0.0.9/pycore/utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-12 05:30:36.000000 pycore-utils-0.0.9/pycore/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/pycore_utils.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-11-15 02:51:35.000000 pycore-utils-0.0.9/pycore_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2019-11-15 02:51:35.000000 pycore-utils-0.0.9/pycore_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2019-11-15 02:51:35.000000 pycore-utils-0.0.9/pycore_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2019-11-15 02:51:35.000000 pycore-utils-0.0.9/pycore_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        8 2019-11-12 05:38:20.000000 pycore-utils-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2019-11-15 02:51:36.000000 pycore-utils-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      273 2019-11-15 02:51:05.000000 pycore-utils-0.0.9/setup.py
```

### Comparing `pycore-utils-0.0.8/pycore/data/database/mysql_connection.py` & `pycore-utils-0.0.9/pycore/data/database/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/http/handle.py` & `pycore-utils-0.0.9/pycore/http/handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.logger = LoggerUtils('access').logger
 
     def log_message(self, formatstr, *args):
         self.logger.info("%s:%d - - %s\n" % (self.addr[0], self.addr[1], formatstr % args))
 
     def passRequestLine(self, request_line):
         header_list = request_line.split(' ')
-        self.log_message(header_list)
+        self.log_message(request_line)
         self.method = header_list[0].upper()
         self.url = header_list[1]
         self.protocol = header_list[2]
 
     def passRequestHead(self, request_head):
         head_options = request_head.split('\r\n')
         for option in head_options:
@@ -43,34 +43,34 @@
         request_head = body.split('\r\n\r\n', 1)[0]  # 头部信息
         self.passRequestLine(request_line)
         self.passRequestHead(request_head)
 
         if self.method == 'POST':
             self.request_data = {}
             request_body = body.split('\r\n\r\n', 1)[1]
-            self.log_message("param:%s" % str(request_body))
+            self.log_message("param:%s", str(request_body))
             parameters = request_body.split('&')  # 每一行是一个字段
             for i in parameters:
                 if i == '':
                     continue
                 key, val = i.split('=', 1)
                 self.request_data[key] = val
         if self.method == 'GET':
             if self.url.find('?') != -1:  # 含有参数的get
                 self.request_data = {}
                 req = self.url.split('?', 1)[1]
                 s_url = self.url.split('?', 1)[0]
-                self.log_message("param:%s" % str(req))
+                self.log_message("param:%s", str(req))
                 parameters = req.split('&')
                 for i in parameters:
                     key, val = i.split('=', 1)
                     self.request_data[key] = val
                 self.url = s_url
         self.do()
 
     def do(self):
         pass
 
     def getResponse(self):
         response = self.response_line + StringUtils.dict2str(self.response_head) + '\r\n' + self.response_body
-        self.log_message("return:%s" % str(response))
+        self.log_message("return:%s", str(response))
         return response
```

### Comparing `pycore-utils-0.0.8/pycore/http/http_server.py` & `pycore-utils-0.0.9/pycore/http/http_server.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/http_utils.py` & `pycore-utils-0.0.9/pycore/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/logger_utils.py` & `pycore-utils-0.0.9/pycore/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/multi_queue.py` & `pycore-utils-0.0.9/pycore/utils/multi_queue.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/redis_utils.py` & `pycore-utils-0.0.9/pycore/utils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/stringutils.py` & `pycore-utils-0.0.9/pycore/utils/stringutils.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore/utils/tcp_count.py` & `pycore-utils-0.0.9/pycore/utils/tcp_count.py`

 * *Files identical despite different names*

### Comparing `pycore-utils-0.0.8/pycore_utils.egg-info/SOURCES.txt` & `pycore-utils-0.0.9/pycore_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

