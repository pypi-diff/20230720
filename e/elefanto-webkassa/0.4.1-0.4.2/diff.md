# Comparing `tmp/elefanto_webkassa-0.4.1.tar.gz` & `tmp/elefanto_webkassa-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.4.1.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.4.2.tar", max compression
```

## Comparing `elefanto_webkassa-0.4.1.tar` & `elefanto_webkassa-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2665 2023-07-20 08:48:54.224521 elefanto_webkassa-0.4.1/README.md
--rw-r--r--   0        0        0      873 2023-07-20 08:49:01.036378 elefanto_webkassa-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      568 2023-07-20 07:40:50.490900 elefanto_webkassa-0.4.1/webkassa/__init__.py
--rw-r--r--   0        0        0     5375 2023-07-20 06:48:17.909994 elefanto_webkassa-0.4.1/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.4.1/webkassa/apps.py
--rw-r--r--   0        0        0     3528 2023-07-20 06:28:21.251072 elefanto_webkassa-0.4.1/webkassa/forms.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.4.1/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0      469 2023-07-19 10:03:59.733639 elefanto_webkassa-0.4.1/webkassa/migrations/0002_check_order_number.py
--rw-r--r--   0        0        0      352 2023-07-20 07:04:33.293265 elefanto_webkassa-0.4.1/webkassa/migrations/0003_remove_webkassaaccount_is_encrypted_and_more.py
--rw-r--r--   0        0        0      576 2023-07-20 06:19:53.245544 elefanto_webkassa-0.4.1/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.4.1/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     3011 2023-07-20 06:19:38.493854 elefanto_webkassa-0.4.1/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.4.1/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.4.1/webkassa/services/__init__.py
--rw-r--r--   0        0        0      777 2023-07-20 07:41:00.042700 elefanto_webkassa-0.4.1/webkassa/services/cron.py
--rw-r--r--   0        0        0     6749 2023-07-20 07:28:50.118110 elefanto_webkassa-0.4.1/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.4.1/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      328 2023-07-20 07:48:06.765779 elefanto_webkassa-0.4.1/webkassa/settings.py
--rw-r--r--   0        0        0     2068 2023-07-20 07:17:01.685713 elefanto_webkassa-0.4.1/webkassa/templates/change_password_template.html
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 elefanto_webkassa-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2809 2023-07-20 09:01:28.137398 elefanto_webkassa-0.4.2/README.md
+-rw-r--r--   0        0        0      873 2023-07-20 09:01:37.353241 elefanto_webkassa-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      568 2023-07-20 07:40:50.490900 elefanto_webkassa-0.4.2/webkassa/__init__.py
+-rw-r--r--   0        0        0     5375 2023-07-20 06:48:17.909994 elefanto_webkassa-0.4.2/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.4.2/webkassa/apps.py
+-rw-r--r--   0        0        0     3528 2023-07-20 06:28:21.251072 elefanto_webkassa-0.4.2/webkassa/forms.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.4.2/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0      469 2023-07-19 10:03:59.733639 elefanto_webkassa-0.4.2/webkassa/migrations/0002_check_order_number.py
+-rw-r--r--   0        0        0      352 2023-07-20 07:04:33.293265 elefanto_webkassa-0.4.2/webkassa/migrations/0003_remove_webkassaaccount_is_encrypted_and_more.py
+-rw-r--r--   0        0        0      576 2023-07-20 06:19:53.245544 elefanto_webkassa-0.4.2/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.4.2/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     3011 2023-07-20 06:19:38.493854 elefanto_webkassa-0.4.2/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.4.2/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.4.2/webkassa/services/__init__.py
+-rw-r--r--   0        0        0      777 2023-07-20 07:41:00.042700 elefanto_webkassa-0.4.2/webkassa/services/cron.py
+-rw-r--r--   0        0        0     6749 2023-07-20 07:28:50.118110 elefanto_webkassa-0.4.2/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.4.2/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      328 2023-07-20 07:48:06.765779 elefanto_webkassa-0.4.2/webkassa/settings.py
+-rw-r--r--   0        0        0     2068 2023-07-20 07:17:01.685713 elefanto_webkassa-0.4.2/webkassa/templates/change_password_template.html
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 elefanto_webkassa-0.4.2/PKG-INFO
```

### Comparing `elefanto_webkassa-0.4.1/README.md` & `elefanto_webkassa-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 about
 =====
-
+# [Home page](https://github.com/elefanto-organization/elefanto-webkassa)
 integration with [webkassa.kz](https://webkassa.kz)
 
+This package developed for Elefantoteam, for using in future projects
+
 # For contributors
 
 **NOTE:** After clone this repository you should run command:
 
    ```bash
    chmod ug+x.githooks/pre-commit
    ```
@@ -63,17 +65,15 @@
 ```
 
 Usage
 ===
 after configure project, you should run `migrate`
 
 ```python
-python
-manage.py
-migrate
+python manage.py migrate
 ```
 
 then go to admin page, find `Webkassa accounts` in `WEBKASSA` app and add new account
 ![img.png](assets/img.png)
 
 now you can use package
```

### Comparing `elefanto_webkassa-0.4.1/pyproject.toml` & `elefanto_webkassa-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.4.1/webkassa/__init__.py` & `elefanto_webkassa-0.4.2/webkassa/__init__.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/admin.py` & `elefanto_webkassa-0.4.2/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/forms.py` & `elefanto_webkassa-0.4.2/webkassa/forms.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.4.2/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py` & `elefanto_webkassa-0.4.2/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/models.py` & `elefanto_webkassa-0.4.2/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/serializers.py` & `elefanto_webkassa-0.4.2/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/services/cron.py` & `elefanto_webkassa-0.4.2/webkassa/services/cron.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/services/manager.py` & `elefanto_webkassa-0.4.2/webkassa/services/manager.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/webkassa/templates/change_password_template.html` & `elefanto_webkassa-0.4.2/webkassa/templates/change_password_template.html`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.4.1/PKG-INFO` & `elefanto_webkassa-0.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,17 +13,19 @@
 Requires-Dist: django-crontab (>=0.7.1,<0.8.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Description-Content-Type: text/markdown
 
 about
 =====
-
+# [Home page](https://github.com/elefanto-organization/elefanto-webkassa)
 integration with [webkassa.kz](https://webkassa.kz)
 
+This package developed for Elefantoteam, for using in future projects
+
 # For contributors
 
 **NOTE:** After clone this repository you should run command:
 
    ```bash
    chmod ug+x.githooks/pre-commit
    ```
@@ -80,17 +82,15 @@
 ```
 
 Usage
 ===
 after configure project, you should run `migrate`
 
 ```python
-python
-manage.py
-migrate
+python manage.py migrate
 ```
 
 then go to admin page, find `Webkassa accounts` in `WEBKASSA` app and add new account
 ![img.png](assets/img.png)
 
 now you can use package
```

