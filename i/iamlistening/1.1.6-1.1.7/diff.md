# Comparing `tmp/iamlistening-1.1.6.tar.gz` & `tmp/iamlistening-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-1.1.6.tar", max compression
+gzip compressed data, was "iamlistening-1.1.7.tar", max compression
```

## Comparing `iamlistening-1.1.6.tar` & `iamlistening-1.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-19 15:23:14.135730 iamlistening-1.1.6/LICENSE
--rw-r--r--   0        0        0     2910 2023-07-19 15:23:14.135730 iamlistening-1.1.6/README.md
--rw-r--r--   0        0        0       99 2023-07-19 15:23:15.611758 iamlistening-1.1.6/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-19 15:23:14.139730 iamlistening-1.1.6/iamlistening/config.py
--rw-r--r--   0        0        0     1490 2023-07-19 15:23:14.139730 iamlistening-1.1.6/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4307 2023-07-19 15:23:14.139730 iamlistening-1.1.6/iamlistening/main.py
--rw-r--r--   0        0        0     3109 2023-07-19 15:23:15.603758 iamlistening-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 14:53:29.280232 iamlistening-1.1.7/LICENSE
+-rw-r--r--   0        0        0     2910 2023-07-20 14:53:29.280232 iamlistening-1.1.7/README.md
+-rw-r--r--   0        0        0       99 2023-07-20 14:53:31.052356 iamlistening-1.1.7/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-20 14:53:29.280232 iamlistening-1.1.7/iamlistening/config.py
+-rw-r--r--   0        0        0     2087 2023-07-20 14:53:29.280232 iamlistening-1.1.7/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4307 2023-07-20 14:53:29.280232 iamlistening-1.1.7/iamlistening/main.py
+-rw-r--r--   0        0        0     3109 2023-07-20 14:53:31.040355 iamlistening-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.7/PKG-INFO
```

### Comparing `iamlistening-1.1.6/LICENSE` & `iamlistening-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.6/README.md` & `iamlistening-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.6/iamlistening/config.py` & `iamlistening-1.1.7/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.6/iamlistening/default_settings.toml` & `iamlistening-1.1.7/iamlistening/default_settings.toml`

 * *Files 15% similar despite different names*

```diff
@@ -19,20 +19,41 @@
 bot_token = ""
 bot_channel_id = ""
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
 matrix_user = ""
 matrix_pass = ""
+iamlistening_commands = "/help"
 
 
 
 
 
 
+ 
+########################################
+###     END OF DEFAULT SETTINGS      ###
+########################################
+
+
+
+
+                                        
+# _   _                           _   ___  
+#| | | |                         | | |__ \ 
+#| |_| |__   ___    ___ _ __   __| |    )|
+#| __| '_ \ / _ \  / _ \ '_ \ / _` |   / / 
+#| |_| | | |  __/ |  __/ | | | (_| |  |_|  
+# \__|_| |_|\___|  \___|_| |_|\__,_|  (_)  
+########################################                                                                                      
+
+
+
+
 
 
 
 
 ########################################
 ###         TESTING SETTINGS         ###
 ########################################
@@ -67,8 +88,8 @@
 iamlistening_enabled = true
 bot_token = "1234556"
 bot_channel_id = "1234556"
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = "123456789"
 matrix_user = "123456789"
-matrix_pass = "123456789"
+matrix_pass = "123456789"
```

### Comparing `iamlistening-1.1.6/iamlistening/main.py` & `iamlistening-1.1.7/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.6/pyproject.toml` & `iamlistening-1.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "1.1.6"
+version = "1.1.7"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix",
```

### Comparing `iamlistening-1.1.6/PKG-INFO` & `iamlistening-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 1.1.6
+Version: 1.1.7
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 1.1.6 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 1.1.7 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-Dist:
```

