# Comparing `tmp/sdss_lvmscp-0.6.0.tar.gz` & `tmp/sdss_lvmscp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.6.0.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.6.1.tar", max compression
```

## Comparing `sdss_lvmscp-0.6.0.tar` & `sdss_lvmscp-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-07-18 16:46:38.763487 sdss_lvmscp-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-18 16:46:38.763707 sdss_lvmscp-0.6.0/README.md
--rw-r--r--   0        0        0     2715 2023-07-18 16:46:38.805588 sdss_lvmscp-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-18 16:46:38.805984 sdss_lvmscp-0.6.0/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-18 16:46:38.806198 sdss_lvmscp-0.6.0/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-18 16:46:38.806462 sdss_lvmscp-0.6.0/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-18 16:46:38.806778 sdss_lvmscp-0.6.0/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-18 16:46:38.807452 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-18 16:46:38.807710 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-18 16:46:38.808061 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-18 16:46:38.808328 sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-18 16:46:38.808603 sdss_lvmscp-0.6.0/python/lvmscp/controller.py
--rw-r--r--   0        0        0    13727 2023-07-18 16:46:38.808877 sdss_lvmscp-0.6.0/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40889 2023-07-18 16:46:38.809375 sdss_lvmscp-0.6.0/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5736 2023-07-18 16:46:38.809690 sdss_lvmscp-0.6.0/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-18 16:46:38.809975 sdss_lvmscp-0.6.0/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-18 16:46:38.810293 sdss_lvmscp-0.6.0/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-20 18:04:02.949696 sdss_lvmscp-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-20 18:04:02.950110 sdss_lvmscp-0.6.1/README.md
+-rw-r--r--   0        0        0     2715 2023-07-20 18:04:02.995709 sdss_lvmscp-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-20 18:04:02.996393 sdss_lvmscp-0.6.1/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-20 18:04:02.996711 sdss_lvmscp-0.6.1/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-20 18:04:02.997109 sdss_lvmscp-0.6.1/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-20 18:04:02.997464 sdss_lvmscp-0.6.1/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-20 18:04:02.997884 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-20 18:04:02.998097 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-20 18:04:02.998619 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-20 18:04:02.998851 sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-20 18:04:02.999044 sdss_lvmscp-0.6.1/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    13947 2023-07-20 18:04:02.999296 sdss_lvmscp-0.6.1/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40889 2023-07-20 18:04:02.999703 sdss_lvmscp-0.6.1/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5736 2023-07-20 18:04:02.999985 sdss_lvmscp-0.6.1/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-20 18:04:03.000178 sdss_lvmscp-0.6.1/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-20 18:04:03.000443 sdss_lvmscp-0.6.1/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.1/PKG-INFO
```

### Comparing `sdss_lvmscp-0.6.0/LICENSE.md` & `sdss_lvmscp-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/README.md` & `sdss_lvmscp-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/pyproject.toml` & `sdss_lvmscp-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.6.0"
+version = "0.6.1"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
```

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/__main__.py` & `sdss_lvmscp-0.6.1/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.6.1/python/lvmscp/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.6.1/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/controller.py` & `sdss_lvmscp-0.6.1/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/delegate.py` & `sdss_lvmscp-0.6.1/python/lvmscp/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 # @Date: 2021-05-29
 # @Filename: delegate.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
+import os
 from typing import TYPE_CHECKING, Any, List, Literal, Tuple
 
 import numpy
 from astropy.io import fits
 
 from archon.actor import ExposureDelegate
 from archon.controller.controller import ArchonController
+from sdsstools.time import get_sjd
 
 
 if TYPE_CHECKING:
     from .actor import SCPActor  # noqa
 
 
 class LVMExposeDelegate(ExposureDelegate["SCPActor"]):
@@ -158,14 +160,18 @@
             else:
                 hartmann[key]["status"] = "0" if hartmann[key]["open"] else "1"
 
         left = hartmann[f"{controller.name}_hartmann_left"]["status"]
         right = hartmann[f"{controller.name}_hartmann_right"]["status"]
 
         for hdu in hdus:
+            # Add SDSS MJD.
+            SJD = get_sjd() if "OBSERVATORY" in os.environ else "?"
+            hdu.header["SMJD"] = (SJD, "SDSS Modified Julian Date (MJD+0.4)")
+
             hdu.header["HARTMANN"] = (f"{left} {right}", "Left/right. 0=open 1=closed")
 
             for lamp_name, value in self.extra_data.get("lamps", {}).items():
                 hdu.header[lamp_name.upper()] = (value, f"Status of lamp {lamp_name}")
 
             ccd = hdu.header["CCD"]
             pressure = self.extra_data.get("pressure", {}).get(ccd, -999.0)
```

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.6.1/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.6.1/python/lvmscp/etc/lvmscp.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/python/lvmscp/ln2.py` & `sdss_lvmscp-0.6.1/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.0/PKG-INFO` & `sdss_lvmscp-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.6.0
+Version: 0.6.1
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
```

