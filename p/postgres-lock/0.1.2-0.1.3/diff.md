# Comparing `tmp/postgres_lock-0.1.2.tar.gz` & `tmp/postgres_lock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_lock-0.1.2.tar", max compression
+gzip compressed data, was "postgres_lock-0.1.3.tar", max compression
```

## Comparing `postgres_lock-0.1.2.tar` & `postgres_lock-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.2/LICENSE
--rw-r--r--   0        0        0     3755 2023-06-05 18:56:38.234398 postgres_lock-0.1.2/README.md
--rw-r--r--   0        0        0      341 2023-06-02 20:16:52.298972 postgres_lock-0.1.2/postgres_lock/__init__.py
--rw-r--r--   0        0        0     2443 2023-06-05 17:59:32.127064 postgres_lock-0.1.2/postgres_lock/asyncpg.py
--rw-r--r--   0        0        0      589 2023-06-05 16:57:57.287722 postgres_lock-0.1.2/postgres_lock/errors.py
--rw-r--r--   0        0        0     9627 2023-06-05 18:26:09.323824 postgres_lock-0.1.2/postgres_lock/lock.py
--rw-r--r--   0        0        0     2575 2023-06-05 18:18:16.609045 postgres_lock-0.1.2/postgres_lock/psycopg2.py
--rw-r--r--   0        0        0     2993 2023-06-05 18:20:32.444223 postgres_lock-0.1.2/postgres_lock/psycopg3.py
--rw-r--r--   0        0        0     2813 2023-06-05 18:12:25.912861 postgres_lock-0.1.2/postgres_lock/sqlalchemy.py
--rw-r--r--   0        0        0      542 2023-06-05 18:57:01.854977 postgres_lock-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 postgres_lock-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-05-30 13:15:35.574393 postgres_lock-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3793 2023-07-20 18:00:21.778712 postgres_lock-0.1.3/README.md
+-rw-r--r--   0        0        0      341 2023-06-06 13:49:51.530416 postgres_lock-0.1.3/postgres_lock/__init__.py
+-rw-r--r--   0        0        0     2443 2023-06-05 17:59:32.127064 postgres_lock-0.1.3/postgres_lock/asyncpg.py
+-rw-r--r--   0        0        0      589 2023-06-05 16:57:57.287722 postgres_lock-0.1.3/postgres_lock/errors.py
+-rw-r--r--   0        0        0     9658 2023-07-09 00:29:44.119035 postgres_lock-0.1.3/postgres_lock/lock.py
+-rw-r--r--   0        0        0     2575 2023-06-05 18:18:16.609045 postgres_lock-0.1.3/postgres_lock/psycopg2.py
+-rw-r--r--   0        0        0     2993 2023-06-05 18:20:32.444223 postgres_lock-0.1.3/postgres_lock/psycopg3.py
+-rw-r--r--   0        0        0     2813 2023-06-05 18:12:25.912861 postgres_lock-0.1.3/postgres_lock/sqlalchemy.py
+-rw-r--r--   0        0        0      542 2023-07-20 17:59:50.250069 postgres_lock-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4582 1970-01-01 00:00:00.000000 postgres_lock-0.1.3/PKG-INFO
```

### Comparing `postgres_lock-0.1.2/LICENSE` & `postgres_lock-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/README.md` & `postgres_lock-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -171,12 +171,14 @@
 lock = Lock(conn, "shared-identifier", rollback_on_error=False)
 
 # do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.3**
+  - Key can be any object
 - **0.1.2**
   - Add Lock.rollback_on_error (default true)
   - Add Lock.handle_error() & Lock.handle_error_async()
 - **0.1.1**
   - Key can be str or int
```

### Comparing `postgres_lock-0.1.2/postgres_lock/asyncpg.py` & `postgres_lock-0.1.3/postgres_lock/asyncpg.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/postgres_lock/errors.py` & `postgres_lock-0.1.3/postgres_lock/errors.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/postgres_lock/lock.py` & `postgres_lock-0.1.3/postgres_lock/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,30 @@
         - nonblocking: return immediately with or without the lock being acquired
 
     Sharing (locks can or cannot be reacquired from the same scope)
     """
 
     conn: Any
     interface: str
-    key: str | int
+    key: Any
     lock_id: int
     rollback_on_error: bool
     scope: str
-    shared: bool
+    _locked: bool
+    _ref_count: int
+    _shared: bool
 
     blocking_lock_func: str
     nonblocking_lock_func: str
     unlock_func: str
 
     def __init__(
         self,
         conn: Any,
-        key: str | int,
+        key: Any,
         interface: Literal[
             "auto",
             "asyncpg",
             "psycopg2",
             "psycopg3",
             "sqlalchemy",
         ] = "auto",
@@ -75,27 +77,27 @@
         shared: bool = False,
     ):
         """
         Create a new Lock instance.
 
         Parameters:
             conn (object): Database connection.
-            key (str|int): Unique lock key.
+            key (object): Unique lock key.
             interface (str): Database interface.
             rollback_on_error (bool): Rollback if an error occurs while in a `with` statement.
             scope (str): Lock scope.
             shared (bool): Use a shared lock.
         """
         self.conn = conn
         self.interface = interface
         self.impl = self._load_impl()
         self.key = key
-        self.lock_id = str(int(hashlib.sha1(str(key).encode("utf-8")).hexdigest(), 16))[
-            :18
-        ]
+        self.lock_id = int(
+            str(int(hashlib.sha1(str(key).encode("utf-8")).hexdigest(), 16))[:18]
+        )
         self.rollback_on_error = rollback_on_error
         self.scope = scope
         self._locked = False
         self._ref_count = 0
         self._shared = shared
 
         infix = "_xact"
```

### Comparing `postgres_lock-0.1.2/postgres_lock/psycopg2.py` & `postgres_lock-0.1.3/postgres_lock/psycopg2.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/postgres_lock/psycopg3.py` & `postgres_lock-0.1.3/postgres_lock/psycopg3.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/postgres_lock/sqlalchemy.py` & `postgres_lock-0.1.3/postgres_lock/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `postgres_lock-0.1.2/pyproject.toml` & `postgres_lock-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgres-lock"
-version = "0.1.2"
+version = "0.1.3"
 description = "Lock mechanism implemented with Postgres advisory locks."
 license = "BSD-3-Clause"
 authors = ["Sean Kerr <sean@code-box.org>"]
 readme = "README.md"
 repository = "https://github.com/seankerr/py-postgres-lock"
 keywords = ["postgres", "postgresql", "distributed", "lock"]
 packages = [{include = "postgres_lock"}]
```

### Comparing `postgres_lock-0.1.2/PKG-INFO` & `postgres_lock-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres-lock
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lock mechanism implemented with Postgres advisory locks.
 Home-page: https://github.com/seankerr/py-postgres-lock
 License: BSD-3-Clause
 Keywords: postgres,postgresql,distributed,lock
 Author: Sean Kerr
 Author-email: sean@code-box.org
 Requires-Python: >=3.7,<4.0
@@ -191,13 +191,15 @@
 lock = Lock(conn, "shared-identifier", rollback_on_error=False)
 
 # do things with the lock
 ```
 
 ### Changelog
 
+- **0.1.3**
+  - Key can be any object
 - **0.1.2**
   - Add Lock.rollback_on_error (default true)
   - Add Lock.handle_error() & Lock.handle_error_async()
 - **0.1.1**
   - Key can be str or int
```

