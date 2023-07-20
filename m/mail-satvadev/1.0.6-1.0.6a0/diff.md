# Comparing `tmp/mail_satvadev-1.0.6.tar.gz` & `tmp/mail_satvadev-1.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail_satvadev-1.0.6.tar", max compression
+gzip compressed data, was "mail_satvadev-1.0.6a0.tar", max compression
```

## Comparing `mail_satvadev-1.0.6.tar` & `mail_satvadev-1.0.6a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/LICENSE
--rw-r--r--   0        0        0     5498 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6/README.md
--rw-r--r--   0        0        0      732 2023-07-20 11:06:34.826085 mail_satvadev-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/src/mail_satvadev/__init__.py
--rw-r--r--   0        0        0      148 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6/src/mail_satvadev/apps.py
--rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6/src/mail_satvadev/filters.py
--rw-r--r--   0        0        0     2011 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6/src/mail_satvadev/messages.py
--rw-r--r--   0        0        0      859 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6/src/mail_satvadev/tasks.py
--rw-r--r--   0        0        0     6377 1970-01-01 00:00:00.000000 mail_satvadev-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6a0/LICENSE
+-rw-r--r--   0        0        0     5498 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6a0/README.md
+-rw-r--r--   0        0        0      733 2023-07-20 16:15:52.329444 mail_satvadev-1.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6a0/src/mail_satvadev/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-10 09:48:13.141367 mail_satvadev-1.0.6a0/src/mail_satvadev/apps.py
+-rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.6a0/src/mail_satvadev/filters.py
+-rw-r--r--   0        0        0     2011 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6a0/src/mail_satvadev/messages.py
+-rw-r--r--   0        0        0      859 2023-07-10 09:48:13.145367 mail_satvadev-1.0.6a0/src/mail_satvadev/tasks.py
+-rw-r--r--   0        0        0     6379 1970-01-01 00:00:00.000000 mail_satvadev-1.0.6a0/PKG-INFO
```

### Comparing `mail_satvadev-1.0.6/LICENSE` & `mail_satvadev-1.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.6/README.md` & `mail_satvadev-1.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.6/pyproject.toml` & `mail_satvadev-1.0.6a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mail_satvadev"
-version = "1.0.6"
+version = "1.0.6a"
 description = "Template for email"
 authors = ["satva.dev <info@satva.dev>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `mail_satvadev-1.0.6/src/mail_satvadev/filters.py` & `mail_satvadev-1.0.6a0/src/mail_satvadev/filters.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.6/src/mail_satvadev/messages.py` & `mail_satvadev-1.0.6a0/src/mail_satvadev/messages.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.6/src/mail_satvadev/tasks.py` & `mail_satvadev-1.0.6a0/src/mail_satvadev/tasks.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.6/PKG-INFO` & `mail_satvadev-1.0.6a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mail-satvadev
-Version: 1.0.6
+Version: 1.0.6a0
 Summary: Template for email
 Author: satva.dev
 Author-email: info@satva.dev
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

