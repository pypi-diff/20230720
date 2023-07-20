# Comparing `tmp/TinetApiRequest-1.0.0.tar.gz` & `tmp/TinetApiRequest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.0.tar", last modified: Tue Jul 18 08:05:28 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.1.tar", last modified: Thu Jul 20 09:28:09 2023, max compression
```

## Comparing `TinetApiRequest-1.0.0.tar` & `TinetApiRequest-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/
--rw-rw-rw-   0        0        0      272 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      653 2023-07-18 08:05:13.000000 TinetApiRequest-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:05:28.000000 TinetApiRequest-1.0.0/tinet/
--rw-rw-rw-   0        0        0    21950 2023-07-18 07:04:01.000000 TinetApiRequest-1.0.0/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.0/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.0/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.0/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.0/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.0/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.0/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/
+-rw-rw-rw-   0        0        0      272 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-20 09:28:05.000000 TinetApiRequest-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:28:09.000000 TinetApiRequest-1.0.1/tinet/
+-rw-rw-rw-   0        0        0    22202 2023-07-20 09:27:19.000000 TinetApiRequest-1.0.1/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.1/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.1/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.1/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.1/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.0/README.md` & `TinetApiRequest-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.0/setup.py` & `TinetApiRequest-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.0",
+    version="1.0.1",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
     license='MIT',
-)
+)
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

### Comparing `TinetApiRequest-1.0.0/tinet/APIRequest.py` & `TinetApiRequest-1.0.1/tinet/APIRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,19 @@
                 # 5. 处理断言
                 if testcase.get('assertFail'):
                     failtype = testcase.get('assertFail')
                 else:
                     failtype = self.assertFail
                 self.assertType(testcase.get('assert'), response, dataSaveBean, failtype)
                 # 6. 处理response,根据data 来进行变量存取
-                self.addAttrSaveBean(dataSaveBean, self.globalBean, testcase.get('saveData'), response.json())
+                # try 里面的代码是为了处理response不是json格式的情况
+                try:
+                    self.addAttrSaveBean(dataSaveBean, self.globalBean, testcase.get('saveData'), response.json())
+                except:
+                    self.addAttrSaveBean(dataSaveBean, self.globalBean, testcase.get('saveData'), response.text)
 
     # 处理断言方法  - eq: [ 'body.userId', 1 ]  通过testcase中的assert来判断断言方式  先取断言的方式 再取断言的内容跟值
     def assertType(self, assertType, response, bean, failType):
         log.info(f"开始处理断言: {assertType}")
         allure.attach(f"{assertType}", name=f"开始处理断言", attachment_type=allure.attachment_type.TEXT)
         # 判断assertType是否为空
         if assertType is None:
```

### Comparing `TinetApiRequest-1.0.0/tinet/ApiConfig.py` & `TinetApiRequest-1.0.1/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.0/tinet/LogUtil.py` & `TinetApiRequest-1.0.1/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.0/tinet/RequestUtil.py` & `TinetApiRequest-1.0.1/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.0/tinet/SignUtil.py` & `TinetApiRequest-1.0.1/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.0/tinet/YamlUtil.py` & `TinetApiRequest-1.0.1/tinet/YamlUtil.py`

 * *Files identical despite different names*

