# Comparing `tmp/gwdg_idm_api-2.1.0.tar.gz` & `tmp/gwdg_idm_api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdg_idm_api-2.1.0.tar", last modified: Tue Jun 13 08:28:01 2023, max compression
+gzip compressed data, was "gwdg_idm_api-2.2.0.tar", last modified: Thu Jul 20 16:33:34 2023, max compression
```

## Comparing `gwdg_idm_api-2.1.0.tar` & `gwdg_idm_api-2.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.322036 gwdg_idm_api-2.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.326036 gwdg_idm_api-2.1.0/src/gwdg_idm_api/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4442 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/benutzerverwaltung.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6878 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/string_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tests/examples.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tests/predict_username.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.093876 gwdg_idm_api-2.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.097876 gwdg_idm_api-2.2.0/src/gwdg_idm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5096 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/benutzerverwaltung.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6878 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/string_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tests/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tests/predict_username.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tox.ini
```

### Comparing `gwdg_idm_api-2.1.0/.pre-commit-config.yaml` & `gwdg_idm_api-2.2.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.1
+    rev: v2.4.0
     hooks:
       - id: setup-cfg-fmt
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [--py38-plus, --keep-runtime-typing]
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v2.2.0
     hooks:
       - id: autoflake
         args: ["--in-place", "--remove-all-unused-imports"]
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.7.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-typing-imports>=1.9.0]
   # https://mypy.readthedocs.io/en/stable/introduction.html
   # you may wish to add this as well!
   # - repo: https://github.com/pre-commit/mirrors-mypy
   #   rev: v0.910-1
```

### Comparing `gwdg_idm_api-2.1.0/LICENSE` & `gwdg_idm_api-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/PKG-INFO` & `gwdg_idm_api-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: gwdg_idm_api
-Version: 2.1.0
+Version: 2.2.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # gwdg_idm_api
```

### Comparing `gwdg_idm_api-2.1.0/setup.cfg` & `gwdg_idm_api-2.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 description = Interface to the GWDG IDM api
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 author = Markus Stabrin
 author_email = markus.stabrin@mpi-dortmund.mpg.de
 license = MIT
-license_file = LICENSE
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.10
 
 [options]
 packages = find:
 install_requires = 
-	pydantic
+	pydantic==1
 	requests
 python_requires = >=3.10
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
```

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api/benutzerverwaltung.py` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api/benutzerverwaltung.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,36 +97,53 @@
         self, user: ChangeTemplate, expire_datetime: datetime.datetime | datetime.date
     ):
         today: datetime.date
         expire_date: datetime.date
         activate_now: bool
         change_data: dict[str, str]
 
+        today = datetime.datetime.now().date()
+        try:
+            expire_date = expire_datetime.date()
+        except AttributeError:
+            expire_date = expire_datetime
+
         current_user_status = self.get_single_user(user.id)
-        if current_user_status.goesternUserStatus in ("2", "255"):
-            raise AlreadyDeletedError
+
+        activate_now = (expire_date - today).total_seconds() <= 0
+        status_deleted = current_user_status.goesternUserStatus in ("2", "255")
 
         change_data = {}
         if current_user_status.isScheduledForDeletion == "TRUE":
             change_data["isScheduledForDeletion"] = "FALSE"
         elif current_user_status.goesternExpirationDate:
             change_data["goesternExpirationDate"] = ""
 
         self.update_user(user, change_data)  # type: ignore
 
-        today = datetime.datetime.now().date()
-        try:
-            expire_date = expire_datetime.date()
-        except AttributeError:
-            expire_date = expire_datetime
-
-        activate_now = (expire_date - today).total_seconds() <= 0
-        if activate_now:
+        if activate_now and not status_deleted:
             change_data = {
                 "isScheduledForDeletion": "TRUE",
             }
+        elif activate_now:
+            change_data = {}
         else:
             change_data = {
                 "goesternExpirationDate": expire_date.strftime("%d.%m.%Y"),
             }
 
         return self.update_user(user, change_data)  # type: ignore
+
+    def reactivate_user(self, user: ChangeTemplate):
+        current_user_status = self.get_single_user(user.id)
+
+        if current_user_status.goesternUserStatus == "255":
+            raise AlreadyDeletedError
+        elif current_user_status.goesternUserStatus != "2":
+            return user
+
+        if current_user_status.goesternExpirationDate:
+            change_data = {"goesternExpirationDate": ""}
+            user = self.update_user(user, change_data)  # type: ignore
+
+        change_data = {"goesternUserStatus": "0"}
+        return self.update_user(user, change_data)  # type: ignore
```

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api/models.py` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api/models.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api/string_cleaner.py` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api/util.py` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api/util.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/PKG-INFO` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: gwdg-idm-api
-Version: 2.1.0
+Version: 2.2.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # gwdg_idm_api
```

### Comparing `gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/SOURCES.txt` & `gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/tests/examples.py` & `gwdg_idm_api-2.2.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.1.0/tests/predict_username.py` & `gwdg_idm_api-2.2.0/tests/predict_username.py`

 * *Files identical despite different names*

