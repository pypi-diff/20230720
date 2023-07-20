# Comparing `tmp/social_auth_mitxpro-0.6.1.tar.gz` & `tmp/social_auth_mitxpro-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_auth_mitxpro-0.6.1.tar", max compression
+gzip compressed data, was "social_auth_mitxpro-0.6.2.tar", max compression
```

## Comparing `social_auth_mitxpro-0.6.1.tar` & `social_auth_mitxpro-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1530 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.1/LICENSE
--rw-r--r--   0        0        0     1622 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.1/README.md
--rw-r--r--   0        0        0     1099 2022-10-19 14:51:09.866215 social_auth_mitxpro-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.1/social_auth_mitxpro/__init__.py
--rw-r--r--   0        0        0     1843 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.1/social_auth_mitxpro/backends.py
--rw-r--r--   0        0        0     2359 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.1/social_auth_mitxpro/backends_test.py
--rw-r--r--   0        0        0      201 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.1/social_auth_mitxpro/conftest.py
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 social_auth_mitxpro-0.6.1/setup.py
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 social_auth_mitxpro-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1530 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1622 2021-09-28 18:12:18.635556 social_auth_mitxpro-0.6.2/README.md
+-rw-r--r--   0        0        0     1101 2023-07-20 15:48:52.788421 social_auth_mitxpro-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.2/social_auth_mitxpro/__init__.py
+-rw-r--r--   0        0        0     1843 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.2/social_auth_mitxpro/backends.py
+-rw-r--r--   0        0        0     2359 2021-09-28 20:27:44.529698 social_auth_mitxpro-0.6.2/social_auth_mitxpro/backends_test.py
+-rw-r--r--   0        0        0      201 2021-09-28 18:12:18.638889 social_auth_mitxpro-0.6.2/social_auth_mitxpro/conftest.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 social_auth_mitxpro-0.6.2/PKG-INFO
```

### Comparing `social_auth_mitxpro-0.6.1/LICENSE` & `social_auth_mitxpro-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `social_auth_mitxpro-0.6.1/README.md` & `social_auth_mitxpro-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `social_auth_mitxpro-0.6.1/pyproject.toml` & `social_auth_mitxpro-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "social-auth-mitxpro"
-version = "0.6.1"
+version = "0.6.2"
 description = "python-social-auth backend for mitxpro"
 
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://pypi.org/project/social-auth-mitxpro"
@@ -25,30 +25,30 @@
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 
 python = "~3.8 || ~3.9"
 social-auth-core = "^4.1.0"
-attrs = "22.1.0"
+attrs = "^22.2.0"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
-black = { version = "=22.10.0", python = "~3.8" }
-isort = "=5.10.1"
+black = { version = "=22.12.0", python = "~3.8" }
+isort = "=5.12.0"
 
 # Linters
-pylint = { version = "2.12.2", python = "~3.8" }
+pylint = { version = "2.17.4", python = "~3.8" }
 
 # Testing
-pytest = "6.1.2"
+pytest = "6.2.5"
 pytest-cov = "3.0.0"
-pytest-mock = "3.6.1"
-responses = "0.16.0"
+pytest-mock = "3.11.1"
+responses = "0.23.1"
 typing = { version = "^3.6.6", python = "~3.8" }
 codecov = "*"
 
 [build-system]
 
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `social_auth_mitxpro-0.6.1/social_auth_mitxpro/backends.py` & `social_auth_mitxpro-0.6.2/social_auth_mitxpro/backends.py`

 * *Files identical despite different names*

### Comparing `social_auth_mitxpro-0.6.1/social_auth_mitxpro/backends_test.py` & `social_auth_mitxpro-0.6.2/social_auth_mitxpro/backends_test.py`

 * *Files identical despite different names*

### Comparing `social_auth_mitxpro-0.6.1/PKG-INFO` & `social_auth_mitxpro-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: social-auth-mitxpro
-Version: 0.6.1
+Version: 0.6.2
 Summary: python-social-auth backend for mitxpro
 Home-page: https://pypi.org/project/social-auth-mitxpro
 License: MIT
 Author: MIT Office of Open Learning
 Author-email: mitx-devops@mit.edu
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: attrs (==22.1.0)
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: social-auth-core (>=4.1.0,<5.0.0)
 Project-URL: Repository, https://github.com/mitodl/social-auth-mitxpro/
 Description-Content-Type: text/markdown
 
 
 social-auth-mitxpro
 ---
```

