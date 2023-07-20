# Comparing `tmp/django-imgwidget-0.0.2.4.tar.gz` & `tmp/django-imgwidget-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.2.4.tar", last modified: Mon Jun  5 01:06:41 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.2.5.tar", last modified: Thu Jul 20 08:07:03 2023, max compression
```

## Comparing `django-imgwidget-0.0.2.4.tar` & `django-imgwidget-0.0.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.735777 django-imgwidget-0.0.2.4/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.4/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-06-05 01:06:41.735634 django-imgwidget-0.0.2.4/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1883 2023-06-03 12:13:00.000000 django-imgwidget-0.0.2.4/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.731823 django-imgwidget-0.0.2.4/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.4/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.732120 django-imgwidget-0.0.2.4/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.4/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      940 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.4/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.732369 django-imgwidget-0.0.2.4/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.729795 django-imgwidget-0.0.2.4/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.729946 django-imgwidget-0.0.2.4/django_imguploder/static/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.732452 django-imgwidget-0.0.2.4/django_imguploder/static/admin/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2160 2023-06-05 01:06:25.000000 django-imgwidget-0.0.2.4/django_imguploder/static/admin/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.732681 django-imgwidget-0.0.2.4/django_imguploder/static/admin/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.4/django_imguploder/static/admin/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.733414 django-imgwidget-0.0.2.4/django_imguploder/static/admin/js/
--rw-r--r--   0 donghao    (501) staff       (20)     5318 2023-06-03 12:06:56.000000 django-imgwidget-0.0.2.4/django_imguploder/static/admin/js/img_multi_upload.js
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.4/django_imguploder/static/admin/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.730040 django-imgwidget-0.0.2.4/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.730076 django-imgwidget-0.0.2.4/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.734240 django-imgwidget-0.0.2.4/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     2677 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.4/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.4/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-05 01:06:41.735454 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-06-05 01:06:41.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      803 2023-06-05 01:06:41.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-05 01:06:41.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-05 01:06:41.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-05 01:06:41.000000 django-imgwidget-0.0.2.4/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-05 01:06:41.735828 django-imgwidget-0.0.2.4/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-05 01:06:38.000000 django-imgwidget-0.0.2.4/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.890079 django-imgwidget-0.0.2.5/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.5/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-07-20 08:07:03.889893 django-imgwidget-0.0.2.5/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1883 2023-06-03 12:13:00.000000 django-imgwidget-0.0.2.5/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.887211 django-imgwidget-0.0.2.5/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.5/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.887409 django-imgwidget-0.0.2.5/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.5/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      940 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.5/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.887634 django-imgwidget-0.0.2.5/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.885481 django-imgwidget-0.0.2.5/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.885653 django-imgwidget-0.0.2.5/django_imguploder/static/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.887707 django-imgwidget-0.0.2.5/django_imguploder/static/admin/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2172 2023-07-20 08:07:00.000000 django-imgwidget-0.0.2.5/django_imguploder/static/admin/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.887806 django-imgwidget-0.0.2.5/django_imguploder/static/admin/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.5/django_imguploder/static/admin/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.888237 django-imgwidget-0.0.2.5/django_imguploder/static/admin/js/
+-rw-r--r--   0 donghao    (501) staff       (20)     5318 2023-06-03 12:06:56.000000 django-imgwidget-0.0.2.5/django_imguploder/static/admin/js/img_multi_upload.js
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.5/django_imguploder/static/admin/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.885789 django-imgwidget-0.0.2.5/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.885833 django-imgwidget-0.0.2.5/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.888961 django-imgwidget-0.0.2.5/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     2677 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.5/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.5/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:07:03.889715 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      803 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-07-20 08:07:03.000000 django-imgwidget-0.0.2.5/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-07-20 08:07:03.890137 django-imgwidget-0.0.2.5/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      878 2023-07-20 08:07:00.000000 django-imgwidget-0.0.2.5/setup.py
```

### Comparing `django-imgwidget-0.0.2.4/PKG-INFO` & `django-imgwidget-0.0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.2.4/README.md` & `django-imgwidget-0.0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.2.5/django_imguploder/forms/widget.py`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/static/admin/css/imgwidget.css` & `django-imgwidget-0.0.2.5/django_imguploder/static/admin/css/imgwidget.css`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,24 @@
     position: relative;
     display: inline-block;
     overflow: hidden;
     border: solid #b1c6c1 1px;
     border-radius: 10px;
     margin-right: 10px;
 }
-
+.widget_imgs{
+    width: 100%;
+    height: 100%;
+}
 /*缩略图片聚焦样式*/
 .selected-img:hover {
     cursor: pointer;
 }
 
+
 /*上传图片按钮样式*/
 .file-button {
     width: 160px;
     height: 100px;
     position: relative;
     display: inline-block;
     overflow: hidden;
@@ -94,11 +98,7 @@
     height: 100%;
     display: none;
 }
 
 #bigimg {
     border: 5px solid #fff;
 }
-
-.selected-img img {
-    width: 100%;
-}
```

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/static/admin/imgs/add.png` & `django-imgwidget-0.0.2.5/django_imguploder/static/admin/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/static/admin/js/img_multi_upload.js` & `django-imgwidget-0.0.2.5/django_imguploder/static/admin/js/img_multi_upload.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/static/admin/js/jquery.min.js` & `django-imgwidget-0.0.2.5/django_imguploder/static/admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imguploder/templates/admin/widgets/img_multi_upload.html` & `django-imgwidget-0.0.2.5/django_imguploder/templates/admin/widgets/img_multi_upload.html`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.2.5/django_imgwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.4
+Version: 0.0.2.5
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.2.4/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.2.5/django_imgwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.4/setup.py` & `django-imgwidget-0.0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.2.4'
+VERSION = '0.0.2.5'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
```

