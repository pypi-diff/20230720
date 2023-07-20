# Comparing `tmp/ros_license_toolkit-1.0.0.tar.gz` & `tmp/ros_license_toolkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ros_license_toolkit-1.0.0.tar", last modified: Tue Jul 18 12:32:45 2023, max compression
+gzip compressed data, was "ros_license_toolkit-1.1.0.tar", last modified: Thu Jul 20 18:41:57 2023, max compression
```

## Comparing `ros_license_toolkit-1.0.0.tar` & `ros_license_toolkit-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-18 12:32:45.661589 ros_license_toolkit-1.0.0/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    11358 2022-12-12 09:53:16.000000 ros_license_toolkit-1.0.0/LICENSE
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      993 2023-03-30 14:25:23.000000 ros_license_toolkit-1.0.0/NOTICE
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18179 2023-07-18 12:32:45.661589 ros_license_toolkit-1.0.0/PKG-INFO
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     4154 2023-07-18 11:31:39.000000 ros_license_toolkit-1.0.0/README.md
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1410 2023-07-18 12:32:24.000000 ros_license_toolkit-1.0.0/pyproject.toml
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      100 2023-07-18 12:32:45.661589 ros_license_toolkit-1.0.0/setup.cfg
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-18 12:32:45.657589 ros_license_toolkit-1.0.0/src/
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-18 12:32:45.661589 ros_license_toolkit-1.0.0/src/ros_license_toolkit/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)        0 2023-02-27 14:58:21.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/__init__.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    10695 2023-03-30 14:25:30.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/checks.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1083 2023-03-30 14:25:30.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/common.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     2987 2023-07-01 17:05:01.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/copyright.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5537 2023-07-01 17:05:01.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/license_tag.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5153 2023-07-18 12:32:24.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/main.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     8700 2023-07-01 17:05:01.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/package.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     3081 2023-04-21 17:10:05.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/repo.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1846 2023-03-30 14:25:30.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit/ui_elements.py
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-18 12:32:45.661589 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18179 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      651 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)        1 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       70 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       53 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/requires.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       20 2023-07-18 12:32:45.000000 ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    11358 2022-12-12 09:53:16.000000 ros_license_toolkit-1.1.0/LICENSE
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      993 2023-03-30 14:25:23.000000 ros_license_toolkit-1.1.0/NOTICE
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18314 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/PKG-INFO
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     4269 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/README.md
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1556 2023-07-20 18:37:26.000000 ros_license_toolkit-1.1.0/pyproject.toml
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      319 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/setup.cfg
+drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.002402 ros_license_toolkit-1.1.0/src/
+drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.002402 ros_license_toolkit-1.1.0/src/ros_license_toolkit/
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       22 2023-07-20 18:37:26.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/__init__.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    10580 2023-07-20 14:38:25.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/checks.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1083 2023-03-30 14:25:30.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/common.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     2966 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/copyright.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5487 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/license_tag.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5167 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/main.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    10048 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/package.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     3081 2023-04-21 17:10:05.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/repo.py
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1830 2023-07-20 14:38:25.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/ui_elements.py
+drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18314 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      651 2023-07-20 18:41:57.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)        1 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       70 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      116 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       20 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/top_level.txt
```

### Comparing `ros_license_toolkit-1.0.0/LICENSE` & `ros_license_toolkit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.0.0/NOTICE` & `ros_license_toolkit-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.0.0/PKG-INFO` & `ros_license_toolkit-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros_license_toolkit
-Version: 1.0.0
+Version: 1.1.0
 Summary: Checks ROS packages for correct license declaration.
 Author-email: Christian Henkel <christian.henkel2@de.bosch.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -217,14 +217,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # ros_license_toolkit
 
 [![Pytest](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/pytest.yml) [![Lint](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/lint.yml) [![GitHub issues](https://img.shields.io/github/issues/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/issues) [![GitHub prs](https://img.shields.io/github/issues-pr/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/pulls) [![python](https://img.shields.io/github/languages/top/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/search?l=python) [![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://github.com/boschresearch/ros_license_toolkit/blob/main/LICENSE)
 
@@ -273,25 +274,27 @@
 ```bash
 ros_license_toolkit my_ros_package
 ```
 
 ### All Options
 ```
 $ ros_license_toolkit -h
-usage: ros_license_toolkit [-h] [-v] [-q] path
+usage: ros_license_toolkit [-h] [-c] [-v] [-q] path
 
 Checks ROS packages for correct license declaration.
 
 positional arguments:
-  path           path to ROS2 package or repo containing packages
+  path                  path to ROS2 package or repo containing packages
 
 optional arguments:
-  -h, --help     show this help message and exit
-  -v, --verbose  enable verbose output
-  -q, --quiet    disable most output
+  -h, --help            show this help message and exit
+  -c, --generate_copyright_file
+                        generate a copyright file
+  -v, --verbose         enable verbose output
+  -q, --quiet           disable most output
 ```
 
 ## State of Development
 *WORK IN PROGRESS*
 This is currently working and feature complete to the point it was originally intended.
 But there are still open points concerning testing and it is also very important to make sure how this behaves with existing ROS packages.
 In particular, the following things will have to be done:
```

### Comparing `ros_license_toolkit-1.0.0/README.md` & `ros_license_toolkit-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,25 +47,27 @@
 ```bash
 ros_license_toolkit my_ros_package
 ```
 
 ### All Options
 ```
 $ ros_license_toolkit -h
-usage: ros_license_toolkit [-h] [-v] [-q] path
+usage: ros_license_toolkit [-h] [-c] [-v] [-q] path
 
 Checks ROS packages for correct license declaration.
 
 positional arguments:
-  path           path to ROS2 package or repo containing packages
+  path                  path to ROS2 package or repo containing packages
 
 optional arguments:
-  -h, --help     show this help message and exit
-  -v, --verbose  enable verbose output
-  -q, --quiet    disable most output
+  -h, --help            show this help message and exit
+  -c, --generate_copyright_file
+                        generate a copyright file
+  -v, --verbose         enable verbose output
+  -q, --quiet           disable most output
 ```
 
 ## State of Development
 *WORK IN PROGRESS*
 This is currently working and feature complete to the point it was originally intended.
 But there are still open points concerning testing and it is also very important to make sure how this behaves with existing ROS packages.
 In particular, the following things will have to be done:
```

### Comparing `ros_license_toolkit-1.0.0/pyproject.toml` & `ros_license_toolkit-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ros_license_toolkit"
-version = "1.0.0"
+version = "1.1.0"
 description = "Checks ROS packages for correct license declaration."
 readme = "README.md"
 authors = [
     {name = "Christian Henkel", email = "christian.henkel2@de.bosch.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
@@ -31,13 +31,19 @@
 # https://github.com/nexB/scancode-toolkit/blob/develop/
 # CHANGELOG.rst#v3200---2023-05-23
     "scancode-toolkit<=31.2.6",
     "spdx-tools"
 ]
 requires-python = ">=3.7"
 
+[project.optional-dependencies]
+dev = ["pytest", "pytest-cov", "pycodestyle", "flake8", "mypy", "isort", "bumpver"]
+
 [project.urls]
 homepage = "https://github.com/boschresearch/ros_license_toolkit"
 repository = "https://github.com/boschresearch/ros_license_toolkit"
 
 [project.scripts]
-ros_license_toolkit = "ros_license_toolkit.main:main"
+ros_license_toolkit = "ros_license_toolkit.main:main"
+
+[isort]
+profile = "google"
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/checks.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,20 @@
 
 """This module contains the checks for the linter."""
 
 import os
 from pprint import pformat
 from typing import Dict, List, Optional
 
-from ros_license_toolkit.license_tag import is_license_name_in_spdx_list
-from ros_license_toolkit.license_tag import LicenseTag
-from ros_license_toolkit.package import get_spdx_license_name
-from ros_license_toolkit.package import is_license_text_file
-from ros_license_toolkit.package import Package
-from ros_license_toolkit.package import PackageException
-from ros_license_toolkit.ui_elements import green
-from ros_license_toolkit.ui_elements import NO_REASON_STR
-from ros_license_toolkit.ui_elements import red
+from ros_license_toolkit.license_tag import (LicenseTag,
+                                             is_license_name_in_spdx_list)
+from ros_license_toolkit.package import (Package, PackageException,
+                                         get_spdx_license_name,
+                                         is_license_text_file)
+from ros_license_toolkit.ui_elements import NO_REASON_STR, green, red
 
 
 class Check:
     """Base class for checks."""
 
     def __init__(self: 'Check'):
         """Initialize a check."""
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/common.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/common.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/copyright.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/copyright.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,29 +14,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Assemble copyright notices for a package."""
 
 import os
 import re
-from typing import Any, Dict, List, Set, Tuple, Union
+from typing import Any, Dict, List, Tuple, Union
 
 from scancode.api import get_copyrights
 
-from ros_license_toolkit.license_tag import LicenseTag
-from ros_license_toolkit.package import Package
-
 
 def _get_copyright_strs_from_results(
         scan_results: Dict[str, Any]) -> List[str]:
     """Get copyright strings from scan results."""
-    cprs = []
-    for cpr in scan_results['copyrights']:
-        cprs.append(cpr['copyright'])
-    return cprs
+    return [cpr['copyright'] for cpr in scan_results['copyrights']]
 
 
 def _get_year_from_copyright_str(cpr_str: str) -> Union[int, Tuple[int, int]]:
     """Get the year from a copyright string."""
     finds = re.findall(r"\d{4}", cpr_str)
     if len(finds) == 1:
         return int(finds[0])
@@ -47,36 +41,43 @@
 
 
 class CopyrightPerFile:
     """A copyright notice for a single file."""
 
     def __init__(self, file_path: str, copyright_text: str):
         self.file_path = file_path
+        for prefix_to_remove in [
+            'copyright',
+            'Copyright (c) ',
+            'Copyright ',
+            'Copyright'
+        ]:
+            if copyright_text.startswith(prefix_to_remove):
+                copyright_text = copyright_text[len(prefix_to_remove):]
+                break
         self.copyright_text = copyright_text
 
+    def __str__(self):
+        return self.copyright_text
 
-class Copyright:
 
-    def __init__(self, pkg: Package):
+class CopyrightPerPkg:
+    def __init__(self, pkg):
         self.pkg = pkg
         # one section per license tag
         # each section is a list of unique copyright lines
-        self.copyright_sections: Dict[str, Set[CopyrightPerFile]] = {}
-        for license_tag in self.pkg.license_tags.values():  # type: LicenseTag
-            self.copyright_sections[license_tag.source_files_str] = set()
+        self.copyright_strings: Dict[str, List[str]] = {}
+        for key, license_tag in self.pkg.license_tags.items():
+            cprs = set()
             for source_file in license_tag.source_files:
                 fpath = os.path.join(self.pkg.abspath, source_file)
                 res = get_copyrights(fpath)
                 if len(res) == 0:
                     continue
                 for cpr in _get_copyright_strs_from_results(res):
-                    self.copyright_sections[license_tag.source_files_str].add(
-                        CopyrightPerFile(source_file, cpr))
+                    cprs.add(CopyrightPerFile(source_file, cpr))
+            self.copyright_strings[key] = sorted(
+                {cpr.copyright_text for cpr in cprs})
 
     def __str__(self):
-        """Get a string representation of the copyright notice."""
-        cpr_str = ""
-        for files_str, cprs in self.copyright_sections.items():
-            cpr_str += f"{files_str}:\n"
-            for cpr in cprs:
-                cpr_str += f"  {cpr.copyright_text}\n"
-        return cpr_str
+        return " ".join(" ".join(copyrights)
+                        for copyrights in self.copyright_strings.values())
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/license_tag.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/license_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # limitations under the License.
 
 """
 Module containing the LicenseTag class and related functions to handle
 license tags in package.xml files.
 """
 
-from glob import glob
 import os
-from typing import List, Optional, Set
 import xml.etree.ElementTree as ET
+from glob import glob
+from typing import List, Optional, Set
 
 from spdx.config import LICENSE_MAP
 
 
 def is_license_name_in_spdx_list(license_name: str) -> bool:
     """Check if a license name is in the SPDX list of licenses."""
     return license_name in LICENSE_MAP or \
@@ -65,58 +65,58 @@
         """Initialize a license tag from an XML element."""
         self.element = element
         assert self.element.text is not None, "License tag must have text."
 
         raw_license_name: str = str(self.element.text)
         # Name of the license (in SPDX tag format for comparability)
         try:
-            self.license_id = to_spdx_license_tag(raw_license_name)
+            self.id = to_spdx_license_tag(raw_license_name)
         except ValueError:
             # If the license name is not in the SPDX list,
             # we assume it is a custom license and use the name as-is.
             # This will be detected in `LicenseTagIsInSpdxListCheck`.
-            self.license_id = raw_license_name
+            self.id = raw_license_name
 
         # Path to the file containing the license text
         # (relative to package root)
         self.license_text_file: Optional[str] = element.attrib.get(
             "file", None)
 
         # Paths to the source files that are licensed under this license
         self._source_files: Optional[Set[str]] = None
         self.source_files_str: str = element.attrib.get("source-files", '')
-        if self.source_files_str == '':
+        if not self.source_files_str:
             # If no source-files attribute is given, assume all files
             # are licensed under this license.
             self.source_files_str = "**"
         else:
             self._source_files = set()
             for src_glob in self.source_files_str.split(" "):
                 self._source_files.update(_eval_glob(src_glob, pkg_path))
 
         # Path of package file this is in
         self.package_path: str = pkg_path
 
     def __str__(self) -> str:
         """Return a string representation of this license tag."""
-        assert self.license_id is not None, "License must have a name."
-        return self.license_id
+        assert self.id is not None, "License must have a name."
+        return self.id
 
     def has_license_text_file(self) -> bool:
         """Return whether this license tag has a file attribute."""
         return self.license_text_file is not None
 
     def has_source_files(self) -> bool:
         """Return whether this license tag has a source-files attribute."""
         return self._source_files is not None
 
     def get_license_id(self) -> str:
         """Return the license name."""
-        assert self.license_id is not None, "License tag must have an id."
-        return self.license_id
+        assert self.id is not None, "License tag must have an id."
+        return self.id
 
     def get_license_text_file(self) -> str:
         """Return the file attribute."""
         assert self.license_text_file is not None, \
             "License tag must have file attribute."
         return self.license_text_file
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/main.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,27 +20,22 @@
 
 import argparse
 import os
 import sys
 import timeit
 from typing import Optional, Sequence
 
-from ros_license_toolkit.checks import LicensesInCodeCheck
-from ros_license_toolkit.checks import LicenseTagExistsCheck
-from ros_license_toolkit.checks import LicenseTagIsInSpdxListCheck
-from ros_license_toolkit.checks import LicenseTextExistsCheck
+from ros_license_toolkit.checks import (LicensesInCodeCheck,
+                                        LicenseTagExistsCheck,
+                                        LicenseTagIsInSpdxListCheck,
+                                        LicenseTextExistsCheck)
 from ros_license_toolkit.package import get_packages_in_path
-from ros_license_toolkit.ui_elements import FAILURE_STR
-from ros_license_toolkit.ui_elements import green
-from ros_license_toolkit.ui_elements import major_sep
-from ros_license_toolkit.ui_elements import minor_sep
-from ros_license_toolkit.ui_elements import red
-from ros_license_toolkit.ui_elements import rll_print_factory
-from ros_license_toolkit.ui_elements import SUCCESS_STR
-from ros_license_toolkit.ui_elements import Verbosity
+from ros_license_toolkit.ui_elements import (FAILURE_STR, SUCCESS_STR,
+                                             Verbosity, green, major_sep,
+                                             minor_sep, red, rll_print_factory)
 
 
 def main(args: Optional[Sequence[str]] = None) -> int:
     """Main entry point for the ros_license_toolkit CLI.
 
     :param args: the command line arguments, defaults to sys.argv[1:]
     :type args: Sequence[str], optional
@@ -49,21 +44,25 @@
     :rtype: int
     """
     if not args:
         args = sys.argv[1:]
     parser = argparse.ArgumentParser(
         description='Checks ROS packages for correct license declaration.')
     parser.add_argument(
-        'path',
-        default='.',
+        'path', default='.',
         help='path to ROS2 package or repo containing packages')
-    parser.add_argument('-v', '--verbose', dest='verbose', action='store_true',
-                        default=False, help='enable verbose output')
-    parser.add_argument('-q', '--quiet', dest='quiet', action='store_true',
-                        default=False, help='disable most output')
+    parser.add_argument(
+        '-c', '--generate_copyright_file', action='store_true',
+        default=False, help='generate a copyright file')
+    parser.add_argument(
+        '-v', '--verbose', dest='verbose', action='store_true',
+        default=False, help='enable verbose output')
+    parser.add_argument(
+        '-q', '--quiet', dest='quiet', action='store_true',
+        default=False, help='disable most output')
     parsed_args = parser.parse_args(args)
 
     # Determine the verbosity level
     if parsed_args.quiet:
         verbosity = Verbosity.QUIET
     elif parsed_args.verbose:
         verbosity = Verbosity.VERBOSE
@@ -119,14 +118,16 @@
             results_per_package[package.abspath] = True
         else:
             rll_print(minor_sep())
             rll_print(f"[{package.name}] Overall:" + red(
                 f"\n {FAILURE_STR}"))
             rll_print(major_sep())
             results_per_package[package.abspath] = False
+        if parsed_args.generate_copyright_file:
+            package.write_copyright_file()
 
     stop = timeit.default_timer()
     rll_print(f'Execution time: {stop - start:.2f} seconds', Verbosity.QUIET)
 
     # Print the overall results
     if all(results_per_package.values()):
         rll_print("All packages:" + green(
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/package.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/package.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # limitations under the License.
 
 """
 This module contains the Package class.
 """
 
 import os
-from typing import Any, Dict, List, Optional
 import xml.etree.ElementTree as ET
+from typing import Any, Dict, List, Optional
 
-from rospkg import list_by_path
-from rospkg import RosPack
+from rospkg import RosPack, list_by_path
 from rospkg.common import PACKAGE_FILE
 from scancode.api import get_licenses
 
 from ros_license_toolkit.common import is_license_text_file
+from ros_license_toolkit.copyright import CopyrightPerPkg
 from ros_license_toolkit.license_tag import LicenseTag
-from ros_license_toolkit.repo import NotARepoError
-from ros_license_toolkit.repo import Repo
+from ros_license_toolkit.repo import NotARepoError, Repo
 
 # files we ignore in scan results
 IGNORED_FILES = [
     "package.xml",
     "setup.py",
     "setup.cfg",
     "CMakeLists.txt"
@@ -200,14 +199,46 @@
 
     def get_license_files(self) -> List[str]:
         """Get all license text files associated with license tags
         in the package.xml."""
         return [x.get_license_text_file() for x in
                 self.license_tags.values()]
 
+    def get_copyright_file_contents(self) -> str:
+        """Get a string representation of the copyright notice."""
+        copyright = CopyrightPerPkg(self)
+        cpr_str = "".join((
+            "Format: https://www.debian.org/doc/packaging-manuals/copyright",
+            "-format/1.0/\n",
+            "Source: tbd\n",
+            f"Upstream-Name: {self.name}\n\n",))
+        for key, cprs in copyright.copyright_strings.items():
+            source_files_str = self.license_tags[key].source_files_str
+            cpr_str += f"Files:\n {source_files_str}\n"
+            cpr_str += "Copyright: "
+            cpr_str += "\n           ".join(cprs)
+            license = self.license_tags[key]
+            cpr_str += f"\nLicense: {license.id}\n"
+            assert license.license_text_file, \
+                "License text file must be defined."
+            with open(os.path.join(
+                    self.abspath,
+                    license.license_text_file)) as f:
+                license_lines = f.readlines()
+            for line in license_lines:
+                cpr_str += f" {line}"
+            cpr_str += "\n\n"
+        return cpr_str
+
+    def write_copyright_file(self):
+        with open(os.path.join(
+                self.abspath,
+                'copyright'), 'w') as f:
+            f.write(self.get_copyright_file_contents())
+
 
 def get_packages_in_path(path: str) -> List[Package]:
     """Get all ROS packages in a given path."""
     packages = []
     try:
         repo: Optional[Repo] = Repo(os.path.abspath(path))
     except NotARepoError:
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/repo.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/repo.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit/ui_elements.py` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit/ui_elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 This module contains UI elements for the CLI.
 """
 
-from enum import auto
-from enum import Enum
+from enum import Enum, auto
 
 # colors
 
 GREEN = "\033[92m"
 RED = "\033[91m"
 NC = "\033[00m"
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/PKG-INFO` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-license-toolkit
-Version: 1.0.0
+Version: 1.1.0
 Summary: Checks ROS packages for correct license declaration.
 Author-email: Christian Henkel <christian.henkel2@de.bosch.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -217,14 +217,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # ros_license_toolkit
 
 [![Pytest](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/pytest.yml) [![Lint](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/boschresearch/ros_license_toolkit/actions/workflows/lint.yml) [![GitHub issues](https://img.shields.io/github/issues/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/issues) [![GitHub prs](https://img.shields.io/github/issues-pr/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/pulls) [![python](https://img.shields.io/github/languages/top/boschresearch/ros_license_toolkit.svg)](https://github.com/boschresearch/ros_license_toolkit/search?l=python) [![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://github.com/boschresearch/ros_license_toolkit/blob/main/LICENSE)
 
@@ -273,25 +274,27 @@
 ```bash
 ros_license_toolkit my_ros_package
 ```
 
 ### All Options
 ```
 $ ros_license_toolkit -h
-usage: ros_license_toolkit [-h] [-v] [-q] path
+usage: ros_license_toolkit [-h] [-c] [-v] [-q] path
 
 Checks ROS packages for correct license declaration.
 
 positional arguments:
-  path           path to ROS2 package or repo containing packages
+  path                  path to ROS2 package or repo containing packages
 
 optional arguments:
-  -h, --help     show this help message and exit
-  -v, --verbose  enable verbose output
-  -q, --quiet    disable most output
+  -h, --help            show this help message and exit
+  -c, --generate_copyright_file
+                        generate a copyright file
+  -v, --verbose         enable verbose output
+  -q, --quiet           disable most output
 ```
 
 ## State of Development
 *WORK IN PROGRESS*
 This is currently working and feature complete to the point it was originally intended.
 But there are still open points concerning testing and it is also very important to make sure how this behaves with existing ROS packages.
 In particular, the following things will have to be done:
```

### Comparing `ros_license_toolkit-1.0.0/src/ros_license_toolkit.egg-info/SOURCES.txt` & `ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

