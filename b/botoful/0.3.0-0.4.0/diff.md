# Comparing `tmp/botoful-0.3.0.tar.gz` & `tmp/botoful-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botoful-0.3.0.tar", last modified: Fri Mar 12 16:53:57 2021, max compression
+gzip compressed data, was "botoful-0.4.0.tar", max compression
```

## Comparing `botoful-0.3.0.tar` & `botoful-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2021-03-09 11:09:58.236579 botoful-0.3.0/LICENSE
--rw-r--r--   0        0        0       53 2021-03-12 16:19:49.388250 botoful-0.3.0/botoful/__init__.py
--rw-r--r--   0        0        0      738 2021-03-12 16:31:04.750636 botoful-0.3.0/botoful/filters.py
--rw-r--r--   0        0        0     8585 2021-03-12 16:51:55.752031 botoful-0.3.0/botoful/query.py
--rw-r--r--   0        0        0     7158 2021-03-09 06:28:52.921741 botoful-0.3.0/botoful/reserved.py
--rw-r--r--   0        0        0      274 2021-03-09 08:48:46.422109 botoful-0.3.0/botoful/serializers.py
--rw-r--r--   0        0        0      625 2021-03-12 16:27:44.275136 botoful-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      642 2021-03-12 16:53:57.374003 botoful-0.3.0/setup.py
--rw-r--r--   0        0        0      712 2021-03-12 16:53:57.374435 botoful-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-20 07:25:54.490522 botoful-0.4.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-07-20 11:03:03.737257 botoful-0.4.0/botoful/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/filters.py
+-rw-r--r--   0        0        0     8653 2023-07-20 08:36:05.228656 botoful-0.4.0/botoful/query.py
+-rw-r--r--   0        0        0     7158 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/reserved.py
+-rw-r--r--   0        0        0      274 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/serializers.py
+-rw-r--r--   0        0        0     4109 2023-07-20 11:11:31.681387 botoful-0.4.0/botoful/table.py
+-rw-r--r--   0        0        0      677 2023-07-20 11:09:26.123384 botoful-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 botoful-0.4.0/PKG-INFO
```

### Comparing `botoful-0.3.0/LICENSE` & `botoful-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botoful-0.3.0/botoful/filters.py` & `botoful-0.4.0/botoful/filters.py`

 * *Files identical despite different names*

### Comparing `botoful-0.3.0/botoful/query.py` & `botoful-0.4.0/botoful/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .serializers import deserialize, serialize
 
 
 def fluent(func):
     # Decorator that assists in a fluent api.
     # It clones the current 'self', calls the wrapped method on the clone and returns the clone
     @wraps(func)
-    def fluent_wrapper(self, *args, **kwargs):
+    def fluent_wrapper(self, *args, **kwargs) -> Query:
         new_self = copy.deepcopy(self)
         return func(new_self, *args, **kwargs)
 
     return fluent_wrapper
 
 
 class QueryResult:
@@ -101,14 +101,15 @@
         self._scan_index_forward = True
 
     @fluent
     def page_size(self, page_size) -> Query:
         self._page_size = page_size
         return self
 
+    @fluent
     def limit(self, limit) -> Query:
         return self.page_size(page_size=limit)
 
     @fluent
     def index(self, index_name: str) -> Query:
         self._index = index_name
         return self
@@ -124,35 +125,35 @@
             key = self._name_variable(tokens[0])
             operator = tokens[1]
             self._key_conditions.append(Condition(key=key, operator=operator, value=condition))
 
         return self
 
     @fluent
-    def attributes(self, keys: List[str]):
+    def attributes(self, keys: List[str]) -> Query:
         self._attributes_to_fetch.update(keys)
         return self
 
     @fluent
-    def filter(self, condition: ConditionBase):
+    def filter(self, condition: ConditionBase) -> Query:
         self._filter = condition
         return self
 
     @fluent
-    def consistent(self, consistent_read: bool=True):
+    def consistent(self, consistent_read: bool = True) -> Query:
         self._consistent_read = consistent_read
         return self
 
     @fluent
-    def forwards(self):
+    def forwards(self) -> Query:
         self._scan_index_forward = True
         return self
 
     @fluent
-    def backwards(self):
+    def backwards(self) -> Query:
         self._scan_index_forward = False
         return self
 
     def _name_variable(self, variable):
         if variable.upper() not in RESERVED_KEYWORDS:
             return variable
```

### Comparing `botoful-0.3.0/botoful/reserved.py` & `botoful-0.4.0/botoful/reserved.py`

 * *Files identical despite different names*

### Comparing `botoful-0.3.0/pyproject.toml` & `botoful-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "botoful"
-version = "0.3.0"
+version = "0.4.0"
 description = "A beautiful boto wrapper"
 authors = ["Imtiaz Mangerah <Imtiaz_Mangerah@a2d24.com>"]
 license = "MIT"
 homepage = "https://www.botoful.com"
 repository = "https://github.com/a2d24/botoful"
 documentation = "https://www.botoful.com"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 boto3 = {version = "^1.17.23", optional = true}
+moto = {extras = ["dynamodb"], version = "^4.1.13"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 pytest-cov = "^2.11.1"
 Pygments = "^2.8.1"
 boto3 = "^1.17.23"
```

### Comparing `botoful-0.3.0/PKG-INFO` & `botoful-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: botoful
-Version: 0.3.0
+Version: 0.4.0
 Summary: A beautiful boto wrapper
 Home-page: https://www.botoful.com
 License: MIT
 Author: Imtiaz Mangerah
 Author-email: Imtiaz_Mangerah@a2d24.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: boto
-Requires-Dist: boto3 (>=1.17.23,<2.0.0); extra == "boto"
+Requires-Dist: boto3 (>=1.17.23,<2.0.0) ; extra == "boto"
+Requires-Dist: moto[dynamodb] (>=4.1.13,<5.0.0)
 Project-URL: Documentation, https://www.botoful.com
 Project-URL: Repository, https://github.com/a2d24/botoful
```

