# Comparing `tmp/auth_satvadev-1.0.2.tar.gz` & `tmp/auth_satvadev-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_satvadev-1.0.2.tar", max compression
+gzip compressed data, was "auth_satvadev-1.0.2a0.tar", max compression
```

## Comparing `auth_satvadev-1.0.2.tar` & `auth_satvadev-1.0.2a0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1052 2023-07-03 14:27:43.030928 auth_satvadev-1.0.2/LICENSE
--rw-r--r--   0        0        0     1323 2023-07-18 14:32:23.278884 auth_satvadev-1.0.2/README.md
--rw-r--r--   0        0        0     1029 2023-07-20 11:07:35.045262 auth_satvadev-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.030928 auth_satvadev-1.0.2/src/auth_satvadev/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2/src/auth_satvadev/api/__init__.py
--rw-r--r--   0        0        0      351 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2/src/auth_satvadev/api/exceptions.py
--rw-r--r--   0        0        0      812 2023-07-18 14:32:23.278884 auth_satvadev-1.0.2/src/auth_satvadev/api/serializers.py
--rw-r--r--   0        0        0      558 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2/src/auth_satvadev/api/urls.py
--rw-r--r--   0        0        0     2774 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2/src/auth_satvadev/api/views.py
--rw-r--r--   0        0        0      251 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2/src/auth_satvadev/apps.py
--rw-r--r--   0        0        0     1488 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2/src/auth_satvadev/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2/src/auth_satvadev/migrations/__init__.py
--rw-r--r--   0        0        0      546 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2/src/auth_satvadev/models.py
--rw-r--r--   0        0        0     3069 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2/src/auth_satvadev/senders.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 auth_satvadev-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-03 14:27:43.030928 auth_satvadev-1.0.2a0/LICENSE
+-rw-r--r--   0        0        0     1323 2023-07-18 14:32:23.278884 auth_satvadev-1.0.2a0/README.md
+-rw-r--r--   0        0        0     1133 2023-07-20 07:42:19.680925 auth_satvadev-1.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.030928 auth_satvadev-1.0.2a0/src/auth_satvadev/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2a0/src/auth_satvadev/api/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2a0/src/auth_satvadev/api/exceptions.py
+-rw-r--r--   0        0        0      812 2023-07-18 14:32:23.278884 auth_satvadev-1.0.2a0/src/auth_satvadev/api/serializers.py
+-rw-r--r--   0        0        0      558 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2a0/src/auth_satvadev/api/urls.py
+-rw-r--r--   0        0        0     2774 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2a0/src/auth_satvadev/api/views.py
+-rw-r--r--   0        0        0      251 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2a0/src/auth_satvadev/apps.py
+-rw-r--r--   0        0        0     1488 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2a0/src/auth_satvadev/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.2a0/src/auth_satvadev/migrations/__init__.py
+-rw-r--r--   0        0        0      546 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2a0/src/auth_satvadev/models.py
+-rw-r--r--   0        0        0     3069 2023-07-18 14:32:23.282884 auth_satvadev-1.0.2a0/src/auth_satvadev/senders.py
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 auth_satvadev-1.0.2a0/setup.py
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 auth_satvadev-1.0.2a0/PKG-INFO
```

### Comparing `auth_satvadev-1.0.2/LICENSE` & `auth_satvadev-1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/README.md` & `auth_satvadev-1.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/pyproject.toml` & `auth_satvadev-1.0.2a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 [tool.poetry]
 name = "auth_satvadev"
-version = "1.0.2"
+version = "1.0.2a"
 description = "Registration with confirmation by code and token authorization"
 authors = ["satva.dev <info@satva.dev>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[[tool.poetry.source]]
+name = "satvadev_pypi"
+url = "https://test.pypi.org/legacy/"
+default = false
+secondary = true
+
 [tool.poetry.urls]
 "Homepage" = "https://gitlab.com/satvaspace/_tools/python/auth_satvadev"
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
-Django = ">=3.2.12, <=4.*"
+Django = "^4.0.0"
 psycopg2 = "^2.9.3"
 celery = "^5.2.3"
 django-celery-beat = "^2.2.1"
 django-celery-results = "^2.2.0"
 uWSGI = "^2.0.20"
 djangorestframework-simplejwt = "^4.8.0"
 mail-satvadev = "^1.0.6"
@@ -27,15 +33,15 @@
 
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.2"
 pytest = "^7.0.1"
 pytest-xdist = "^2.5.0"
 pytest-django = "^4.5.2"
-pytest-cov = ">=3.*, <=4.*"
+pytest-cov = "^4.0.0"
 factory-boy = "^3.2.1"
 pytest-freezegun = "^0.4.2"
 ipython = "^8.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/api/serializers.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/api/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/api/urls.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/api/urls.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/api/views.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/api/views.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/migrations/0001_initial.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/models.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/models.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/src/auth_satvadev/senders.py` & `auth_satvadev-1.0.2a0/src/auth_satvadev/senders.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.2/PKG-INFO` & `auth_satvadev-1.0.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: auth-satvadev
-Version: 1.0.2
+Version: 1.0.2a0
 Summary: Registration with confirmation by code and token authorization
 Author: satva.dev
 Author-email: info@satva.dev
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=3.2.12,<=4)
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: Django (>=4.0.0,<5.0.0)
 Requires-Dist: celery (>=5.2.3,<6.0.0)
 Requires-Dist: django-celery-beat (>=2.2.1,<3.0.0)
 Requires-Dist: django-celery-results (>=2.2.0,<3.0.0)
 Requires-Dist: djangorestframework-simplejwt (>=4.8.0,<5.0.0)
 Requires-Dist: mail-satvadev (>=1.0.6,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.5.6,<2.0.0)
```

