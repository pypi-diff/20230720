# Comparing `tmp/phc-ingestion-0.3.42.tar.gz` & `tmp/phc-ingestion-0.3.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.42.tar", last modified: Tue Jul 18 15:38:58 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.43.tar", last modified: Thu Jul 20 12:09:00 2023, max compression
```

## Comparing `phc-ingestion-0.3.42.tar` & `phc-ingestion-0.3.43.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-07-18 15:38:30.902901 phc-ingestion-0.3.42/PYPI.md
--rw-r--r--   0        0        0        0 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1636 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4676 2023-07-18 15:38:30.910900 phc-ingestion-0.3.42/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21663 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     6933 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3142 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     5489 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-07-18 15:38:30.914900 phc-ingestion-0.3.42/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.42/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-07-20 12:08:35.643091 phc-ingestion-0.3.43/PYPI.md
+-rw-r--r--   0        0        0        0 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1636 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4676 2023-07-20 12:08:35.651092 phc-ingestion-0.3.43/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21663 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     6933 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5489 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-07-20 12:08:35.655092 phc-ingestion-0.3.43/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.43/PKG-INFO
```

### Comparing `phc-ingestion-0.3.42/ingestion/caris/process.py` & `phc-ingestion-0.3.43/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.43/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.43/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.43/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.43/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/json.py` & `phc-ingestion-0.3.43/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.43/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.43/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.43/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.43/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/foundation/process.py` & `phc-ingestion-0.3.43/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.43/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.43/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.43/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.43/ingestion/foundation/util/vcf_etl.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,40 +99,42 @@
     elif vendsig in ["unknown"]:
         return "VENDSIG=Uncertain significance"
     else:
         return "VENDSIG=Unknown"
 
 
 def add_vendsig_to_info(var: str, xml_short_vars: dict) -> str:
-    info = var.split("\t")[7]
-    # using transcript name, find it in xml_short_vars
-    transcript_name = info.split(";")[-1].split("=")[1].strip()
+    split_var = var.split("\t")
+    # get 'chr:pos' from var
+    var_position = f"{split_var[0]}:{split_var[1]}"
+
+    # Info section -> dict, get depth
+    info_dict = {x.split("=")[0]: x.split("=")[1] for x in split_var[7].split(";")}
+    var_depth = info_dict["depth"]
+
     # dictionary comprehension to get the short_var in xml_short_vars that matches the transcript_name
     if xml_short_vars == {}:
         vendsig = "Unknown"
     else:
         if isinstance(xml_short_vars, dict):
-            if xml_short_vars.get("@transcript", "") == transcript_name:
-                vendsig = xml_short_vars["@status"]
-            else:
-                vendsig = "Unknown"
+            xml_short_vars = [xml_short_vars]
 
+        matched_xml_var = [
+            short_var
+            for short_var in xml_short_vars
+            if short_var.get("@position", "") == var_position
+            and short_var.get("@depth", "") == var_depth
+        ]
+        if not matched_xml_var:
+            vendsig = "Unknown"
         else:
-            matched_xml_var = [
-                short_var
-                for short_var in xml_short_vars
-                if short_var.get("@transcript", "") == transcript_name
-            ]
-            if not matched_xml_var:
-                vendsig = "Unknown"
-            else:
-                vendsig = matched_xml_var[0]["@status"]
+            vendsig = matched_xml_var[0]["@status"]
 
     mapped_vendsig = map_vendsig(vendsig)
-    new_vcf_info = f"{info.strip()};{mapped_vendsig}"
+    new_vcf_info = f"{split_var[7].strip()};{mapped_vendsig}"
     return new_vcf_info
 
 
 def transform_scientific_notation_in_af(var: str) -> str:
     var_split = var.split("\t")
     var_info = var_split[-1]
     var_info_split = var_info.split(";")
```

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/process.py` & `phc-ingestion-0.3.43/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.43/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.43/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.43/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.43/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.43/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.43/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.43/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.43/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.43/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.42/pyproject.toml` & `phc-ingestion-0.3.43/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.42"
+version = "0.3.43"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

