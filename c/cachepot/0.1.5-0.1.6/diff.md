# Comparing `tmp/cachepot-0.1.5.tar.gz` & `tmp/cachepot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachepot-0.1.5.tar", last modified: Mon Jan  9 13:27:49 2023, max compression
+gzip compressed data, was "cachepot-0.1.6.tar", last modified: Thu Jul 20 14:37:09 2023, max compression
```

## Comparing `cachepot-0.1.5.tar` & `cachepot-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.160168 cachepot-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.144168 cachepot-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.152168 cachepot-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-09 13:27:32.000000 cachepot-0.1.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-09 13:27:32.000000 cachepot-0.1.5/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-09 13:27:32.000000 cachepot-0.1.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-01-09 13:27:32.000000 cachepot-0.1.5/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-09 13:27:32.000000 cachepot-0.1.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-09 13:27:32.000000 cachepot-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-09 13:27:32.000000 cachepot-0.1.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-01-09 13:27:49.160168 cachepot-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-09 13:27:32.000000 cachepot-0.1.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-01-09 13:27:32.000000 cachepot-0.1.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-01-09 13:27:32.000000 cachepot-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.152168 cachepot-0.1.5/cachepot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.152168 cachepot-0.1.5/cachepot/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/backend/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/backend/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/backend/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/expire.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.156168 cachepot-0.1.5/cachepot/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/serializer/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/serializer/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/serializer/str.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.156168 cachepot-0.1.5/cachepot/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-01-09 13:27:32.000000 cachepot-0.1.5/cachepot/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.152168 cachepot-0.1.5/cachepot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-09 13:27:49.000000 cachepot-0.1.5/cachepot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-09 13:27:32.000000 cachepot-0.1.5/docker-compose.test.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.156168 cachepot-0.1.5/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-09 13:27:32.000000 cachepot-0.1.5/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-09 13:27:32.000000 cachepot-0.1.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-09 13:27:32.000000 cachepot-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-09 13:27:32.000000 cachepot-0.1.5/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-01-09 13:27:49.160168 cachepot-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.156168 cachepot-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.156168 cachepot-0.1.5/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/backend/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/backend/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/backend/test_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:49.160168 cachepot-0.1.5/tests/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/serializer/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/serializer/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/serializer/test_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/test_expire.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-09 13:27:32.000000 cachepot-0.1.5/tests/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.058869 cachepot-0.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:36:41.000000 cachepot-0.1.6/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.058869 cachepot-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:36:41.000000 cachepot-0.1.6/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:36:41.000000 cachepot-0.1.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-20 14:36:41.000000 cachepot-0.1.6/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:36:41.000000 cachepot-0.1.6/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:36:41.000000 cachepot-0.1.6/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-20 14:36:41.000000 cachepot-0.1.6/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 14:36:41.000000 cachepot-0.1.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 14:36:41.000000 cachepot-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-20 14:37:09.062869 cachepot-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-20 14:36:41.000000 cachepot-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.058869 cachepot-0.1.6/cachepot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/cachepot/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/backend/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/backend/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/backend/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/expire.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/cachepot/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/serializer/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/serializer/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/serializer/str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/cachepot/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-20 14:36:41.000000 cachepot-0.1.6/cachepot/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/cachepot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 14:37:09.000000 cachepot-0.1.6/cachepot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 14:36:41.000000 cachepot-0.1.6/docker-compose.test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-20 14:36:41.000000 cachepot-0.1.6/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56363 2023-07-20 14:36:41.000000 cachepot-0.1.6/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-20 14:36:41.000000 cachepot-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-20 14:37:09.062869 cachepot-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/backend/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/backend/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/backend/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:37:09.062869 cachepot-0.1.6/tests/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/serializer/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/serializer/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/serializer/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/test_expire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-20 14:36:41.000000 cachepot-0.1.6/tests/test_store.py
```

### Comparing `cachepot-0.1.5/.gitignore` & `cachepot-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/LICENSE` & `cachepot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/PKG-INFO` & `cachepot-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachepot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Yet another Python cache library
 Home-page: https://github.com/kitsuyui/cachepot
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -101,24 +101,23 @@
 - Save to SQLite3 DB records ... [cachepot.backend.sqlite.SQLiteCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/sqlite.py)
 - Save to Redis DB ... [cachepot.backend.redis.RedisCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/redis.py)
 
 Of course you can define own backend.
 
 ## Development
 
-You can install requirements with pipenv
+You can install requirements with poetry.
 
 ```shell
-$ pipenv install --dev
+$ poetry install
 ```
 
 ### Test
 
 ```shell
-$ flake8
-$ mypy .
-$ python3 -m unittest discover
+$ poetry poe check  # lint and type check
+$ poetry poe test  # run tests
 ```
 
 # LICENSE
 
 The 3-Clause BSD License. See also LICENSE file.
```

### Comparing `cachepot-0.1.5/README.md` & `cachepot-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,24 +79,23 @@
 - Save to SQLite3 DB records ... [cachepot.backend.sqlite.SQLiteCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/sqlite.py)
 - Save to Redis DB ... [cachepot.backend.redis.RedisCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/redis.py)
 
 Of course you can define own backend.
 
 ## Development
 
-You can install requirements with pipenv
+You can install requirements with poetry.
 
 ```shell
-$ pipenv install --dev
+$ poetry install
 ```
 
 ### Test
 
 ```shell
-$ flake8
-$ mypy .
-$ python3 -m unittest discover
+$ poetry poe check  # lint and type check
+$ poetry poe test  # run tests
 ```
 
 # LICENSE
 
 The 3-Clause BSD License. See also LICENSE file.
```

### Comparing `cachepot-0.1.5/cachepot/backend/filesystem.py` & `cachepot-0.1.6/cachepot/backend/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             self.path = pathlib.Path(path)
         else:
             self.path = path
 
     def __get_real_path(self, key: bytes) -> pathlib.Path:
         return self.path / hashlib.sha256(key).hexdigest()
 
-    def save(self, key: bytes, value: bytes, expire_seconds: ExpireSeconds) -> None:
+    def save(
+        self, key: bytes, value: bytes, expire_seconds: ExpireSeconds
+    ) -> None:
         expire_at = datetime.now() + to_timedelta(expire_seconds)
         expire_timestamp = time.mktime(expire_at.timetuple())
 
         realpath = self.__get_real_path(key)
         with cast(BinaryIO, realpath.open("wb")) as f:
             f.write(value)
         os.utime(str(realpath), (expire_timestamp, expire_timestamp))
```

### Comparing `cachepot-0.1.5/cachepot/backend/redis.py` & `cachepot-0.1.6/cachepot/backend/redis.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 class RedisCacheBackend(CacheBackendProtocol):
     redis_connection: redis.Redis
 
     def __init__(self, redis_connection: redis.Redis):
         self.redis = redis_connection
 
-    def save(self, key: bytes, value: bytes, *, expire_seconds: ExpireSeconds) -> None:
+    def save(
+        self, key: bytes, value: bytes, *, expire_seconds: ExpireSeconds
+    ) -> None:
         with self.redis.pipeline() as pipe:
             pipe.set(key, value)
             pipe.expire(key, to_timedelta(expire_seconds))
             pipe.execute()
 
     def load(self, key: bytes) -> Optional[bytes]:
         return cast(bytes, self.redis.get(key))
```

### Comparing `cachepot-0.1.5/cachepot/backend/sqlite.py` & `cachepot-0.1.6/cachepot/backend/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,17 @@
                  ON cachepot
                   ( key
                   , expire_at
                   )"""
         )
         self.conn = conn
 
-    def save(self, key: bytes, value: bytes, *, expire_seconds: ExpireSeconds) -> None:
+    def save(
+        self, key: bytes, value: bytes, *, expire_seconds: ExpireSeconds
+    ) -> None:
         expire_at = datetime.now() + to_timedelta(expire_seconds)
         self.conn.execute(
             """\
 INSERT OR REPLACE INTO cachepot
             (key, value, expire_at)
      VALUES (?, ?, ?)""",
             (key, value, expire_at),
```

### Comparing `cachepot-0.1.5/cachepot/serializer/json.py` & `cachepot-0.1.6/cachepot/serializer/json.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/cachepot/store/__init__.py` & `cachepot-0.1.6/cachepot/store/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 
 
 class CacheStoreProtocol(Protocol[T, S]):
     def get(self, key: T) -> Optional[S]:
         ...
 
     def put(
-        self, key: T, value: S, *, expire_seconds: Optional[ExpireSeconds] = None
+        self,
+        key: T,
+        value: S,
+        *,
+        expire_seconds: Optional[ExpireSeconds] = None
     ) -> None:
         ...
 
     def proxy(self, original_function: Callable[..., S]) -> Callable[..., S]:
         ...
 
     def remove(self, key: T) -> None:
@@ -55,21 +59,27 @@
         real_key = self.__get_real_key(key)
         loaded = self.backend.load(real_key)
         if loaded is None:
             return None
         return self.value_serializer.deserialize(loaded)
 
     def put(
-        self, key: T, value: S, *, expire_seconds: Optional[ExpireSeconds] = None
+        self,
+        key: T,
+        value: S,
+        *,
+        expire_seconds: Optional[ExpireSeconds] = None
     ) -> None:
         if expire_seconds is None:
             expire_seconds = self.default_expire_seconds
         real_key = self.__get_real_key(key)
         serialized_value = self.value_serializer.serialize(value)
-        self.backend.save(real_key, serialized_value, expire_seconds=expire_seconds)
+        self.backend.save(
+            real_key, serialized_value, expire_seconds=expire_seconds
+        )
 
     def proxy(self, original_function: Callable[..., S]) -> Callable[..., S]:
         def _proxy(
             *args: Any,
             cache_key: T,
             expire_seconds: Optional[ExpireSeconds] = None,
             **kwargs: Any
```

### Comparing `cachepot-0.1.5/cachepot.egg-info/PKG-INFO` & `cachepot-0.1.6/cachepot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachepot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Yet another Python cache library
 Home-page: https://github.com/kitsuyui/cachepot
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -101,24 +101,23 @@
 - Save to SQLite3 DB records ... [cachepot.backend.sqlite.SQLiteCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/sqlite.py)
 - Save to Redis DB ... [cachepot.backend.redis.RedisCacheBackend](https://github.com/kitsuyui/cachepot/blob/master/cachepot/backend/redis.py)
 
 Of course you can define own backend.
 
 ## Development
 
-You can install requirements with pipenv
+You can install requirements with poetry.
 
 ```shell
-$ pipenv install --dev
+$ poetry install
 ```
 
 ### Test
 
 ```shell
-$ flake8
-$ mypy .
-$ python3 -m unittest discover
+$ poetry poe check  # lint and type check
+$ poetry poe test  # run tests
 ```
 
 # LICENSE
 
 The 3-Clause BSD License. See also LICENSE file.
```

### Comparing `cachepot-0.1.5/cachepot.egg-info/SOURCES.txt` & `cachepot-0.1.6/cachepot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 .gitignore
 .gitignore.in
 .isort.cfg
 LICENSE
-Makefile
-Pipfile
-Pipfile.lock
 README.md
 docker-compose.test.yml
-mypy.ini
+poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
+.github/renovate.json5
+.github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 cachepot/__init__.py
 cachepot/_version.py
 cachepot/expire.py
 cachepot/py.typed
 cachepot.egg-info/PKG-INFO
 cachepot.egg-info/SOURCES.txt
 cachepot.egg-info/dependency_links.txt
```

### Comparing `cachepot-0.1.5/example/__init__.py` & `cachepot-0.1.6/example/__init__.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/setup.cfg` & `cachepot-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/tests/backend/test_filesystem.py` & `cachepot-0.1.6/tests/backend/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/tests/backend/test_redis.py` & `cachepot-0.1.6/tests/backend/test_redis.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/tests/backend/test_sqlite.py` & `cachepot-0.1.6/tests/backend/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/tests/serializer/test_str.py` & `cachepot-0.1.6/tests/serializer/test_str.py`

 * *Files identical despite different names*

### Comparing `cachepot-0.1.5/tests/test_store.py` & `cachepot-0.1.6/tests/test_store.py`

 * *Files identical despite different names*

