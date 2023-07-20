# Comparing `tmp/django-imgwidget-0.0.3.tar.gz` & `tmp/django-imgwidget-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.3.tar", last modified: Thu Jul 20 08:09:32 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.3.1.tar", last modified: Thu Jul 20 08:11:01 2023, max compression
```

## Comparing `django-imgwidget-0.0.3.tar` & `django-imgwidget-0.0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.573051 django-imgwidget-0.0.3/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.3/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2308 2023-07-20 08:09:32.572912 django-imgwidget-0.0.3/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1883 2023-06-03 12:13:00.000000 django-imgwidget-0.0.3/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.570147 django-imgwidget-0.0.3/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.3/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.570345 django-imgwidget-0.0.3/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.3/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      940 2023-06-03 12:07:49.000000 django-imgwidget-0.0.3/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.570571 django-imgwidget-0.0.3/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.568405 django-imgwidget-0.0.3/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.568547 django-imgwidget-0.0.3/django_imguploder/static/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.570655 django-imgwidget-0.0.3/django_imguploder/static/admin/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2172 2023-07-20 08:07:00.000000 django-imgwidget-0.0.3/django_imguploder/static/admin/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.570853 django-imgwidget-0.0.3/django_imguploder/static/admin/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.3/django_imguploder/static/admin/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.571306 django-imgwidget-0.0.3/django_imguploder/static/admin/js/
--rw-r--r--   0 donghao    (501) staff       (20)     5318 2023-06-03 12:06:56.000000 django-imgwidget-0.0.3/django_imguploder/static/admin/js/img_multi_upload.js
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.3/django_imguploder/static/admin/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.568636 django-imgwidget-0.0.3/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.568671 django-imgwidget-0.0.3/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.571977 django-imgwidget-0.0.3/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     2677 2023-06-03 12:07:49.000000 django-imgwidget-0.0.3/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:09:32.572762 django-imgwidget-0.0.3/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2308 2023-07-20 08:09:32.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      803 2023-07-20 08:09:32.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:09:32.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:07:03.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-07-20 08:09:32.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-07-20 08:09:32.000000 django-imgwidget-0.0.3/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-07-20 08:09:32.573090 django-imgwidget-0.0.3/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      876 2023-07-20 08:09:28.000000 django-imgwidget-0.0.3/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.713221 django-imgwidget-0.0.3.1/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.3.1/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-07-20 08:11:01.713060 django-imgwidget-0.0.3.1/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1883 2023-06-03 12:13:00.000000 django-imgwidget-0.0.3.1/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.710154 django-imgwidget-0.0.3.1/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.3.1/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.710341 django-imgwidget-0.0.3.1/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.3.1/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      940 2023-06-03 12:07:49.000000 django-imgwidget-0.0.3.1/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.710560 django-imgwidget-0.0.3.1/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.708456 django-imgwidget-0.0.3.1/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.708597 django-imgwidget-0.0.3.1/django_imguploder/static/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.710639 django-imgwidget-0.0.3.1/django_imguploder/static/admin/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2172 2023-07-20 08:07:00.000000 django-imgwidget-0.0.3.1/django_imguploder/static/admin/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.710844 django-imgwidget-0.0.3.1/django_imguploder/static/admin/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.3.1/django_imguploder/static/admin/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.711205 django-imgwidget-0.0.3.1/django_imguploder/static/admin/js/
+-rw-r--r--   0 donghao    (501) staff       (20)     5330 2023-07-20 08:10:51.000000 django-imgwidget-0.0.3.1/django_imguploder/static/admin/js/img_multi_upload.js
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.3.1/django_imguploder/static/admin/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.708685 django-imgwidget-0.0.3.1/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.708723 django-imgwidget-0.0.3.1/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.711947 django-imgwidget-0.0.3.1/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     2677 2023-06-03 12:07:49.000000 django-imgwidget-0.0.3.1/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.3.1/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-07-20 08:11:01.712885 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2310 2023-07-20 08:11:01.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      803 2023-07-20 08:11:01.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:11:01.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-07-20 08:07:03.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-07-20 08:11:01.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-07-20 08:11:01.000000 django-imgwidget-0.0.3.1/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-07-20 08:11:01.713270 django-imgwidget-0.0.3.1/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      878 2023-07-20 08:10:59.000000 django-imgwidget-0.0.3.1/setup.py
```

### Comparing `django-imgwidget-0.0.3/PKG-INFO` & `django-imgwidget-0.0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.3/README.md` & `django-imgwidget-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.3.1/django_imguploder/forms/widget.py`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imguploder/static/admin/css/imgwidget.css` & `django-imgwidget-0.0.3.1/django_imguploder/static/admin/css/imgwidget.css`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imguploder/static/admin/imgs/add.png` & `django-imgwidget-0.0.3.1/django_imguploder/static/admin/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imguploder/static/admin/js/img_multi_upload.js` & `django-imgwidget-0.0.3.1/django_imguploder/static/admin/js/img_multi_upload.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 function add_selected_img(src, widget_name) {
     $("#upload_image_" + widget_name).before("<div class=\"selected-img\">\n" +
         "    <i class=\"iconfont icon-delete delete_icon_image\" data-widgetname=\"" + widget_name + "\" title=\"删除图片\" onclick='delete_img(this)'></i>\n" +
-        "    <img class=\"" + widget_name + "_values\" src=\"" + src.replace("'", '').replace("'", '') + "\" alt=\"待选图片\" onclick='show_big_img(this)'>\n" +
+        "    <img class=\"widget_imgs " + widget_name + "_values\" src=\"" + src.replace("'", '').replace("'", '') + "\" alt=\"待选图片\" onclick='show_big_img(this)'>\n" +
         "</div>");
     updateTextareaValue(widget_name);
 }
 
 function getRotate(_this, index) {
     var degree = (_this.data('rotate') || 0) - 90;
     set_big_img_degree(degree);
```

### Comparing `django-imgwidget-0.0.3/django_imguploder/static/admin/js/jquery.min.js` & `django-imgwidget-0.0.3.1/django_imguploder/static/admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imguploder/templates/admin/widgets/img_multi_upload.html` & `django-imgwidget-0.0.3.1/django_imguploder/templates/admin/widgets/img_multi_upload.html`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.3.1/django_imgwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.3/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.3.1/django_imgwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.3/setup.py` & `django-imgwidget-0.0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.3'
+VERSION = '0.0.3.1'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
```

