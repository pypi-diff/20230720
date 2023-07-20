# Comparing `tmp/adsbcot-6.0.0.tar.gz` & `tmp/adsbcot-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-6.0.0.tar", last modified: Sat Jun 10 03:17:47 2023, max compression
+gzip compressed data, was "adsbcot-6.1.0.tar", last modified: Thu Jul 20 19:54:10 2023, max compression
```

## Comparing `adsbcot-6.0.0.tar` & `adsbcot-6.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.043357 adsbcot-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-10 03:17:36.000000 adsbcot-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 03:17:36.000000 adsbcot-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-10 03:17:47.043357 adsbcot-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-10 03:17:36.000000 adsbcot-6.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.039357 adsbcot-6.0.0/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.043357 adsbcot-6.0.0/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 03:17:47.000000 adsbcot-6.0.0/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-10 03:17:47.043357 adsbcot-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-10 03:17:36.000000 adsbcot-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:54:10.910112 adsbcot-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-20 19:53:56.000000 adsbcot-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 19:53:56.000000 adsbcot-6.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-20 19:54:10.910112 adsbcot-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-20 19:53:56.000000 adsbcot-6.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:54:10.910112 adsbcot-6.1.0/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 19:53:56.000000 adsbcot-6.1.0/adsbcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-07-20 19:53:56.000000 adsbcot-6.1.0/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-20 19:53:56.000000 adsbcot-6.1.0/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-20 19:53:56.000000 adsbcot-6.1.0/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-20 19:53:56.000000 adsbcot-6.1.0/adsbcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:54:10.910112 adsbcot-6.1.0/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 19:54:10.000000 adsbcot-6.1.0/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-20 19:54:10.914112 adsbcot-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-20 19:53:56.000000 adsbcot-6.1.0/setup.py
```

### Comparing `adsbcot-6.0.0/LICENSE` & `adsbcot-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adsbcot-6.0.0/PKG-INFO` & `adsbcot-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.0.0
+Version: 6.1.0
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.0.0/README.rst` & `adsbcot-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adsbcot-6.0.0/adsbcot/__init__.py` & `adsbcot-6.1.0/adsbcot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """ADS-B to TAK Gateway.
 
 :author: Greg Albrecht <gba@snstac.com>
 :source: <https://github.com/snstac/adsbcot>
 """
 
-__version__ = "6.0.0"
+__version__ = "6.1.0"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 # Python 3.6 test/build work-around:
 try:
     from .constants import (  # NOQA
```

### Comparing `adsbcot-6.0.0/adsbcot/classes.py` & `adsbcot-6.1.0/adsbcot/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import importlib.util
 import json
 import os
 import warnings
 
 from pathlib import Path
 from typing import Optional
-from urllib.parse import ParseResult, urlparse
+from urllib.parse import ParseResult, ParseResultBytes, urlparse
 
 import aiohttp
 import pytak
 import aircot
 import adsbcot
 
 
@@ -119,15 +119,19 @@
                 continue
 
             self._logger.debug("Handling %s/%s ICAO: %s", i, lod, icao)
             await self.put_queue(event)
 
     async def get_feed(self, url: bytes) -> None:
         """Poll the ADS-B feed and pass data to the data handler."""
-        async with self.session.get(url) as resp:
+        if not self.session:
+            return
+
+        url_b = str(url)
+        async with self.session.get(url_b) as resp:
             if resp.status != 200:
                 response_content = await resp.text()
                 self._logger.error("Received HTTP Status %s for %s", resp.status, url)
                 self._logger.error(response_content)
                 return
 
             json_resp = await resp.json()
@@ -162,41 +166,49 @@
             "POLL_INTERVAL", adsbcot.DEFAULT_POLL_INTERVAL
         )
 
         if known_craft:
             self._logger.info("Using KNOWN_CRAFT: %s", known_craft)
             self.known_craft_db = aircot.read_known_craft(known_craft)
 
-        feed_url: ParseResult = urlparse(url)
+        alt_upper: int = int(self.config.get("ALT_UPPER", "0"))
+        alt_lower: int = int(self.config.get("ALT_LOWER", "0"))
+        if alt_upper or alt_lower:
+            self._logger.info("Using Altitude Filters: Upper = %s, Lower = %s", alt_upper, alt_lower)
+
+        feed_url: ParseResultBytes = urlparse(url)
+
+        url_scheme = str(feed_url.scheme)
 
-        if "http" in feed_url.scheme:
+        if "http" in url_scheme:
             async with aiohttp.ClientSession() as self.session:
                 while 1:
                     self._logger.info(
                         "%s polling every %ss: %s", self.__class__, poll_interval, url
                     )
                     await self.get_feed(url)
                     await asyncio.sleep(int(poll_interval))
-        elif "file" in feed_url.scheme:
+        elif "file" in url_scheme:
             if importlib.util.find_spec("asyncinotify") is None:
                 while 1:
                     self._logger.info(
                         "%s polling every %ss: %s", self.__class__, poll_interval, url
                     )
                     await self.get_file_feed(url)
                     await asyncio.sleep(int(poll_interval))
             else:
                 with Inotify() as inotify:
+                    path = str(feed_url.path)
                     inotify.add_watch(
-                        Path(feed_url.path).parents[0],
+                        Path(path).parents[0],
                         Mask.MODIFY | Mask.CREATE | Mask.MOVE | Mask.MOVED_TO,
                     )
 
                     async for event in inotify:
-                        if str(event.path) == str(feed_url.path):
+                        if str(event.path) == path:
                             await self.get_file_feed(feed_url)
 
     async def get_file_feed(self, feed_url) -> None:
         """Read data from an aircraft JSON file."""
         jdata = {}
         with open(feed_url.path, "r", encoding="UTF-8") as feed_fd:
             jdata = json.loads(feed_fd.read())
```

### Comparing `adsbcot-6.0.0/adsbcot/commands.py` & `adsbcot-6.1.0/adsbcot/commands.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.0.0/adsbcot/constants.py` & `adsbcot-6.1.0/adsbcot/constants.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.0.0/adsbcot/functions.py` & `adsbcot-6.1.0/adsbcot/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,27 @@
     icao_hex: str = str(craft.get("hex", craft.get("icao", ""))).strip().upper()
     reg: str = str(craft.get("reg", craft.get("r", ""))).strip().upper()
     flight: str = str(craft.get("flight", "")).strip().upper()
     cat: str = str(craft.get("category", "")).strip().upper()
     squawk: str = str(craft.get("squawk", "")).strip().upper()
     craft_type: str = str(craft.get("t", "")).strip().upper()
 
+    alt_upper: int = int(config.get("ALT_UPPER", "0"))
+    alt_lower: int = int(config.get("ALT_LOWER", "0"))
+
+    alt_geom = craft.get("alt_geom")
+
+    if alt_geom:
+        if alt_upper and alt_upper != 0:
+            if alt_geom > alt_upper:
+                return None
+        if alt_lower and alt_lower != 0:
+            if alt_geom < alt_lower:
+                return None
+
     if flight:
         remarks_fields.append(flight)
         aircotx.set("flight", flight)
 
     if reg:
         remarks_fields.append(reg)
         aircotx.set("reg", reg)
@@ -196,15 +209,16 @@
     cot_type = aircot.set_cot_type(icao_hex, cat, flight, known_craft)
 
     point: etree.Element = etree.Element("point")
     point.set("lat", str(lat))
     point.set("lon", str(lon))
     point.set("ce", str(craft.get("nac_p", "9999999.0")))
     point.set("le", str(craft.get("nac_v", "9999999.0")))
-    point.set("hae", aircot.functions.get_hae(craft.get("alt_geom")))
+    # Multiply alt_geom by "Clarke 1880 (international foot)"
+    point.set("hae", aircot.functions.get_hae(alt_geom))
 
     contact: etree.Element = etree.Element("contact")
     contact.set("callsign", callsign)
 
     track: etree.Element = etree.Element("track")
     track.set("course", str(craft.get("trk", craft.get("track", "9999999.0"))))
     track.set("speed", aircot.functions.get_speed(craft.get("gs")))
```

### Comparing `adsbcot-6.0.0/adsbcot.egg-info/PKG-INFO` & `adsbcot-6.1.0/adsbcot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.0.0
+Version: 6.1.0
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.0.0/setup.cfg` & `adsbcot-6.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adsbcot-6.0.0/setup.py` & `adsbcot-6.1.0/setup.py`

 * *Files identical despite different names*

