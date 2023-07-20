# Comparing `tmp/cosmicexcelchecker-0.2.2a0.tar.gz` & `tmp/cosmicexcelchecker-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicexcelchecker-0.2.2a0.tar", last modified: Wed Jul 19 08:36:48 2023, max compression
+gzip compressed data, was "cosmicexcelchecker-0.2.2b0.tar", last modified: Wed Jul 19 08:59:16 2023, max compression
```

## Comparing `cosmicexcelchecker-0.2.2a0.tar` & `cosmicexcelchecker-0.2.2b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.507470 cosmicexcelchecker-0.2.2a0/
--rw-rw-rw-   0        0        0    11168 2023-07-19 08:36:48.506470 cosmicexcelchecker-0.2.2a0/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-07-18 07:08:36.000000 cosmicexcelchecker-0.2.2a0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.476365 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/
--rw-rw-rw-   0        0        0      358 2023-07-19 08:35:18.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/__init__.py
--rw-rw-rw-   0        0        0     2856 2023-07-14 01:30:24.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/_baseclass.py
--rw-rw-rw-   0        0        0     7183 2023-07-18 07:30:39.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/conf.py
--rw-rw-rw-   0        0        0    33542 2023-07-18 08:49:25.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/cosmic.py
--rw-rw-rw-   0        0        0      825 2023-07-07 02:29:19.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/errors.py
--rw-rw-rw-   0        0        0      897 2023-07-11 01:28:39.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/find.py
--rw-rw-rw-   0        0        0     2520 2023-07-18 06:54:21.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/obf.py
--rw-rw-rw-   0        0        0     3708 2023-07-12 07:11:45.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/openpyxltest.py
--rw-rw-rw-   0        0        0    43355 2023-07-18 07:19:56.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/test.py
--rw-rw-rw-   0        0        0     1334 2023-07-12 06:19:53.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/testaio.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.502878 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/
--rw-rw-rw-   0        0        0    11168 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 08:36:48.507470 cosmicexcelchecker-0.2.2a0/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-07-19 08:35:48.000000 cosmicexcelchecker-0.2.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:59:16.656901 cosmicexcelchecker-0.2.2b0/
+-rw-rw-rw-   0        0        0    11172 2023-07-19 08:59:16.654977 cosmicexcelchecker-0.2.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-07-18 07:08:36.000000 cosmicexcelchecker-0.2.2b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 08:59:16.628897 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/
+-rw-rw-rw-   0        0        0      357 2023-07-19 08:56:48.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/__init__.py
+-rw-rw-rw-   0        0        0     2856 2023-07-14 01:30:24.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/_baseclass.py
+-rw-rw-rw-   0        0        0     7183 2023-07-18 07:30:39.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/conf.py
+-rw-rw-rw-   0        0        0    33509 2023-07-19 08:55:51.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/cosmic.py
+-rw-rw-rw-   0        0        0      825 2023-07-07 02:29:19.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/errors.py
+-rw-rw-rw-   0        0        0      898 2023-07-19 08:55:51.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/find.py
+-rw-rw-rw-   0        0        0     2521 2023-07-19 08:55:51.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/obf.py
+-rw-rw-rw-   0        0        0     3708 2023-07-12 07:11:45.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/openpyxltest.py
+-rw-rw-rw-   0        0        0    43355 2023-07-18 07:19:56.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/test.py
+-rw-rw-rw-   0        0        0     1334 2023-07-12 06:19:53.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/testaio.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:59:16.645896 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/
+-rw-rw-rw-   0        0        0    11172 2023-07-19 08:59:15.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-07-19 08:59:16.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:59:15.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-19 08:59:16.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-19 08:59:16.000000 cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 08:59:16.657899 cosmicexcelchecker-0.2.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-07-19 08:58:44.000000 cosmicexcelchecker-0.2.2b0/setup.py
```

### Comparing `cosmicexcelchecker-0.2.2a0/PKG-INFO` & `cosmicexcelchecker-0.2.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmicexcelchecker
-Version: 0.2.2a0
+Version: 0.2.2b0
 Summary: A high flexibility package for checking cosmic-related excels under CMDI cosmic standards
 Author: TimG233
 Author-email: gaosh0830@gmail.com
 Maintainer: TimG233
 License: GPL-3.0-only
 Keywords: cosmic,excel,CMDI,checker,data
 Platform: any
@@ -227,7 +227,9 @@
 - **静态方法 `similarity(string1: str, string2: str, ratio: float) -> bool`**
   
   - 通过`compare(string1, string2)`方法来获取编辑距离，对比两个字符串中的较长者来对比比率，若大于ratio则判定为相似，返回布尔值。
     
     - 对比公式：`(len(string_longer) - edit_distance) / len(string_longer)`
     
     - **请注意**：此静态方法使用四舍五入到小数点后2位，所以实际值大于等于`ratio - 0.005`即可判定相似。
+
+
```

### Comparing `cosmicexcelchecker-0.2.2a0/README.md` & `cosmicexcelchecker-0.2.2b0/README.md`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/_baseclass.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/_baseclass.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/conf.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/conf.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/cosmic.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/cosmic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Core COSMIC File
 
-from _baseclass import PdExcel
+from ._baseclass import PdExcel
 from typing import Union, Dict, List
-from errors import CosmicExcelCheckerException ,IncorrectFileTypeException, RepeatedREQNumException, \
+from .errors import CosmicExcelCheckerException ,IncorrectFileTypeException, RepeatedREQNumException, \
     SheetNotFoundException, UnknownREQNumException
 from tabulate import tabulate
-from conf import CFP_SHEET_NAMES ,CFP_COLUMN_NAME, SUB_PROCESS_NAME, RS_SKIP_ROWS, RS_TOTAL_CFP_NAME, \
+from .conf import CFP_SHEET_NAMES ,CFP_COLUMN_NAME, SUB_PROCESS_NAME, RS_SKIP_ROWS, RS_TOTAL_CFP_NAME, \
     RS_WORKLOAD_NAME, RS_REQ_NUM, RS_REQ_NAME, SR_COSMIC_REQ_NAME,  SR_NONCOSMIC_REQ_NAME, SR_SUBFOLDER_NAME, \
     SR_COSMIC_FILE_PREFIX, SR_NONCOSMIC_FILE_PREFIX, RS_QLF_COSMIC, COEFFICIENT_SHEET_NAME, \
     COEFFICIENT_SHEET_DATA_COL_NAME, NONCFP_SHEET_NAMES, SR_NONCOSMIC_PROJECT_NAME, SR_NONCOSMIC_REQ_NUM, \
     SR_AC_REPORT_NUM, SR_AC_FINAL_NUM, SR_FINAL_CONFIRMATION, SR_AC_REQ_NUM, SR_AC_REQ_NAME, SR_AC_FINAL_NUM_LIMIT
 
-from find import FindExcels
-
-from deprecated import deprecated
+from .find import FindExcels
 
 import pandas as pd
 import numpy as np
 import time
 import re
 import math
 import xlrd
```

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/errors.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/errors.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/find.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/find.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is used to find possible files by requirement
 
-from _baseclass import UnionExcels
+from ._baseclass import UnionExcels
 
 import glob
 
 class FindExcels(UnionExcels):
     '''
     Concrete class for finding all possible Excels under certain paths
     '''
```

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/obf.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/obf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # script related to obfuscation (fuzzy word)
 
-from _baseclass import AbstractObf
+from ._baseclass import AbstractObf
 
 class CheckObf(AbstractObf):
     '''
     Concrete implementation of the AbstractObf class
     Provide static method to compare two strings
     '''
```

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/openpyxltest.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/openpyxltest.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/test.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/test.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/testaio.py` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker/testaio.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/PKG-INFO` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmicexcelchecker
-Version: 0.2.2a0
+Version: 0.2.2b0
 Summary: A high flexibility package for checking cosmic-related excels under CMDI cosmic standards
 Author: TimG233
 Author-email: gaosh0830@gmail.com
 Maintainer: TimG233
 License: GPL-3.0-only
 Keywords: cosmic,excel,CMDI,checker,data
 Platform: any
@@ -227,7 +227,9 @@
 - **静态方法 `similarity(string1: str, string2: str, ratio: float) -> bool`**
   
   - 通过`compare(string1, string2)`方法来获取编辑距离，对比两个字符串中的较长者来对比比率，若大于ratio则判定为相似，返回布尔值。
     
     - 对比公式：`(len(string_longer) - edit_distance) / len(string_longer)`
     
     - **请注意**：此静态方法使用四舍五入到小数点后2位，所以实际值大于等于`ratio - 0.005`即可判定相似。
+
+
```

### Comparing `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/SOURCES.txt` & `cosmicexcelchecker-0.2.2b0/cosmicexcelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.2a0/setup.py` & `cosmicexcelchecker-0.2.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as f:
     long_des = f.read()
 
 setup(
     name="cosmicexcelchecker",
-    version="0.2.2a",
+    version="0.2.2b",
     license="GPL-3.0-only",
     author="TimG233",
     author_email="gaosh0830@gmail.com",
     maintainer="TimG233",
     description="A high flexibility package for checking cosmic-related excels under CMDI cosmic standards",
     long_description=long_des,
     long_description_content_type="text/markdown",
```

