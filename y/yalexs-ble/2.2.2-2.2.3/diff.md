# Comparing `tmp/yalexs_ble-2.2.2.tar.gz` & `tmp/yalexs_ble-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs_ble-2.2.2.tar", max compression
+gzip compressed data, was "yalexs_ble-2.2.3.tar", max compression
```

## Comparing `yalexs_ble-2.2.2.tar` & `yalexs_ble-2.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-07-20 00:36:02.513116 yalexs_ble-2.2.2/LICENSE
--rw-r--r--   0        0        0     3663 2023-07-20 00:36:02.513116 yalexs_ble-2.2.2/README.md
--rw-r--r--   0        0        0     2419 2023-07-20 00:36:03.541130 yalexs_ble-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      871 2023-07-20 00:36:03.505130 yalexs_ble-2.2.2/src/yalexs_ble/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-20 00:36:02.513116 yalexs_ble-2.2.2/src/yalexs_ble/const.py
--rw-r--r--   0        0        0    16785 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/lock.py
--rw-r--r--   0        0        0    39986 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/push.py
--rw-r--r--   0        0        0        0 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/py.typed
--rw-r--r--   0        0        0     2324 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/secure_session.py
--rw-r--r--   0        0        0    11250 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/session.py
--rw-r--r--   0        0        0     2642 2023-07-20 00:36:02.517116 yalexs_ble-2.2.2/src/yalexs_ble/util.py
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 yalexs_ble-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/LICENSE
+-rw-r--r--   0        0        0     3663 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/README.md
+-rw-r--r--   0        0        0     2447 2023-07-20 16:59:04.659253 yalexs_ble-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0      871 2023-07-20 16:59:04.627252 yalexs_ble-2.2.3/src/yalexs_ble/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/const.py
+-rw-r--r--   0        0        0    16785 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/lock.py
+-rw-r--r--   0        0        0    39986 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/push.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/py.typed
+-rw-r--r--   0        0        0     2324 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/secure_session.py
+-rw-r--r--   0        0        0    10181 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/session.py
+-rw-r--r--   0        0        0     2642 2023-07-20 16:59:03.739238 yalexs_ble-2.2.3/src/yalexs_ble/util.py
+-rw-r--r--   0        0        0     5171 1970-01-01 00:00:00.000000 yalexs_ble-2.2.3/PKG-INFO
```

### Comparing `yalexs_ble-2.2.2/LICENSE` & `yalexs_ble-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/README.md` & `yalexs_ble-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/pyproject.toml` & `yalexs_ble-2.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yalexs-ble"
-version = "2.2.2"
+version = "2.2.3"
 description = "Bluetooth control of Yale and August locks"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/yalexs-ble"
 documentation = "https://yalexs-ble.readthedocs.io"
 classifiers = [
@@ -30,14 +30,15 @@
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 bleak = ">=0.19.0"
 bleak-retry-connector = ">=2.9.0"
 async-timeout = ">=3.0.1"
 cryptography = ">=38.0.0"
 lru-dict = ">=1.1.4"
+async-interrupt = ">=1.1.1"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/__init__.py` & `yalexs_ble-2.2.3/src/yalexs_ble/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     local_name_is_unique,
     local_name_to_serial,
     serial_to_local_name,
     unique_id_from_device_adv,
     unique_id_from_local_name_address,
 )
 
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 
 __all__ = [
     "AuthError",
     "ConnectionInfo",
     "DisconnectedError",
     "DoorStatus",
     "Lock",
```

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/const.py` & `yalexs_ble-2.2.3/src/yalexs_ble/const.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/lock.py` & `yalexs_ble-2.2.3/src/yalexs_ble/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/push.py` & `yalexs_ble-2.2.3/src/yalexs_ble/push.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/secure_session.py` & `yalexs_ble-2.2.3/src/yalexs_ble/secure_session.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/session.py` & `yalexs_ble-2.2.3/src/yalexs_ble/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import time
-from functools import partial
-from typing import Any, Callable
+from typing import Callable
 
 import async_timeout
+from async_interrupt import interrupt
 from bleak import BleakClient
 from bleak_retry_connector import BleakError
 from cryptography.hazmat.primitives.ciphers import (
     Cipher,
     CipherContext,
     algorithms,
     modes,
@@ -44,19 +44,14 @@
     """No advertisement data."""
 
 
 class BluetoothError(YaleXSBLEError):
     """Bluetooth error."""
 
 
-def _on_disconnected(task: asyncio.Task[Any], fut: asyncio.Future[None]) -> None:
-    if task and not task.done():
-        task.cancel()
-
-
 class Session:
     _write_characteristic = WRITE_CHARACTERISTIC
     _read_characteristic = READ_CHARACTERISTIC
 
     def __init__(
         self,
         client: BleakClient,
@@ -263,42 +258,23 @@
             # it means a battery pull is required to recover.
             await asyncio.sleep(COOLDOWN_TIME - cooldown_remain)
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         self._write_checksum(command)
         disconnected_future = asyncio.get_running_loop().create_future()
         disconnected_futures = self._disconnected_futures
         disconnected_futures.add(disconnected_future)
-        task = asyncio.current_task()
-        disconnected_callback = partial(_on_disconnected, task)
-        disconnected_future.add_done_callback(disconnected_callback)
         try:
-            return await self._write(command, command_name)
+            async with interrupt(
+                disconnected_future, DisconnectedError, f"{self.name}: Disconnected"
+            ):
+                return await self._write(command, command_name)
         except BleakError as err:
             if self._first_request and util.is_key_error(err):
                 raise AuthError(
                     f"Authentication error: key or slot (key index) is incorrect: {err}"
                 ) from err
             if util.is_disconnected_error(err):
                 raise DisconnectedError(f"{self.name}: {err}") from err
             raise
-        except asyncio.CancelledError:
-            if not disconnected_future.done():
-                # If we get cancelled and the disconnect callback hasn't
-                # been called yet, it came from somewhere else and we should
-                # raise to propagate it
-                raise
-            _LOGGER.debug(
-                "%s: `%s` cancelled due to disconnect during write",
-                self.name,
-                command_name,
-            )
-            # On python 3.11+ we use task.uncancel()
-            # since we catch the CancelledError
-            if uncancel := getattr(task, "uncancel", None):
-                uncancel()
-            # Do not propagate the cancellation to the caller
-            # with from exception chaining
-            raise DisconnectedError(f"{self.name}: Disconnected")
         finally:
             disconnected_futures.discard(disconnected_future)
-            disconnected_future.remove_done_callback(disconnected_callback)
             self._first_request = False
```

### Comparing `yalexs_ble-2.2.2/src/yalexs_ble/util.py` & `yalexs_ble-2.2.3/src/yalexs_ble/util.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.2/PKG-INFO` & `yalexs_ble-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs-ble
-Version: 2.2.2
+Version: 2.2.3
 Summary: Bluetooth control of Yale and August locks
 Home-page: https://github.com/bdraco/yalexs-ble
 License: GNU General Public License v3.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
+Requires-Dist: async-interrupt (>=1.1.1)
 Requires-Dist: async-timeout (>=3.0.1)
 Requires-Dist: bleak (>=0.19.0)
 Requires-Dist: bleak-retry-connector (>=2.9.0)
 Requires-Dist: cryptography (>=38.0.0)
 Requires-Dist: lru-dict (>=1.1.4)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: yalexs-ble Version: 2.2.2 Summary: Bluetooth
+Metadata-Version: 2.1 Name: yalexs-ble Version: 2.2.3 Summary: Bluetooth
 control of Yale and August locks Home-page: https://github.com/bdraco/yalexs-
 ble License: GNU General Public License v3.0 Author: J. Nick Koston Author-
 email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Provides-
 Extra: docs Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist:
-async-timeout (>=3.0.1) Requires-Dist: bleak (>=0.19.0) Requires-Dist: bleak-
-retry-connector (>=2.9.0) Requires-Dist: cryptography (>=38.0.0) Requires-Dist:
-lru-dict (>=1.1.4) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug
-Tracker, https://github.com/bdraco/yalexs-ble/issues Project-URL: Changelog,
-https://github.com/bdraco/yalexs-ble/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://yalexs-ble.readthedocs.io Project-URL: Repository,
-https://github.com/bdraco/yalexs-ble Description-Content-Type: text/markdown #
-Yale Access BLE
+async-interrupt (>=1.1.1) Requires-Dist: async-timeout (>=3.0.1) Requires-Dist:
+bleak (>=0.19.0) Requires-Dist: bleak-retry-connector (>=2.9.0) Requires-Dist:
+cryptography (>=38.0.0) Requires-Dist: lru-dict (>=1.1.4) Requires-Dist: myst-
+parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: sphinx-rtd-theme
+(>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://github.com/
+bdraco/yalexs-ble/issues Project-URL: Changelog, https://github.com/bdraco/
+yalexs-ble/blob/main/CHANGELOG.md Project-URL: Documentation, https://yalexs-
+ble.readthedocs.io Project-URL: Repository, https://github.com/bdraco/yalexs-
+ble Description-Content-Type: text/markdown # Yale Access BLE
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Bluetooth control of Yale and August locks ## Installation Install this via pip
 (or your favourite package manager): `pip install yalexs-ble` ## Fork history
 Thanks to: https://github.com/Friendly0Fire/augustpy https://github.com/
 terrcin/augustctl https://github.com/ethitter/augustctl https://github.com/
```

