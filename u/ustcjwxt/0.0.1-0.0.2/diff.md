# Comparing `tmp/ustcjwxt-0.0.1.tar.gz` & `tmp/ustcjwxt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ustcjwxt-0.0.1.tar", last modified: Wed Jul 19 06:38:41 2023, max compression
+gzip compressed data, was "ustcjwxt-0.0.2.tar", last modified: Thu Jul 20 09:16:06 2023, max compression
```

## Comparing `ustcjwxt-0.0.1.tar` & `ustcjwxt-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:38:41.802032 ustcjwxt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-19 06:38:41.798032 ustcjwxt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:38:41.802032 ustcjwxt-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:38:41.798032 ustcjwxt-0.0.1/ustcjwxt/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/ustcjwxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/ustcjwxt/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/ustcjwxt/request_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/ustcjwxt/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-19 06:38:27.000000 ustcjwxt-0.0.1/ustcjwxt/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:38:41.798032 ustcjwxt-0.0.1/ustcjwxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-19 06:38:41.000000 ustcjwxt-0.0.1/ustcjwxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-19 06:38:41.000000 ustcjwxt-0.0.1/ustcjwxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:38:41.000000 ustcjwxt-0.0.1/ustcjwxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 06:38:41.000000 ustcjwxt-0.0.1/ustcjwxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 06:38:41.000000 ustcjwxt-0.0.1/ustcjwxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:16:06.039921 ustcjwxt-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 09:16:06.039921 ustcjwxt-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:16:06.039921 ustcjwxt-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:16:06.039921 ustcjwxt-0.0.2/ustcjwxt/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/course_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/request_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-20 09:15:54.000000 ustcjwxt-0.0.2/ustcjwxt/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:16:06.039921 ustcjwxt-0.0.2/ustcjwxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 09:16:06.000000 ustcjwxt-0.0.2/ustcjwxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 09:16:06.000000 ustcjwxt-0.0.2/ustcjwxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:16:06.000000 ustcjwxt-0.0.2/ustcjwxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 09:16:06.000000 ustcjwxt-0.0.2/ustcjwxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 09:16:06.000000 ustcjwxt-0.0.2/ustcjwxt.egg-info/top_level.txt
```

### Comparing `ustcjwxt-0.0.1/LICENSE` & `ustcjwxt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ustcjwxt-0.0.1/setup.py` & `ustcjwxt-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ustcjwxt",
-    version="v0.0.1",
+    version="v0.0.2",
     author="brealid",
     author_email="brealid@mail.ustc.edu.cn",
     description="ustc jwxt api, for study only",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/brealid/ustcjwxt-python-lib",
     classifiers=[
```

### Comparing `ustcjwxt-0.0.1/ustcjwxt/log.py` & `ustcjwxt-0.0.2/ustcjwxt/log.py`

 * *Files identical despite different names*

### Comparing `ustcjwxt-0.0.1/ustcjwxt/request_info.py` & `ustcjwxt-0.0.2/ustcjwxt/request_info.py`

 * *Files identical despite different names*

### Comparing `ustcjwxt-0.0.1/ustcjwxt/score.py` & `ustcjwxt-0.0.2/ustcjwxt/score.py`

 * *Files identical despite different names*

### Comparing `ustcjwxt-0.0.1/ustcjwxt/session.py` & `ustcjwxt-0.0.2/ustcjwxt/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ustcjwxt import log, request_info
 
 
 class StudentSession:
     def __init__(self, username=None, password=None, session=None):
         self.request_session = requests.Session()
         self.password_useable = False
+        self.cache = dict()
         for key in request_info.base_cookie:
             self.request_session.cookies.set(key, request_info.base_cookie[key])
         # login with session
         if session is not None:
             self.login_with_session(session)
         # login with username and password
         if username is not None and password is not None:
@@ -23,46 +24,50 @@
 
     def get(self, url, params=None, data=None, headers=request_info.header_uaonly, **kwargs) -> requests.Response:
         response = self.request_session.get(url, headers=headers, params=params, data=data, **kwargs)
         if response.url.startswith('https://jw.ustc.edu.cn/login'):
             log.log_warning(f'get {url} redirect to {response.url}')
             if self.password_useable:
                 log.log_warning('session 无效, 正在尝试重新用密码登录')
-                self.clear_cookie()
+                self.clear_cache()
                 if self.login_with_password(self.username, self.password):
                     response = self.request_session.get(url, headers=headers, params=params, data=data, **kwargs)
                 else:
                     log.log_error('密码登录失败')
             else:
                 log.log_error('session 无效')
-                self.clear_cookie()
+                self.clear_cache()
         return response
    
-    def post(self, url, data=None, params=None, headers=request_info.header_uaonly, **kwargs) -> requests.Response:
+    def post(self, url, data=None, params=None, headers=request_info.header_uaonly, content_type = '', **kwargs) -> requests.Response:
+        if content_type:
+            headers['content-type'] = content_type + '; charset=UTF-8'
         response = self.request_session.post(url, headers=headers, params=params, data=data, **kwargs)
         if response.url.startswith('https://jw.ustc.edu.cn/login'):
             log.log_warning(f'post {url} redirect to {response.url}')
             if self.password_useable:
                 log.log_warning('session 无效, 正在尝试重新用密码登录')
-                self.clear_cookie()
+                self.clear_cache()
                 if self.login_with_password(self.username, self.password):
                     response = self.request_session.post(url, headers=headers, params=params, data=data, **kwargs)
                 else:
                     log.log_error('密码登录失败')
             else:
                 log.log_error('session 无效')
-                self.clear_cookie()
+                self.clear_cache()
         return response
 
-    def clear_cookie(self) -> None:
+    def clear_cache(self) -> None:
         self.request_session.cookies.clear()
         for key in request_info.base_cookie:
             self.request_session.cookies.set(key, request_info.base_cookie[key])
+        self.cache = dict()
 
     def login_with_password(self, username: str, password: str) -> bool:
+        self.clear_cache()
         self.username = username
         self.password = password
 
         loginParams = {
             'service': 'https://jw.ustc.edu.cn/ucas-sso/login',
         }
         response = self.get('https://passport.ustc.edu.cn/login', params=loginParams)
@@ -80,42 +85,58 @@
         log.log_debug(f'login response status code {response.status_code}')
         if response.url == 'https://jw.ustc.edu.cn/home' and self.check_cookie_useable():
             self.password_useable = True
             return True
         else:
             log.log_error('username 和 password 无效, 登陆失败')
             self.password_useable = False
-            self.clear_cookie()
+            self.clear_cache()
             return False
 
     def login_with_session(self, session: str) -> bool:
+        self.clear_cache()
         self.request_session.cookies['SESSION'] = session
         if not self.check_cookie_useable():
             log.log_error('session 无效')
-            self.clear_cookie()
+            self.clear_cache()
             return False
         return True
         
     def check_cookie_useable(self) -> bool:
         response = self.get('https://jw.ustc.edu.cn/my/profile')
         if response.url.startswith('https://jw.ustc.edu.cn/login'):
             return False
         return True
     
-    # return binary data with jpg format
-    def get_student_avator(self) -> bytes:
+    # return binary data with jpg format(will not cache avatar)
+    def get_student_avatar(self) -> bytes:
         response = self.get('https://jw.ustc.edu.cn/my/avatar')
         return response.content
 
-    def get_student_info(self) -> dict:
+    def get_student_info(self, force_retrieve = False) -> dict:
+        if not force_retrieve and 'profile_info' in self.cache:
+            return self.cache['profile_info']
         response = self.get('https://jw.ustc.edu.cn/my/profile')
         stuinfo_list = ['名称', '性别', '证件类型', '证件号', '生日', '政治面貌', '邮箱', '电话', '手机', '地址', '邮编', '简介']
         stuinfo = {}
         for dtype in stuinfo_list:
             specify = f'<span class="pull-left"><strong>{dtype}</strong></span>'
             p = response.text.find(specify)
             if p == -1:
                 log.log_warning(f'get_student_info: {dtype} not found')
                 continue
             data = response.text[p+len(specify):].split('</span>')[0].split('<span>')[-1]
             stuinfo[dtype] = data
+        self.cache['profile_info'] = stuinfo
         return stuinfo
+    
+    def get_student_assocID(self, force_retrieve = False) -> int:
+        if not force_retrieve and 'assocID' in self.cache:
+            return self.cache['assocID']
+        response = self.get('https://jw.ustc.edu.cn/for-std/course-select')
+        if response.url.startswith('https://jw.ustc.edu.cn/for-std/course-select/turns/'):
+            assocID = int(response.url.split('/')[-1])
+            log.log_info(f'学生唯一 assocID 获取成功: {assocID}')
+            self.cache['assocID'] = assocID
+            return assocID
+        log.log_error(f'学生唯一 assocID 获取失败')
+        return -1
```

