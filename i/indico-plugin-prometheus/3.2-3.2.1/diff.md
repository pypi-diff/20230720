# Comparing `tmp/indico_plugin_prometheus-3.2-py3-none-any.whl.zip` & `tmp/indico_plugin_prometheus-3.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7831 bytes, number of entries: 11
--rw-r--r--  2.0 unx      330 b- defN 23-May-03 14:59 indico_prometheus/__init__.py
--rw-r--r--  2.0 unx      468 b- defN 23-May-03 14:59 indico_prometheus/blueprint.py
--rw-r--r--  2.0 unx     1920 b- defN 23-May-03 14:59 indico_prometheus/controllers.py
--rw-r--r--  2.0 unx     7372 b- defN 23-May-03 14:59 indico_prometheus/metrics.py
--rw-r--r--  2.0 unx     2488 b- defN 23-May-03 14:59 indico_prometheus/plugin.py
--rw-r--r--  2.0 unx     4409 b- defN 23-May-03 14:59 indico_prometheus/queries.py
--rw-r--r--  2.0 unx     1398 b- defN 23-May-03 15:35 indico_plugin_prometheus-3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 15:35 indico_plugin_prometheus-3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-May-03 15:35 indico_plugin_prometheus-3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-May-03 15:35 indico_plugin_prometheus-3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      982 b- defN 23-May-03 15:35 indico_plugin_prometheus-3.2.dist-info/RECORD
-11 files, 19549 bytes uncompressed, 6139 bytes compressed:  68.6%
+Zip file size: 7889 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-01 10:35 indico_prometheus/__init__.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jun-01 10:35 indico_prometheus/blueprint.py
+-rw-r--r--  2.0 unx     1920 b- defN 23-Jun-01 10:35 indico_prometheus/controllers.py
+-rw-r--r--  2.0 unx     7372 b- defN 23-Jun-01 10:35 indico_prometheus/metrics.py
+-rw-r--r--  2.0 unx     2488 b- defN 23-Jun-01 10:35 indico_prometheus/plugin.py
+-rw-r--r--  2.0 unx     4409 b- defN 23-Jun-01 10:35 indico_prometheus/queries.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-Jul-20 19:36 indico_plugin_prometheus-3.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:36 indico_plugin_prometheus-3.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-20 19:36 indico_plugin_prometheus-3.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-20 19:36 indico_plugin_prometheus-3.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-20 19:36 indico_plugin_prometheus-3.2.1.dist-info/RECORD
+11 files, 19685 bytes uncompressed, 6177 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: indico_prometheus/plugin.py
 Comment: 
 
 Filename: indico_prometheus/queries.py
 Comment: 
 
-Filename: indico_plugin_prometheus-3.2.dist-info/METADATA
+Filename: indico_plugin_prometheus-3.2.1.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_prometheus-3.2.dist-info/WHEEL
+Filename: indico_plugin_prometheus-3.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_prometheus-3.2.dist-info/entry_points.txt
+Filename: indico_plugin_prometheus-3.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_prometheus-3.2.dist-info/top_level.txt
+Filename: indico_plugin_prometheus-3.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_prometheus-3.2.dist-info/RECORD
+Filename: indico_plugin_prometheus-3.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `indico_plugin_prometheus-3.2.dist-info/METADATA` & `indico_plugin_prometheus-3.2.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: indico-plugin-prometheus
-Version: 3.2
+Version: 3.2.1
 Summary: Prometheus metrics in Indico servers
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.9.0
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: indico (>=3.2)
-Requires-Dist: prometheus-client (==0.16.0)
+Requires-Dist: prometheus-client (==0.17.1)
 
 # Indico Prometheus Plugin
 
 This plugin exposes a `/metrics` endpoint which provides Prometheus-compatible output.
 
 ![](https://raw.githubusercontent.com/indico/indico-plugins/master/prometheus/screenshot.png)
 
@@ -41,10 +42,15 @@
 ```yaml
     tls_config:
       insecure_skip_verify: false
 ```
 
 ## Changelog
 
+### 3.2.1
+
+- Support Python 3.11
+- Use latest prometheus-client library
+
 ### 3.2
 
 - Initial release for Indico 3.2
```

## Comparing `indico_plugin_prometheus-3.2.dist-info/RECORD` & `indico_plugin_prometheus-3.2.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 indico_prometheus/__init__.py,sha256=MYYkawNT7Az7NKemuzOTF8d8sdIJ7piijhrhLV0YSj0,330
 indico_prometheus/blueprint.py,sha256=zCpN0ZXcWjJXrlnuQfutsEqDK5SNv2Dlaeb9dVLQfIc,468
 indico_prometheus/controllers.py,sha256=LbT0SAfRKPFU3HEArMrXcQyG9w6kJ1gpfA1RXA44Vos,1920
 indico_prometheus/metrics.py,sha256=fbBrIcGw1dsZ94xhJWD9hTMwc83gbyCZk2fzPb-YIWw,7372
 indico_prometheus/plugin.py,sha256=Nqqub7XVvmsoqv9cen3Y-BAPBOEQ5BiWIy4nEFQntRg,2488
 indico_prometheus/queries.py,sha256=BQ5OJb0IfdBmOM8pzZihZ5w4mFzsbnM4s-H8QEOfqoE,4409
-indico_plugin_prometheus-3.2.dist-info/METADATA,sha256=sZe1i_6ZPhNJv19DjOspLSXU7Y1hYB8y2sIeC55mNUk,1398
-indico_plugin_prometheus-3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-indico_plugin_prometheus-3.2.dist-info/entry_points.txt,sha256=MX-uVjJGiaGM3nTbz3JNVy8QtRkQl-W8aGC3FueF5TY,72
-indico_plugin_prometheus-3.2.dist-info/top_level.txt,sha256=NgY6m8lpJP9yiLdmC_Cw5yLl4i91qeIDXHHkUQCgkDM,18
-indico_plugin_prometheus-3.2.dist-info/RECORD,,
+indico_plugin_prometheus-3.2.1.dist-info/METADATA,sha256=oaDpAwNbY2frUm1CYIN_LNGP64XfKzJmBKq_dijpNnI,1524
+indico_plugin_prometheus-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_prometheus-3.2.1.dist-info/entry_points.txt,sha256=MX-uVjJGiaGM3nTbz3JNVy8QtRkQl-W8aGC3FueF5TY,72
+indico_plugin_prometheus-3.2.1.dist-info/top_level.txt,sha256=NgY6m8lpJP9yiLdmC_Cw5yLl4i91qeIDXHHkUQCgkDM,18
+indico_plugin_prometheus-3.2.1.dist-info/RECORD,,
```

