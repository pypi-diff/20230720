# Comparing `tmp/meringue-1.1.0.dev2.tar.gz` & `tmp/meringue-1.1.0.dev3.tar.gz`

## Comparing `meringue-1.1.0.dev2.tar` & `meringue-1.1.0.dev3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/handlers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/api/utils.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/conf/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/LICENSE
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/README.md
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 meringue-1.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/routers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/utils.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/LICENSE
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/README.md
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/PKG-INFO
```

### Comparing `meringue-1.1.0.dev2/meringue/api/handlers.py` & `meringue-1.1.0.dev3/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/api/utils.py` & `meringue-1.1.0.dev3/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/conf/__init__.py` & `meringue-1.1.0.dev3/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/conf/default_settings.py` & `meringue-1.1.0.dev3/meringue/conf/default_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,7 +30,15 @@
 A dict of links to the frontend
 """
 
 FRONTEND_DOMAIN: Final[str] = None
 """
 Domain for generating absolute links
 """
+
+
+# API #############################################################################################
+
+API_ENABLE_ROOT_VIEW: Final[str] = settings.DEBUG
+"""
+Option to enable or disable the root view of the [Router][meringue.api.routers.DefaultRouter]
+"""
```

### Comparing `meringue-1.1.0.dev2/meringue/core/models.py` & `meringue-1.1.0.dev3/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/query.py` & `meringue-1.1.0.dev3/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/translation.py` & `meringue-1.1.0.dev3/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/upload_handlers.py` & `meringue-1.1.0.dev3/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.1.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.1.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/templatetags/meringue_base.py` & `meringue-1.1.0.dev3/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/utils/crypt.py` & `meringue-1.1.0.dev3/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/utils/datetime.py` & `meringue-1.1.0.dev3/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/meringue/core/utils/frontend.py` & `meringue-1.1.0.dev3/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/LICENSE` & `meringue-1.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev2/README.md` & `meringue-1.1.0.dev3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 * [x] Universal manager worked with all abstract models
 * [x] Tests of all functionality
 * [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
 * [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
  generating form based on response from api).
-* [ ] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
+* [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
 * [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
 * [ ] Functionality for working with images.
 	* [ ] Image editor like easy_thumbnails.
 	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 encrypting and decrypting text content (To create various secrets, such as a
 link to change your password or activate your profile). * [x] Functionality for
 obtaining absolute links to resources presented on the front, located on
 another domain (When working through api) (utils methods, template tags and
 filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
 serializer for automatic form generation on the front when working through rest
 api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
-generating form based on response from api). * [ ] Extended [drf router](https:
+generating form based on response from api). * [x] Extended [drf router](https:
 //www.django-rest-framework.org/api-guide/routers/) that allows you to add
 resources like `/profile` returning the profile data of an authorized user
 without his id. * [ ] Authorization backend for authorization by a pair of
 email and password. * [ ] Helpers to extend documentation generated by [drf-
 spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
 easily add links to different deployed environments (production, test, local,
 etc.) or let's say for more digestible tags instead of initially generated ones
```

### Comparing `meringue-1.1.0.dev2/pyproject.toml` & `meringue-1.1.0.dev3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 	"Topic :: Software Development :: Libraries",
 ]
 dependencies = [
 	"Django>=1.11.17",
 ]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+modeltranslation = ["django-modeltranslation>=0.17,<0.19"]
+drf = ["djangorestframework>=3.13,<4"]
+
 [project.urls]
 "Homepage" = "https://github.com/dd/Meringue"
 "Documentation" = "https://dd.github.io/Meringue/"
 "Repository" = "https://github.com/dd/Meringue"
 "Changelog" = "https://github.com/dd/Meringue/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/dd/Meringue/issues"
 
@@ -258,15 +262,15 @@
 	# "B027",
 	# # Ignore checks for possible passwords
 	# "S105", "S106", "S107",
 	# # Ignore complexity
 	# "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 	# "PLC1901", # empty string comparisons
 	# "PLW2901", # `for` loop variable overwritten
-	# "SIM114", # Combine `if` branches using logical `or` operator
+	"SIM114", # Combine `if` branches using logical `or` operator
 ]
 # unfixable = [
 # 	# Don't touch unused imports
 # 	"F401",
 # ]
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401", "F403"]
```

### Comparing `meringue-1.1.0.dev2/PKG-INFO` & `meringue-1.1.0.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.1.0.dev2
+Version: 1.1.0.dev3
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
@@ -43,14 +43,18 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: django>=1.11.17
+Provides-Extra: drf
+Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
+Provides-Extra: modeltranslation
+Requires-Dist: django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation'
 Description-Content-Type: text/markdown
 
 <h1 align="center" >Meringue</h1>
 
 <p align="center">
 	<a href="https://pypi.org/project/meringue">
 		<img src="https://img.shields.io/pypi/status/meringue.svg" alt="PyPI - Status" />
@@ -120,15 +124,15 @@
 
 * [x] Universal manager worked with all abstract models
 * [x] Tests of all functionality
 * [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
 * [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
  generating form based on response from api).
-* [ ] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
+* [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
 * [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
 * [ ] Functionality for working with images.
 	* [ ] Image editor like easy_thumbnails.
 	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev2 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev3 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
@@ -23,15 +23,18 @@
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=3.10 Requires-Dist: django>=1.11.17
-Description-Content-Type: text/markdown
+Provides-Extra: drf Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
+Provides-Extra: modeltranslation Requires-Dist: django-
+modeltranslation<0.19,>=0.17; extra == 'modeltranslation' Description-Content-
+Type: text/markdown
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
 Full documentation for the project is available at [dd.github.io/Meringue]
 (https://dd.github.io/Meringue/). Package with various functional (such as
@@ -50,15 +53,15 @@
 encrypting and decrypting text content (To create various secrets, such as a
 link to change your password or activate your profile). * [x] Functionality for
 obtaining absolute links to resources presented on the front, located on
 another domain (When working through api) (utils methods, template tags and
 filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
 serializer for automatic form generation on the front when working through rest
 api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
-generating form based on response from api). * [ ] Extended [drf router](https:
+generating form based on response from api). * [x] Extended [drf router](https:
 //www.django-rest-framework.org/api-guide/routers/) that allows you to add
 resources like `/profile` returning the profile data of an authorized user
 without his id. * [ ] Authorization backend for authorization by a pair of
 email and password. * [ ] Helpers to extend documentation generated by [drf-
 spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
 easily add links to different deployed environments (production, test, local,
 etc.) or let's say for more digestible tags instead of initially generated ones
```

