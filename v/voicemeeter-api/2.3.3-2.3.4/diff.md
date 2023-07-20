# Comparing `tmp/voicemeeter_api-2.3.3.tar.gz` & `tmp/voicemeeter_api-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.3.3.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.3.4.tar", max compression
```

## Comparing `voicemeeter_api-2.3.3.tar` & `voicemeeter_api-2.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.3/LICENSE
--rw-r--r--   0        0        0     1102 2023-07-13 00:07:03.426961 voicemeeter_api-2.3.3/pyproject.toml
--rw-r--r--   0        0        0    18156 2023-07-11 18:43:59.775001 voicemeeter_api-2.3.3/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.3/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.3.3/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.3/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.3/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.3/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.3/voicemeeterlib/device.py
--rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.3/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.3/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.3/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.3/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.3/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2370 2023-07-12 04:22:12.387405 voicemeeter_api-2.3.3/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.3.3/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.3/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.3/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.3/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12215 2023-07-12 23:19:54.651350 voicemeeter_api-2.3.3/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-07-12 07:44:11.180313 voicemeeter_api-2.3.3/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.3/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-07-10 02:00:50.034407 voicemeeter_api-2.3.3/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2449 2023-07-12 10:43:20.524893 voicemeeter_api-2.3.3/voicemeeterlib/util.py
--rw-r--r--   0        0        0     6316 2023-07-12 10:43:20.525893 voicemeeter_api-2.3.3/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17969 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.4/LICENSE
+-rw-r--r--   0        0        0     1102 2023-07-20 10:11:55.345129 voicemeeter_api-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0    18957 2023-07-13 07:54:12.378858 voicemeeter_api-2.3.4/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.4/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.3.4/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.4/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.4/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.4/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.4/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.4/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.4/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.4/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.4/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.4/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.3.4/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1081 2023-07-14 11:53:50.976482 voicemeeter_api-2.3.4/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.4/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.4/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.4/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12072 2023-07-18 13:15:47.727817 voicemeeter_api-2.3.4/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15352 2023-07-14 11:51:40.640708 voicemeeter_api-2.3.4/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.4/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.3.4/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2436 2023-07-18 13:03:59.421646 voicemeeter_api-2.3.4/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.3.4/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.4/PKG-INFO
```

### Comparing `voicemeeter_api-2.3.3/LICENSE` & `voicemeeter_api-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/pyproject.toml` & `voicemeeter_api-2.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.3.3"
+version = "2.3.4"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.3.3/README.md` & `voicemeeter_api-2.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -736,15 +736,15 @@
 
 example:
 
 ```python
 import voicemeeterlib
 # Set event updates to occur every 50ms
 # Listen for level updates only
-with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True}) as vm:
+with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True) as vm:
     ...
 ```
 
 #### `vm.observer`
 
 Use the Subject class to register an app as event observer.
 
@@ -823,31 +823,57 @@
 vm.get('Strip[2].Mute')
 vm.set('Strip[4].Label', 'stripname')
 vm.set('Strip[0].Gain', -3.6)
 ```
 
 Access to lower level polling functions are provided with the following property objects:
 
-#### `vm.pdirty`
+##### `vm.pdirty`
 
 True iff a parameter has been updated.
 
-#### `vm.mdirty`
+##### `vm.mdirty`
 
 True iff a macrobutton has been updated.
 
-#### `vm.ldirty`
+##### `vm.ldirty`
 
 True iff a level has been updated.
 
 
+### Errors
+
+-   `errors.VMError`: Exception raised when general errors occur.
+-   `errors.InstallError`: Exception raised when installation errors occur.
+-   `errors.CAPIError`: Exception raised when the C-API returns error values.
+    -   Error codes are stored in {Exception Class}.code. For a full list of error codes [check the VoicemeeterRemote header file][Voicemeeter Remote Header].
+
+
+### Logging
+
+It's possible to see the messages sent by the interface's setters and getters, may be useful for debugging.
+
+example:
+```python
+import voicemeeterlib
+
+logging.basicConfig(level=logging.DEBUG)
+
+with voicemeeterlib.api("banana") as vm:
+        ...
+```
+
+
 ### Run tests
 
 To run all tests:
 
 ```
 pytest -v
 ```
 
 ### Official Documentation
 
 -   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)
+
+
+[Voicemeeter Remote Header]: https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemote.h
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/bus.py` & `voicemeeter_api-2.3.4/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.3.4/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/command.py` & `voicemeeter_api-2.3.4/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/config.py` & `voicemeeter_api-2.3.4/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/device.py` & `voicemeeter_api-2.3.4/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/error.py` & `voicemeeter_api-2.3.4/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/event.py` & `voicemeeter_api-2.3.4/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/factory.py` & `voicemeeter_api-2.3.4/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/inst.py` & `voicemeeter_api-2.3.4/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/iremote.py` & `voicemeeter_api-2.3.4/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/kinds.py` & `voicemeeter_api-2.3.4/voicemeeterlib/kinds.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,37 +28,45 @@
     ins: tuple
     outs: tuple
     vban: tuple
     asio: tuple
     insert: int
 
     @property
-    def phys_in(self):
+    def phys_in(self) -> int:
         return self.ins[0]
 
     @property
-    def virt_in(self):
+    def virt_in(self) -> int:
         return self.ins[-1]
 
     @property
-    def phys_out(self):
+    def phys_out(self) -> int:
         return self.outs[0]
 
     @property
-    def virt_out(self):
+    def virt_out(self) -> int:
         return self.outs[-1]
 
     @property
-    def num_strip(self):
+    def num_strip(self) -> int:
         return sum(self.ins)
 
     @property
-    def num_bus(self):
+    def num_bus(self) -> int:
         return sum(self.outs)
 
+    @property
+    def num_strip_levels(self) -> int:
+        return 2 * self.phys_in + 8 * self.virt_in
+
+    @property
+    def num_bus_levels(self) -> int:
+        return 8 * (self.phys_out + self.virt_out)
+
     def __str__(self) -> str:
         return self.name.capitalize()
 
 
 @dataclass
 class BasicMap(KindMapClass):
     name: str
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.3.4/voicemeeterlib/macrobutton.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
         return f"{type(self).__name__}{self._remote.kind}{self.index}"
 
     @property
     def state(self) -> bool:
         return self.getter(1) == 1
 
     @state.setter
-    def state(self, val):
+    def state(self, val: bool):
         self.setter(1 if val else 0, 1)
 
     @property
     def stateonly(self) -> bool:
         return self.getter(2) == 1
 
     @stateonly.setter
-    def stateonly(self, val):
+    def stateonly(self, val: bool):
         self.setter(1 if val else 0, 2)
 
     @property
     def trigger(self) -> bool:
         return self.getter(3) == 1
 
     @trigger.setter
-    def trigger(self, val):
+    def trigger(self, val: bool):
         self.setter(1 if val else 0, 3)
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/meta.py` & `voicemeeter_api-2.3.4/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/misc.py` & `voicemeeter_api-2.3.4/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/recorder.py` & `voicemeeter_api-2.3.4/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/remote.py` & `voicemeeter_api-2.3.4/voicemeeterlib/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import ctypes as ct
 import logging
 import time
 from abc import abstractmethod
 from queue import Queue
 from typing import Iterable, NoReturn, Optional, Union
 
@@ -240,20 +239,17 @@
     def _get_levels(self) -> Iterable:
         """
         returns both level arrays (strip_levels, bus_levels) BEFORE math conversion
         """
         return (
             tuple(
                 self.get_level(self.strip_mode, i)
-                for i in range(2 * self.kind.phys_in + 8 * self.kind.virt_in)
-            ),
-            tuple(
-                self.get_level(3, i)
-                for i in range(8 * (self.kind.phys_out + self.kind.virt_out))
+                for i in range(self.kind.num_strip_levels)
             ),
+            tuple(self.get_level(3, i) for i in range(self.kind.num_bus_levels)),
         )
 
     def get_midi_message(self):
         n = ct.c_long(1024)
         buf = ct.create_string_buffer(1024)
         res = self.call(
             self.vm_get_midi_message,
@@ -321,21 +317,21 @@
             }
             self.logger.debug(
                 f"profile '{name}' extends '{extended}', profiles merged.."
             )
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
+    def end_thread(self):
+        self.logger.debug("events thread shutdown started")
+        self.running = False
+
     def logout(self) -> NoReturn:
-        """Wait for dirty parameters to clear, then logout of the API"""
+        """Logout of the API"""
         time.sleep(0.1)
         self.call(self.vm_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
-    def end_thread(self):
-        self.logger.debug("events thread shutdown started")
-        self.running = False
-
     def __exit__(self, exc_type, exc_value, exc_traceback) -> NoReturn:
         """teardown procedures"""
         self.end_thread()
         self.logout()
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/strip.py` & `voicemeeter_api-2.3.4/voicemeeterlib/strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,33 +360,33 @@
         return int(self.getter("karaoke"))
 
     @k.setter
     def k(self, val: int):
         self.setter("karaoke", val)
 
     @property
-    def bass(self):
+    def bass(self) -> float:
         return round(self.getter("EQGain1"), 1)
 
     @bass.setter
     def bass(self, val: float):
         self.setter("EQGain1", val)
 
     @property
-    def mid(self):
+    def mid(self) -> float:
         return round(self.getter("EQGain2"), 1)
 
     @mid.setter
     def mid(self, val: float):
         self.setter("EQGain2", val)
 
     med = mid
 
     @property
-    def treble(self):
+    def treble(self) -> float:
         return round(self.getter("EQGain3"), 1)
 
     high = treble
 
     @treble.setter
     def treble(self, val: float):
         self.setter("EQGain3", val)
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/subject.py` & `voicemeeter_api-2.3.4/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/updater.py` & `voicemeeter_api-2.3.4/voicemeeterlib/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 
 
 class Updater(threading.Thread):
     def __init__(self, remote, queue):
         super().__init__(name="updater", daemon=True)
         self._remote = remote
         self.queue = queue
-        self._remote._strip_comp = [False] * (
-            2 * self._remote.kind.phys_in + 8 * self._remote.kind.virt_in
-        )
-        self._remote._bus_comp = [False] * (self._remote.kind.num_bus * 8)
+        self._remote._strip_comp = [False] * (self._remote.kind.num_strip_levels)
+        self._remote._bus_comp = [False] * (self._remote.kind.num_bus_levels)
         (
             self._remote.cache["strip_level"],
             self._remote.cache["bus_level"],
         ) = self._remote._get_levels()
         self.logger = logger.getChild(self.__class__.__name__)
 
     def _update_comps(self, strip_level, bus_level):
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/util.py` & `voicemeeter_api-2.3.4/voicemeeterlib/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import functools
 from itertools import zip_longest
 from typing import Iterator
 
 
 def polling(func):
     """
```

### Comparing `voicemeeter_api-2.3.3/voicemeeterlib/vban.py` & `voicemeeter_api-2.3.4/voicemeeterlib/vban.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,26 +131,23 @@
 
     @property
     def bit(self) -> int:
         return super(VbanInstream, self).bit
 
 
 class VbanAudioInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Audio Instream"""
 
 
 class VbanMidiInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Midi Instream"""
 
 
 class VbanTextInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Text Instream"""
 
 
 class VbanOutstream(VbanStream):
     """
     class representing a vban outstream
 
     Subclasses VbanStream
@@ -161,21 +158,19 @@
 
     @property
     def direction(self) -> str:
         return "out"
 
 
 class VbanAudioOutstream(VbanOutstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Audio Outstream"""
 
 
 class VbanMidiOutstream(VbanOutstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Midi Outstream"""
 
 
 def _make_stream_pair(remote, kind):
     num_instream, num_outstream, num_midi, num_text = kind.vban
 
     def _generate_streams(i, dir):
         """generator function for instream/outstream types"""
```

### Comparing `voicemeeter_api-2.3.3/PKG-INFO` & `voicemeeter_api-2.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.3.3
+Version: 2.3.4
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -753,15 +753,15 @@
 
 example:
 
 ```python
 import voicemeeterlib
 # Set event updates to occur every 50ms
 # Listen for level updates only
-with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True}) as vm:
+with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True) as vm:
     ...
 ```
 
 #### `vm.observer`
 
 Use the Subject class to register an app as event observer.
 
@@ -840,32 +840,57 @@
 vm.get('Strip[2].Mute')
 vm.set('Strip[4].Label', 'stripname')
 vm.set('Strip[0].Gain', -3.6)
 ```
 
 Access to lower level polling functions are provided with the following property objects:
 
-#### `vm.pdirty`
+##### `vm.pdirty`
 
 True iff a parameter has been updated.
 
-#### `vm.mdirty`
+##### `vm.mdirty`
 
 True iff a macrobutton has been updated.
 
-#### `vm.ldirty`
+##### `vm.ldirty`
 
 True iff a level has been updated.
 
 
+### Errors
+
+-   `errors.VMError`: Exception raised when general errors occur.
+-   `errors.InstallError`: Exception raised when installation errors occur.
+-   `errors.CAPIError`: Exception raised when the C-API returns error values.
+    -   Error codes are stored in {Exception Class}.code. For a full list of error codes [check the VoicemeeterRemote header file][Voicemeeter Remote Header].
+
+
+### Logging
+
+It's possible to see the messages sent by the interface's setters and getters, may be useful for debugging.
+
+example:
+```python
+import voicemeeterlib
+
+logging.basicConfig(level=logging.DEBUG)
+
+with voicemeeterlib.api("banana") as vm:
+        ...
+```
+
+
 ### Run tests
 
 To run all tests:
 
 ```
 pytest -v
 ```
 
 ### Official Documentation
 
 -   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)
 
+
+[Voicemeeter Remote Header]: https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemote.h
```

