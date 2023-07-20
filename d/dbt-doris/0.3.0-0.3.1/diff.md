# Comparing `tmp/dbt-doris-0.3.0.tar.gz` & `tmp/dbt-doris-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doris-0.3.0.tar", last modified: Mon Jul 10 03:22:59 2023, max compression
+gzip compressed data, was "dbt-doris-0.3.1.tar", last modified: Thu Jul 20 09:19:47 2023, max compression
```

## Comparing `dbt-doris-0.3.0.tar` & `dbt-doris-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.937630 dbt-doris-0.3.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-10 02:50:27.000000 dbt-doris-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-10 02:50:27.000000 dbt-doris-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-10 03:22:59.937630 dbt-doris-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-07-10 02:50:27.000000 dbt-doris-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.932630 dbt-doris-0.3.0/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.932630 dbt-doris-0.3.0/dbt/adapters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.933630 dbt-doris-0.3.0/dbt/adapters/doris/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/__init__.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/column.py
--rw-r--r--   0 root         (0) root         (0)     4880 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/connections.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/impl.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/adapters/doris/relation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.932630 dbt-doris-0.3.0/dbt/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.934630 dbt-doris-0.3.0/dbt/include/doris/
--rw-r--r--   0 root         (0) root         (0)      879 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/dbt_project.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.932630 dbt-doris-0.3.0/dbt/include/doris/macros/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.935629 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/columns.sql
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/freshness.sql
--rw-r--r--   0 root         (0) root         (0)     3336 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/metadata.sql
--rw-r--r--   0 root         (0) root         (0)     6112 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/relation.sql
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/adapters/schema.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.932630 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.935629 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/incremental/
--rw-r--r--   0 root         (0) root         (0)     2751 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/incremental/help.sql
--rw-r--r--   0 root         (0) root         (0)     5197 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.935629 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/helpers.sql
--rw-r--r--   0 root         (0) root         (0)     4804 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/partition.sql
--rw-r--r--   0 root         (0) root         (0)     1162 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/replace.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.935629 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/seed/
--rw-r--r--   0 root         (0) root         (0)     2003 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/seed/helpers.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.936630 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/snapshot/
--rw-r--r--   0 root         (0) root         (0)     3137 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.936630 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/table/
--rw-r--r--   0 root         (0) root         (0)     1703 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/table/create_table_as.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.936630 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/view/
--rw-r--r--   0 root         (0) root         (0)     1009 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/macros/materializations/view/create_view_as.sql
--rw-r--r--   0 root         (0) root         (0)     1386 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/profile_template.yml
--rw-r--r--   0 root         (0) root         (0)     1007 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/dbt/include/doris/sample_profiles.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:22:59.936630 dbt-doris-0.3.0/dbt_doris.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-10 03:22:59.000000 dbt-doris-0.3.0/dbt_doris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1412 2023-07-10 03:22:59.000000 dbt-doris-0.3.0/dbt_doris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:22:59.000000 dbt-doris-0.3.0/dbt_doris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-10 03:22:59.000000 dbt-doris-0.3.0/dbt_doris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-10 03:22:59.000000 dbt-doris-0.3.0/dbt_doris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 03:22:59.937630 dbt-doris-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1619 2023-07-10 02:50:26.000000 dbt-doris-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.503066 dbt-doris-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-20 09:19:47.503066 dbt-doris-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.496066 dbt-doris-0.3.1/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.496066 dbt-doris-0.3.1/dbt/adapters/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.499066 dbt-doris-0.3.1/dbt/adapters/doris/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/adapters/doris/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-07-20 09:17:27.000000 dbt-doris-0.3.1/dbt/adapters/doris/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/adapters/doris/column.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/adapters/doris/connections.py
+-rw-r--r--   0 root         (0) root         (0)     7593 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/adapters/doris/impl.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/adapters/doris/relation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.496066 dbt-doris-0.3.1/dbt/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.499066 dbt-doris-0.3.1/dbt/include/doris/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-20 09:17:31.000000 dbt-doris-0.3.1/dbt/include/doris/dbt_project.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.497066 dbt-doris-0.3.1/dbt/include/doris/macros/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.500066 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/columns.sql
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/freshness.sql
+-rw-r--r--   0 root         (0) root         (0)     3336 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/metadata.sql
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-07-20 09:15:02.000000 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/relation.sql
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/adapters/schema.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.497066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.500066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/incremental/
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/incremental/help.sql
+-rw-r--r--   0 root         (0) root         (0)     5494 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.501066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/helpers.sql
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/partition.sql
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/replace.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.501066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/seed/
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/seed/helpers.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.501066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/snapshot/
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.501066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/table/
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/table/create_table_as.sql
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-20 09:15:02.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/table/table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.502066 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/view/
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/view/create_view_as.sql
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/macros/materializations/view/view.sql
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/profile_template.yml
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-07-19 04:07:26.000000 dbt-doris-0.3.1/dbt/include/doris/sample_profiles.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 09:19:47.502066 dbt-doris-0.3.1/dbt_doris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-20 09:19:47.000000 dbt-doris-0.3.1/dbt_doris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-20 09:19:47.000000 dbt-doris-0.3.1/dbt_doris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 09:19:47.000000 dbt-doris-0.3.1/dbt_doris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-20 09:19:47.000000 dbt-doris-0.3.1/dbt_doris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-20 09:19:47.000000 dbt-doris-0.3.1/dbt_doris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 09:19:47.503066 dbt-doris-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-07-20 09:17:21.000000 dbt-doris-0.3.1/setup.py
```

### Comparing `dbt-doris-0.3.0/LICENSE` & `dbt-doris-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/MANIFEST.in` & `dbt-doris-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/__init__.py` & `dbt-doris-0.3.1/dbt/adapters/doris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/__version__.py` & `dbt-doris-0.3.1/dbt/adapters/doris/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 # this 'version' must be set !!!
 # otherwise the adapters will not be found after the 'dbt init xxx' command 
 
-version = "0.3.0"
+version = "0.3.1"
```

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/column.py` & `dbt-doris-0.3.1/dbt/adapters/doris/column.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/connections.py` & `dbt-doris-0.3.1/dbt/adapters/doris/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/impl.py` & `dbt-doris-0.3.1/dbt/adapters/doris/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,28 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from dbt.adapters.sql import SQLAdapter
 
 from concurrent.futures import Future
 from enum import Enum
-from typing import Callable, Dict, List, Optional, Set, Tuple
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+)
 
 import agate
 import dbt.exceptions
 from dbt.adapters.base.impl import _expect_row_value, catch_as_completed
 from dbt.adapters.base.relation import InformationSchema, BaseRelation
 from dbt.adapters.doris.column import DorisColumn
 from dbt.adapters.doris.connections import DorisConnectionManager
@@ -182,8 +195,22 @@
 
     # Methods used in adapter tests
     def timestamp_add_sql(self, add_to: str, number: int = 1, interval: str = "hour") -> str:
         # for backwards compatibility, we're compelled to set some sort of
         # default. A lot of searching has lead me to believe that the
         # '+ interval' syntax used in postgres/redshift is relatively common
         # and might even be the SQL standard's intention.
-        return f"{add_to} + interval {number} {interval}"    
+        return f"{add_to} + interval {number} {interval}"
+
+    @classmethod
+    def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
+        rendered_column_constraints = []
+        for v in raw_columns.values():
+            col_name = cls.quote(v["name"]) if v.get("quote") else v["name"]
+            data_type = v.get('data_type')
+            if data_type is not None:
+                rendered_column_constraint = [f"cast(`{col_name}` as {data_type}) as `{col_name}`"]
+            else:
+                rendered_column_constraint = [f"`{col_name}` as `{col_name}`"]
+            rendered_column_constraints.append(" ".join(rendered_column_constraint))
+
+        return rendered_column_constraints
```

### Comparing `dbt-doris-0.3.0/dbt/adapters/doris/relation.py` & `dbt-doris-0.3.1/dbt/adapters/doris/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/__init__.py` & `dbt-doris-0.3.1/dbt/include/doris/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/dbt_project.yml` & `dbt-doris-0.3.1/dbt/include/doris/dbt_project.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 name: dbt_doris
-version: 0.3.0
+version: 0.3.1
 config-version: 2
 
 macro-paths: ["macros"]
```

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/adapters/columns.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/adapters/schema.sql`

 * *Files 25% similar despite different names*

```diff
@@ -11,25 +11,22 @@
 -- Unless required by applicable law or agreed to in writing,
 -- software distributed under the License is distributed on an
 -- "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 -- KIND, either express or implied. See the License for the
 -- specific language governing permissions and limitations
 -- under the License.
 
-{% macro doris__get_columns_in_relation(relation) -%}
-    {% call statement('get_columns_in_relation', fetch_result=True) %}
-        select column_name              as `column`,
-       data_type                as 'dtype',
-       character_maximum_length as char_size,
-       numeric_precision,
-       numeric_scale
-from information_schema.columns
-where table_schema = '{{ relation.schema }}'
-  and table_name = '{{ relation.identifier }}'
-    {% endcall %}
-    {% set table = load_result('get_columns_in_relation').table %}
-    {{ return(sql_convert_columns_in_relation(table)) }}
-{%- endmacro %}
 
-{% macro doris__alter_column_type(relation,column_name,new_column_type) -%}
-'''Changes column name or data type'''
-{% endmacro %}
+-- doris have not 'schema' to make a collection of table or view
+
+{% macro doris__drop_schema(relation) -%}
+  {%- call statement('drop_schema') -%}
+    drop database if exists {{ relation.without_identifier().include(database=False) }} 
+  {%- endcall -%}
+{% endmacro %}
+
+
+{% macro doris__create_schema(relation) -%}
+  {%- call statement('create_schema') -%}
+    create database if not exists {{ relation.without_identifier().include(database=False) }}
+  {% endcall %}
+{% endmacro %}
```

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/adapters/freshness.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/adapters/metadata.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/adapters/relation.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/adapters/relation.sql`

 * *Files 13% similar despite different names*

```diff
@@ -54,14 +54,19 @@
         {{ item }}
       {% if not loop.last %},{% endif %}
       {% endfor %}
     )
   {% endif %}
 {%- endmacro %}
 
+{% macro doris__table_comment() -%}
+  {% set description = model.get('description', "") %}
+  COMMENT '{{description}}'
+{%- endmacro %}
+
 {% macro doris__unique_key() -%}
   {% set cols = config.get('unique_key', validator=validation.any[list, basestring]) %}
 
   {% if cols is not none %}
     {%- if cols is string -%}
       {%- set cols = [cols] -%}
     {%- endif -%}
@@ -111,21 +116,24 @@
           "{{ key }}" = "{{ value }}"{% if not loop.last %},{% endif %}
         {% endfor %}
     )
   {% endif %}
 {%- endmacro%}
 
 {% macro doris__drop_relation(relation) -%}
+  {% if relation is not none %}
     {% set relation_type = relation.type %}
-    {% if relation_type is none %}
+    {% if not relation_type or relation_type is none %}
         {% set relation_type = 'table' %}
     {% endif %}
     {% call statement('drop_relation', auto_begin=False) %}
-    drop {{ relation_type }} if exists {{ relation }}
+      drop {{ relation_type }} if exists {{ relation }}
     {% endcall %}
+  {% endif %}
+
 {%- endmacro %}
 
 {% macro doris__truncate_relation(relation) -%}
     {% call statement('truncate_relation') %}
       truncate table {{ relation }}
     {% endcall %}
 {%- endmacro %}
@@ -133,53 +141,77 @@
 {% macro doris__rename_relation(from_relation, to_relation) -%}
   {% call statement('drop_relation') %}
     drop {{ to_relation.type }} if exists {{ to_relation }}
   {% endcall %}
   {% call statement('rename_relation') %}
     {% if to_relation.is_view %}
     {% set results = run_query('show create view ' + from_relation.render() ) %}
-    create view {{ to_relation }} as {{ results[0]['Create View'].replace(from_relation.table, to_relation.table).split('AS',1)[1] }}
+    create view {{ to_relation }} as {{ results[0]['Create View'].split('AS',1)[1] }}
     {% else %}
     alter table {{ from_relation }} rename {{ to_relation.table }}
     {% endif %}
   {% endcall %}
 
   {% if to_relation.is_view %}
     {% call statement('rename_relation_end_drop_old') %}
       drop view if exists {{ from_relation }}
     {% endcall %}
   {% endif %}
 
-  {%- endmacro %}
+{%- endmacro %}
+
+
+{% macro exchange_relation(relation1, relation2, is_drop_r1=false) -%}
+
+  {% if relation2.is_view %}
+    {% set from_results = run_query('show create view ' + relation1.render() ) %}
+    {% set to_results = run_query('show create view ' + relation2.render() ) %}
+      {% call statement('exchange_view_relation') %}
+        alter view {{ relation1 }} as {{  to_results[0]['Create View'].split('AS',1)[1] }}
+      {% endcall %}
+    {% if is_drop_r1 %}
+      {% do doris__drop_relation(relation2) %}
+    {% else %}
+      {% call statement('exchange_view_relation') %}
+        alter view {{ relation2 }} as {{  from_results[0]['Create View'].split('AS',1)[1] }}
+      {% endcall %}
+    {% endif %}
+  {% else %}
+    {% call statement('exchange_relation') %}
+      ALTER TABLE {{ relation1 }} REPLACE WITH TABLE `{{ relation2.table }}` PROPERTIES('swap' = '{{not is_drop_r1}}');
+    {% endcall %}
+  {% endif %}
+
+{%- endmacro %}
 
 {% macro doris__timestimp_id() -%}
  {{ return( (modules.datetime.datetime.now() ~ "").replace('-','').replace(':','').replace('.','').replace(' ','') ) }}
 {%- endmacro %}
 
 {% macro doris__with_label() -%}
   {% set lable_suffix_id = config.get('label_id', validator=validation.any[basestring]) %}
   {% if lable_suffix_id in [none,'DEFAULT'] %}
     WITH LABEL dbt_doris_label_{{doris__timestimp_id()}}
   {% else %}
     WITH LABEL dbt_doris_label_{{ lable_suffix_id }}
-  {% endif %}  
+  {% endif %}
 {%- endmacro %}
 
 {% macro doris__get_or_create_relation(database, schema, identifier, type) %}
   {%- set target_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) %}
-  
+
   {% if target_relation %}
     {% do return([true, target_relation]) %}
   {% endif %}
-  
+
   {%- set new_relation = api.Relation.create(
       database=none,
       schema=schema,
       identifier=identifier,
       type=type
   ) -%}
   {% do return([false, new_relation]) %}
 {% endmacro %}
 
 {% macro catalog_source(catalog,database,table) -%}
-  `{{catalog}}`.`{{database}}`.`{{table}}` 
+  `{{catalog}}`.`{{database}}`.`{{table}}`
 {%- endmacro %}
```

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/incremental/help.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/incremental/help.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/incremental/incremental.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/incremental/incremental.sql`

 * *Files 8% similar despite different names*

```diff
@@ -24,45 +24,53 @@
   {% set tmp_relation = make_temp_relation(this) %}
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
   {% set to_drop = [] %}
   {#-- append or no unique key --#}
 
 
-  {% if unique_key is none or strategy == 'append'  %}
+
+  {% if not unique_key or strategy == 'append'  %}
         {#-- create table first --#}
         {% if existing_relation is none  %}
             {% set build_sql = doris__create_table_as(False, target_relation, sql) %}
         {% elif existing_relation.is_view or full_refresh_mode %}
-            {#-- backup data before drop old table #}
+            {#-- backup table is new table ,exchange table backup and old table #}
             {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
             {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
             {% do adapter.drop_relation(backup_relation) %} {#-- likes 'drop table if exists ... ' --#}
-            {% do adapter.rename_relation(target_relation, backup_relation) %}
-            {% set build_sql = doris__create_table_as(False, target_relation, sql) %}
-            {% do to_drop.append(backup_relation) %}
+            {% set run_sql = doris__create_table_as(False, backup_relation, sql) %}
+            {% call statement("run_sql") %}
+                {{ run_sql }}
+            {% endcall %}
+            {% do exchange_relation(target_relation, backup_relation, True) %}
+            {% set build_sql = "show frontends" %}
         {#-- append data --#}
         {% else %}
+            {% do to_drop.append(tmp_relation) %}
             {% do run_query(create_table_as(True, tmp_relation, sql)) %}
             {% set build_sql = tmp_insert(tmp_relation, target_relation, unique_key=none) %}
         {% endif %}
   {#-- insert overwrite --#}
   {% elif strategy == 'insert_overwrite' %}
         {#-- create table first --#}
         {% if existing_relation is none  %}
             {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
         {#-- insert data refresh --#}
         {% elif existing_relation.is_view or full_refresh_mode %}
-            {#-- backup data before drop old table #}
+            {#-- backup table is new table ,exchange table backup and old table #}
             {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
             {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
             {% do adapter.drop_relation(backup_relation) %} {#-- likes 'drop table if exists ... ' --#}
-            {% do adapter.rename_relation(target_relation, backup_relation) %}
-            {% set build_sql = doris__create_unique_table_as(False, target_relation, sql) %}
-            {% do to_drop.append(backup_relation) %}
+            {% set run_sql = doris__create_unique_table_as(False, backup_relation, sql) %}
+            {% call statement("run_sql") %}
+                {{ run_sql }}
+            {% endcall %}
+            {% do exchange_relation(target_relation, backup_relation, True) %}
+            {% set build_sql = "show frontends" %}
         {#-- append data --#}
         {% else %}
           {#-- check doris unique table  --#}
           {% if not is_unique_model(target_relation) %}
                 {% do exceptions.raise_compiler_error("doris table:"~ target_relation ~ ", model must be 'UNIQUE'" ) %}
           {% endif %}
           {#-- create temp duplicate table for this incremental task  --#}
```

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/helpers.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/partition.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/partition.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/partition/replace.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/partition/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/seed/helpers.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/seed/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/snapshot/snapshot.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/snapshot/strategies.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/table/create_table_as.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/table/create_table_as.sql`

 * *Files 22% similar despite different names*

```diff
@@ -20,24 +20,36 @@
     {% set table = relation.include(database=False) %}
     {{ sql_header if sql_header is not none }}
     {%if temporary %}
         {{doris__drop_relation(relation)}}
     {% endif %}
     create table {{ table }}
     {{ doris__duplicate_key() }}
+    {{ doris__table_comment()}}
     {{ doris__partition_by() }}
     {{ doris__distributed_by() }}
-    {{ doris__properties() }} as {{ sql }};
+    {{ doris__properties() }} as {{ doris__table_colume_type(sql) }};
 
 {%- endmacro %}
 
 {% macro doris__create_unique_table_as(temporary, relation, sql) -%}
     {% set sql_header = config.get('sql_header', none) %}
     {% set table = relation.include(database=False) %}
     {{ sql_header if sql_header is not none }}
     create table {{ table }}
     {{ doris__unique_key() }}
+    {{ doris__table_comment()}}
     {{ doris__partition_by() }}
     {{ doris__distributed_by() }}
-    {{ doris__properties() }} as {{ sql }};
+    {{ doris__properties() }} as {{ doris__table_colume_type(sql) }};
 
+{%- endmacro %}
+
+
+{% macro doris__table_colume_type(sql) -%}
+    {% set cols = model.get('columns') %}
+    {% if cols %}
+        select {{get_table_columns_and_constraints()}} from ({{sql}}) `_table_colume_type_name`
+    {% else %}
+        {{sql}}
+    {%- endif -%}
 {%- endmacro %}
```

### Comparing `dbt-doris-0.3.0/dbt/include/doris/macros/materializations/view/create_view_as.sql` & `dbt-doris-0.3.1/dbt/include/doris/macros/materializations/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/profile_template.yml` & `dbt-doris-0.3.1/dbt/include/doris/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt/include/doris/sample_profiles.yml` & `dbt-doris-0.3.1/dbt/include/doris/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-doris-0.3.0/dbt_doris.egg-info/SOURCES.txt` & `dbt-doris-0.3.1/dbt_doris.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,13 +22,15 @@
 dbt/include/doris/macros/materializations/partition/helpers.sql
 dbt/include/doris/macros/materializations/partition/partition.sql
 dbt/include/doris/macros/materializations/partition/replace.sql
 dbt/include/doris/macros/materializations/seed/helpers.sql
 dbt/include/doris/macros/materializations/snapshot/snapshot.sql
 dbt/include/doris/macros/materializations/snapshot/strategies.sql
 dbt/include/doris/macros/materializations/table/create_table_as.sql
+dbt/include/doris/macros/materializations/table/table.sql
 dbt/include/doris/macros/materializations/view/create_view_as.sql
+dbt/include/doris/macros/materializations/view/view.sql
 dbt_doris.egg-info/PKG-INFO
 dbt_doris.egg-info/SOURCES.txt
 dbt_doris.egg-info/dependency_links.txt
 dbt_doris.egg-info/requires.txt
 dbt_doris.egg-info/top_level.txt
```

### Comparing `dbt-doris-0.3.0/setup.py` & `dbt-doris-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-doris"
 # make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "0.3.0"
+package_version = "0.3.1"
 dbt_core_version = "1.5.0"
 description = """The doris adapter plugin for dbt """
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -35,10 +35,11 @@
     author_email="1391869588@qq.com",
     url="https://github.com/apache/doris/tree/master/extension/dbt-doris",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
         "mysql-connector-python>=8.0.0,<8.1",
+        "urllib3~=1.0",
     ],
     python_requires=">=3.7.2",
 )
```

