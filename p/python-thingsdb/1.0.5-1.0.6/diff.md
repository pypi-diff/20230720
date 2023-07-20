# Comparing `tmp/python-thingsdb-1.0.5.tar.gz` & `tmp/python-thingsdb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-thingsdb-1.0.5.tar", last modified: Fri Nov 11 21:50:12 2022, max compression
+gzip compressed data, was "python-thingsdb-1.0.6.tar", last modified: Thu Jul 20 18:05:01 2023, max compression
```

## Comparing `python-thingsdb-1.0.5.tar` & `python-thingsdb-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/
--rw-rw-r--   0 joente    (1000) joente    (1000)    21342 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)    15860 2022-11-11 21:19:00.000000 python-thingsdb-1.0.5/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)    21342 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      631 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       20 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        9 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/python_thingsdb.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2022-11-11 21:20:06.000000 python-thingsdb-1.0.5/setup.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/thingsdb/
--rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.0.5/thingsdb/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/thingsdb/client/
--rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.0.5/thingsdb/client/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    13659 2021-09-10 14:49:48.000000 python-thingsdb-1.0.5/thingsdb/client/buildin.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    24581 2022-10-14 16:12:31.000000 python-thingsdb-1.0.5/thingsdb/client/client.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1848 2021-09-22 12:02:58.000000 python-thingsdb-1.0.5/thingsdb/client/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8317 2021-09-22 12:02:58.000000 python-thingsdb-1.0.5/thingsdb/client/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.0.5/thingsdb/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/thingsdb/room/
--rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.0.5/thingsdb/room/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.0.5/thingsdb/room/event.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.0.5/thingsdb/room/room.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8547 2022-11-11 21:46:34.000000 python-thingsdb-1.0.5/thingsdb/room/roombase.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-11-11 21:50:12.000000 python-thingsdb-1.0.5/thingsdb/util/
--rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.0.5/thingsdb/util/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.0.5/thingsdb/util/access.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.0.5/thingsdb/util/cleancode.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.0.5/thingsdb/util/cnscope.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      501 2022-08-31 12:17:56.000000 python-thingsdb-1.0.5/thingsdb/util/id.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2022-11-11 21:49:24.000000 python-thingsdb-1.0.5/thingsdb/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.381265 python-thingsdb-1.0.6/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.373265 python-thingsdb-1.0.6/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.373265 python-thingsdb-1.0.6/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      679 2021-09-17 13:27:25.000000 python-thingsdb-1.0.6/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)      119 2021-09-14 09:36:12.000000 python-thingsdb-1.0.6/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1066 2019-12-20 12:14:05.000000 python-thingsdb-1.0.6/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)    16611 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)    15886 2022-11-11 21:53:28.000000 python-thingsdb-1.0.6/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.373265 python-thingsdb-1.0.6/examples/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.373265 python-thingsdb-1.0.6/examples/bookstore/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3377 2022-02-23 09:48:18.000000 python-thingsdb-1.0.6/examples/bookstore/webserver.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/python_thingsdb.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)    16611 2023-07-20 18:05:00.000000 python-thingsdb-1.0.6/python_thingsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      741 2023-07-20 18:05:01.000000 python-thingsdb-1.0.6/python_thingsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-07-20 18:05:00.000000 python-thingsdb-1.0.6/python_thingsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       20 2023-07-20 18:05:01.000000 python-thingsdb-1.0.6/python_thingsdb.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        9 2023-07-20 18:05:01.000000 python-thingsdb-1.0.6/python_thingsdb.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       27 2019-12-17 14:25:00.000000 python-thingsdb-1.0.6/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-07-20 18:05:01.381265 python-thingsdb-1.0.6/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2023-02-10 12:47:09.000000 python-thingsdb-1.0.6/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      800 2022-11-11 21:22:06.000000 python-thingsdb-1.0.6/test_thingsdb.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/thingsdb/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.0.6/thingsdb/__init__.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/thingsdb/client/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.0.6/thingsdb/client/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    13730 2023-05-01 14:12:23.000000 python-thingsdb-1.0.6/thingsdb/client/buildin.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    24589 2023-07-20 17:59:07.000000 python-thingsdb-1.0.6/thingsdb/client/client.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1851 2023-07-20 17:58:48.000000 python-thingsdb-1.0.6/thingsdb/client/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8317 2021-09-22 12:02:58.000000 python-thingsdb-1.0.6/thingsdb/client/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.0.6/thingsdb/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/thingsdb/room/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.0.6/thingsdb/room/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.0.6/thingsdb/room/event.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.0.6/thingsdb/room/room.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8704 2023-07-20 17:58:48.000000 python-thingsdb-1.0.6/thingsdb/room/roombase.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-20 18:05:01.377265 python-thingsdb-1.0.6/thingsdb/util/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.0.6/thingsdb/util/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.0.6/thingsdb/util/access.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.0.6/thingsdb/util/cleancode.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.0.6/thingsdb/util/cnscope.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      501 2023-07-20 17:58:21.000000 python-thingsdb-1.0.6/thingsdb/util/id.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-07-20 18:03:49.000000 python-thingsdb-1.0.6/thingsdb/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-thingsdb-1.0.5/README.md` & `python-thingsdb-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     * [wait_closed](#wait_closed)
   * [Room](#room)
     * [methods](#room-methods)
     * [properties](#room-properties)
     * [join](#join)
     * [leave](#leave)
     * [emit](#emit)
+    * [no_join](#no_join)
   * [Failed packages](#failed-packages)
 ---------------------------------------
 
 ## Installation
 
 Just use pip:
```

### Comparing `python-thingsdb-1.0.5/python_thingsdb.egg-info/SOURCES.txt` & `python-thingsdb-1.0.6/python_thingsdb.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+.gitignore
+LICENSE
 README.md
+requirements.txt
 setup.py
+test_thingsdb.py
+.github/workflows/ci.yml
+examples/bookstore/webserver.py
 python_thingsdb.egg-info/PKG-INFO
 python_thingsdb.egg-info/SOURCES.txt
 python_thingsdb.egg-info/dependency_links.txt
 python_thingsdb.egg-info/requires.txt
 python_thingsdb.egg-info/top_level.txt
 thingsdb/__init__.py
 thingsdb/exceptions.py
```

### Comparing `python-thingsdb-1.0.5/setup.py` & `python-thingsdb-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.5/thingsdb/client/buildin.py` & `python-thingsdb-1.0.6/thingsdb/client/buildin.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     async def del_module(self, name: str):
         """Delete a module. A SIGTERM signal will be send to the process for
         the module which might cancel running futures.
 
         This function generates a change.
         """
-        return await self.query('del_module(key)', name=name, scope='@t')
+        return await self.query('del_module(name)', name=name, scope='@t')
 
     async def del_node(self, node_id: int):
         """Delete a node from ThingsDB.
 
         Before deleting a node, the node must be offline. As long is the node
         is active, you are not allowed to delete the node. See shutdown for
         shutting down a node by using a query.
@@ -368,15 +368,20 @@
         deploy_module(name, None) function with None as second argument.
 
         This function does not generate a change.
         """
         return await self.query('restart_module(name)', name=name, scope='@t')
 
     async def set_log_level(self, log_level: str, scope='@n') -> None:
-        assert log_level in ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL')
+        log_level = (
+            'DEBUG',
+            'INFO',
+            'WARNING',
+            'ERROR',
+            'CRITICAL').index(log_level)
         return await self.query(
             'set_log_level(log_level)', log_level=log_level, scope=scope)
 
     async def shutdown(self, scope='@n') -> None:
         """Shutdown the node in the selected scope.
 
         This is a clean shutdown, allowing all other nodes (and clients) to
```

### Comparing `python-thingsdb-1.0.5/thingsdb/client/client.py` & `python-thingsdb-1.0.6/thingsdb/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
                 used. Defaults to `None`.
         """
 
         self._loop = loop if loop else asyncio.get_event_loop()
         self._auth = None
         self._pool = None
         self._protocol = None
-        self._pid = 0
         self._write_pkg = self._ensure_write if auto_reconnect else self._write
         self._reconnect = auto_reconnect
         self._scope = '@t'  # default to thingsdb scope
         self._pool_idx = 0
         self._reconnecting = False
         self._rooms = dict()
         self._rooms_lock = asyncio.Lock()
@@ -558,15 +557,15 @@
             self._pool_idx %= len(self._pool)
 
     async def _on_room(self, room_id, pkg):
         async with self._rooms_lock:
             try:
                 room = self._rooms[room_id]
             except KeyError:
-                logging.warn(
+                logging.warning(
                     f'Got an event (tp:{pkg.tp}) for room Id {room_id} but '
                     f'the room is not known by the ThingsDB client')
             else:
                 task = room._on_event(pkg)
                 if isinstance(task, asyncio.Task):
                     await task
 
@@ -582,19 +581,20 @@
             return
 
         try:
             room_id = pkg.data['id']
         except KeyError:
             if pkg.tp == Proto.ON_WARN:
                 warn = pkg.data
-                logging.warn(
+                logging.warning(
                     f'ThingsDB: '
                     f'{warn["warn_msg"]} ({warn["warn_code"]})')
             else:
-                logging.warn(f'Unexpected event: tp:{pkg.tp} data:{pkg.data}')
+                logging.warning(
+                    f'Unexpected event: tp:{pkg.tp} data:{pkg.data}')
         else:
             asyncio.ensure_future(self._on_room(room_id, pkg), loop=self._loop)
 
     def _on_connection_lost(self, protocol, exc):
         if self._protocol is not protocol:
             return
         self._protocol = None
```

### Comparing `python-thingsdb-1.0.5/thingsdb/client/package.py` & `python-thingsdb-1.0.6/thingsdb/client/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 try:
                     with open(_fail_file, 'wb') as f:
                         f.write(
                             barray[self.__class__.st_package.size:self.total])
                 except Exception:
                     logging.exception('')
                 else:
-                    logging.warn(
+                    logging.warning(
                         f'Wrote the content from {self} to `{_fail_file}`')
             raise e
         finally:
             del barray[:self.total]
 
     def __repr__(self) -> str:
         return '<id: {0.pid} size: {0.length} tp: {0.tp}>'.format(self)
```

### Comparing `python-thingsdb-1.0.5/thingsdb/client/protocol.py` & `python-thingsdb-1.0.6/thingsdb/client/protocol.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.5/thingsdb/exceptions.py` & `python-thingsdb-1.0.6/thingsdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.5/thingsdb/room/room.py` & `python-thingsdb-1.0.6/thingsdb/room/room.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.5/thingsdb/room/roombase.py` & `python-thingsdb-1.0.6/thingsdb/room/roombase.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 Examples are:
                    - 123
                    - '.my_room.id();'
             scope (str):
                 Collection scope. If no scope is given, the scope will later
                 be set to the default client scope once the room is joined.
         """
-        self._client = None
+        self._client: Optional[Client] = None
         self._id = room
         self._scope = scope
         self._wait_join = False
 
     @property
     def id(self):
         return self._id if isinstance(self._id, int) else None
@@ -117,15 +117,15 @@
                 assert isinstance(self._id, int)
                 res = await client._join(self._id, scope=self._scope)
                 if res[0] is None:
                     raise LookupError(f'room with Id {self._id} not found')
 
             if self._id in client._rooms:
                 prev = client._rooms[self._id]
-                logging.warn(
+                logging.warning(
                     f'Room Id {self._id} is previously registered by {prev} '
                     f'and will be overwritten with {self}')
 
             client._rooms[self._id] = self
             self.on_init()
             if wait:
                 self._wait_join = asyncio.Future()
@@ -157,14 +157,17 @@
                 Additional argument to send with the event.
 
         Returns:
             asyncio.Future (None):
                 Future which should be awaited. The result of the future will
                 be set to `None` when successful.
         """
+        if self._client is None:
+            raise RuntimeError(
+                'must call join(..) or no_join(..) before using emit')
         return self._client._emit(self._id, event, *args, scope=self._scope)
 
     def _on_event(self, pkg) -> Optional[asyncio.Task]:
         return self.__class__._ROOM_EVENT_MAP[pkg.tp](self, pkg.data)
 
     @abc.abstractmethod
     def on_init(self) -> None:
```

### Comparing `python-thingsdb-1.0.5/thingsdb/util/cnscope.py` & `python-thingsdb-1.0.6/thingsdb/util/cnscope.py`

 * *Files identical despite different names*

