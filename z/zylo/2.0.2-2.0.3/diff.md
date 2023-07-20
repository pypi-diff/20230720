# Comparing `tmp/zylo-2.0.2.tar.gz` & `tmp/zylo-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-2.0.2.tar", last modified: Mon Jul 17 17:37:58 2023, max compression
+gzip compressed data, was "zylo-2.0.3.tar", last modified: Thu Jul 20 08:03:48 2023, max compression
```

## Comparing `zylo-2.0.2.tar` & `zylo-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:37:58.790048 zylo-2.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-07-17 17:30:54.000000 zylo-2.0.2/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-17 17:37:58.790048 zylo-2.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-17 17:30:44.000000 zylo-2.0.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-17 17:19:23.000000 zylo-2.0.2/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.2/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-07-17 17:37:28.000000 zylo-2.0.2/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-17 17:30:16.000000 zylo-2.0.2/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.2/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.2/zylo/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-2.0.2/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.2/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5184 2023-07-20 08:03:48.200309 zylo-2.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4558 2023-07-20 07:54:02.000000 zylo-2.0.3/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-20 08:03:48.200309 zylo-2.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-20 07:53:01.000000 zylo-2.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-17 17:19:23.000000 zylo-2.0.3/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.3/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2023-07-20 07:51:03.000000 zylo-2.0.3/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-17 17:30:16.000000 zylo-2.0.3/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.3/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.3/zylo/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3003 2023-07-20 07:52:15.000000 zylo-2.0.3/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.3/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 08:03:48.200309 zylo-2.0.3/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5184 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-20 08:03:47.000000 zylo-2.0.3/zylo.egg-info/top_level.txt
```

### Comparing `zylo-2.0.2/PKG-INFO` & `zylo-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.2
+Version: 2.0.3
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,21 +51,21 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.2
-- Last update of beta
-- Bug fixed with update --> 2.0.2
-- Improved session management & Security
+- Beta version 2.0.3
+- Latest update of beta
+- Bug fixed with update --> 2.0.3
 - Updated Usage Guide 1.2.1
-- Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
+- Bug fixes in Zylo
+- Mailer updated to --> 1.0.3
 
 ```python
 
 from zylo.limiter import Limiter, render_template
 
 app = Zylo(__name__)
 limiter = Limiter(app)
```

### Comparing `zylo-2.0.2/README.md` & `zylo-2.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.2
-- Last update of beta
-- Bug fixed with update --> 2.0.2
-- Improved session management & Security
+- Beta version 2.0.3
+- Latest update of beta
+- Bug fixed with update --> 2.0.3
 - Updated Usage Guide 1.2.1
-- Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
+- Bug fixes in Zylo
+- Mailer updated to --> 1.0.3
 
 ```python
 
 from zylo.limiter import Limiter, render_template
 
 app = Zylo(__name__)
 limiter = Limiter(app)
```

### Comparing `zylo-2.0.2/setup.py` & `zylo-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='2.0.2',
+    version='2.0.3',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
```

### Comparing `zylo-2.0.2/zylo/JwT.py` & `zylo-2.0.3/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.2/zylo/app.py` & `zylo-2.0.3/zylo/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,20 +96,25 @@
     def wsgi_app(self, environ, start_response):
         request = Request(environ)
         for blueprint in self.blueprints:
             if request.path.startswith(blueprint.url_prefix):
                 request.blueprint = blueprint
                 response = blueprint.wsgi_app(environ, start_response)
                 return response
+
         session_id = request.cookies.get('session_id')
         session_data = session_manager.load_session(session_id)
         request.session = session_data
         response = self.handle_request(request)
         session_id = session_manager.save_session(request.session)
-        response.set_cookie('session_id', session_id, secure=True, httponly=True)
+
+        # Make sure response is a valid Response object before setting the cookie
+        if isinstance(response, Response):
+            response.set_cookie('session_id', session_id, secure=True, httponly=True)
+
         return response(environ, start_response)
 
     def __call__(self, environ, start_response):
         app = self.wsgi_app
         for middleware in reversed(self.middlewares):
             app = middleware(app)
         return app(environ, start_response)
```

### Comparing `zylo-2.0.2/zylo/blueprint.py` & `zylo-2.0.3/zylo/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.2/zylo/chiper.py` & `zylo-2.0.3/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.2/zylo/limiter.py` & `zylo-2.0.3/zylo/limiter.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.2/zylo/mailer.py` & `zylo-2.0.3/zylo/mailer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
+from .app import Response
 
 class Mailer:
     def __init__(self):
         self.config = {
             'SMTP': '',
             'SMTP_PORT': 587,
             'SENDER_EMAIL': '',
@@ -35,17 +36,20 @@
             message['Cc'] = cc
             recipient = [recipient] + cc.split(',')
 
         if bcc:
             message['Bcc'] = bcc
             recipient = recipient + bcc.split(',')
 
+        if isinstance(body, Response):
+            body = body.response[0]
+
         if body:
-            body_type = 'html' if '<' in body and '>' in body else 'plain'
-            message.attach(MIMEText(body, body_type))
+            body_type = 'html' if body and any(char in body.decode('utf-8') for char in ['<', '>']) else 'plain'
+            message.attach(MIMEText(body.decode('utf-8'), body_type))
 
         if attachments:
             for attachment in attachments:
                 try:
                     with open(attachment, 'rb') as file:
                         attachment_part = MIMEText(file.read(), 'plain')
                         attachment_part.add_header('Content-Disposition', 'attachment', filename=attachment)
```

### Comparing `zylo-2.0.2/zylo/sessions.py` & `zylo-2.0.3/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.2/zylo.egg-info/PKG-INFO` & `zylo-2.0.3/zylo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.2
+Version: 2.0.3
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,21 +51,21 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.2
-- Last update of beta
-- Bug fixed with update --> 2.0.2
-- Improved session management & Security
+- Beta version 2.0.3
+- Latest update of beta
+- Bug fixed with update --> 2.0.3
 - Updated Usage Guide 1.2.1
-- Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
+- Bug fixes in Zylo
+- Mailer updated to --> 1.0.3
 
 ```python
 
 from zylo.limiter import Limiter, render_template
 
 app = Zylo(__name__)
 limiter = Limiter(app)
```

