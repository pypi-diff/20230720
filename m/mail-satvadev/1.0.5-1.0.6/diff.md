# Comparing `tmp/mail_satvadev-1.0.5.tar.gz` & `tmp/mail_satvadev-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail_satvadev-1.0.5.tar", max compression
+gzip compressed data, was "mail_satvadev-1.0.6.tar", max compression
```

## Comparing `mail_satvadev-1.0.5.tar` & `mail_satvadev-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.5/LICENSE
--rw-r--r--   0        0        0     5498 2023-07-10 09:48:13.141367 mail_satvadev-1.0.5/README.md
--rw-r--r--   0        0        0      718 2023-07-19 09:30:54.928830 mail_satvadev-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.5/src/mail_satvadev/__init__.py
--rw-r--r--   0        0        0      148 2023-07-10 09:48:13.141367 mail_satvadev-1.0.5/src/mail_satvadev/apps.py
--rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.5/src/mail_satvadev/filters.py
--rw-r--r--   0        0        0     2011 2023-07-10 09:48:13.145367 mail_satvadev-1.0.5/src/mail_satvadev/messages.py
--rw-r--r--   0        0        0      859 2023-07-10 09:48:13.145367 mail_satvadev-1.0.5/src/mail_satvadev/tasks.py
--rw-r--r--   0        0        0     6387 1970-01-01 00:00:00.000000 mail_satvadev-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5498 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6/README.md
+-rw-r--r--   0        0        0      732 2023-07-20 11:06:34.826085 mail_satvadev-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/src/mail_satvadev/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6/src/mail_satvadev/apps.py
+-rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/src/mail_satvadev/filters.py
+-rw-r--r--   0        0        0     2011 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6/src/mail_satvadev/messages.py
+-rw-r--r--   0        0        0      859 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6/src/mail_satvadev/tasks.py
+-rw-r--r--   0        0        0     6377 1970-01-01 00:00:00.000000 mail_satvadev-1.0.6/PKG-INFO
```

### Comparing `mail_satvadev-1.0.5/LICENSE` & `mail_satvadev-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.5/README.md` & `mail_satvadev-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.5/pyproject.toml` & `mail_satvadev-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "mail_satvadev"
-version = "1.0.5"
+version = "1.0.6"
 description = "Template for email"
 authors = ["satva.dev <info@satva.dev>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.urls]
 "Homepage" = "https://gitlab.com/satvaspace/_tools/python/mail_satvadev"
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
-django = "^3.2.12"
+django = ">=3.2.12, <=4.*"
 celery = "^5.2.3"
 pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
+pytest-cov = ">=3.*, <=4.*"
 pytest-django = "^4.5.2"
 django-celery-results = "^2.2.0"
 django-celery-beat = "^2.2.1"
 psycopg2 = "^2.9.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `mail_satvadev-1.0.5/src/mail_satvadev/filters.py` & `mail_satvadev-1.0.6/src/mail_satvadev/filters.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.5/src/mail_satvadev/messages.py` & `mail_satvadev-1.0.6/src/mail_satvadev/messages.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.5/src/mail_satvadev/tasks.py` & `mail_satvadev-1.0.6/src/mail_satvadev/tasks.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.5/PKG-INFO` & `mail_satvadev-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mail-satvadev
-Version: 1.0.5
+Version: 1.0.6
 Summary: Template for email
 Author: satva.dev
 Author-email: info@satva.dev
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.3,<6.0.0)
-Requires-Dist: django (>=3.2.12,<4.0.0)
+Requires-Dist: django (>=3.2.12,<=4)
 Requires-Dist: django-celery-beat (>=2.2.1,<3.0.0)
 Requires-Dist: django-celery-results (>=2.2.0,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: pytest (>=7.0.1,<8.0.0)
-Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
+Requires-Dist: pytest-cov (>=3,<=4)
 Requires-Dist: pytest-django (>=4.5.2,<5.0.0)
 Project-URL: Homepage, https://gitlab.com/satvaspace/_tools/python/mail_satvadev
 Description-Content-Type: text/markdown
 
 # Django приложение шаблона письма email с поддержкой отправки через Celery task
 
 ## Конфигурация
```

