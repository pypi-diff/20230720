# Comparing `tmp/rubiran-2.0.3.tar.gz` & `tmp/rubiran-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.3.tar", last modified: Thu Jul 20 19:24:58 2023, max compression
+gzip compressed data, was "rubiran-2.0.4.tar", last modified: Thu Jul 20 19:42:59 2023, max compression
```

## Comparing `rubiran-2.0.3.tar` & `rubiran-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:58.022005 rubiran-2.0.3/
--rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.3/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:24:58.026005 rubiran-2.0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:57.858005 rubiran-2.0.3/rubiran/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.3/rubiran/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     1103 2023-07-20 19:15:52.000000 rubiran-2.0.3/rubiran/How.py
--rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.3/rubiran/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.3/rubiran/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53639 2023-07-20 19:14:55.000000 rubiran-2.0.3/rubiran/client.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.3/rubiran/encryption.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:24:57.994005 rubiran-2.0.3/rubiran.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 19:24:57.000000 rubiran-2.0.3/rubiran.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 19:24:58.038005 rubiran-2.0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1830 2023-07-20 19:13:46.000000 rubiran-2.0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.682005 rubiran-2.0.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.4/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:42:59.686005 rubiran-2.0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.522005 rubiran-2.0.4/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.4/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1102 2023-07-20 19:41:19.000000 rubiran-2.0.4/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.4/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.4/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53638 2023-07-20 19:37:26.000000 rubiran-2.0.4/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.4/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 19:42:59.650005 rubiran-2.0.4/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1586 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 19:42:58.000000 rubiran-2.0.4/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 19:42:59.694005 rubiran-2.0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1830 2023-07-20 19:41:43.000000 rubiran-2.0.4/setup.py
```

### Comparing `rubiran-2.0.3/LICENCE` & `rubiran-2.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.3/PKG-INFO` & `rubiran-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.3
+Version: 2.0.4
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rubiran-2.0.3/rubiran/An_Wb.py` & `rubiran-2.0.4/rubiran/An_Wb.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.3/rubiran/How.py` & `rubiran-2.0.4/rubiran/How.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.3   
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.4  
 
 {color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2023 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
 """
```

### Comparing `rubiran-2.0.3/rubiran/Socket.py` & `rubiran-2.0.4/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.3/rubiran/client.py` & `rubiran-2.0.4/rubiran/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1421,15 +1421,15 @@
 								break
 							except Exception as e:
 								continue
 						return [REQUES, p]
 
 
 	@staticmethod
-	def _getThumbInline(image_bytes:,bytes):
+	def _getThumbInline(image_bytes:bytes):
 		import io, base64, PIL.Image
 		im = PIL.Image.open(io.BytesIO(image_bytes))
 		width, height = im.size
 		if height > width:
 			new_height = 40
 			new_width  = round(new_height * width / height)
 		else:
```

### Comparing `rubiran-2.0.3/rubiran/encryption.py` & `rubiran-2.0.4/rubiran/encryption.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.3/rubiran.egg-info/PKG-INFO` & `rubiran-2.0.4/rubiran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.3
+Version: 2.0.4
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rubiran-2.0.3/setup.py` & `rubiran-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ``` bash
 @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.3",
+    version = "2.0.4",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

