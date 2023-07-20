# Comparing `tmp/sdss_clu-2.1.1.tar.gz` & `tmp/sdss_clu-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.1.1.tar", max compression
+gzip compressed data, was "sdss_clu-2.1.2.tar", max compression
```

## Comparing `sdss_clu-2.1.1.tar` & `sdss_clu-2.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1504 2023-07-13 23:14:45.798150 sdss_clu-2.1.1/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-07-13 23:14:45.798512 sdss_clu-2.1.1/README.rst
--rw-r--r--   0        0        0     2774 2023-07-13 23:14:45.810979 sdss_clu-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      889 2023-07-13 23:14:45.811399 sdss_clu-2.1.1/python/clu/__init__.py
--rwxr-xr-x   0        0        0     9086 2023-07-13 23:14:45.811650 sdss_clu-2.1.1/python/clu/__main__.py
--rw-r--r--   0        0        0    13556 2023-07-13 23:14:45.811913 sdss_clu-2.1.1/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-07-13 23:14:45.812217 sdss_clu-2.1.1/python/clu/base.py
--rw-r--r--   0        0        0    14705 2023-07-13 23:14:45.812519 sdss_clu-2.1.1/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-07-13 23:14:45.812815 sdss_clu-2.1.1/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-07-13 23:14:45.813191 sdss_clu-2.1.1/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-07-13 23:14:45.813419 sdss_clu-2.1.1/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-07-13 23:14:45.813698 sdss_clu-2.1.1/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-07-13 23:14:45.813988 sdss_clu-2.1.1/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-07-13 23:14:45.814278 sdss_clu-2.1.1/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-07-13 23:14:45.814482 sdss_clu-2.1.1/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-07-13 23:14:45.814714 sdss_clu-2.1.1/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-07-13 23:14:45.815022 sdss_clu-2.1.1/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-07-13 23:14:45.815432 sdss_clu-2.1.1/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-07-13 23:14:45.815729 sdss_clu-2.1.1/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-07-13 23:14:45.816023 sdss_clu-2.1.1/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-07-13 23:14:45.816385 sdss_clu-2.1.1/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-07-13 23:14:45.817092 sdss_clu-2.1.1/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-07-13 23:14:45.817627 sdss_clu-2.1.1/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-07-13 23:14:45.818414 sdss_clu-2.1.1/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-07-13 23:14:45.818724 sdss_clu-2.1.1/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-07-13 23:14:45.818955 sdss_clu-2.1.1/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-07-13 23:14:45.819238 sdss_clu-2.1.1/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11789 2023-07-13 23:14:45.819534 sdss_clu-2.1.1/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-07-13 23:14:45.819946 sdss_clu-2.1.1/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-07-13 23:14:45.824817 sdss_clu-2.1.1/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-07-13 23:14:45.825170 sdss_clu-2.1.1/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-07-13 23:14:45.825509 sdss_clu-2.1.1/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-07-13 23:14:45.825788 sdss_clu-2.1.1/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-07-13 23:14:45.826117 sdss_clu-2.1.1/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-07-13 23:14:45.826432 sdss_clu-2.1.1/python/clu/tools.py
--rw-r--r--   0        0        0     3648 2023-07-13 23:14:45.826802 sdss_clu-2.1.1/python/clu/websocket.py
--rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-20 15:34:14.327438 sdss_clu-2.1.2/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-07-20 15:34:14.408466 sdss_clu-2.1.2/README.rst
+-rw-r--r--   0        0        0     2774 2023-07-20 15:34:17.207379 sdss_clu-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-07-20 15:34:17.328344 sdss_clu-2.1.2/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     9086 2023-07-20 15:34:17.449005 sdss_clu-2.1.2/python/clu/__main__.py
+-rw-r--r--   0        0        0    13556 2023-07-20 15:34:17.569279 sdss_clu-2.1.2/python/clu/actor.py
+-rw-r--r--   0        0        0    19832 2023-07-20 15:34:17.609935 sdss_clu-2.1.2/python/clu/base.py
+-rw-r--r--   0        0        0    14706 2023-07-20 15:34:17.690889 sdss_clu-2.1.2/python/clu/client.py
+-rw-r--r--   0        0        0    20069 2023-07-20 15:34:17.731289 sdss_clu-2.1.2/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-07-20 15:34:17.851501 sdss_clu-2.1.2/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-07-20 15:34:17.932576 sdss_clu-2.1.2/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-07-20 15:34:17.973459 sdss_clu-2.1.2/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    17892 2023-07-20 15:34:18.054967 sdss_clu-2.1.2/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-07-20 15:34:18.096028 sdss_clu-2.1.2/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-07-20 15:34:18.177534 sdss_clu-2.1.2/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-07-20 15:34:18.177887 sdss_clu-2.1.2/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-07-20 15:34:18.218575 sdss_clu-2.1.2/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-07-20 15:34:18.299383 sdss_clu-2.1.2/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-07-20 15:34:18.423132 sdss_clu-2.1.2/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-07-20 15:34:18.464332 sdss_clu-2.1.2/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-07-20 15:34:18.546530 sdss_clu-2.1.2/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-07-20 15:34:18.671963 sdss_clu-2.1.2/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-07-20 15:34:18.795903 sdss_clu-2.1.2/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-07-20 15:34:18.837071 sdss_clu-2.1.2/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-07-20 15:34:18.917938 sdss_clu-2.1.2/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-07-20 15:34:18.958843 sdss_clu-2.1.2/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-07-20 15:34:19.040751 sdss_clu-2.1.2/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11789 2023-07-20 15:34:19.081647 sdss_clu-2.1.2/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-07-20 15:34:19.163983 sdss_clu-2.1.2/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20428 2023-07-20 15:34:19.204399 sdss_clu-2.1.2/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-07-20 15:34:19.287197 sdss_clu-2.1.2/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-07-20 15:34:19.328753 sdss_clu-2.1.2/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-07-20 15:34:19.411667 sdss_clu-2.1.2/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-07-20 15:34:19.453190 sdss_clu-2.1.2/python/clu/testing.py
+-rw-r--r--   0        0        0    16901 2023-07-20 15:34:19.535400 sdss_clu-2.1.2/python/clu/tools.py
+-rw-r--r--   0        0        0     3648 2023-07-20 15:34:19.576545 sdss_clu-2.1.2/python/clu/websocket.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.2/PKG-INFO
```

### Comparing `sdss_clu-2.1.1/LICENSE.md` & `sdss_clu-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/README.rst` & `sdss_clu-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/pyproject.toml` & `sdss_clu-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.1.1"
+version = "2.1.2"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
@@ -30,15 +30,15 @@
 python = "^3.8,<4.0"
 click = "^8.0"
 aio_pika = "^9.0.0"
 jsonschema = "^4.0.1"
 sdsstools = "^1.0.0"
 prompt_toolkit = "^3.0.6"
 aiormq = "^6.6.4"
-unclick = "^0.1.0b4"
+unclick = "^0.1.0b5"
 websockets = {version = "^11.0.3", optional = true}
 click-default-group = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
```

### Comparing `sdss_clu-2.1.1/python/clu/__init__.py` & `sdss_clu-2.1.2/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/__main__.py` & `sdss_clu-2.1.2/python/clu/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/actor.py` & `sdss_clu-2.1.2/python/clu/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.commands_queue = await self.connection.add_queue(
             f"{self.name}_commands",
             callback=self.new_command,
             bindings=[f"command.{self.name}.#"],
         )
 
         self.log.debug(
-            f"commands queue {self.commands_queue.name!r} "
+            f"Commands queue {self.commands_queue.name!r} "
             f"bound to {self.connection.connection.url!s}"
         )
 
         self.timed_commands.start()
 
         return self
```

### Comparing `sdss_clu-2.1.1/python/clu/base.py` & `sdss_clu-2.1.2/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/client.py` & `sdss_clu-2.1.2/python/clu/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         if self.connection.connection:
             assert isinstance(self.connection.connection, apika.Connection)
             url = self.connection.connection.url
         else:
             url = "???"
 
-        self.log.info(f"replies queue {self.replies_queue.name!r} bound to {url!s}")
+        self.log.debug(f"Replies queue {self.replies_queue.name!r} bound to {url!s}")
 
         # Initialises the models.
         await self.models.load_schemas()
 
         return self
 
     async def stop(self):
```

### Comparing `sdss_clu-2.1.1/python/clu/command.py` & `sdss_clu-2.1.2/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/device.py` & `sdss_clu-2.1.2/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/exceptions.py` & `sdss_clu-2.1.2/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/actor.py` & `sdss_clu-2.1.2/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/tron.py` & `sdss_clu-2.1.2/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/html.py` & `sdss_clu-2.1.2/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/keys.py` & `sdss_clu-2.1.2/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/messages.py` & `sdss_clu-2.1.2/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/parser.py` & `sdss_clu-2.1.2/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.1.2/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.1.2/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.1.2/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.1.2/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.1.2/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/pvt.py` & `sdss_clu-2.1.2/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/legacy/types/types.py` & `sdss_clu-2.1.2/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/model.py` & `sdss_clu-2.1.2/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/parsers/click.py` & `sdss_clu-2.1.2/python/clu/parsers/click.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/parsers/json.py` & `sdss_clu-2.1.2/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/protocol.py` & `sdss_clu-2.1.2/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/store.py` & `sdss_clu-2.1.2/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/testing.py` & `sdss_clu-2.1.2/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/tools.py` & `sdss_clu-2.1.2/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/python/clu/websocket.py` & `sdss_clu-2.1.2/python/clu/websocket.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.1/PKG-INFO` & `sdss_clu-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.1.1
+Version: 2.1.2
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -24,15 +24,15 @@
 Requires-Dist: aio_pika (>=9.0.0,<10.0.0)
 Requires-Dist: aiormq (>=6.6.4,<7.0.0)
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: jsonschema (>=4.0.1,<5.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.6,<4.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
-Requires-Dist: unclick (>=0.1.0b4,<0.2.0)
+Requires-Dist: unclick (>=0.1.0b5,<0.2.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0) ; extra == "websocket"
 Project-URL: Documentation, https://clu.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/clu
 Description-Content-Type: text/x-rst
 
 `CLU <https://tron.fandom.com/wiki/Clu>`__
 ==========================================
```

