# Comparing `tmp/velait_api-0.5.3.tar.gz` & `tmp/velait_api-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velait_api-0.5.3.tar", last modified: Mon May 15 07:15:28 2023, max compression
+gzip compressed data, was "velait_api-0.5.4.tar", last modified: Thu Jul 20 08:08:10 2023, max compression
```

## Comparing `velait_api-0.5.3.tar` & `velait_api-0.5.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.831667 velait_api-0.5.3/
--rw-rw-rw-   0        0        0      189 2023-05-15 07:15:28.831667 velait_api-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 06:59:16.000000 velait_api-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 07:15:28.832672 velait_api-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-05-15 07:15:19.000000 velait_api-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.299459 velait_api-0.5.3/velait/
--rw-rw-rw-   0        0        0        0 2023-03-15 06:47:28.000000 velait_api-0.5.3/velait/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.482454 velait_api-0.5.3/velait/main/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.579235 velait_api-0.5.3/velait/main/api/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/api/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-03-16 05:55:42.000000 velait_api-0.5.3/velait/main/api/exception_handlers.py
--rw-rw-rw-   0        0        0     5012 2023-03-15 06:50:44.000000 velait_api-0.5.3/velait/main/api/pagination.py
--rw-rw-rw-   0        0        0     1408 2023-05-15 07:15:06.000000 velait_api-0.5.3/velait/main/api/responses.py
--rw-rw-rw-   0        0        0     1444 2023-05-02 05:28:13.000000 velait_api-0.5.3/velait/main/api/serializers.py
--rw-rw-rw-   0        0        0     5346 2023-03-16 05:57:04.000000 velait_api-0.5.3/velait/main/api/views.py
--rw-rw-rw-   0        0        0      210 2023-04-07 09:18:38.000000 velait_api-0.5.3/velait/main/apps.py
--rw-rw-rw-   0        0        0      507 2023-03-15 06:51:08.000000 velait_api-0.5.3/velait/main/exceptions.py
--rw-rw-rw-   0        0        0     3475 2023-04-04 10:05:12.000000 velait_api-0.5.3/velait/main/logging.py
--rw-rw-rw-   0        0        0      590 2023-04-04 09:22:28.000000 velait_api-0.5.3/velait/main/middleware.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.581238 velait_api-0.5.3/velait/main/migrations/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/migrations/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-07 09:01:13.000000 velait_api-0.5.3/velait/main/models.py
--rw-rw-rw-   0        0        0      506 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/parser.py
--rw-rw-rw-   0        0        0      479 2023-03-15 06:45:44.000000 velait_api-0.5.3/velait/main/render.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.596236 velait_api-0.5.3/velait/main/services/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.651764 velait_api-0.5.3/velait/main/services/search/
--rw-rw-rw-   0        0        0        0 2023-03-15 06:49:26.000000 velait_api-0.5.3/velait/main/services/search/__init__.py
--rw-rw-rw-   0        0        0     3895 2023-03-15 06:53:04.000000 velait_api-0.5.3/velait/main/services/search/base_search.py
--rw-rw-rw-   0        0        0     2135 2023-03-15 06:52:14.000000 velait_api-0.5.3/velait/main/services/search/search.py
--rw-rw-rw-   0        0        0      380 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/main/services/utils.py
--rw-rw-rw-   0        0        0      818 2023-04-04 09:59:51.000000 velait_api-0.5.3/velait/main/settings.py
--rw-rw-rw-   0        0        0     2633 2023-04-07 09:23:26.000000 velait_api-0.5.3/velait/main/signals.py
--rw-rw-rw-   0        0        0      193 2023-04-04 09:22:21.000000 velait_api-0.5.3/velait/main/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.755787 velait_api-0.5.3/velait/velait_users/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/velait_users/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.784773 velait_api-0.5.3/velait/velait_users/api/
--rw-rw-rw-   0        0        0        0 2023-04-07 08:52:46.000000 velait_api-0.5.3/velait/velait_users/api/__init__.py
--rw-rw-rw-   0        0        0      322 2023-04-07 08:53:32.000000 velait_api-0.5.3/velait/velait_users/api/serializers.py
--rw-rw-rw-   0        0        0      421 2023-04-07 08:55:32.000000 velait_api-0.5.3/velait/velait_users/api/views.py
--rw-rw-rw-   0        0        0      168 2023-03-15 06:45:44.000000 velait_api-0.5.3/velait/velait_users/apps.py
--rw-rw-rw-   0        0        0      263 2023-03-15 06:48:57.000000 velait_api-0.5.3/velait/velait_users/exceptions.py
--rw-rw-rw-   0        0        0     2799 2023-04-04 09:56:27.000000 velait_api-0.5.3/velait/velait_users/middleware.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.786770 velait_api-0.5.3/velait/velait_users/migrations/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.3/velait/velait_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-03-15 06:45:44.000000 velait_api-0.5.3/velait/velait_users/services.py
--rw-rw-rw-   0        0        0      388 2023-03-15 06:45:44.000000 velait_api-0.5.3/velait/velait_users/urls.py
--rw-rw-rw-   0        0        0     1873 2023-04-07 08:53:00.000000 velait_api-0.5.3/velait/velait_users/views.py
-drwxrwxrwx   0        0        0        0 2023-05-15 07:15:28.829667 velait_api-0.5.3/velait_api.egg-info/
--rw-rw-rw-   0        0        0      189 2023-05-15 07:15:27.000000 velait_api-0.5.3/velait_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2023-05-15 07:15:27.000000 velait_api-0.5.3/velait_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 07:15:27.000000 velait_api-0.5.3/velait_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-05-15 07:15:27.000000 velait_api-0.5.3/velait_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 07:15:27.000000 velait_api-0.5.3/velait_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.937407 velait_api-0.5.4/
+-rw-rw-rw-   0        0        0      119 2023-07-20 08:08:10.937407 velait_api-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:15:48.000000 velait_api-0.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:08:10.937407 velait_api-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-07-20 08:08:04.000000 velait_api-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.899410 velait_api-0.5.4/velait/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.910408 velait_api-0.5.4/velait/main/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.916414 velait_api-0.5.4/velait/main/api/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/exception_handlers.py
+-rw-rw-rw-   0        0        0     5012 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/pagination.py
+-rw-rw-rw-   0        0        0     1408 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/responses.py
+-rw-rw-rw-   0        0        0     1444 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/serializers.py
+-rw-rw-rw-   0        0        0     5346 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/api/views.py
+-rw-rw-rw-   0        0        0      210 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/apps.py
+-rw-rw-rw-   0        0        0      507 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/exceptions.py
+-rw-rw-rw-   0        0        0     3475 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/logging.py
+-rw-rw-rw-   0        0        0      590 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.917408 velait_api-0.5.4/velait/main/migrations/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/models.py
+-rw-rw-rw-   0        0        0      506 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/parser.py
+-rw-rw-rw-   0        0        0      479 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/render.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.918408 velait_api-0.5.4/velait/main/services/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.921409 velait_api-0.5.4/velait/main/services/search/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/services/search/__init__.py
+-rw-rw-rw-   0        0        0     3917 2023-07-19 08:26:22.000000 velait_api-0.5.4/velait/main/services/search/base_search.py
+-rw-rw-rw-   0        0        0     2316 2023-07-19 08:26:02.000000 velait_api-0.5.4/velait/main/services/search/search.py
+-rw-rw-rw-   0        0        0      380 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/services/utils.py
+-rw-rw-rw-   0        0        0      818 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/settings.py
+-rw-rw-rw-   0        0        0     2633 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/signals.py
+-rw-rw-rw-   0        0        0      193 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/main/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.927407 velait_api-0.5.4/velait/velait_users/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.930408 velait_api-0.5.4/velait/velait_users/api/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/api/__init__.py
+-rw-rw-rw-   0        0        0      322 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/api/serializers.py
+-rw-rw-rw-   0        0        0      421 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/api/views.py
+-rw-rw-rw-   0        0        0      168 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/apps.py
+-rw-rw-rw-   0        0        0      263 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/exceptions.py
+-rw-rw-rw-   0        0        0     2799 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.931407 velait_api-0.5.4/velait/velait_users/migrations/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/services.py
+-rw-rw-rw-   0        0        0      388 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/urls.py
+-rw-rw-rw-   0        0        0     1873 2023-07-19 05:53:58.000000 velait_api-0.5.4/velait/velait_users/views.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:10.936407 velait_api-0.5.4/velait_api.egg-info/
+-rw-rw-rw-   0        0        0      119 2023-07-20 08:08:10.000000 velait_api-0.5.4/velait_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-07-20 08:08:10.000000 velait_api-0.5.4/velait_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:08:10.000000 velait_api-0.5.4/velait_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-20 08:08:10.000000 velait_api-0.5.4/velait_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 08:08:10.000000 velait_api-0.5.4/velait_api.egg-info/top_level.txt
```

### Comparing `velait_api-0.5.3/velait/main/api/exception_handlers.py` & `velait_api-0.5.4/velait/main/api/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/api/pagination.py` & `velait_api-0.5.4/velait/main/api/pagination.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/api/responses.py` & `velait_api-0.5.4/velait/main/api/responses.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/api/serializers.py` & `velait_api-0.5.4/velait/main/api/serializers.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/api/views.py` & `velait_api-0.5.4/velait/main/api/views.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/logging.py` & `velait_api-0.5.4/velait/main/logging.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/middleware.py` & `velait_api-0.5.4/velait/main/middleware.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/models.py` & `velait_api-0.5.4/velait/main/models.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/services/search/base_search.py` & `velait_api-0.5.4/velait/main/services/search/base_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class SearchOperator(Enum):
     LESS = "less"
     EQUAL = "equal"
     GREATER = "greater"
     CONTAINS = "contains"
     LESS_OR_EQUAL = "lessOrEqual"
     GREATER_OR_EQUAL = "greaterOrEqual"
-
+    IS_NULL = "isNull"
 
 class Search(ABC):
     def _parse_json(self, data, key_name: str):
         try:
             return json.loads(data)
         except (json.JSONDecodeError, TypeError, ValueError):
             if data is not None:
```

### Comparing `velait_api-0.5.3/velait/main/services/search/search.py` & `velait_api-0.5.4/velait/main/services/search/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
             return [f"{field_name}__gt", field_value]
         elif operator == SearchOperator.CONTAINS.value:
             return [f"{field_name}__in", field_value]
         elif operator == SearchOperator.LESS_OR_EQUAL.value:
             return [f"{field_name}__lte", field_value]
         elif operator == SearchOperator.GREATER_OR_EQUAL.value:
             return [f"{field_name}__gte", field_value]
+        elif operator == SearchOperator.IS_NULL.value:
+            boolean = True if field_value == "True" else False
+            return [f"{field_name}__isnull", bool(boolean)]
         else:
             raise SearchError(name="query", description=_("Операция не найдена"))
 
 
 __all__ = [
     'SearchOperator',
     'SearchError',
```

### Comparing `velait_api-0.5.3/velait/main/settings.py` & `velait_api-0.5.4/velait/main/settings.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/main/signals.py` & `velait_api-0.5.4/velait/main/signals.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/velait_users/middleware.py` & `velait_api-0.5.4/velait/velait_users/middleware.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/velait_users/services.py` & `velait_api-0.5.4/velait/velait_users/services.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait/velait_users/views.py` & `velait_api-0.5.4/velait/velait_users/views.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.3/velait_api.egg-info/SOURCES.txt` & `velait_api-0.5.4/velait_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

