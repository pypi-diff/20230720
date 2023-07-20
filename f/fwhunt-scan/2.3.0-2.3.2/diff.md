# Comparing `tmp/fwhunt_scan-2.3.0.tar.gz` & `tmp/fwhunt_scan-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwhunt_scan-2.3.0.tar", last modified: Mon Jun  5 17:51:58 2023, max compression
+gzip compressed data, was "fwhunt_scan-2.3.2.tar", last modified: Thu Jul 20 11:25:59 2023, max compression
```

## Comparing `fwhunt_scan-2.3.0.tar` & `fwhunt_scan-2.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.222045 fwhunt_scan-2.3.0/
--rw-r--r--   0 yv         (501) staff       (20)    35149 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/LICENSE
--rw-r--r--   0 yv         (501) staff       (20)     4411 2023-06-05 17:51:58.222085 fwhunt_scan-2.3.0/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)     3837 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/README.md
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221191 fwhunt_scan-2.3.0/fwhunt_scan/
--rw-r--r--   0 yv         (501) staff       (20)      615 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/__init__.py
--rw-r--r--   0 yv         (501) staff       (20)      362 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/__init__.pyi
--rw-r--r--   0 yv         (501) staff       (20)       64 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/py.typed
--rw-r--r--   0 yv         (501) staff       (20)      817 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/test_internal.py
--rw-r--r--   0 yv         (501) staff       (20)    30184 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     2728 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5494 2023-05-09 12:22:20.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_extractor.py
--rw-r--r--   0 yv         (501) staff       (20)   305195 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_protocols.py
--rw-r--r--   0 yv         (501) staff       (20)    35819 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.py
--rw-r--r--   0 yv         (501) staff       (20)     2592 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.pyi
--rw-r--r--   0 yv         (501) staff       (20)    14733 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.py
--rw-r--r--   0 yv         (501) staff       (20)     1430 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5508 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.py
--rw-r--r--   0 yv         (501) staff       (20)      280 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3035 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.py
--rw-r--r--   0 yv         (501) staff       (20)      727 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.pyi
--rw-r--r--   0 yv         (501) staff       (20)     4277 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.py
--rw-r--r--   0 yv         (501) staff       (20)     1922 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.pyi
--rw-r--r--   0 yv         (501) staff       (20)     2112 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.py
--rw-r--r--   0 yv         (501) staff       (20)      418 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.pyi
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221781 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/
--rw-r--r--   0 yv         (501) staff       (20)     4411 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)      857 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/SOURCES.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/dependency_links.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2023-06-05 12:35:02.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/not-zip-safe
--rw-r--r--   0 yv         (501) staff       (20)      127 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/requires.txt
--rw-r--r--   0 yv         (501) staff       (20)       12 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/top_level.txt
--rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-13 18:05:03.000000 fwhunt_scan-2.3.0/fwhunt_scan_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     3860 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan_docker.py
--rw-r--r--   0 yv         (501) staff       (20)      116 2023-06-05 17:51:58.222247 fwhunt_scan-2.3.0/setup.cfg
--rw-r--r--   0 yv         (501) staff       (20)     1408 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/setup.py
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221964 fwhunt_scan-2.3.0/test/
--rw-r--r--   0 yv         (501) staff       (20)     1208 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.0/test/test.py
--rw-r--r--   0 yv         (501) staff       (20)      230 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.0/test/test_variants.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-07-20 11:25:59.856498 fwhunt_scan-2.3.2/
+-rw-r--r--   0 yv         (501) staff       (20)    35149 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/LICENSE
+-rw-r--r--   0 yv         (501) staff       (20)     4411 2023-07-20 11:25:59.856543 fwhunt_scan-2.3.2/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)     3837 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/README.md
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-07-20 11:25:59.855587 fwhunt_scan-2.3.2/fwhunt_scan/
+-rw-r--r--   0 yv         (501) staff       (20)      615 2023-07-20 11:24:01.000000 fwhunt_scan-2.3.2/fwhunt_scan/__init__.py
+-rw-r--r--   0 yv         (501) staff       (20)      362 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/__init__.pyi
+-rw-r--r--   0 yv         (501) staff       (20)       64 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/fwhunt_scan/py.typed
+-rw-r--r--   0 yv         (501) staff       (20)      817 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/fwhunt_scan/test_internal.py
+-rw-r--r--   0 yv         (501) staff       (20)    30184 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     2728 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_analyzer.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5635 2023-07-11 00:06:14.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_extractor.py
+-rw-r--r--   0 yv         (501) staff       (20)   305195 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_protocols.py
+-rw-r--r--   0 yv         (501) staff       (20)    35819 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_scanner.py
+-rw-r--r--   0 yv         (501) staff       (20)     2592 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_scanner.pyi
+-rw-r--r--   0 yv         (501) staff       (20)    14733 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_smm.py
+-rw-r--r--   0 yv         (501) staff       (20)     1430 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_smm.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5508 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_tables.py
+-rw-r--r--   0 yv         (501) staff       (20)      280 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_tables.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3035 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_te.py
+-rw-r--r--   0 yv         (501) staff       (20)      727 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_te.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     4277 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_types.py
+-rw-r--r--   0 yv         (501) staff       (20)     1922 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_types.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     2112 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_utils.py
+-rw-r--r--   0 yv         (501) staff       (20)      418 2023-07-20 11:25:49.000000 fwhunt_scan-2.3.2/fwhunt_scan/uefi_utils.pyi
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-07-20 11:25:59.856217 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/
+-rw-r--r--   0 yv         (501) staff       (20)     4411 2023-07-20 11:25:59.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)      857 2023-07-20 11:25:59.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-07-20 11:25:59.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-06-05 12:35:02.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/not-zip-safe
+-rw-r--r--   0 yv         (501) staff       (20)      127 2023-07-20 11:25:59.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/requires.txt
+-rw-r--r--   0 yv         (501) staff       (20)       12 2023-07-20 11:25:59.000000 fwhunt_scan-2.3.2/fwhunt_scan.egg-info/top_level.txt
+-rw-r--r--   0 yv         (501) staff       (20)     7250 2023-07-20 11:18:53.000000 fwhunt_scan-2.3.2/fwhunt_scan_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     3860 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/fwhunt_scan_docker.py
+-rw-r--r--   0 yv         (501) staff       (20)      116 2023-07-20 11:25:59.856719 fwhunt_scan-2.3.2/setup.cfg
+-rw-r--r--   0 yv         (501) staff       (20)     1408 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.2/setup.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-07-20 11:25:59.856401 fwhunt_scan-2.3.2/test/
+-rw-r--r--   0 yv         (501) staff       (20)     1208 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.2/test/test.py
+-rw-r--r--   0 yv         (501) staff       (20)      230 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.2/test/test_variants.py
```

### Comparing `fwhunt_scan-2.3.0/LICENSE` & `fwhunt_scan-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/PKG-INFO` & `fwhunt_scan-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt_scan
-Version: 2.3.0
+Version: 2.3.2
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.3.0/README.md` & `fwhunt_scan-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/__init__.py` & `fwhunt_scan-2.3.2/fwhunt_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 """
 
 __author__ = "FwHunt team"
 __email__ = "fwhunt@binarly.io"
-__version__ = "2.3.0"
+__version__ = "2.3.2"
 
 from .uefi_analyzer import UefiAnalyzer, UefiAnalyzerError
 from .uefi_scanner import UefiRule, UefiScanner, UefiScannerError
 from .uefi_te import TerseExecutableParser
 from .uefi_extractor import UefiBinary, UefiExtractor
 
 __all__ = [
```

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/test_internal.py` & `fwhunt_scan-2.3.2/fwhunt_scan/test_internal.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_analyzer.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.pyi` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_analyzer.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_extractor.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,33 +65,42 @@
         self._firmware_data: bytes = firmware_data
         self._file_guids: List[str] = [g.lower() for g in file_guids]
         self._parsers: List[uefi_firmware.AutoParser] = list()
         self._info: Dict[str, Any] = dict()
         self.binaries: List[UefiBinary] = list()
 
     def _compressed_search(self, object: Any, root_guid: str) -> None:
+        if object is None:
+            return
+
         for component in object.iterate_objects():
             attrs = component.get("attrs", None)
             if attrs is not None:
                 type = attrs.get("type", None)
                 if type in UefiExtractor.UI:
                     self._info[root_guid]["name"] = component["label"]
                 if type in UefiExtractor.SECTION_TYPES:
                     self._info[root_guid]["content"] = component["_self"].content
             self._compressed_search(component["_self"], root_guid)
 
     def _compressed_handle(self, object: Any, root_guid: str) -> None:
+        if object is None:
+            return
+
         for obj in object.iterate_objects():
             if (
                 obj.get("attrs", None) is not None
                 and obj["attrs"].get("attrs", None) == 0x01
             ):  # if compressed
                 self._compressed_search(obj["_self"], root_guid)
 
     def _append_binaries(self, object: Any) -> None:
+        if object is None:
+            return
+
         for component in object.iterate_objects():
             guid = component.get("guid", None)
             attrs = component.get("attrs", None)
             if guid is not None and attrs is not None:
                 if guid not in self._info:
                     self._info[guid] = {"name": None, "ext": None, "content": None}
                 type = attrs.get("type", None)
```

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_protocols.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_protocols.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_scanner.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.pyi` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_scanner.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_smm.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.pyi` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_smm.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_tables.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_te.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.pyi` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_te.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_types.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.pyi` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_types.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.py` & `fwhunt_scan-2.3.2/fwhunt_scan/uefi_utils.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan.egg-info/PKG-INFO` & `fwhunt_scan-2.3.2/fwhunt_scan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt-scan
-Version: 2.3.0
+Version: 2.3.2
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan.egg-info/SOURCES.txt` & `fwhunt_scan-2.3.2/fwhunt_scan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan_analyzer.py` & `fwhunt_scan-2.3.2/fwhunt_scan_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     rules_guids: Dict[str, List[UefiRule]] = dict()
     for uefi_rule in uefi_rules:
         if uefi_rule.volume_guids is None:
             print(f"[I] Specify volume_guids in {uefi_rule.name} or use scan command")
             continue
         for guid in [g.lower() for g in uefi_rule.volume_guids]:
             lower_guid = guid.lower()
-            if not lower_guid in rules_guids:
+            if lower_guid not in rules_guids:
                 rules_guids[lower_guid] = list()
             rules_guids[lower_guid].append(uefi_rule)
 
     if not rules_guids.keys():
         print(
             f"{error_prefix} None of the rules specify volume_guids (use scan command)"
         )
```

### Comparing `fwhunt_scan-2.3.0/fwhunt_scan_docker.py` & `fwhunt_scan-2.3.2/fwhunt_scan_docker.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/setup.py` & `fwhunt_scan-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.3.0/test/test.py` & `fwhunt_scan-2.3.2/test/test.py`

 * *Files identical despite different names*

