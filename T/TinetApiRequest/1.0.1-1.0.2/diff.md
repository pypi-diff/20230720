# Comparing `tmp/TinetApiRequest-1.0.1.tar.gz` & `tmp/TinetApiRequest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.1.tar", last modified: Thu Jul 20 09:28:09 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.2.tar", last modified: Thu Jul 20 11:57:31 2023, max compression
```

## Comparing `TinetApiRequest-1.0.1.tar` & `TinetApiRequest-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/
--rw-rw-rw-   0        0        0      272 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-20 09:28:05.000000 TinetApiRequest-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/tinet/
--rw-rw-rw-   0        0        0    22202 2023-07-20 09:27:19.000000 TinetApiRequest-1.0.1/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.1/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.1/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.1/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/
+-rw-rw-rw-   0        0        0      272 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-20 10:09:15.000000 TinetApiRequest-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/tinet/
+-rw-rw-rw-   0        0        0    22202 2023-07-20 11:43:44.000000 TinetApiRequest-1.0.2/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.2/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.2/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3401 2023-07-20 11:56:57.000000 TinetApiRequest-1.0.2/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.2/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.2/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.2/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.1/README.md` & `TinetApiRequest-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.1/setup.py` & `TinetApiRequest-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.1",
+    version="1.0.2",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.1/tinet/APIRequest.py` & `TinetApiRequest-1.0.2/tinet/APIRequest.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.1/tinet/ApiConfig.py` & `TinetApiRequest-1.0.2/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.1/tinet/LogUtil.py` & `TinetApiRequest-1.0.2/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.1/tinet/RequestUtil.py` & `TinetApiRequest-1.0.2/tinet/RequestUtil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import jsonpath
 import requests
-from requests import HTTPError
+from urllib.parse import urlparse
 
 
 class HttpClient:
     """
     对 requests 库进行简单封装的类，可以方便地进行 HTTP 请求和处理响应。
     """
 
@@ -23,14 +24,27 @@
         :param method: str 请求方法，例如 GET、POST、PUT 等。
         :param url: str 请求 URL，会和 base_url 拼接成完整的 URL。
         :param kwargs: dict 其他 requests.request 方法支持的参数。
         :return: requests.Response 响应对象。
         """
 
         response = self.session.request(method, url, **kwargs)
+        # 判断请求url 是否包含 openapi_login
+        if 'openapi_login' in url:
+            # 需要请求接口 获取 Tsessionid
+            # 先从url 中解析出请求域名
+            parsed_url = urlparse(url)
+            domain = parsed_url.scheme + '://' + parsed_url.netloc
+            # 进行接口请求 拿到响应
+            personalResponse = self.session.request(method='GET', url=domain + '/api/personal/info/get')
+            # 拿响应的$.result.authToken
+            authToken = jsonpath.jsonpath(personalResponse.json(), '$.result.authToken')[0]
+            # 后续的请求头上都需要带上 Tsessionid
+            self.session.headers.update({'Tsessionid': authToken})
+
 
         http_error_msg = None
         if 400 <= response.status_code < 500:
             http_error_msg = (
                 f"{response.status_code} 客户端错误 Error: {response.text} for url: {response.url}"
             )
 
@@ -59,8 +73,7 @@
         :param url: str 请求 URL，会和 base_url 拼接成完整的 URL。
         :param data: dict 请求体参数，以表单形式提交。
         :param json: dict 请求体参数，以 JSON 格式提交。
         :param kwargs: dict 其他 requests.post 方法支持的参数。
         :return: requests.Response 响应对象。
         """
         return self.request('POST', url, data=data, json=json, **kwargs)
-
```

### Comparing `TinetApiRequest-1.0.1/tinet/SignUtil.py` & `TinetApiRequest-1.0.2/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.1/tinet/YamlUtil.py` & `TinetApiRequest-1.0.2/tinet/YamlUtil.py`

 * *Files identical despite different names*

