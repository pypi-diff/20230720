# Comparing `tmp/dingtalk-stream-0.7.2.tar.gz` & `tmp/dingtalk-stream-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.7.2.tar", last modified: Thu Jul 20 03:00:50 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.7.3.tar", last modified: Thu Jul 20 08:21:27 2023, max compression
```

## Comparing `dingtalk-stream-0.7.2.tar` & `dingtalk-stream-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:00:50.198818 dingtalk-stream-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 03:00:50.198818 dingtalk-stream-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:00:50.198818 dingtalk-stream-0.7.2/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:00:50.198818 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 03:00:50.000000 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 03:00:50.000000 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:00:50.000000 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 03:00:50.000000 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 03:00:50.000000 dingtalk-stream-0.7.2/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:00:50.198818 dingtalk-stream-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 03:00:49.000000 dingtalk-stream-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 08:21:27.000000 dingtalk-stream-0.7.3/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:21:27.139819 dingtalk-stream-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 08:21:26.000000 dingtalk-stream-0.7.3/setup.py
```

### Comparing `dingtalk-stream-0.7.2/LICENSE` & `dingtalk-stream-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/PKG-INFO` & `dingtalk-stream-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.2/README.md` & `dingtalk-stream-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/__init__.py` & `dingtalk-stream-0.7.3/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.7.3/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.7.3/dingtalk_stream/card_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,27 @@
         :param button_list:
         :param markdown:
         :return:
         """
         self.button_list = button_list
         self.card_instance_id = self.create_and_send_card(self.card_template_id, self._get_card_data(markdown, tips))
 
-    def update(self, markdown: str, tips: str = ""):
+    def update(self, markdown: str, button_list: list, tips: str = ""):
         """
         更新markdown内容，如果你reply了多次，这里只会更新最后一张卡片
+        :param button_list:
         :param tips:
         :param markdown:
         :return:
         """
         if self.card_instance_id is None or self.card_instance_id == "":
             self.logger.error('MarkdownButtonCardInstance.update failed, you should send card first.')
             return
 
+        self.button_list = button_list
         self.put_card_data(self.card_instance_id, self._get_card_data(markdown, tips))
 
 
 class AIMarkdownCardInstance(AICardReplier):
     """
     一款超级通用的AI Markdown卡片
     ai_start --> ai_streaming --> ai_streaming --> ai_finish/ai_fail
```

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.7.3/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.7.3/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/frames.py` & `dingtalk-stream-0.7.3/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/handlers.py` & `dingtalk-stream-0.7.3/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.7.3/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream/stream.py` & `dingtalk-stream-0.7.3/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.7.3/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.2/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.7.3/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.2/setup.py` & `dingtalk-stream-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.7.2',
+    version='0.7.3',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

