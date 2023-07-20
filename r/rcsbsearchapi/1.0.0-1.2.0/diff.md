# Comparing `tmp/rcsbsearchapi-1.0.0.tar.gz` & `tmp/rcsbsearchapi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsbsearchapi-1.0.0.tar", last modified: Fri Jun  9 18:37:35 2023, max compression
+gzip compressed data, was "rcsbsearchapi-1.2.0.tar", last modified: Thu Jul 20 15:05:48 2023, max compression
```

## Comparing `rcsbsearchapi-1.0.0.tar` & `rcsbsearchapi-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 18:37:35.187482 rcsbsearchapi-1.0.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1543 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     6087 2023-06-09 18:37:35.187482 rcsbsearchapi-1.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5189 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 18:37:35.183481 rcsbsearchapi-1.0.0/rcsbsearchapi/
--rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/const.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 18:37:35.183481 rcsbsearchapi-1.0.0/rcsbsearchapi/resources/
--rw-r--r--   0 vsts      (1001) docker     (122)  1191737 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/resources/metadata_schema.json
--rw-r--r--   0 vsts      (1001) docker     (122)     5822 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/schema.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32951 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/search.py
--rw-r--r--   0 vsts      (1001) docker     (122)      484 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/rcsbsearchapi/update_schema.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 18:37:35.183481 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     6087 2023-06-09 18:37:35.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      498 2023-06-09 18:37:35.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 18:37:35.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 18:37:05.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-06-09 18:37:35.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-06-09 18:37:35.000000 rcsbsearchapi-1.0.0/rcsbsearchapi.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-06-09 18:37:35.187482 rcsbsearchapi-1.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 18:37:35.187482 rcsbsearchapi-1.0.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)     1791 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/tests/testschema.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15454 2023-06-09 18:36:46.000000 rcsbsearchapi-1.0.0/tests/testsearch.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1543 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    12444 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    11548 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.637082 rcsbsearchapi-1.2.0/rcsbsearchapi/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/const.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/
+-rw-r--r--   0 vsts      (1001) docker     (122)   173785 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/chemical_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (122)  1290883 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/resources/metadata_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     5766 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/schema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    37888 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/search.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/rcsbsearchapi/update_schema.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.637082 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12444 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-20 15:05:16.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-07-20 15:05:48.000000 rcsbsearchapi-1.2.0/rcsbsearchapi.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2572 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-20 15:05:48.641083 rcsbsearchapi-1.2.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2881 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/tests/testschema.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25332 2023-07-20 15:04:54.000000 rcsbsearchapi-1.2.0/tests/testsearch.py
```

### Comparing `rcsbsearchapi-1.0.0/LICENSE` & `rcsbsearchapi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsbsearchapi-1.0.0/rcsbsearchapi/__init__.py` & `rcsbsearchapi-1.2.0/rcsbsearchapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RCSB PDB Search API"""
 from typing import TYPE_CHECKING, Any, List
 
 from .search import Terminal  # noqa: F401
 from .search import Attr, Group, Query, Session, TextQuery, Value
 
-__version__ = "1.0.0"
+__version__ = "1.2.0"
 
 
 # loading rcsb_attributes can cause errors, so load it lazily
 if TYPE_CHECKING:
     from .schema import SchemaGroup
 
 
@@ -41,15 +41,14 @@
 
 
 def __getattr__(name: str) -> Any:
     # delay instantiating rcsb_attributes until it is needed
     if name == "rcsb_attributes":
         if "rcsb_attributes" not in globals():
             from .schema import rcsb_attributes as attrs
-
             globals()["rcsb_attributes"] = attrs
         return globals()["rcsb_attributes"]
     raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
 
 
 def __dir__() -> List[str]:
     return sorted(__all__)
```

### Comparing `rcsbsearchapi-1.0.0/rcsbsearchapi/resources/metadata_schema.json` & `rcsbsearchapi-1.2.0/rcsbsearchapi/resources/metadata_schema.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9374934286511776%*

 * *Differences: {"'$comment'": "'Schema version: 1.42.3'",*

 * * "'properties'": "{'rcsb_ligand_neighbors': {'items': {'properties': {'distance': "*

 * *                 "{'rcsb_current_maximum_value': 5}}}}, 'diffrn_detector': {'items': "*

 * *                 "{'properties': {'pdbx_collection_date': {'rcsb_current_maximum_value': "*

 * *                 "1686873600000}}}}, 'em_image_recording': {'items': {'properties': "*

 * *                 "{'num_grids_imaged': {'rcsb_current_maximum_value': 7770}}}}, "*

 * *                 "'rcsb_accession_info' […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$comment": "Schema version: 1.42.0",
+    "$comment": "Schema version: 1.42.3",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "",
     "properties": {
         "audit_author": {
             "items": {
                 "additionalProperties": false,
@@ -156,15 +156,15 @@
                         }
                     ],
                     "rcsb_units": "degrees",
                     "type": "number"
                 },
                 "angle_gamma": {
                     "description": "Unit-cell angle gamma of the reported structure in degrees.",
-                    "rcsb_current_maximum_value": 125.0,
+                    "rcsb_current_maximum_value": 125,
                     "rcsb_current_minimum_value": 57.76,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Unit-cell angle gamma of the reported structure in degrees."
                         },
                         {
@@ -192,16 +192,16 @@
                             "text": "The number of the formula units in the unit cell as specified\n by _chemical_formula.structural, _chemical_formula.moiety or\n _chemical_formula.sum."
                         }
                     ],
                     "type": "integer"
                 },
                 "length_a": {
                     "description": "Unit-cell length a corresponding to the structure reported in\nangstroms.",
-                    "rcsb_current_maximum_value": 1255.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 1255,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Unit-cell length a corresponding to the structure reported in\nangstroms."
                         },
                         {
                             "context": "brief",
@@ -218,16 +218,16 @@
                         }
                     ],
                     "rcsb_units": "angstroms",
                     "type": "number"
                 },
                 "length_b": {
                     "description": "Unit-cell length b corresponding to the structure reported in\n angstroms.",
-                    "rcsb_current_maximum_value": 1255.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 1255,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Unit-cell length b corresponding to the structure reported in\n angstroms."
                         },
                         {
                             "context": "brief",
@@ -245,15 +245,15 @@
                     ],
                     "rcsb_units": "angstroms",
                     "type": "number"
                 },
                 "length_c": {
                     "description": "Unit-cell length c corresponding to the structure reported in\nangstroms.",
                     "rcsb_current_maximum_value": 1933.3,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Unit-cell length c corresponding to the structure reported in\nangstroms."
                         },
                         {
                             "context": "brief",
@@ -762,16 +762,16 @@
                         "rcsb_search_context": [
                             "exact-match"
                         ],
                         "type": "string"
                     },
                     "year": {
                         "description": "The year of the citation; relevant for journal articles, books\n and book chapters.",
-                        "rcsb_current_maximum_value": 2023.0,
-                        "rcsb_current_minimum_value": 1947.0,
+                        "rcsb_current_maximum_value": 2023,
+                        "rcsb_current_minimum_value": 1947,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The year of the citation; relevant for journal articles, books\n and book chapters."
                             },
                             {
                                 "context": "deposition",
@@ -806,16 +806,16 @@
         },
         "diffrn": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "ambient_pressure": {
                         "description": "The mean hydrostatic pressure in kilopascals at which the\n intensities were measured.",
-                        "rcsb_current_maximum_value": 430000.0,
-                        "rcsb_current_minimum_value": 101.0,
+                        "rcsb_current_maximum_value": 430000,
+                        "rcsb_current_minimum_value": 101,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The mean hydrostatic pressure in kilopascals at which the\n intensities were measured."
                             },
                             {
                                 "context": "brief",
@@ -827,15 +827,15 @@
                         ],
                         "rcsb_units": "kilopascals",
                         "type": "number"
                     },
                     "ambient_temp": {
                         "description": "The mean temperature in kelvins at which the intensities were\n measured.",
                         "rcsb_current_maximum_value": 446.15,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The mean temperature in kelvins at which the intensities were\n measured."
                             },
                             {
                                 "context": "deposition",
@@ -1032,16 +1032,16 @@
                     },
                     "pdbx_collection_date": {
                         "description": "The date of data collection.",
                         "examples": [
                             "1996-12-25"
                         ],
                         "format": "date-time",
-                        "rcsb_current_maximum_value": 1683331200000.0,
-                        "rcsb_current_minimum_value": -27080352000000.0,
+                        "rcsb_current_maximum_value": 1686873600000,
+                        "rcsb_current_minimum_value": -27080352000000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The date of data collection."
                             },
                             {
                                 "context": "deposition",
@@ -1491,16 +1491,16 @@
         },
         "em_2d_crystal_entity": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "angle_gamma": {
                         "description": "Unit-cell angle gamma in degrees.",
-                        "rcsb_current_maximum_value": 120.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 120,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell angle gamma in degrees."
                             },
                             {
                                 "context": "brief",
@@ -1511,16 +1511,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "degrees",
                         "type": "number"
                     },
                     "c_sampling_length": {
                         "description": "Length used to sample the reciprocal lattice lines in the c-direction.",
-                        "rcsb_current_maximum_value": 320.0,
-                        "rcsb_current_minimum_value": 10.0,
+                        "rcsb_current_maximum_value": 320,
+                        "rcsb_current_minimum_value": 10,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Length used to sample the reciprocal lattice lines in the c-direction."
                             },
                             {
                                 "context": "brief",
@@ -1554,16 +1554,16 @@
                         "type": "string"
                     },
                     "length_a": {
                         "description": "Unit-cell length a in angstroms.",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 220.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 220,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell length a in angstroms."
                             },
                             {
                                 "context": "brief",
@@ -1577,16 +1577,16 @@
                         "type": "number"
                     },
                     "length_b": {
                         "description": "Unit-cell length b in angstroms.",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 304.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 304,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell length b in angstroms."
                             },
                             {
                                 "context": "brief",
@@ -1600,16 +1600,16 @@
                         "type": "number"
                     },
                     "length_c": {
                         "description": "Thickness of 2D crystal",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 320.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 320,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Thickness of 2D crystal"
                             },
                             {
                                 "context": "brief",
@@ -1735,15 +1735,15 @@
         "em_3d_crystal_entity": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "angle_alpha": {
                         "description": "Unit-cell angle alpha in degrees.",
                         "examples": [
-                            120.0
+                            120
                         ],
                         "rcsb_current_maximum_value": 109.52,
                         "rcsb_current_minimum_value": 62.8,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell angle alpha in degrees."
@@ -1758,15 +1758,15 @@
                         ],
                         "rcsb_units": "degrees",
                         "type": "number"
                     },
                     "angle_beta": {
                         "description": "Unit-cell angle beta in degrees.",
                         "examples": [
-                            120.0
+                            120
                         ],
                         "rcsb_current_maximum_value": 116.15,
                         "rcsb_current_minimum_value": 77.16,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell angle beta in degrees."
@@ -1781,17 +1781,17 @@
                         ],
                         "rcsb_units": "degrees",
                         "type": "number"
                     },
                     "angle_gamma": {
                         "description": "Unit-cell angle gamma in degrees.",
                         "examples": [
-                            120.0
+                            120
                         ],
-                        "rcsb_current_maximum_value": 120.0,
+                        "rcsb_current_maximum_value": 120,
                         "rcsb_current_minimum_value": 81.124,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell angle gamma in degrees."
                             },
                             {
@@ -1826,16 +1826,16 @@
                         "type": "string"
                     },
                     "length_a": {
                         "description": "Unit-cell length a in angstroms.",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 600.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 600,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell length a in angstroms."
                             },
                             {
                                 "context": "brief",
@@ -1849,16 +1849,16 @@
                         "type": "number"
                     },
                     "length_b": {
                         "description": "Unit-cell length b in angstroms.",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 600.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 600,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell length b in angstroms."
                             },
                             {
                                 "context": "brief",
@@ -1872,16 +1872,16 @@
                         "type": "number"
                     },
                     "length_c": {
                         "description": "Unit-cell length c in angstroms.",
                         "examples": [
                             62.4
                         ],
-                        "rcsb_current_maximum_value": 600.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 600,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Unit-cell length c in angstroms."
                             },
                             {
                                 "context": "brief",
@@ -1916,16 +1916,16 @@
                         "rcsb_search_context": [
                             "exact-match"
                         ],
                         "type": "string"
                     },
                     "space_group_num": {
                         "description": "Space group number.",
-                        "rcsb_current_maximum_value": 197.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 197,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Space group number."
                             },
                             {
                                 "context": "brief",
@@ -1999,15 +1999,15 @@
                         "rcsb_search_context": [
                             "full-text"
                         ],
                         "type": "string"
                     },
                     "overall_b_value": {
                         "description": "The overall B (temperature factor) value for the 3d-em volume.",
-                        "rcsb_current_maximum_value": 1000.0,
+                        "rcsb_current_maximum_value": 1000,
                         "rcsb_current_minimum_value": 0.836,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The overall B (temperature factor) value for the 3d-em volume."
                             },
                             {
@@ -2324,16 +2324,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "number"
                     },
                     "num_class_averages": {
                         "description": "The number of classes used in the final 3d reconstruction",
-                        "rcsb_current_maximum_value": 340465.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 340465,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of classes used in the final 3d reconstruction"
                             },
                             {
                                 "context": "brief",
@@ -2343,16 +2343,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "num_particles": {
                         "description": "The number of 2D projections or 3D subtomograms used in the 3d reconstruction",
-                        "rcsb_current_maximum_value": 8709340.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 8709340,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of 2D projections or 3D subtomograms used in the 3d reconstruction"
                             },
                             {
                                 "context": "brief",
@@ -2389,17 +2389,17 @@
                         ],
                         "type": "string"
                     },
                     "resolution": {
                         "description": "The final resolution (in angstroms) of the 3D reconstruction.",
                         "examples": [
                             8.9,
-                            10.0
+                            10
                         ],
-                        "rcsb_current_maximum_value": 70.0,
+                        "rcsb_current_maximum_value": 70,
                         "rcsb_current_minimum_value": 0.6,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The final resolution (in angstroms) of the 3D reconstruction."
                             },
                             {
@@ -2550,15 +2550,15 @@
         },
         "em_diffraction": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "camera_length": {
                         "description": "The camera length (in millimeters). The camera length is the\n product of the objective focal length and the combined magnification\n of the intermediate and projector lenses when the microscope is\n operated in the diffraction mode.",
-                        "rcsb_current_maximum_value": 4705.0,
+                        "rcsb_current_maximum_value": 4705,
                         "rcsb_current_minimum_value": 0.1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The camera length (in millimeters). The camera length is the\n product of the objective focal length and the combined magnification\n of the intermediate and projector lenses when the microscope is\n operated in the diffraction mode."
                             },
                             {
@@ -2630,15 +2630,15 @@
                         "type": "string"
                     },
                     "fourier_space_coverage": {
                         "description": "Completeness of the structure factor data within this resolution shell, in percent",
                         "examples": [
                             93.2
                         ],
-                        "rcsb_current_maximum_value": 100.0,
+                        "rcsb_current_maximum_value": 100,
                         "rcsb_current_minimum_value": 0.1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Completeness of the structure factor data within this resolution shell, in percent"
                             },
                             {
@@ -2685,15 +2685,15 @@
                         "type": "string"
                     },
                     "low_resolution": {
                         "description": "Low resolution limit for this shell (angstroms)",
                         "examples": [
                             5.5
                         ],
-                        "rcsb_current_maximum_value": 200.0,
+                        "rcsb_current_maximum_value": 200,
                         "rcsb_current_minimum_value": 0.1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Low resolution limit for this shell (angstroms)"
                             },
                             {
@@ -2708,15 +2708,15 @@
                         "type": "number"
                     },
                     "multiplicity": {
                         "description": "Multiplicity (average number of measurements) for the structure factors in this resolution shell",
                         "examples": [
                             2.5
                         ],
-                        "rcsb_current_maximum_value": 300.0,
+                        "rcsb_current_maximum_value": 300,
                         "rcsb_current_minimum_value": 0.1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Multiplicity (average number of measurements) for the structure factors in this resolution shell"
                             },
                             {
@@ -2727,16 +2727,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "number"
                     },
                     "num_structure_factors": {
                         "description": "Number of measured structure factors in this resolution shell",
-                        "rcsb_current_maximum_value": 6901357.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 6901357,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of measured structure factors in this resolution shell"
                             },
                             {
                                 "context": "brief",
@@ -2799,15 +2799,15 @@
                         "type": "string"
                     },
                     "fourier_space_coverage": {
                         "description": "Completeness of the structure factor data within the defined space group\n at the reported resolution (percent).",
                         "examples": [
                             89.3
                         ],
-                        "rcsb_current_maximum_value": 100.0,
+                        "rcsb_current_maximum_value": 100,
                         "rcsb_current_minimum_value": 0.1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Completeness of the structure factor data within the defined space group\n at the reported resolution (percent)."
                             },
                             {
@@ -2861,16 +2861,16 @@
                                 "text": "Pointer to _em_image_processing.id"
                             }
                         ],
                         "type": "string"
                     },
                     "num_intensities_measured": {
                         "description": "Total number of diffraction intensities measured (before averaging)",
-                        "rcsb_current_maximum_value": 9650574.0,
-                        "rcsb_current_minimum_value": 943.0,
+                        "rcsb_current_maximum_value": 9650574,
+                        "rcsb_current_minimum_value": 943,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Total number of diffraction intensities measured (before averaging)"
                             },
                             {
                                 "context": "brief",
@@ -2880,16 +2880,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "num_structure_factors": {
                         "description": "Number of structure factors obtained (merged amplitudes + phases)",
-                        "rcsb_current_maximum_value": 6901357.0,
-                        "rcsb_current_minimum_value": 325.0,
+                        "rcsb_current_maximum_value": 6901357,
+                        "rcsb_current_minimum_value": 325,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of structure factors obtained (merged amplitudes + phases)"
                             },
                             {
                                 "context": "brief",
@@ -2903,15 +2903,15 @@
                     },
                     "overall_phase_error": {
                         "description": "Overall phase error in degrees",
                         "examples": [
                             17.5
                         ],
                         "rcsb_current_maximum_value": 179.9,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Overall phase error in degrees"
                             },
                             {
                                 "context": "brief",
@@ -2961,15 +2961,15 @@
                         "type": "string"
                     },
                     "r_merge": {
                         "description": "Rmerge value (percent)",
                         "examples": [
                             19.8
                         ],
-                        "rcsb_current_maximum_value": 99.0,
+                        "rcsb_current_maximum_value": 99,
                         "rcsb_current_minimum_value": 0.093,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Rmerge value (percent)"
                             },
                             {
@@ -2983,15 +2983,15 @@
                         "type": "number"
                     },
                     "r_sym": {
                         "description": "Rsym value (percent)",
                         "examples": [
                             24.4
                         ],
-                        "rcsb_current_maximum_value": 100.0,
+                        "rcsb_current_maximum_value": 100,
                         "rcsb_current_minimum_value": 0.01,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Rsym value (percent)"
                             },
                             {
@@ -3160,16 +3160,16 @@
                                 "text": "oligomeric details"
                             }
                         ],
                         "type": "string"
                     },
                     "parent_id": {
                         "description": "The parent of this assembly.\n This data item is an internal category pointer to _em_entity_assembly.id.\n By convention, the full assembly (top of hierarchy) is assigned parent id 0 (zero).",
-                        "rcsb_current_maximum_value": 12.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 12,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The parent of this assembly.\n This data item is an internal category pointer to _em_entity_assembly.id.\n By convention, the full assembly (top of hierarchy) is assigned parent id 0 (zero)."
                             },
                             {
                                 "context": "brief",
@@ -3333,15 +3333,15 @@
                 "additionalProperties": false,
                 "properties": {
                     "angular_rotation_per_subunit": {
                         "description": "The angular rotation per helical subunit in degrees. Negative values indicate left-handed helices; positive values indicate right handed helices.",
                         "examples": [
                             -34.616
                         ],
-                        "rcsb_current_maximum_value": 180.0,
+                        "rcsb_current_maximum_value": 180,
                         "rcsb_current_minimum_value": -179.9,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The angular rotation per helical subunit in degrees. Negative values indicate left-handed helices; positive values indicate right handed helices."
                             },
                             {
@@ -3450,15 +3450,15 @@
                 "additionalProperties": false,
                 "properties": {
                     "average_exposure_time": {
                         "description": "The average exposure time for each image.",
                         "examples": [
                             2
                         ],
-                        "rcsb_current_maximum_value": 150.0,
+                        "rcsb_current_maximum_value": 150,
                         "rcsb_current_minimum_value": 0.006,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The average exposure time for each image."
                             },
                             {
@@ -3471,17 +3471,17 @@
                         ],
                         "rcsb_units": "seconds",
                         "type": "number"
                     },
                     "avg_electron_dose_per_image": {
                         "description": "The electron dose received by the specimen per image (electrons per square angstrom).",
                         "examples": [
-                            30.0
+                            30
                         ],
-                        "rcsb_current_maximum_value": 1200.0,
+                        "rcsb_current_maximum_value": 1200,
                         "rcsb_current_minimum_value": 0.00025,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The electron dose received by the specimen per image (electrons per square angstrom)."
                             },
                             {
@@ -3575,16 +3575,16 @@
                                 "text": "This data item the id of the microscopy settings used in the imaging."
                             }
                         ],
                         "type": "string"
                     },
                     "num_diffraction_images": {
                         "description": "The number of diffraction images collected.",
-                        "rcsb_current_maximum_value": 32000.0,
-                        "rcsb_current_minimum_value": 22.0,
+                        "rcsb_current_maximum_value": 32000,
+                        "rcsb_current_minimum_value": 22,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of diffraction images collected."
                             },
                             {
                                 "context": "brief",
@@ -3594,16 +3594,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "num_grids_imaged": {
                         "description": "Number of grids in the microscopy session",
-                        "rcsb_current_maximum_value": 6746.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 7770,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of grids in the microscopy session"
                             },
                             {
                                 "context": "brief",
@@ -3613,16 +3613,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "num_real_images": {
                         "description": "The number of micrograph images collected.",
-                        "rcsb_current_maximum_value": 9080999.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 9080999,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of micrograph images collected."
                             },
                             {
                                 "context": "brief",
@@ -3647,16 +3647,16 @@
         },
         "em_imaging": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "accelerating_voltage": {
                         "description": "A value of accelerating voltage (in kV) used for imaging.",
-                        "rcsb_current_maximum_value": 400.0,
-                        "rcsb_current_minimum_value": 45.0,
+                        "rcsb_current_maximum_value": 400,
+                        "rcsb_current_minimum_value": 45,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "A value of accelerating voltage (in kV) used for imaging."
                             },
                             {
                                 "context": "brief",
@@ -3708,15 +3708,15 @@
                                 "text": "astigmatism"
                             }
                         ],
                         "type": "string"
                     },
                     "c2_aperture_diameter": {
                         "description": "The open diameter of the c2 condenser lens,\n in microns.",
-                        "rcsb_current_maximum_value": 150.0,
+                        "rcsb_current_maximum_value": 150,
                         "rcsb_current_minimum_value": 2.6,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The open diameter of the c2 condenser lens,\n in microns."
                             },
                             {
@@ -3728,16 +3728,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "microns",
                         "type": "number"
                     },
                     "calibrated_defocus_max": {
                         "description": "The maximum calibrated defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus.",
-                        "rcsb_current_maximum_value": 30000.0,
-                        "rcsb_current_minimum_value": -7000.0,
+                        "rcsb_current_maximum_value": 30000,
+                        "rcsb_current_minimum_value": -7000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum calibrated defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus."
                             },
                             {
                                 "context": "brief",
@@ -3748,16 +3748,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "nanometers",
                         "type": "number"
                     },
                     "calibrated_defocus_min": {
                         "description": "The minimum calibrated defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus.",
-                        "rcsb_current_maximum_value": 15000.0,
-                        "rcsb_current_minimum_value": -2000.0,
+                        "rcsb_current_maximum_value": 15000,
+                        "rcsb_current_minimum_value": -2000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum calibrated defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus."
                             },
                             {
                                 "context": "brief",
@@ -3768,16 +3768,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "nanometers",
                         "type": "number"
                     },
                     "calibrated_magnification": {
                         "description": "The magnification value obtained for a known standard just\n prior to, during or just after the imaging experiment.",
-                        "rcsb_current_maximum_value": 587963.0,
-                        "rcsb_current_minimum_value": 2250.0,
+                        "rcsb_current_maximum_value": 587963,
+                        "rcsb_current_minimum_value": 2250,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The magnification value obtained for a known standard just\n prior to, during or just after the imaging experiment."
                             },
                             {
                                 "context": "brief",
@@ -3813,16 +3813,16 @@
                     },
                     "date": {
                         "description": "Date (YYYY-MM-DD) of imaging experiment or the date at which\n a series of experiments began.",
                         "examples": [
                             "2001-05-08"
                         ],
                         "format": "date",
-                        "rcsb_current_maximum_value": 1577059200000.0,
-                        "rcsb_current_minimum_value": 686275200000.0,
+                        "rcsb_current_maximum_value": 1577059200000,
+                        "rcsb_current_minimum_value": 686275200000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Date (YYYY-MM-DD) of imaging experiment or the date at which\n a series of experiments began."
                             },
                             {
                                 "context": "brief",
@@ -3845,16 +3845,16 @@
                                 "text": "Any additional imaging details."
                             }
                         ],
                         "type": "string"
                     },
                     "detector_distance": {
                         "description": "The camera length (in millimeters). The camera length is the\n product of the objective focal length and the combined magnification\n of the intermediate and projector lenses when the microscope is\n operated in the diffraction mode.",
-                        "rcsb_current_maximum_value": 800.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 800,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The camera length (in millimeters). The camera length is the\n product of the objective focal length and the combined magnification\n of the intermediate and projector lenses when the microscope is\n operated in the diffraction mode."
                             },
                             {
                                 "context": "brief",
@@ -4046,15 +4046,15 @@
                     },
                     "nominal_cs": {
                         "description": "The spherical aberration coefficient (Cs) in millimeters,\n of the objective lens.",
                         "examples": [
                             2
                         ],
                         "rcsb_current_maximum_value": 6.3,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The spherical aberration coefficient (Cs) in millimeters,\n of the objective lens."
                             },
                             {
                                 "context": "brief",
@@ -4065,16 +4065,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "millimetres",
                         "type": "number"
                     },
                     "nominal_defocus_max": {
                         "description": "The maximum defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus.",
-                        "rcsb_current_maximum_value": 45000.0,
-                        "rcsb_current_minimum_value": -20000.0,
+                        "rcsb_current_maximum_value": 45000,
+                        "rcsb_current_minimum_value": -20000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus."
                             },
                             {
                                 "context": "brief",
@@ -4085,16 +4085,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "nanometers",
                         "type": "number"
                     },
                     "nominal_defocus_min": {
                         "description": "The minimum defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus.",
-                        "rcsb_current_maximum_value": 15000.0,
-                        "rcsb_current_minimum_value": -8000.0,
+                        "rcsb_current_maximum_value": 15000,
+                        "rcsb_current_minimum_value": -8000,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum defocus value of the objective lens (in nanometers) used\n to obtain the recorded images. Negative values refer to overfocus."
                             },
                             {
                                 "context": "brief",
@@ -4105,16 +4105,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "nanometers",
                         "type": "number"
                     },
                     "nominal_magnification": {
                         "description": "The magnification indicated by the microscope readout.",
-                        "rcsb_current_maximum_value": 310000.0,
-                        "rcsb_current_minimum_value": 2250.0,
+                        "rcsb_current_maximum_value": 310000,
+                        "rcsb_current_minimum_value": 2250,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The magnification indicated by the microscope readout."
                             },
                             {
                                 "context": "brief",
@@ -4124,15 +4124,15 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "recording_temperature_maximum": {
                         "description": "The specimen temperature maximum (kelvin) for the duration\n of imaging.",
-                        "rcsb_current_maximum_value": 298.0,
+                        "rcsb_current_maximum_value": 298,
                         "rcsb_current_minimum_value": 4.2,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The specimen temperature maximum (kelvin) for the duration\n of imaging."
                             },
                             {
@@ -4144,15 +4144,15 @@
                             "default-match"
                         ],
                         "rcsb_units": "kelvins",
                         "type": "number"
                     },
                     "recording_temperature_minimum": {
                         "description": "The specimen temperature minimum (kelvin) for the duration\n of imaging.",
-                        "rcsb_current_maximum_value": 293.0,
+                        "rcsb_current_maximum_value": 293,
                         "rcsb_current_minimum_value": 4.2,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The specimen temperature minimum (kelvin) for the duration\n of imaging."
                             },
                             {
@@ -4164,15 +4164,15 @@
                             "default-match"
                         ],
                         "rcsb_units": "kelvins",
                         "type": "number"
                     },
                     "residual_tilt": {
                         "description": "Residual tilt of the electron beam (in miliradians)",
-                        "rcsb_current_maximum_value": 350.0,
+                        "rcsb_current_maximum_value": 350,
                         "rcsb_current_minimum_value": 0.001,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Residual tilt of the electron beam (in miliradians)"
                             },
                             {
@@ -4253,16 +4253,16 @@
                                 "text": "Foreign key to the EM_SPECIMEN category"
                             }
                         ],
                         "type": "string"
                     },
                     "temperature": {
                         "description": "The mean specimen stage temperature (in kelvin) during imaging\n in the microscope.",
-                        "rcsb_current_maximum_value": 300.0,
-                        "rcsb_current_minimum_value": 4.0,
+                        "rcsb_current_maximum_value": 300,
+                        "rcsb_current_minimum_value": 4,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The mean specimen stage temperature (in kelvin) during imaging\n in the microscope."
                             },
                             {
                                 "context": "brief",
@@ -4273,16 +4273,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "kelvins",
                         "type": "number"
                     },
                     "tilt_angle_max": {
                         "description": "The maximum angle at which the specimen was tilted to obtain\n recorded images.",
-                        "rcsb_current_maximum_value": 79.0,
-                        "rcsb_current_minimum_value": -9999.0,
+                        "rcsb_current_maximum_value": 79,
+                        "rcsb_current_minimum_value": -9999,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum angle at which the specimen was tilted to obtain\n recorded images."
                             },
                             {
                                 "context": "brief",
@@ -4293,16 +4293,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "degrees",
                         "type": "number"
                     },
                     "tilt_angle_min": {
                         "description": "The minimum angle at which the specimen was tilted to obtain\n recorded images.",
-                        "rcsb_current_maximum_value": 60.0,
-                        "rcsb_current_minimum_value": -9999.0,
+                        "rcsb_current_maximum_value": 60,
+                        "rcsb_current_minimum_value": -9999,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum angle at which the specimen was tilted to obtain\n recorded images."
                             },
                             {
                                 "context": "brief",
@@ -4360,16 +4360,16 @@
                                 "text": "The value of _em_particle_selection.image_processing_id points to\n the EM_IMAGE_PROCESSING category."
                             }
                         ],
                         "type": "string"
                     },
                     "num_particles_selected": {
                         "description": "The number of particles selected from the projection set of images.",
-                        "rcsb_current_maximum_value": 2145158999.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 2145158999,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of particles selected from the projection set of images."
                             },
                             {
                                 "context": "brief",
@@ -4612,15 +4612,15 @@
                 "additionalProperties": false,
                 "properties": {
                     "concentration": {
                         "description": "The concentration (in milligrams per milliliter, mg/ml)\n of the complex in the sample.",
                         "examples": [
                             1.35
                         ],
-                        "rcsb_current_maximum_value": 200.0,
+                        "rcsb_current_maximum_value": 200,
                         "rcsb_current_minimum_value": 7.5e-05,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The concentration (in milligrams per milliliter, mg/ml)\n of the complex in the sample."
                             },
                             {
@@ -4870,15 +4870,15 @@
         "em_vitrification": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "chamber_temperature": {
                         "description": "The temperature (in kelvin) of the sample just prior to vitrification.",
                         "rcsb_current_maximum_value": 375.15,
-                        "rcsb_current_minimum_value": 4.0,
+                        "rcsb_current_minimum_value": 4,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The temperature (in kelvin) of the sample just prior to vitrification."
                             },
                             {
                                 "context": "brief",
@@ -4931,16 +4931,16 @@
                                 "text": "Any additional details relating to vitrification."
                             }
                         ],
                         "type": "string"
                     },
                     "humidity": {
                         "description": "Relative humidity (%) of air surrounding the specimen just prior to\nvitrification.",
-                        "rcsb_current_maximum_value": 100.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 100,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Relative humidity (%) of air surrounding the specimen just prior to\nvitrification."
                             },
                             {
                                 "context": "brief",
@@ -5032,16 +5032,16 @@
                                 "text": "This data item is a pointer to _em_specimen.id"
                             }
                         ],
                         "type": "string"
                     },
                     "temp": {
                         "description": "The vitrification temperature (in kelvin), e.g.,\n  temperature of the plunge instrument cryogen bath.",
-                        "rcsb_current_maximum_value": 277.0,
-                        "rcsb_current_minimum_value": 76.0,
+                        "rcsb_current_maximum_value": 277,
+                        "rcsb_current_minimum_value": 76,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The vitrification temperature (in kelvin), e.g.,\n  temperature of the plunge instrument cryogen bath."
                             },
                             {
                                 "context": "brief",
@@ -5315,16 +5315,16 @@
                             "text": "Number of monomer insertions relative to the reference sequence."
                         }
                     ],
                     "type": "integer"
                 },
                 "rcsb_mutation_count": {
                     "description": "Number of engineered mutations engineered in the sample sequence.",
-                    "rcsb_current_maximum_value": 657.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 657,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Number of engineered mutations engineered in the sample sequence."
                         },
                         {
                             "context": "brief",
@@ -5374,16 +5374,16 @@
                             "text": "For polymer BIRD molecules the BIRD identifier for the entity."
                         }
                     ],
                     "type": "string"
                 },
                 "rcsb_sample_sequence_length": {
                     "description": "The monomer length of the sample sequence.",
-                    "rcsb_current_maximum_value": 19000.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 19000,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The monomer length of the sample sequence."
                         },
                         {
                             "context": "brief",
@@ -6652,16 +6652,16 @@
         },
         "exptl": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "crystals_number": {
                         "description": "The total number of crystals used in the  measurement of\n intensities.",
-                        "rcsb_current_maximum_value": 1029868.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 1029868,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The total number of crystals used in the  measurement of\n intensities."
                             },
                             {
                                 "context": "deposition",
@@ -6838,15 +6838,15 @@
                     },
                     "density_Matthews": {
                         "description": "The density of the crystal, expressed as the ratio of the\n volume of the asymmetric unit to the molecular mass of a\n monomer of the structure, in units of angstroms^3^ per dalton.\n\n Ref: Matthews, B. W. (1968). J. Mol. Biol. 33, 491-497.",
                         "examples": [
                             3.1
                         ],
                         "rcsb_current_maximum_value": 45.14,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The density of the crystal, expressed as the ratio of the\n volume of the asymmetric unit to the molecular mass of a\n monomer of the structure, in units of angstroms^3^ per dalton.\n\n Ref: Matthews, B. W. (1968). J. Mol. Biol. 33, 491-497."
                             },
                             {
                                 "context": "deposition",
@@ -6888,15 +6888,15 @@
                         ],
                         "rcsb_units": "megagrams_per_cubic_metre",
                         "type": "number"
                     },
                     "density_percent_sol": {
                         "description": "Density value P calculated from the crystal cell and contents,\n expressed as per cent solvent.\n\n P = 1 - (1.23 N MMass) / V\n\n N     = the number of molecules in the unit cell\n MMass = the molecular mass of each molecule (gm/mole)\n V     = the volume of the unit cell (A^3^)\n 1.23  = a conversion factor evaluated as:\n\n         (0.74 cm^3^/g) (10^24^ A^3^/cm^3^)\n         --------------------------------------\n              (6.02*10^23^) molecules/mole\n\n         where 0.74 is an assumed value for the partial specific\n         volume of the molecule",
                         "rcsb_current_maximum_value": 96.06,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Density value P calculated from the crystal cell and contents,\n expressed as per cent solvent.\n\n P = 1 - (1.23 N MMass) / V\n\n N     = the number of molecules in the unit cell\n MMass = the molecular mass of each molecule (gm/mole)\n V     = the volume of the unit cell (A^3^)\n 1.23  = a conversion factor evaluated as:\n\n         (0.74 cm^3^/g) (10^24^ A^3^/cm^3^)\n         --------------------------------------\n              (6.02*10^23^) molecules/mole\n\n         where 0.74 is an assumed value for the partial specific\n         volume of the molecule"
                             },
                             {
                                 "context": "deposition",
@@ -6937,15 +6937,15 @@
                             }
                         ],
                         "type": "string"
                     },
                     "pdbx_mosaicity": {
                         "description": "Isotropic approximation of the distribution of mis-orientation angles\nspecified in degrees of all the mosaic domain blocks in the crystal,\nrepresented as a standard deviation. Here, a mosaic block is a set of\ncontiguous unit cells assumed to be perfectly aligned. Lower mosaicity\nindicates better ordered crystals. See for example:\n\nNave, C. (1998). Acta Cryst. D54, 848-853.\n\nNote that many software packages estimate the mosaic rotation distribution\ndifferently and may combine several physical properties of the experiment\ninto a single mosaic term. This term will help fit the modeled spots\nto the observed spots without necessarily being directly related to the\nphysics of the crystal itself.",
                         "rcsb_current_maximum_value": 20.715,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Isotropic approximation of the distribution of mis-orientation angles\nspecified in degrees of all the mosaic domain blocks in the crystal,\nrepresented as a standard deviation. Here, a mosaic block is a set of\ncontiguous unit cells assumed to be perfectly aligned. Lower mosaicity\nindicates better ordered crystals. See for example:\n\nNave, C. (1998). Acta Cryst. D54, 848-853.\n\nNote that many software packages estimate the mosaic rotation distribution\ndifferently and may combine several physical properties of the experiment\ninto a single mosaic term. This term will help fit the modeled spots\nto the observed spots without necessarily being directly related to the\nphysics of the crystal itself."
                             },
                             {
                                 "context": "brief",
@@ -7061,16 +7061,16 @@
                     "pH": {
                         "description": "The pH at which the crystal was grown. If more than one pH was\n employed during the crystallization process, the final pH should\n be noted here and the protocol involving multiple pH values\n should be described in _exptl_crystal_grow.details.",
                         "examples": [
                             7.4,
                             7.6,
                             4.3
                         ],
-                        "rcsb_current_maximum_value": 12.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 12,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The pH at which the crystal was grown. If more than one pH was\n employed during the crystallization process, the final pH should\n be noted here and the protocol involving multiple pH values\n should be described in _exptl_crystal_grow.details."
                             },
                             {
                                 "context": "deposition",
@@ -7130,16 +7130,16 @@
                                 "text": "The range of pH values at which the crystal was grown.   Used when\n a point estimate of pH is not appropriate."
                             }
                         ],
                         "type": "string"
                     },
                     "temp": {
                         "description": "The temperature in kelvins at which the crystal was grown.\n If more than one temperature was employed during the\n crystallization process, the final temperature should be noted\n here and the protocol  involving multiple temperatures should be\n described in _exptl_crystal_grow.details.",
-                        "rcsb_current_maximum_value": 328.0,
-                        "rcsb_current_minimum_value": 100.0,
+                        "rcsb_current_maximum_value": 328,
+                        "rcsb_current_minimum_value": 100,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The temperature in kelvins at which the crystal was grown.\n If more than one temperature was employed during the\n crystallization process, the final temperature should be noted\n here and the protocol  involving multiple temperatures should be\n described in _exptl_crystal_grow.details."
                             },
                             {
                                 "context": "brief",
@@ -9563,16 +9563,16 @@
             "uniqueItems": true
         },
         "pdbx_entity_branch": {
             "additionalProperties": false,
             "properties": {
                 "rcsb_branched_component_count": {
                     "description": "Number of constituent chemical components in the branched entity.",
-                    "rcsb_current_maximum_value": 36.0,
-                    "rcsb_current_minimum_value": 2.0,
+                    "rcsb_current_maximum_value": 36,
+                    "rcsb_current_minimum_value": 2,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Number of constituent chemical components in the branched entity."
                         },
                         {
                             "context": "brief",
@@ -11358,16 +11358,16 @@
                                 "text": "Further details about the NMR spectrometer."
                             }
                         ],
                         "type": "string"
                     },
                     "field_strength": {
                         "description": "The field strength in MHz of the spectrometer",
-                        "rcsb_current_maximum_value": 3400.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 3400,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The field strength in MHz of the spectrometer"
                             },
                             {
                                 "context": "deposition",
@@ -11829,15 +11829,15 @@
         "pdbx_serial_crystallography_measurement": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "collection_time_total": {
                         "description": "The total number of hours required to measure this data set.",
                         "examples": [
-                            120.0
+                            120
                         ],
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The total number of hours required to measure this data set."
                             }
                         ],
@@ -13559,16 +13559,16 @@
                 "deposit_date": {
                     "description": "The entry deposition date.",
                     "examples": [
                         "2020-07-11",
                         "2013-10-01"
                     ],
                     "format": "date",
-                    "rcsb_current_maximum_value": 1684886400000.0,
-                    "rcsb_current_minimum_value": 82339200000.0,
+                    "rcsb_current_maximum_value": 1688947200000,
+                    "rcsb_current_minimum_value": 82339200000,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The entry deposition date."
                         },
                         {
                             "context": "brief",
@@ -13621,16 +13621,16 @@
                 "initial_release_date": {
                     "description": "The entry initial release date.",
                     "examples": [
                         "2020-01-10",
                         "2018-01-23"
                     ],
                     "format": "date",
-                    "rcsb_current_maximum_value": 1685491200000.0,
-                    "rcsb_current_minimum_value": 201312000000.0,
+                    "rcsb_current_maximum_value": 1689724800000,
+                    "rcsb_current_minimum_value": 201312000000,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The entry initial release date."
                         },
                         {
                             "context": "brief",
@@ -13671,16 +13671,16 @@
                 "revision_date": {
                     "description": "The latest entry revision date.",
                     "examples": [
                         "2020-02-11",
                         "2018-10-23"
                     ],
                     "format": "date",
-                    "rcsb_current_maximum_value": 1685491200000.0,
-                    "rcsb_current_minimum_value": 973641600000.0,
+                    "rcsb_current_maximum_value": 1689724800000,
+                    "rcsb_current_minimum_value": 973641600000,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The latest entry revision date."
                         },
                         {
                             "context": "brief",
@@ -13822,16 +13822,16 @@
                             "text": "Entity identifier for the container."
                         }
                     ],
                     "type": "string"
                 },
                 "atom_count": {
                     "description": "The assembly non-hydrogen atomic coordinate count.",
-                    "rcsb_current_maximum_value": 39959280.0,
-                    "rcsb_current_minimum_value": 7.0,
+                    "rcsb_current_maximum_value": 39959280,
+                    "rcsb_current_minimum_value": 7,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly non-hydrogen atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -13847,16 +13847,16 @@
                             "priority_order": 5
                         }
                     ],
                     "type": "integer"
                 },
                 "branched_atom_count": {
                     "description": "The assembly non-hydrogen branched entity atomic coordinate count.",
-                    "rcsb_current_maximum_value": 43920.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 43920,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly non-hydrogen branched entity atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -13866,16 +13866,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "branched_entity_count": {
                     "description": "The number of distinct branched entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 16.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 16,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct branched entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -13885,16 +13885,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "branched_entity_instance_count": {
                     "description": "The number of branched instances in the generated assembly data set.\n This is the total count of branched entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 780.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 780,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of branched instances in the generated assembly data set.\n This is the total count of branched entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -13917,16 +13917,16 @@
                             "text": "The PDB entry accession code."
                         }
                     ],
                     "type": "string"
                 },
                 "hydrogen_atom_count": {
                     "description": "The assembly hydrogen atomic coordinate count.",
-                    "rcsb_current_maximum_value": 5795340.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 5795340,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly hydrogen atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -13942,16 +13942,16 @@
                             "priority_order": 10
                         }
                     ],
                     "type": "integer"
                 },
                 "modeled_polymer_monomer_count": {
                     "description": "The number of modeled polymer monomers in the assembly coordinate data.\n This is the total count of monomers with reported coordinate data for all polymer\n entity instances in the generated assembly coordinate data.",
-                    "rcsb_current_maximum_value": 5086680.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 5086680,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of modeled polymer monomers in the assembly coordinate data.\n This is the total count of monomers with reported coordinate data for all polymer\n entity instances in the generated assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14017,16 +14017,16 @@
                     "rcsb_search_context": [
                         "exact-match"
                     ],
                     "type": "string"
                 },
                 "nonpolymer_atom_count": {
                     "description": "The assembly non-hydrogen non-polymer entity atomic coordinate count.",
-                    "rcsb_current_maximum_value": 206954.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 206954,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly non-hydrogen non-polymer entity atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -14036,16 +14036,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "nonpolymer_entity_count": {
                     "description": "The number of distinct non-polymer entities in the generated assembly exclusive of solvent.",
-                    "rcsb_current_maximum_value": 30.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 30,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct non-polymer entities in the generated assembly exclusive of solvent."
                         },
                         {
                             "context": "brief",
@@ -14055,16 +14055,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "nonpolymer_entity_instance_count": {
                     "description": "The number of non-polymer instances in the generated assembly data set exclusive of solvent.\n This is the total count of non-polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 4593.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 4593,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of non-polymer instances in the generated assembly data set exclusive of solvent.\n This is the total count of non-polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14116,16 +14116,16 @@
                 },
                 "num_protein_interface_entities": {
                     "description": "Number of protein-protein interface entities",
                     "type": "integer"
                 },
                 "polymer_atom_count": {
                     "description": "The assembly non-hydrogen polymer entity atomic coordinate count.",
-                    "rcsb_current_maximum_value": 39959280.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 39959280,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly non-hydrogen polymer entity atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -14230,16 +14230,16 @@
                     "rcsb_search_context": [
                         "exact-match"
                     ],
                     "type": "string"
                 },
                 "polymer_entity_count": {
                     "description": "The number of distinct polymer entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct polymer entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14249,16 +14249,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_DNA": {
                     "description": "The number of distinct DNA polymer entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct DNA polymer entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14268,16 +14268,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_RNA": {
                     "description": "The number of distinct RNA polymer entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 36.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 36,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct RNA polymer entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14287,16 +14287,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_nucleic_acid": {
                     "description": "The number of distinct nucleic acid polymer entities (DNA or RNA) in the generated assembly.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct nucleic acid polymer entities (DNA or RNA) in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14306,16 +14306,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_nucleic_acid_hybrid": {
                     "description": "The number of distinct hybrid nucleic acid polymer entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 2.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 2,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct hybrid nucleic acid polymer entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14325,16 +14325,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_protein": {
                     "description": "The number of distinct protein polymer entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 145.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 150,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct protein polymer entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14344,16 +14344,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count": {
                     "description": "The number of polymer instances in the generated assembly data set.\n This is the total count of polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 8280.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 8280,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of polymer instances in the generated assembly data set.\n This is the total count of polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14369,16 +14369,16 @@
                             "priority_order": 35
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count_DNA": {
                     "description": "The number of DNA polymer instances in the generated assembly data set.\n This is the total count of DNA polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of DNA polymer instances in the generated assembly data set.\n This is the total count of DNA polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14394,16 +14394,16 @@
                             "priority_order": 50
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count_RNA": {
                     "description": "The number of RNA polymer instances in the generated assembly data set.\n This is the total count of RNA polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 180.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 180,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of RNA polymer instances in the generated assembly data set.\n This is the total count of RNA polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14419,16 +14419,16 @@
                             "priority_order": 55
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count_nucleic_acid": {
                     "description": "The number of nucleic acid polymer instances in the generated assembly data set.\n This is the total count of nucleic acid polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of nucleic acid polymer instances in the generated assembly data set.\n This is the total count of nucleic acid polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14438,16 +14438,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count_nucleic_acid_hybrid": {
                     "description": "The number of hybrid nucleic acide polymer instances in the generated assembly data set.\n This is the total count of hybrid nucleic acid polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 8.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 8,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of hybrid nucleic acide polymer instances in the generated assembly data set.\n This is the total count of hybrid nucleic acid polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14463,16 +14463,16 @@
                             "priority_order": 60
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_instance_count_protein": {
                     "description": "The number of protein polymer instances in the generated assembly data set.\n This is the total count of protein polymer entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 8280.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 8280,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of protein polymer instances in the generated assembly data set.\n This is the total count of protein polymer entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14488,16 +14488,16 @@
                             "priority_order": 45
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_monomer_count": {
                     "description": "The number of polymer monomers in sample entity instances comprising the assembly data set.\n This is the total count of monomers for all polymer entity instances\n in the generated assembly coordinate data.",
-                    "rcsb_current_maximum_value": 5340600.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 5340600,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of polymer monomers in sample entity instances comprising the assembly data set.\n This is the total count of monomers for all polymer entity instances\n in the generated assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14558,16 +14558,16 @@
                     "rcsb_search_context": [
                         "exact-match"
                     ],
                     "type": "string"
                 },
                 "solvent_atom_count": {
                     "description": "The assembly non-hydrogen solvent atomic coordinate count.",
-                    "rcsb_current_maximum_value": 78540.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 78540,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The assembly non-hydrogen solvent atomic coordinate count."
                         },
                         {
                             "context": "brief",
@@ -14583,16 +14583,16 @@
                             "priority_order": 15
                         }
                     ],
                     "type": "integer"
                 },
                 "solvent_entity_count": {
                     "description": "The number of distinct solvent entities in the generated assembly.",
-                    "rcsb_current_maximum_value": 1.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 1,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct solvent entities in the generated assembly."
                         },
                         {
                             "context": "brief",
@@ -14602,16 +14602,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "solvent_entity_instance_count": {
                     "description": "The number of solvent instances in the generated assembly data set.\n This is the total count of solvent entity instances generated in the assembly coordinate data.",
-                    "rcsb_current_maximum_value": 901.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 901,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of solvent instances in the generated assembly data set.\n This is the total count of solvent entity instances generated in the assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14629,16 +14629,16 @@
                 },
                 "total_number_interface_residues": {
                     "description": "Total number of interfacing residues in the assembly, calculated as the sum of interfacing residues over all interfaces",
                     "type": "integer"
                 },
                 "unmodeled_polymer_monomer_count": {
                     "description": "The number of unmodeled polymer monomers in the assembly coordinate data. This is\n the total count of monomers with unreported coordinate data for all polymer\n entity instances in the generated assembly coordinate data.",
-                    "rcsb_current_maximum_value": 515880.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 515880,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of unmodeled polymer monomers in the assembly coordinate data. This is\n the total count of monomers with unreported coordinate data for all polymer\n entity instances in the generated assembly coordinate data."
                         },
                         {
                             "context": "brief",
@@ -14847,86 +14847,86 @@
                             "attributes": [
                                 {
                                     "examples": [
                                         0.8,
                                         14
                                     ],
                                     "path": "rcsb_binding_affinity.value",
-                                    "rcsb_current_maximum_value": 800000000.0,
+                                    "rcsb_current_maximum_value": 800000000,
                                     "rcsb_current_minimum_value": 0.0010000000474974513
                                 }
                             ],
                             "context_value": "IC50"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         0.18,
-                                        23000.0
+                                        23000
                                     ],
                                     "path": "rcsb_binding_affinity.value",
-                                    "rcsb_current_maximum_value": 3000000.0,
+                                    "rcsb_current_maximum_value": 3000000,
                                     "rcsb_current_minimum_value": 0.004000000189989805
                                 }
                             ],
                             "context_value": "EC50"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         6.5,
-                                        220000.0
+                                        220000
                                     ],
                                     "path": "rcsb_binding_affinity.value",
-                                    "rcsb_current_maximum_value": 1400000000.0,
+                                    "rcsb_current_maximum_value": 1400000000,
                                     "rcsb_current_minimum_value": 6.000000212225132e-07
                                 }
                             ],
                             "context_value": "Kd"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         7.5,
-                                        1700.0
+                                        1700
                                     ],
                                     "path": "rcsb_binding_affinity.value",
-                                    "rcsb_current_maximum_value": 100000000376832.0,
+                                    "rcsb_current_maximum_value": 100000000376832,
                                     "rcsb_current_minimum_value": 0.00107999995816499
                                 }
                             ],
                             "context_value": "Ka"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         4,
-                                        390000.0
+                                        390000
                                     ],
                                     "path": "rcsb_binding_affinity.value",
-                                    "rcsb_current_maximum_value": 100000000376832.0,
+                                    "rcsb_current_maximum_value": 100000000376832,
                                     "rcsb_current_minimum_value": 1.1000000085914508e-05
                                 }
                             ],
                             "context_value": "Ki"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         17.2,
                                         21.4
                                     ],
                                     "path": "rcsb_binding_affinity.value",
                                     "rcsb_current_maximum_value": 30.137800216674805,
-                                    "rcsb_current_minimum_value": -1088.0
+                                    "rcsb_current_minimum_value": -1088
                                 }
                             ],
                             "context_value": "&Delta;G"
                         },
                         {
                             "attributes": [
                                 {
@@ -15039,16 +15039,16 @@
                             "priority_order": 10
                         }
                     ],
                     "type": "string"
                 },
                 "pdbx_number_of_molecules": {
                     "description": "The number of molecules of the branched entity in the entry.",
-                    "rcsb_current_maximum_value": 76.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 76,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of molecules of the branched entity in the entry."
                         },
                         {
                             "context": "brief",
@@ -15777,16 +15777,16 @@
         },
         "rcsb_branched_entity_feature_summary": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "count": {
                         "description": "The feature count.",
-                        "rcsb_current_maximum_value": 0.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The feature count."
                             },
                             {
                                 "context": "brief",
@@ -15800,16 +15800,16 @@
                     },
                     "coverage": {
                         "description": "The fractional feature coverage relative to the full branched entity.",
                         "examples": [
                             0.012,
                             0.00132
                         ],
-                        "rcsb_current_maximum_value": 0.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The fractional feature coverage relative to the full branched entity."
                             },
                             {
                                 "context": "brief",
@@ -16804,16 +16804,16 @@
         },
         "rcsb_branched_instance_feature_summary": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "count": {
                         "description": "The feature count.",
-                        "rcsb_current_maximum_value": 952.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 952,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The feature count."
                             },
                             {
                                 "context": "brief",
@@ -16827,16 +16827,16 @@
                     },
                     "coverage": {
                         "description": "The fractional feature coverage relative to the full branched entity.",
                         "examples": [
                             0.5,
                             0.95
                         ],
-                        "rcsb_current_maximum_value": 0.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The fractional feature coverage relative to the full branched entity."
                             },
                             {
                                 "context": "brief",
@@ -16846,16 +16846,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "number"
                     },
                     "maximum_length": {
                         "description": "The maximum feature length.",
-                        "rcsb_current_maximum_value": 0.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum feature length."
                             },
                             {
                                 "context": "brief",
@@ -16879,16 +16879,16 @@
                                 "text": "The maximum feature value."
                             }
                         ],
                         "type": "number"
                     },
                     "minimum_length": {
                         "description": "The minimum feature length.",
-                        "rcsb_current_maximum_value": 0.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum feature length."
                             },
                             {
                                 "context": "brief",
@@ -17343,16 +17343,16 @@
         },
         "rcsb_cluster_membership": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "cluster_id": {
                         "description": "Identifier for a cluster at the specified level of sequence identity within the cluster data set.",
-                        "rcsb_current_maximum_value": 1066028.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 1067236,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Identifier for a cluster at the specified level of sequence identity within the cluster data set."
                             },
                             {
                                 "context": "brief",
@@ -17362,16 +17362,16 @@
                         "rcsb_search_context": [
                             "default-match"
                         ],
                         "type": "integer"
                     },
                     "identity": {
                         "description": "Sequence identity expressed as an integer percent value.",
-                        "rcsb_current_maximum_value": 100.0,
-                        "rcsb_current_minimum_value": 30.0,
+                        "rcsb_current_maximum_value": 100,
+                        "rcsb_current_minimum_value": 30,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Sequence identity expressed as an integer percent value."
                             },
                             {
                                 "context": "brief",
@@ -17655,16 +17655,16 @@
                     },
                     "taxonomy_lineage": {
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "depth": {
                                     "description": "Members of the NCBI Taxonomy lineage as parent taxonomy lineage depth (1-N)",
-                                    "rcsb_current_maximum_value": 35.0,
-                                    "rcsb_current_minimum_value": 1.0,
+                                    "rcsb_current_maximum_value": 35,
+                                    "rcsb_current_minimum_value": 1,
                                     "rcsb_description": [
                                         {
                                             "context": "dictionary",
                                             "text": "Members of the NCBI Taxonomy lineage as parent taxonomy lineage depth (1-N)"
                                         },
                                         {
                                             "context": "brief",
@@ -18020,16 +18020,16 @@
                     },
                     "taxonomy_lineage": {
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "depth": {
                                     "description": "Members of the NCBI Taxonomy lineage as parent taxonomy lineage depth (1-N)",
-                                    "rcsb_current_maximum_value": 36.0,
-                                    "rcsb_current_minimum_value": 1.0,
+                                    "rcsb_current_maximum_value": 36,
+                                    "rcsb_current_minimum_value": 1,
                                     "rcsb_description": [
                                         {
                                             "context": "dictionary",
                                             "text": "Members of the NCBI Taxonomy lineage as parent taxonomy lineage depth (1-N)"
                                         },
                                         {
                                             "context": "brief",
@@ -18396,16 +18396,16 @@
             "uniqueItems": true
         },
         "rcsb_entry_info": {
             "additionalProperties": false,
             "properties": {
                 "assembly_count": {
                     "description": "The number of assemblies defined for this entry including the deposited assembly.",
-                    "rcsb_current_maximum_value": 44.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 44,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of assemblies defined for this entry including the deposited assembly."
                         },
                         {
                             "context": "brief",
@@ -18421,16 +18421,16 @@
                             "priority_order": 20
                         }
                     ],
                     "type": "integer"
                 },
                 "branched_entity_count": {
                     "description": "The number of distinct branched entities in the structure entry.",
-                    "rcsb_current_maximum_value": 16.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 16,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct branched entities in the structure entry."
                         },
                         {
                             "context": "brief",
@@ -18470,16 +18470,16 @@
                         }
                     ],
                     "rcsb_units": "kilodaltons",
                     "type": "number"
                 },
                 "cis_peptide_count": {
                     "description": "The number of cis-peptide linkages per deposited structure model.",
-                    "rcsb_current_maximum_value": 1320.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 1320,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of cis-peptide linkages per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18489,16 +18489,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "deposited_atom_count": {
                     "description": "The number of heavy atom coordinates records per deposited structure model.",
-                    "rcsb_current_maximum_value": 3968189.0,
-                    "rcsb_current_minimum_value": 28.0,
+                    "rcsb_current_maximum_value": 3968189,
+                    "rcsb_current_minimum_value": 28,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of heavy atom coordinates records per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18514,16 +18514,16 @@
                             "priority_order": 70
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_hydrogen_atom_count": {
                     "description": "The number of hydrogen atom coordinates records per deposited structure model.",
-                    "rcsb_current_maximum_value": 680778.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 680778,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of hydrogen atom coordinates records per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18539,16 +18539,16 @@
                             "priority_order": 75
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_model_count": {
                     "description": "The number of model structures deposited.",
-                    "rcsb_current_maximum_value": 640.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 640,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of model structures deposited."
                         },
                         {
                             "context": "brief",
@@ -18564,16 +18564,16 @@
                             "priority_order": 85
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_modeled_polymer_monomer_count": {
                     "description": "The number of modeled polymer monomers in the deposited coordinate data.\n This is the total count of monomers with reported coordinate data for all polymer\n entity instances in the deposited coordinate data.",
-                    "rcsb_current_maximum_value": 503221.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 503221,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of modeled polymer monomers in the deposited coordinate data.\n This is the total count of monomers with reported coordinate data for all polymer\n entity instances in the deposited coordinate data."
                         },
                         {
                             "context": "brief",
@@ -18583,16 +18583,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "deposited_nonpolymer_entity_instance_count": {
                     "description": "The number of non-polymer instances in the deposited data set.\n This is the total count of non-polymer entity instances reported\n per deposited structure model.",
-                    "rcsb_current_maximum_value": 5351.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 5351,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of non-polymer instances in the deposited data set.\n This is the total count of non-polymer entity instances reported\n per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18608,16 +18608,16 @@
                             "priority_order": 60
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_polymer_entity_instance_count": {
                     "description": "The number of polymer instances in the deposited data set.\n This is the total count of polymer entity instances reported\n per deposited structure model.",
-                    "rcsb_current_maximum_value": 1792.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 1792,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of polymer instances in the deposited data set.\n This is the total count of polymer entity instances reported\n per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18633,16 +18633,16 @@
                             "priority_order": 55
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_polymer_monomer_count": {
                     "description": "The number of polymer monomers in sample entity instances in the deposited data set.\n This is the total count of monomers for all polymer entity instances reported\n per deposited structure model.",
-                    "rcsb_current_maximum_value": 566853.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 566853,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of polymer monomers in sample entity instances in the deposited data set.\n This is the total count of monomers for all polymer entity instances reported\n per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18658,16 +18658,16 @@
                             "priority_order": 65
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_solvent_atom_count": {
                     "description": "The number of heavy solvent atom coordinates records per deposited structure model.",
-                    "rcsb_current_maximum_value": 15347.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 15347,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of heavy solvent atom coordinates records per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18683,16 +18683,16 @@
                             "priority_order": 80
                         }
                     ],
                     "type": "integer"
                 },
                 "deposited_unmodeled_polymer_monomer_count": {
                     "description": "The number of unmodeled polymer monomers in the deposited coordinate data. This is\n the total count of monomers with unreported coordinate data for all polymer\n entity instances per deposited structure model.",
-                    "rcsb_current_maximum_value": 81166.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 81166,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of unmodeled polymer monomers in the deposited coordinate data. This is\n the total count of monomers with unreported coordinate data for all polymer\n entity instances per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18702,16 +18702,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "diffrn_radiation_wavelength_maximum": {
                     "description": "The maximum radiation wavelength in angstroms.",
-                    "rcsb_current_maximum_value": 979257.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 979257,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The maximum radiation wavelength in angstroms."
                         },
                         {
                             "context": "brief",
@@ -18728,16 +18728,16 @@
                         }
                     ],
                     "rcsb_units": "angstroms",
                     "type": "number"
                 },
                 "diffrn_radiation_wavelength_minimum": {
                     "description": "The minimum radiation wavelength in angstroms.",
-                    "rcsb_current_maximum_value": 81798.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 81798,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The minimum radiation wavelength in angstroms."
                         },
                         {
                             "context": "brief",
@@ -18786,15 +18786,15 @@
                                     "value": "From the high resolution shell"
                                 }
                             ],
                             "type": "string"
                         },
                         "value": {
                             "description": "The high resolution limit of data collection.",
-                            "rcsb_current_maximum_value": 15.0,
+                            "rcsb_current_maximum_value": 15,
                             "rcsb_current_minimum_value": 0.48,
                             "rcsb_description": [
                                 {
                                     "context": "dictionary",
                                     "text": "The high resolution limit of data collection."
                                 },
                                 {
@@ -18815,16 +18815,16 @@
                             "type": "number"
                         }
                     },
                     "type": "object"
                 },
                 "disulfide_bond_count": {
                     "description": "The number of disulfide bonds per deposited structure model.",
-                    "rcsb_current_maximum_value": 1356.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 1356,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of disulfide bonds per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18840,16 +18840,16 @@
                             "priority_order": 90
                         }
                     ],
                     "type": "integer"
                 },
                 "entity_count": {
                     "description": "The number of distinct polymer, non-polymer, branched molecular, and solvent entities per deposited structure model.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct polymer, non-polymer, branched molecular, and solvent entities per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -18927,16 +18927,16 @@
                             "priority_order": 10
                         }
                     ],
                     "type": "string"
                 },
                 "experimental_method_count": {
                     "description": "The number of experimental methods contributing data to the structure determination.",
-                    "rcsb_current_maximum_value": 3.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 3,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of experimental methods contributing data to the structure determination."
                         },
                         {
                             "context": "brief",
@@ -18952,16 +18952,16 @@
                             "priority_order": 15
                         }
                     ],
                     "type": "integer"
                 },
                 "inter_mol_covalent_bond_count": {
                     "description": "The number of intermolecular covalent bonds.",
-                    "rcsb_current_maximum_value": 9426.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 9426,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of intermolecular covalent bonds."
                         },
                         {
                             "context": "brief",
@@ -18971,16 +18971,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "inter_mol_metalic_bond_count": {
                     "description": "The number of intermolecular metalic bonds.",
-                    "rcsb_current_maximum_value": 7829.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 7829,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of intermolecular metalic bonds."
                         },
                         {
                             "context": "brief",
@@ -19119,16 +19119,16 @@
                         "type": "string"
                     },
                     "type": "array",
                     "uniqueItems": false
                 },
                 "nonpolymer_entity_count": {
                     "description": "The number of distinct non-polymer entities in the structure entry exclusive of solvent.",
-                    "rcsb_current_maximum_value": 30.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 30,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct non-polymer entities in the structure entry exclusive of solvent."
                         },
                         {
                             "context": "brief",
@@ -19149,15 +19149,15 @@
                 "nonpolymer_molecular_weight_maximum": {
                     "description": "The maximum molecular mass (KDa) of a non-polymer entity in the deposited structure entry.",
                     "examples": [
                         0.43,
                         0.91
                     ],
                     "rcsb_current_maximum_value": 7.7,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The maximum molecular mass (KDa) of a non-polymer entity in the deposited structure entry."
                         },
                         {
                             "context": "brief",
@@ -19173,15 +19173,15 @@
                 "nonpolymer_molecular_weight_minimum": {
                     "description": "The minimum molecular mass (KDa) of a non-polymer entity in the deposited structure entry.",
                     "examples": [
                         0.07,
                         0.12
                     ],
                     "rcsb_current_maximum_value": 7.7,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The minimum molecular mass (KDa) of a non-polymer entity in the deposited structure entry."
                         },
                         {
                             "context": "brief",
@@ -19293,16 +19293,16 @@
                             "priority_order": 10
                         }
                     ],
                     "type": "string"
                 },
                 "polymer_entity_count": {
                     "description": "The number of distinct polymer entities in the structure entry.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct polymer entities in the structure entry."
                         },
                         {
                             "context": "brief",
@@ -19312,16 +19312,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_DNA": {
                     "description": "The number of distinct DNA polymer entities.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct DNA polymer entities."
                         },
                         {
                             "context": "brief",
@@ -19337,16 +19337,16 @@
                             "priority_order": 45
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_RNA": {
                     "description": "The number of distinct RNA polymer entities.",
-                    "rcsb_current_maximum_value": 36.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 36,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct RNA polymer entities."
                         },
                         {
                             "context": "brief",
@@ -19362,16 +19362,16 @@
                             "priority_order": 40
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_nucleic_acid": {
                     "description": "The number of distinct nucleic acid polymer entities (DNA or RNA).",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct nucleic acid polymer entities (DNA or RNA)."
                         },
                         {
                             "context": "brief",
@@ -19381,16 +19381,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_nucleic_acid_hybrid": {
                     "description": "The number of distinct hybrid nucleic acid polymer entities.",
-                    "rcsb_current_maximum_value": 3.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 3,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct hybrid nucleic acid polymer entities."
                         },
                         {
                             "context": "brief",
@@ -19406,16 +19406,16 @@
                             "priority_order": 50
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_count_protein": {
                     "description": "The number of distinct protein polymer entities.",
-                    "rcsb_current_maximum_value": 145.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 150,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct protein polymer entities."
                         },
                         {
                             "context": "brief",
@@ -19431,16 +19431,16 @@
                             "priority_order": 35
                         }
                     ],
                     "type": "integer"
                 },
                 "polymer_entity_taxonomy_count": {
                     "description": "The number of distinct taxonomies represented among the polymer entities in the entry.",
-                    "rcsb_current_maximum_value": 455.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 455,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct taxonomies represented among the polymer entities in the entry."
                         },
                         {
                             "context": "brief",
@@ -19498,16 +19498,16 @@
                         "default-match"
                     ],
                     "rcsb_units": "kilodaltons",
                     "type": "number"
                 },
                 "polymer_monomer_count_maximum": {
                     "description": "The maximum monomer count of a polymer entity per deposited structure model.",
-                    "rcsb_current_maximum_value": 19000.0,
-                    "rcsb_current_minimum_value": 2.0,
+                    "rcsb_current_maximum_value": 19000,
+                    "rcsb_current_minimum_value": 2,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The maximum monomer count of a polymer entity per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -19517,16 +19517,16 @@
                     "rcsb_search_context": [
                         "default-match"
                     ],
                     "type": "integer"
                 },
                 "polymer_monomer_count_minimum": {
                     "description": "The minimum monomer count of a polymer entity per deposited structure model.",
-                    "rcsb_current_maximum_value": 5037.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 5037,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The minimum monomer count of a polymer entity per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -19541,15 +19541,15 @@
                 "resolution_combined": {
                     "items": {
                         "description": "Combined estimates of experimental resolution contributing to the refined structural model.\n Resolution reported in \"refine.ls_d_res_high\" is used for X-RAY DIFFRACTION, FIBER DIFFRACTION, \n POWDER DIFFRACTION, ELECTRON CRYSTALLOGRAPHY, and NEUTRON DIFFRACTION as identified in\n \"refine.pdbx_refine_id\". \n Resolution reported in \"em_3d_reconstruction.resolution\" is used for ELECTRON MICROSCOPY. \n The best value corresponding to \"em_3d_reconstruction.resolution_method\" == \"FSC 0.143 CUT-OFF\" \n is used, if available. If not, the best \"em_3d_reconstruction.resolution\" value is used. \n For structures that are not obtained from diffraction-based methods, the resolution values in \n \"refine.ls_d_res_high\" are ignored.\n Multiple values are reported only if multiple methods are used in the structure determination.",
                         "examples": [
                             1.11,
                             2.05
                         ],
-                        "rcsb_current_maximum_value": 70.0,
+                        "rcsb_current_maximum_value": 70,
                         "rcsb_current_minimum_value": 0.48,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Combined estimates of experimental resolution contributing to the refined structural model.\n Resolution reported in \"refine.ls_d_res_high\" is used for X-RAY DIFFRACTION, FIBER DIFFRACTION, \n POWDER DIFFRACTION, ELECTRON CRYSTALLOGRAPHY, and NEUTRON DIFFRACTION as identified in\n \"refine.pdbx_refine_id\". \n Resolution reported in \"em_3d_reconstruction.resolution\" is used for ELECTRON MICROSCOPY. \n The best value corresponding to \"em_3d_reconstruction.resolution_method\" == \"FSC 0.143 CUT-OFF\" \n is used, if available. If not, the best \"em_3d_reconstruction.resolution\" value is used. \n For structures that are not obtained from diffraction-based methods, the resolution values in \n \"refine.ls_d_res_high\" are ignored.\n Multiple values are reported only if multiple methods are used in the structure determination."
                             },
                             {
@@ -19664,16 +19664,16 @@
                         "type": "string"
                     },
                     "type": "array",
                     "uniqueItems": false
                 },
                 "solvent_entity_count": {
                     "description": "The number of distinct solvent entities per deposited structure model.",
-                    "rcsb_current_maximum_value": 1.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 1,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct solvent entities per deposited structure model."
                         },
                         {
                             "context": "brief",
@@ -19724,16 +19724,16 @@
                             "priority_order": 90
                         }
                     ],
                     "type": "string"
                 },
                 "structure_determination_methodology_priority": {
                     "description": "Indicates the priority of the value in _rcsb_entry_info.structure_determination_methodology.\n The lower the number the higher the priority.\n Priority values for \"experimental\" structures is currently set to 10 and\n the values for \"computational\" structures is set to 100.",
-                    "rcsb_current_maximum_value": 100.0,
-                    "rcsb_current_minimum_value": 10.0,
+                    "rcsb_current_maximum_value": 100,
+                    "rcsb_current_minimum_value": 10,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "Indicates the priority of the value in _rcsb_entry_info.structure_determination_methodology.\n The lower the number the higher the priority.\n Priority values for \"experimental\" structures is currently set to 10 and\n the values for \"computational\" structures is set to 100."
                         },
                         {
                             "context": "brief",
@@ -19766,14 +19766,15 @@
                     },
                     "type": {
                         "description": "Internal identifier for external resource.",
                         "enum": [
                             "OLDERADO",
                             "BMRB",
                             "NDB",
+                            "NAKB",
                             "SB GRID",
                             "PROTEIN DIFFRACTION",
                             "EM DATA RESOURCE"
                         ],
                         "rcsb_description": [
                             {
                                 "context": "brief",
@@ -19798,14 +19799,19 @@
                             },
                             {
                                 "detail": "Three-dimensional structural information about nucleic acids",
                                 "name": "NDB",
                                 "value": "NDB"
                             },
                             {
+                                "detail": "Three-dimensional structural information about nucleic acids",
+                                "name": "NAKB",
+                                "value": "NAKB"
+                            },
+                            {
                                 "detail": "Integrated resource for reproducibility in macromolecular crystallography",
                                 "name": "Protein Diffraction",
                                 "value": "PROTEIN DIFFRACTION"
                             },
                             {
                                 "detail": "Supports publication of X-ray diffraction, MicroED, LLSM datasets, as well as structural models",
                                 "name": "SBGrid",
@@ -19987,15 +19993,15 @@
                                 "text": "Component identifier for the target instance."
                             }
                         ],
                         "type": "string"
                     },
                     "distance": {
                         "description": "Distance value for this ligand interaction.",
-                        "rcsb_current_maximum_value": 41.565,
+                        "rcsb_current_maximum_value": 5,
                         "rcsb_current_minimum_value": 0.015,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Distance value for this ligand interaction."
                             },
                             {
@@ -20382,16 +20388,16 @@
             "description": "Information about integral membrane proteins whose crystallographic, or sometimes NMR or cryo-EM, structures have been determined to a resolution sufficient to identify TM helices of helix-bundle membrane proteins (typically 4 - 4.5 A). Mpstruc provides manually curated information about integral membrane proteins. These manual annotations are extended using sequence clusters and according to the following procedure:Single chain transmembrane proteins: Any PDB chain sharing 90% sequence identity to this transmembrane protein is assigned as a transmembrane protein as well, and shares the same transmembrane annotation.Multi-chain transmembrane proteins:If the reference mpstruc entry contains multiple protein entities, it is necessary to identify which of the entities are presumed to be transmembrane chains. This is done in conjunction with Uniprot annotations. Transmembrane protein entities are identified by checking if their corresponding Uniprot sequence has annotations labeled <i>transmembrane</i> or <i>intramembrane region</i>. For transmembrane entities, all members of the sequence cluster (90% sequence identity) are programmatically infered to be members of the same class of transmembrane proteins by applying the above procedure for single entity mpstruc entries. Annotations are denoned with 'Homology' provenance code.",
             "items": {
                 "additionalProperties": false,
                 "description": "Members of the membrane protein classification lineage.",
                 "properties": {
                     "depth": {
                         "description": "Hierarchy depth.",
-                        "rcsb_current_maximum_value": 2.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 2,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "brief",
                                 "text": "Depth (Membrane Lineage)"
                             }
                         ],
                         "rcsb_search_context": [
@@ -20501,16 +20507,16 @@
                     "rcsb_search_context": [
                         "full-text"
                     ],
                     "type": "string"
                 },
                 "pdbx_number_of_molecules": {
                     "description": "The number of molecules of the nonpolymer entity in the entry.",
-                    "rcsb_current_maximum_value": 5345.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 5345,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of molecules of the nonpolymer entity in the entry."
                         },
                         {
                             "context": "brief",
@@ -21201,16 +21207,16 @@
                                 "text": "Non-polymer(ligand) chemical component identifier for the entity."
                             }
                         ],
                         "type": "string"
                     },
                     "count": {
                         "description": "The feature count.",
-                        "rcsb_current_maximum_value": 1.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 1,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The feature count."
                             },
                             {
                                 "context": "brief",
@@ -22222,86 +22228,86 @@
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 102.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 102,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "HAS_COVALENT_LINKAGE"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 166.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 166,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "HAS_METAL_COORDINATION_LINKAGE"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 4500.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 4500,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "MOGUL_ANGLE_OUTLIER"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 3884.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 3884,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "MOGUL_BOND_OUTLIER"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 77.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 77,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "RSCC_OUTLIER"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         5
                                     ],
                                     "path": "rcsb_nonpolymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 0.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 0,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "RSRZ_OUTLIER"
                         }
                     ]
                 }
             ],
@@ -22314,15 +22320,15 @@
                 "properties": {
                     "RSCC": {
                         "description": "The real space correlation coefficient (RSCC) for the non-polymer entity instance.",
                         "examples": [
                             0.9,
                             0.55
                         ],
-                        "rcsb_current_maximum_value": 1.0,
+                        "rcsb_current_maximum_value": 1,
                         "rcsb_current_minimum_value": -0.931,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The real space correlation coefficient (RSCC) for the non-polymer entity instance."
                             },
                             {
@@ -22394,16 +22400,16 @@
                                 "text": "The reported fraction of atomic coordinate records for the non-polymer entity instance."
                             }
                         ],
                         "type": "number"
                     },
                     "intermolecular_clashes": {
                         "description": "The number of intermolecular MolProbity clashes cacluated for reported atomic coordinate records.",
-                        "rcsb_current_maximum_value": 95.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 95,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The number of intermolecular MolProbity clashes cacluated for reported atomic coordinate records."
                             },
                             {
                                 "context": "brief",
@@ -22513,16 +22519,16 @@
                                 "value": "RCSB"
                             }
                         ],
                         "type": "string"
                     },
                     "mogul_angle_outliers": {
                         "description": "Number of bond angle outliers obtained from a CCDC Mogul survey of bond angles  in the CSD small\n   molecule crystal structure database. Outliers are defined as bond angles that have a Z-score\n   less than -2 or greater than 2.",
-                        "rcsb_current_maximum_value": 72.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 72,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of bond angle outliers obtained from a CCDC Mogul survey of bond angles  in the CSD small\n   molecule crystal structure database. Outliers are defined as bond angles that have a Z-score\n   less than -2 or greater than 2."
                             },
                             {
                                 "context": "brief",
@@ -22537,15 +22543,15 @@
                     "mogul_angles_RMSZ": {
                         "description": "The root-mean-square value of the Z-scores of bond angles for the residue in degrees\nobtained from a CCDC Mogul survey of bond angles in the CSD small molecule crystal structure database.",
                         "examples": [
                             7.22,
                             1.16
                         ],
                         "rcsb_current_maximum_value": 47.36,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The root-mean-square value of the Z-scores of bond angles for the residue in degrees\nobtained from a CCDC Mogul survey of bond angles in the CSD small molecule crystal structure database."
                             },
                             {
                                 "context": "brief",
@@ -22556,16 +22562,16 @@
                             "default-match"
                         ],
                         "rcsb_units": "degrees",
                         "type": "number"
                     },
                     "mogul_bond_outliers": {
                         "description": "Number of bond distance outliers obtained from a CCDC Mogul survey of bond lengths in the CSD small\n   molecule crystal structure database.  Outliers are defined as bond distances that have a Z-score\n   less than -2 or greater than 2.",
-                        "rcsb_current_maximum_value": 75.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 75,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of bond distance outliers obtained from a CCDC Mogul survey of bond lengths in the CSD small\n   molecule crystal structure database.  Outliers are defined as bond distances that have a Z-score\n   less than -2 or greater than 2."
                             },
                             {
                                 "context": "brief",
@@ -22580,15 +22586,15 @@
                     "mogul_bonds_RMSZ": {
                         "description": "The root-mean-square value of the Z-scores of bond lengths for the residue in Angstroms\nobtained from a CCDC Mogul survey of bond lengths in the CSD small molecule crystal structure database.",
                         "examples": [
                             0.69,
                             1.32
                         ],
                         "rcsb_current_maximum_value": 1108.53,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The root-mean-square value of the Z-scores of bond lengths for the residue in Angstroms\nobtained from a CCDC Mogul survey of bond lengths in the CSD small molecule crystal structure database."
                             },
                             {
                                 "context": "brief",
@@ -22603,16 +22609,16 @@
                     },
                     "ranking_model_fit": {
                         "description": "The ranking of the model fit score component.",
                         "examples": [
                             0.9,
                             0.55
                         ],
-                        "rcsb_current_maximum_value": 1.0,
-                        "rcsb_current_minimum_value": -0.0,
+                        "rcsb_current_maximum_value": 1,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The ranking of the model fit score component."
                             },
                             {
                                 "context": "brief",
@@ -22626,16 +22632,16 @@
                     },
                     "ranking_model_geometry": {
                         "description": "The ranking of the model geometry score component.",
                         "examples": [
                             0.9,
                             0.55
                         ],
-                        "rcsb_current_maximum_value": 1.0,
-                        "rcsb_current_minimum_value": -0.0,
+                        "rcsb_current_maximum_value": 1,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The ranking of the model geometry score component."
                             },
                             {
                                 "context": "brief",
@@ -22673,16 +22679,16 @@
                                 "text": "The value of the model geometry score component."
                             }
                         ],
                         "type": "number"
                     },
                     "stereo_outliers": {
                         "description": "Number of stereochemical/chirality errors.",
-                        "rcsb_current_maximum_value": 34.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 34,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Number of stereochemical/chirality errors."
                             },
                             {
                                 "context": "brief",
@@ -23027,15 +23033,15 @@
                         }
                     ],
                     "type": "string"
                 },
                 "formula_weight": {
                     "description": "Formula mass (KDa) of the entity.",
                     "examples": [
-                        40.0,
+                        40,
                         105
                     ],
                     "rcsb_current_maximum_value": 6061.921,
                     "rcsb_current_minimum_value": 0.158,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
@@ -23129,16 +23135,16 @@
                             "text": "Details about any polymer entity mutation(s)."
                         }
                     ],
                     "type": "string"
                 },
                 "pdbx_number_of_molecules": {
                     "description": "The number of molecules of the entity in the entry.",
-                    "rcsb_current_maximum_value": 1356.0,
-                    "rcsb_current_minimum_value": 1.0,
+                    "rcsb_current_maximum_value": 1356,
+                    "rcsb_current_minimum_value": 1,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of molecules of the entity in the entry."
                         },
                         {
                             "context": "brief",
@@ -23152,16 +23158,16 @@
                 },
                 "rcsb_ec_lineage": {
                     "items": {
                         "additionalProperties": false,
                         "properties": {
                             "depth": {
                                 "description": "Members of the enzyme classification lineage as parent classification hierarchy depth (1-N).",
-                                "rcsb_current_maximum_value": 4.0,
-                                "rcsb_current_minimum_value": 1.0,
+                                "rcsb_current_maximum_value": 4,
+                                "rcsb_current_minimum_value": 1,
                                 "rcsb_description": [
                                     {
                                         "context": "dictionary",
                                         "text": "Members of the enzyme classification lineage as parent classification hierarchy depth (1-N)."
                                     },
                                     {
                                         "context": "brief",
@@ -23238,16 +23244,16 @@
                 },
                 "rcsb_enzyme_class_combined": {
                     "items": {
                         "additionalProperties": false,
                         "properties": {
                             "depth": {
                                 "description": "The enzyme classification hierarchy depth (1-N).",
-                                "rcsb_current_maximum_value": 4.0,
-                                "rcsb_current_minimum_value": 1.0,
+                                "rcsb_current_maximum_value": 4,
+                                "rcsb_current_minimum_value": 1,
                                 "rcsb_description": [
                                     {
                                         "context": "dictionary",
                                         "text": "The enzyme classification hierarchy depth (1-N)."
                                     },
                                     {
                                         "context": "brief",
@@ -23436,16 +23442,16 @@
                             "type": "string"
                         }
                     },
                     "type": "object"
                 },
                 "rcsb_source_part_count": {
                     "description": "The number of biological sources for the polymer entity. Multiple source contributions\n may come from the same organism (taxonomy).",
-                    "rcsb_current_maximum_value": 21.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 21,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of biological sources for the polymer entity. Multiple source contributions\n may come from the same organism (taxonomy)."
                         },
                         {
                             "context": "brief",
@@ -23461,16 +23467,16 @@
                             "priority_order": 70
                         }
                     ],
                     "type": "integer"
                 },
                 "rcsb_source_taxonomy_count": {
                     "description": "The number of distinct source taxonomies for the polymer entity. Commonly used to identify chimeric polymers.",
-                    "rcsb_current_maximum_value": 5.0,
-                    "rcsb_current_minimum_value": 0.0,
+                    "rcsb_current_maximum_value": 5,
+                    "rcsb_current_minimum_value": 0,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The number of distinct source taxonomies for the polymer entity. Commonly used to identify chimeric polymers."
                         },
                         {
                             "context": "brief",
@@ -23746,16 +23752,16 @@
                     },
                     "annotation_lineage": {
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "depth": {
                                     "description": "Members of the annotation lineage as parent lineage depth (1-N)",
-                                    "rcsb_current_maximum_value": 5.0,
-                                    "rcsb_current_minimum_value": 0.0,
+                                    "rcsb_current_maximum_value": 5,
+                                    "rcsb_current_minimum_value": 0,
                                     "rcsb_description": [
                                         {
                                             "context": "dictionary",
                                             "text": "Members of the annotation lineage as parent lineage depth (1-N)"
                                         },
                                         {
                                             "context": "brief",
@@ -24935,16 +24941,16 @@
                                 "priority_order": 120
                             }
                         ],
                         "type": "number"
                     },
                     "maximum_length": {
                         "description": "The maximum feature length.",
-                        "rcsb_current_maximum_value": 685.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 685,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum feature length."
                             },
                             {
                                 "context": "brief",
@@ -24968,16 +24974,16 @@
                                 "text": "The maximum feature value."
                             }
                         ],
                         "type": "number"
                     },
                     "minimum_length": {
                         "description": "The minimum feature length.",
-                        "rcsb_current_maximum_value": 685.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 685,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum feature length."
                             },
                             {
                                 "context": "brief",
@@ -25133,48 +25139,48 @@
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_entity_feature_summary.count",
-                                    "rcsb_current_maximum_value": 22.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 22,
+                                    "rcsb_current_minimum_value": 0
                                 },
                                 {
                                     "examples": [
                                         0.02,
                                         0.12
                                     ],
                                     "path": "rcsb_polymer_entity_feature_summary.coverage",
                                     "rcsb_current_maximum_value": 0.77839,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "artifact"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         2,
                                         5
                                     ],
                                     "path": "rcsb_polymer_entity_feature_summary.count",
-                                    "rcsb_current_maximum_value": 4128.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 4128,
+                                    "rcsb_current_minimum_value": 0
                                 },
                                 {
                                     "examples": [
                                         0.01,
                                         0.05
                                     ],
                                     "path": "rcsb_polymer_entity_feature_summary.coverage",
-                                    "rcsb_current_maximum_value": 1.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 1,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "modified_monomer"
                         }
                     ]
                 }
             ],
@@ -25263,16 +25269,16 @@
                                 "priority_order": 110
                             }
                         ],
                         "type": "string"
                     },
                     "similarity_cutoff": {
                         "description": "Degree of similarity expressed as a floating-point number",
-                        "rcsb_current_maximum_value": 100.0,
-                        "rcsb_current_minimum_value": 30.0,
+                        "rcsb_current_maximum_value": 100,
+                        "rcsb_current_minimum_value": 30,
                         "rcsb_description": [
                             {
                                 "context": "brief",
                                 "text": "Similarity Cutoff (Polymer Entity Group Membership)"
                             }
                         ],
                         "rcsb_search_context": [
@@ -25538,16 +25544,16 @@
                     },
                     "annotation_lineage": {
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "depth": {
                                     "description": "Members of the annotation lineage as parent lineage depth (1-N)",
-                                    "rcsb_current_maximum_value": 5.0,
-                                    "rcsb_current_minimum_value": 1.0,
+                                    "rcsb_current_maximum_value": 5,
+                                    "rcsb_current_minimum_value": 1,
                                     "rcsb_description": [
                                         {
                                             "context": "dictionary",
                                             "text": "Members of the annotation lineage as parent lineage depth (1-N)"
                                         },
                                         {
                                             "context": "brief",
@@ -26595,16 +26601,16 @@
                                 "priority_order": 20
                             }
                         ],
                         "type": "number"
                     },
                     "maximum_length": {
                         "description": "The maximum feature length.",
-                        "rcsb_current_maximum_value": 18394.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 18394,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The maximum feature length."
                             },
                             {
                                 "context": "brief",
@@ -26628,16 +26634,16 @@
                                 "text": "The maximum feature value."
                             }
                         ],
                         "type": "number"
                     },
                     "minimum_length": {
                         "description": "The minimum feature length.",
-                        "rcsb_current_maximum_value": 18394.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 18394,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The minimum feature length."
                             },
                             {
                                 "context": "brief",
@@ -27015,90 +27021,90 @@
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 301.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 301,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "CIS-PEPTIDE"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 374.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 374,
+                                    "rcsb_current_minimum_value": 0
                                 },
                                 {
                                     "examples": [
                                         0.15,
                                         0.45
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.coverage",
                                     "rcsb_current_maximum_value": 8.06316,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "HELIX_P"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 289.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 289,
+                                    "rcsb_current_minimum_value": 0
                                 },
                                 {
                                     "examples": [
                                         0.15,
                                         0.45
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.coverage",
                                     "rcsb_current_maximum_value": 19.54641,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "SHEET"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 2824.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 2824,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "RSCC_OUTLIER"
                         },
                         {
                             "attributes": [
                                 {
                                     "examples": [
                                         1,
                                         10
                                     ],
                                     "path": "rcsb_polymer_instance_feature_summary.count",
-                                    "rcsb_current_maximum_value": 3388.0,
-                                    "rcsb_current_minimum_value": 0.0
+                                    "rcsb_current_maximum_value": 3388,
+                                    "rcsb_current_minimum_value": 0
                                 }
                             ],
                             "context_value": "RSRZ_OUTLIER"
                         }
                     ]
                 }
             ],
@@ -27872,16 +27878,16 @@
                             "priority_order": 10
                         }
                     ],
                     "type": "string"
                 },
                 "year": {
                     "description": "The year of the citation; relevant for journal articles, books\n and book chapters.",
-                    "rcsb_current_maximum_value": 2023.0,
-                    "rcsb_current_minimum_value": 1969.0,
+                    "rcsb_current_maximum_value": 2023,
+                    "rcsb_current_minimum_value": 1969,
                     "rcsb_description": [
                         {
                             "context": "dictionary",
                             "text": "The year of the citation; relevant for journal articles, books\n and book chapters."
                         },
                         {
                             "context": "deposition",
@@ -27945,16 +27951,16 @@
             "additionalProperties": false,
             "properties": {
                 "pubmed_id": {
                     "description": "UID assigned to each PubMed record.",
                     "examples": [
                         15937111
                     ],
-                    "rcsb_current_maximum_value": 37218877.0,
-                    "rcsb_current_minimum_value": 5.0,
+                    "rcsb_current_maximum_value": 37438348,
+                    "rcsb_current_minimum_value": 5,
                     "rcsb_description": [
                         {
                             "context": "brief",
                             "text": "PubMed ID"
                         }
                     ],
                     "rcsb_search_context": [
@@ -27987,16 +27993,16 @@
         "rcsb_pubmed_mesh_descriptors_lineage": {
             "description": "Members of the MeSH classification lineage.",
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "depth": {
                         "description": "Hierarchy depth.",
-                        "rcsb_current_maximum_value": 13.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 13,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "brief",
                                 "text": "Depth (Pubmed Mesh Descriptors Lineage)"
                             }
                         ],
                         "rcsb_search_context": [
@@ -28314,15 +28320,15 @@
                         "description": "Clusters describe grouping of 'identical' subunits.",
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "avg_rmsd": {
                                     "description": "Average RMSD between members of a given cluster.",
                                     "rcsb_current_maximum_value": 80.22285641881933,
-                                    "rcsb_current_minimum_value": 0.0,
+                                    "rcsb_current_minimum_value": 0,
                                     "rcsb_description": [
                                         {
                                             "context": "brief",
                                             "text": "Average RMSD"
                                         }
                                     ],
                                     "rcsb_search_context": [
@@ -28537,16 +28543,16 @@
         },
         "rcsb_struct_symmetry_lineage": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "depth": {
                         "description": "Hierarchy depth.",
-                        "rcsb_current_maximum_value": 4.0,
-                        "rcsb_current_minimum_value": 1.0,
+                        "rcsb_current_maximum_value": 4,
+                        "rcsb_current_minimum_value": 1,
                         "rcsb_description": [
                             {
                                 "context": "brief",
                                 "text": "Depth (Struct Symmetry Lineage)"
                             }
                         ],
                         "rcsb_search_context": [
@@ -28952,15 +28958,15 @@
                                 "text": "Component identifier for the non-polymer entity instance."
                             }
                         ],
                         "type": "string"
                     },
                     "distance": {
                         "description": "Distance value for this target interaction.",
-                        "rcsb_current_maximum_value": 41.565,
+                        "rcsb_current_maximum_value": 5,
                         "rcsb_current_minimum_value": 0.015,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Distance value for this target interaction."
                             },
                             {
@@ -29235,26 +29241,27 @@
                                 "text": "An identifier for the annotation."
                             },
                             {
                                 "context": "brief",
                                 "text": "Annotation identifier"
                             }
                         ],
-                        "rcsb_full_text_priority": 10,
                         "rcsb_search_context": [
                             "exact-match"
                         ],
                         "type": "string"
                     },
                     "annotation_lineage": {
                         "items": {
                             "additionalProperties": false,
                             "properties": {
                                 "depth": {
                                     "description": "Members of the annotation lineage as parent lineage depth (1-N)",
+                                    "rcsb_current_maximum_value": 2,
+                                    "rcsb_current_minimum_value": 1,
                                     "rcsb_description": [
                                         {
                                             "context": "brief",
                                             "text": "UniProt Annotation Lineage Depth"
                                         }
                                     ],
                                     "rcsb_search_context": [
@@ -29332,61 +29339,128 @@
                         "type": "string"
                     },
                     "name": {
                         "description": "A name for the annotation.",
                         "rcsb_description": [
                             {
                                 "context": "brief",
-                                "text": "UniProt Annotation Name"
+                                "text": "Annotation Name"
                             }
                         ],
                         "rcsb_full_text_priority": 10,
                         "rcsb_search_context": [
                             "exact-match",
                             "full-text"
                         ],
                         "type": "string"
                     },
                     "provenance_source": {
                         "description": "Code identifying the individual, organization or program that\n assigned the annotation.",
                         "rcsb_description": [
                             {
                                 "context": "brief",
-                                "text": "UniProt Annotation Source"
+                                "text": "Annotation Source"
                             }
                         ],
                         "type": "string"
                     },
                     "type": {
                         "description": "A type or category of the annotation.",
                         "enum": [
                             "disease",
-                            "phenotype"
+                            "phenotype",
+                            "GO",
+                            "InterPro"
                         ],
                         "rcsb_description": [
                             {
+                                "context": "dictionary",
+                                "text": "A type or category of the annotation."
+                            },
+                            {
                                 "context": "brief",
-                                "text": "UniProt Annotation Type"
+                                "text": "Annotation Type"
+                            }
+                        ],
+                        "rcsb_enum_annotated": [
+                            {
+                                "detail": "Disease data from OMIM and Disease Ontology represented in Pharos",
+                                "name": "Disease",
+                                "value": "disease"
+                            },
+                            {
+                                "detail": "Phenotypic data including mouse phenotypes, mouse/human orthologs and GWAS results represented in Pharos",
+                                "name": "Phenotype",
+                                "value": "phenotype"
+                            },
+                            {
+                                "detail": "InterPro Protein Family",
+                                "name": "InterPro Protein Family",
+                                "value": "InterPro"
+                            },
+                            {
+                                "detail": "Gene Ontology",
+                                "name": "Gene Ontology",
+                                "value": "GO"
                             }
                         ],
-                        "rcsb_full_text_priority": 10,
                         "rcsb_search_context": [
                             "exact-match"
                         ],
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
             "minItems": 1,
             "rcsb_nested_indexing": true,
             "rcsb_nested_indexing_context": [
                 {
                     "category_name": "annotation_type",
-                    "category_path": "rcsb_uniprot_annotation.type"
+                    "category_path": "rcsb_uniprot_annotation.type",
+                    "context_attributes": [
+                        {
+                            "attributes": [
+                                {
+                                    "examples": [
+                                        "GO:0005575",
+                                        "GO:0005622"
+                                    ],
+                                    "path": "rcsb_uniprot_annotation.annotation_lineage.id"
+                                },
+                                {
+                                    "examples": [
+                                        "cellular_component",
+                                        "intracellular"
+                                    ],
+                                    "path": "rcsb_uniprot_annotation.annotation_lineage.name"
+                                }
+                            ],
+                            "context_value": "GO"
+                        },
+                        {
+                            "attributes": [
+                                {
+                                    "examples": [
+                                        "IPR022352",
+                                        "IPR004825"
+                                    ],
+                                    "path": "rcsb_uniprot_annotation.annotation_lineage.id"
+                                },
+                                {
+                                    "examples": [
+                                        "Insulin family",
+                                        "Insulin"
+                                    ],
+                                    "path": "rcsb_uniprot_annotation.annotation_lineage.name"
+                                }
+                            ],
+                            "context_value": "InterPro"
+                        }
+                    ]
                 }
             ],
             "type": "array",
             "uniqueItems": true
         },
         "rcsb_uniprot_container_identifiers": {
             "additionalProperties": false,
@@ -29565,14 +29639,32 @@
                                 "end_seq_id": {
                                     "description": "An identifier for the monomer at which this segment of the feature ends.",
                                     "type": "integer"
                                 },
                                 "value": {
                                     "description": "The value for the feature over this monomer segment.",
                                     "type": "number"
+                                },
+                                "values": {
+                                    "items": {
+                                        "description": "The value(s) for the feature over this monomer segment.",
+                                        "examples": [
+                                            5,
+                                            0.25
+                                        ],
+                                        "rcsb_description": [
+                                            {
+                                                "context": "dictionary",
+                                                "text": "The value(s) for the feature over this monomer segment."
+                                            }
+                                        ],
+                                        "type": "number"
+                                    },
+                                    "type": "array",
+                                    "uniqueItems": false
                                 }
                             },
                             "required": [
                                 "beg_seq_id"
                             ],
                             "type": "object"
                         },
@@ -30245,15 +30337,15 @@
                             }
                         ],
                         "type": "number"
                     },
                     "ls_R_factor_all": {
                         "description": "Residual factor R for all reflections that satisfy the resolution\n limits established by _refine.ls_d_res_high and\n _refine.ls_d_res_low.\n\n     sum|F~obs~ - F~calc~|\n R = ---------------------\n          sum|F~obs~|\n\n F~obs~  = the observed structure-factor amplitudes\n F~calc~ = the calculated structure-factor amplitudes\n\n sum is taken over the specified reflections",
                         "rcsb_current_maximum_value": 0.999,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Residual factor R for all reflections that satisfy the resolution\n limits established by _refine.ls_d_res_high and\n _refine.ls_d_res_low.\n\n     sum|F~obs~ - F~calc~|\n R = ---------------------\n          sum|F~obs~|\n\n F~obs~  = the observed structure-factor amplitudes\n F~calc~ = the calculated structure-factor amplitudes\n\n sum is taken over the specified reflections"
                             },
                             {
                                 "context": "brief",
@@ -31535,16 +31627,16 @@
                                 "text": "Residual factor Rmerge for reflections that satisfy the\n resolution limits established by _reflns.d_resolution_high\n and _reflns.d_resolution_low and the observation limit\n established by _reflns.observed_criterion.\n\n             sum~i~(sum~j~|F~j~ - <F>|)\n Rmerge(F) = --------------------------\n                  sum~i~(sum~j~<F>)\n\n F~j~ = the amplitude of the jth observation of reflection i\n <F>  = the mean of the amplitudes of all observations of\n        reflection i\n\n sum~i~ is taken over all reflections\n sum~j~ is taken over all observations of each reflection"
                             }
                         ],
                         "type": "number"
                     },
                     "d_resolution_high": {
                         "description": "The smallest value in angstroms for the interplanar spacings\n for the reflection data. This is called the highest resolution.",
-                        "rcsb_current_maximum_value": 24.0,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_maximum_value": 24,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The smallest value in angstroms for the interplanar spacings\n for the reflection data. This is called the highest resolution."
                             },
                             {
                                 "context": "deposition",
@@ -31812,15 +31904,15 @@
                             }
                         ],
                         "type": "number"
                     },
                     "pdbx_Rmerge_I_obs": {
                         "description": "The R value for merging intensities satisfying the observed\n criteria in this data set.",
                         "rcsb_current_maximum_value": 9.9,
-                        "rcsb_current_minimum_value": 0.0,
+                        "rcsb_current_minimum_value": 0,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The R value for merging intensities satisfying the observed\n criteria in this data set."
                             },
                             {
                                 "context": "deposition",
@@ -31945,15 +32037,15 @@
                                 "text": "An ordinal identifier for this set of reflection statistics."
                             }
                         ],
                         "type": "integer"
                     },
                     "pdbx_redundancy": {
                         "description": "Overall redundancy for this data set.",
-                        "rcsb_current_maximum_value": 26558.0,
+                        "rcsb_current_maximum_value": 26558,
                         "rcsb_current_minimum_value": 0.035,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "Overall redundancy for this data set."
                             },
                             {
@@ -31984,15 +32076,15 @@
                                 "text": "Number of reflections rejected in scaling operations."
                             }
                         ],
                         "type": "integer"
                     },
                     "percent_possible_obs": {
                         "description": "The percentage of geometrically possible reflections represented\n by reflections that satisfy the resolution limits established\n by _reflns.d_resolution_high and _reflns.d_resolution_low and\n the observation limit established by\n _reflns.observed_criterion.",
-                        "rcsb_current_maximum_value": 100.0,
+                        "rcsb_current_maximum_value": 100,
                         "rcsb_current_minimum_value": 0.045,
                         "rcsb_description": [
                             {
                                 "context": "dictionary",
                                 "text": "The percentage of geometrically possible reflections represented\n by reflections that satisfy the resolution limits established\n by _reflns.d_resolution_high and _reflns.d_resolution_low and\n the observation limit established by\n _reflns.observed_criterion."
                             },
                             {
```

### Comparing `rcsbsearchapi-1.0.0/rcsbsearchapi/schema.py` & `rcsbsearchapi-1.2.0/rcsbsearchapi/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,43 @@
 """Parse the full RCSB search schema
 
 Provides access to all valid attributes for search queries.
 """
 
 import json
 import logging
-import os
 import pkgutil
 import re
-from typing import Any, Iterator, List, Union
-
 import requests
-
+from typing import Any, Iterator, List, Union
 from .search import Attr
+from .const import STRUCTURE_ATTRIBUTE_SCHEMA_URL, CHEMICAL_ATTRIBUTE_SCHEMA_URL, SEARCH_SCHEMA_URL, STRUCTURE_ATTRIBUTE_SEARCH_SERVICE, CHEMICAL_ATTRIBUTE_SEARCH_SERVICE
 
-METADATA_SCHEMA_URL = "http://search.rcsb.org/rcsbsearch/v2/metadata/schema"
-SEARCH_SCHEMA_URL = "http://search.rcsb.org/json-schema-rcsb_search_query.json"
-
-ENV_RCSBSEARCH_DOWNLOAD_SCHEMA = "RCSBSEARCH_DOWNLOAD_SCHEMA"
-
-
-def _get_json_schema(download=None):
-    """Get the JSON schema
-
-    The RCSBSEARCH_DOWNLOAD_SCHEMA environmental variable controls whether
-    to download the schema from the web each time vs using the version shipped
-    with rcsbsearchapi
-    """
-    if download is True or (
-        download is None
-        and (
-            os.environ.get(ENV_RCSBSEARCH_DOWNLOAD_SCHEMA, "no").lower()
-            in ("1", "yes", "y")
-        )
-    ):
-        return _download_json_schema()
-    return _load_json_schema()
 
-
-def _download_json_schema():
-    "Get the current JSON schema from the web"
-    url = METADATA_SCHEMA_URL
+def _download_schema(url: str):
+    "Get the current schema from the web"
 
     logging.info("Downloading %s", url)
     response = requests.get(url, timeout=None)
     response.raise_for_status()
     return response.json()
 
 
 def _load_json_schema():
-    logging.info("Loading schema from file")
+    logging.info("Loading structure schema from file")
     latest = pkgutil.get_data(__package__, "resources/metadata_schema.json")
     return json.loads(latest)
 
 
+def _load_chem_schema():
+    logging.info("Loading chemical schema from file")
+    latest = pkgutil.get_data(__package__, "resources/chemical_schema.json")
+    return json.loads(latest)
+
+
 class SchemaGroup:
     """A non-leaf node in the RCSB PDB schema. Leaves are Attr values."""
 
     def search(self, pattern: Union[str, re.Pattern], flags=0) -> Iterator[Attr]:
         """Find all attributes in the schema matching a regular expression.
 
         Returns:
@@ -81,64 +61,66 @@
                 if isinstance(v, Attr):
                     yield v
                 elif isinstance(v, SchemaGroup):
                     yield from iter(v)
                 else:
                     # Shouldn't happen
                     raise TypeError(f"Unrecognized member {k!r}: {v!r}")
-
         return leaves(self)
 
     def __str__(self):
         return "\n".join((str(c) for c in self.__dict__.values()))
 
 
-def _make_group(fullname: str, node) -> Union[SchemaGroup, Attr]:
+def _make_group(fullname: str, nodeL: List) -> Union[SchemaGroup, Attr]:
     """Represent this node of the schema as a python object
 
     Params:
     - name: full dot-separated attribute name
 
     Returns:
     An Attr (Leaf nodes) or SchemaGroup (object nodes)
     """
-    if "anyOf" in node:
-        children = {_make_group(fullname, n) for n in node["anyOf"]}
-        # Currently only deal with anyOf in leaf nodes
-        assert len(children) == 1, f"type of {fullname} couldn't be determined"
-        return next(iter(children))
-    if "oneOf" in node:
-        children = {_make_group(fullname, n) for n in node["oneOf"]}
-        # Currently only deal with oneOf in leaf nodes
-        assert len(children) == 1, f"type of {fullname} couldn't be determined"
-        return next(iter(children))
-    if "allOf" in node:
-        children = {_make_group(fullname, n) for n in node["allOf"]}
-        # Currently only deal with allOf in leaf nodes
-        assert len(children) == 1, f"type of {fullname} couldn't be determined"
-        return next(iter(children))
-    if node["type"] in ("string", "number", "integer", "date"):
-        return Attr(fullname)
-    elif node["type"] == "array":
-        # skip to items
-        return _make_group(fullname, node["items"])
-    elif node["type"] == "object":
-        group = SchemaGroup()  # parent, name)
-        for childname, childnode in node["properties"].items():
-            fullchildname = f"{fullname}.{childname}" if fullname else childname
-            childgroup = _make_group(fullchildname, childnode)
-            setattr(group, childname, childgroup)
-        return group
-    else:
-        raise TypeError(f"Unrecognized node type {node['type']!r} of {fullname}")
+    group = SchemaGroup()
+    for (node, attrtype) in nodeL:
+        if "anyOf" in node:
+            children = {_make_group(fullname, [(n, attrtype)]) for n in node["anyOf"]}
+            # Currently only deal with anyOf in leaf nodes
+            assert len(children) == 1, f"type of {fullname} couldn't be determined"
+            return next(iter(children))
+        if "oneOf" in node:
+            children = {_make_group(fullname, [(n, attrtype)]) for n in node["oneOf"]}
+            # Currently only deal with oneOf in leaf nodes
+            assert len(children) == 1, f"type of {fullname} couldn't be determined"
+            return next(iter(children))
+        if "allOf" in node:
+            children = {_make_group(fullname, [(n, attrtype)]) for n in node["allOf"]}
+            # Currently only deal with allOf in leaf nodes
+            assert len(children) == 1, f"type of {fullname} couldn't be determined"
+            return next(iter(children))
+        if node["type"] in ("string", "number", "integer", "date"):
+            return Attr(fullname, attrtype)
+        elif node["type"] == "array":
+            # skip to items
+            return _make_group(fullname, [(node["items"], attrtype)])
+        elif node["type"] == "object":
+            for childname, childnode in node["properties"].items():
+                fullchildname = f"{fullname}.{childname}" if fullname else childname
+                childgroup = _make_group(fullchildname, [(childnode, attrtype)])
+                setattr(group, childname, childgroup)
+        else:
+            raise TypeError(f"Unrecognized node type {node['type']!r} of {fullname}")
+    return group
 
 
 def _make_schema() -> SchemaGroup:
-    json1 = _get_json_schema()
-    schema = _make_group("", json1)
+    json1 = _load_json_schema()
+    json2 = _load_chem_schema()
+    schemas = [(json1, STRUCTURE_ATTRIBUTE_SEARCH_SERVICE), (json2, CHEMICAL_ATTRIBUTE_SEARCH_SERVICE)]
+    schema = _make_group("", schemas)
     assert isinstance(schema, SchemaGroup)  # for type checking
     return schema
 
 
 rcsb_attributes: SchemaGroup
 """Object with all known RCSB PDB attributes.
 
@@ -176,13 +158,13 @@
 
 
 def __dir__() -> List[str]:
     return sorted(__all__)
 
 
 __all__ = [  # noqa: F822
-    "METADATA_SCHEMA_URL",
+    "STRUCTURE_ATTRIBUTE_SCHEMA_URL",
     "SEARCH_SCHEMA_URL",
-    "ENV_RCSBSEARCH_DOWNLOAD_SCHEMA",
+    "CHEMICAL_ATTRIBUTE_SCHEMA_URL",
     "rcsb_attributes",
     "SchemaGroup",
 ]
```

### Comparing `rcsbsearchapi-1.0.0/rcsbsearchapi/search.py` & `rcsbsearchapi-1.2.0/rcsbsearchapi/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,25 +24,30 @@
     Tuple,
     TypeVar,
     Union,
     overload,
 )
 
 import requests
+from .const import STRUCTURE_ATTRIBUTE_SEARCH_SERVICE, REQUESTS_PER_SECOND, FULL_TEXT_SEARCH_SERVICE, SEQUENCE_SEARCH_SERVICE, SEQUENCE_SEARCH_MIN_NUM_OF_RESIDUES
+from .const import RCSB_SEARCH_API_QUERY_URL, SEQMOTIF_SEARCH_SERVICE, SEQMOTIF_SEARCH_MIN_CHARACTERS
 
 if sys.version_info > (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 # tqdm is optional
-
-# Allowed return types for searches. http://search.rcsb.org/#return-type
+# Allowed return types for searches. https://search.rcsb.org/#return-type
 ReturnType = Literal[
-    "entry", "assembly", "polymer_entity", "non_polymer_entity", "polymer_instance"
+    "entry", "assembly", "polymer_entity", "non_polymer_entity", "polymer_instance",
+    "mol_definition"
 ]
+ReturnContentType = Literal["experimental", "computational"]  # results_content_type parameter list values
+SequenceType = Literal["dna", "rna", "protein"]  # possible sequence types for sequence searching
+SeqMode = Literal["simple", "prosite", "regex"]  # possible sequence motif formats
 TAndOr = Literal["and", "or"]
 # All valid types for Terminal values
 TValue = Union[
     str,
     int,
     float,
     date,
@@ -129,163 +134,207 @@
         """Difference: `a - b`"""
         return self & ~other
 
     def __xor__(self, other: "Query") -> "Query":
         """Symmetric difference: `a ^ b`"""
         return (self & ~other) | (~self & other)
 
-    def exec(self, return_type: ReturnType = "entry", rows: int = 10000) -> "Session":
+    def exec(self, return_type: ReturnType = "entry", rows: int = 10000, return_content_type: List[ReturnContentType] = ["experimental"]) -> "Session":
+        # pylint: disable=dangerous-default-value
         """Evaluate this query and return an iterator of all result IDs"""
-        return Session(self, return_type, rows)
+        return Session(self, return_type, rows, return_content_type)
 
-    def __call__(self, return_type: ReturnType = "entry", rows: int = 10000) -> "Session":
+    def __call__(self, return_type: ReturnType = "entry", rows: int = 10000, return_content_type: List[ReturnContentType] = ["experimental"]) -> "Session":
+        # pylint: disable=dangerous-default-value
         """Evaluate this query and return an iterator of all result IDs"""
-        return self.exec(return_type, rows)
+        return self.exec(return_type, rows, return_content_type)
 
     @overload
     def and_(self, other: "Query") -> "Query":
         ...
 
     @overload
     def and_(self, other: Union[str, "Attr"]) -> "PartialQuery":
         ...
 
     def and_(
-        self, other: Union[str, "Query", "Attr"]
+        self, other: Union[str, "Query", "Attr"], qtype=STRUCTURE_ATTRIBUTE_SEARCH_SERVICE
     ) -> Union["Query", "PartialQuery"]:
         """Extend this query with an additional attribute via an AND"""
         if isinstance(other, Query):
             return self & other
         elif isinstance(other, Attr):
             return PartialQuery(self, "and", other)
         elif isinstance(other, str):
-            return PartialQuery(self, "and", Attr(other))
+            return PartialQuery(self, "and", Attr(other, qtype))
         else:
             raise TypeError(f"Expected Query or Attr, got {type(other)}")
 
     @overload
     def or_(self, other: "Query") -> "Query":
         ...
 
     @overload
     def or_(self, other: Union[str, "Attr"]) -> "PartialQuery":
         ...
 
-    def or_(self, other: Union[str, "Query", "Attr"]) -> Union["Query", "PartialQuery"]:
+    def or_(self, other: Union[str, "Query", "Attr"], qtype=STRUCTURE_ATTRIBUTE_SEARCH_SERVICE) -> Union["Query", "PartialQuery"]:
         """Extend this query with an additional attribute via an OR"""
         if isinstance(other, Query):
             return self & other
         elif isinstance(other, Attr):
             return PartialQuery(self, "or", other)
         elif isinstance(other, str):
-            return PartialQuery(self, "or", Attr(other))
+            return PartialQuery(self, "or", Attr(other, qtype))
         else:
             raise TypeError(f"Expected Query or Attr, got {type(other)}")
 
 
 @dataclass(frozen=True)
 class Terminal(Query):
     """A terminal query node.
 
-    Terminals are simple predicates comparing some *attribute* of a structure to a
-    value.
+    Used for doing various types of searches. Accepts a service type and a dictionary of parameters.
+    The set of parameters differs for different search services.
 
-    Examples:
-        >>> Terminal("exptl.method", "exact_match", "X-RAY DIFFRACTION")
-        >>> Terminal("rcsb_id", "in", ["5T89", "1TIM"])
-        >>> Terminal(value="tubulin")
-
-    A full list of attributes is available in the
-    `schema <http://search.rcsb.org/rcsbsearch/v2/metadata/schema>`_.
-    Operators are documented `here <http://search.rcsb.org/#field-queries>`_.
+    Terminal can be built by passing in a service and parameter dictionary, but it's tedious work.
+    Typically, it's built by child classes that each represent a unique type of search.
+    This allows for more concise searching.
 
-    The :py:class:`Attr` class provides a more pythonic way of constructing Terminals.
+    Examples:
+        >>> Terminal("full_text", {"value": "protease"})
+        >>> Terminal("text", {"attribute": "rcsb_id", "operator": "in", "negation": False, "value": ["5T89, "1TIM"]})
     """
-
-    attribute: Optional[str] = None
-    operator: Optional[str] = None
-    value: Optional[TValue] = None
-    service: str = "text"
-    negation: Optional[bool] = False  # investigate whether this can be changed to None
+    service: str
+    params: Dict[str, Any]
     node_id: int = 0
 
     def to_dict(self):
-        params = dict()
-        if self.attribute is not None:
-            params["attribute"] = self.attribute
-        if self.operator is not None:
-            params["operator"] = self.operator
-        if self.value is not None:
-            params["value"] = self.value
-        if self.negation is not None:
-            params["negation"] = self.negation
-
         return dict(
             type="terminal",
             service=self.service,
-            parameters=params,
+            parameters=self.params,
             node_id=self.node_id,
         )
 
     def __invert__(self):
-        return Terminal(
-            self.attribute,
-            self.operator,
-            self.value,
-            self.service,
-            not self.negation,
-            self.node_id,
-        )
+        if isinstance(self, AttributeQuery):
+            return AttributeQuery(
+                attribute=self.params.get("attribute"),
+                operator=self.params.get("operator"),
+                negation=not self.params.get("negation"),
+                value=self.params.get("value")
+            )
+        else:
+            raise TypeError("Negation is not supported by type " + str(type(self)))  # Attribute Queries are the only query type to support inversion.
 
     def _assign_ids(self, node_id=0) -> Tuple[Query, int]:
         if self.node_id == node_id:
             return (self, node_id + 1)
         else:
             return (
-                Terminal(
-                    self.attribute,
-                    self.operator,
-                    self.value,
-                    self.service,
-                    self.negation,
-                    node_id,
-                ),
+                Terminal(self.service, self.params, node_id),
                 node_id + 1,
             )
 
-    def __str__(self):
-        """Return a simplified string representation
+    # def __str__(self): (leaving it commented out to find out what it actually does once something breaks)
+    #     """Return a simplified string representation
+
+    #     Example:
+    #         >>> Terminal(service="serv", params="par")
+
+    #     """
+    #     return f"Terminal(service={self.service!r}, params={self.params!r})"
+
+
+class AttributeQuery(Terminal):
+    """Special case of a Terminal for Structure and Chemical Attribute Searches
+
+    AttributeQueries compares some *attribute* of a structure to a value.
+
+    Examples:
+        >>> AttributeQuery("exptl.method", "exact_match", "X-RAY DIFFRACTION")
+        >>> AttributeQuery(value="tubulin")
+        >>> AttributeQuery("rcsb_entry_container_identifiers.entry_id", operator="in", value=["4HHB", "2GS2"])
+
+    A full list of attributes is available in the
+    `schema <https://search.rcsb.org/rcsbsearch/v2/metadata/schema>`_.
+    Operators are documented `here <https://search.rcsb.org/#field-queries>`_.
+
+    The :py:class:`Attr` class provides a more pythonic way of constructing AttributeQueries.
+    """
 
-        Examples:
-            >>> Terminal("attr", "op", "val")
-            >>> ~Terminal(value="val")
+    def __init__(self, attribute: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 value: Optional[TValue] = None,
+                 service: str = STRUCTURE_ATTRIBUTE_SEARCH_SERVICE,
+                 negation: Optional[bool] = False
+                 ):
+        """Search for the string value given possible attribute or operator
+        Also can specify service and negation
 
+        Args:
+            attribute: specify attribute for search (i.e struct.title, exptl.method, rcsb_id)
+            operator: specify operation to be done for search (i.e "contains_phrase", "exact_match")
+            value: text query
+            service: specify what search service (i.e "text", "text_chem")
+            negation: logical not
         """
-        negation = "~" if self.negation else ""
-        if self.attribute is None and self.operator is None:
-            # value-only
-            return f"{negation}Terminal(value={self.value!r})"
-        else:
-            return (
-                f"{negation}Terminal({self.attribute!r}, {self.operator!r}, "
-                f"{self.value!r})"
-            )
+        super().__init__(params={"attribute": attribute,
+                                 "operator": operator,
+                                 "negation": negation,
+                                 "value": value}, service=service)
 
 
 class TextQuery(Terminal):
     """Special case of a Terminal for free-text queries"""
 
     def __init__(self, value: str):
         """Search for the string value anywhere in the text
 
         Args:
             value: free-text query
-            negation: find structures without the pattern
         """
-        super().__init__(service="full_text", value=value, negation=None)
+        super().__init__(service=FULL_TEXT_SEARCH_SERVICE, params={"value": value})
+
+
+class SequenceQuery(Terminal):
+    """Special case of a terminal for protein, DNA, or RNA sequence queries"""
+
+    def __init__(self, value: str,
+                 evalue_cutoff: Optional[float] = 0.1,
+                 identity_cutoff: Optional[float] = 0,
+                 sequence_type: Optional[SequenceType] = "protein"
+                 ):
+        """The string value is a target sequence that is searched
+        Args:
+            value: sequence query
+        """
+        if len(value) < SEQUENCE_SEARCH_MIN_NUM_OF_RESIDUES:  # (placeholder for now) look into deriving constraints from API Schema programatically
+            raise ValueError("The sequence must contain at least 25 residues")
+        if identity_cutoff < 0.0 or identity_cutoff > 1.0:
+            raise ValueError("Identity cutoff should be between 0 and 1 (inclusive)")
+        else:
+            super().__init__(service=SEQUENCE_SEARCH_SERVICE, params={"evalue_cutoff": evalue_cutoff,
+                                                                      "identity_cutoff": identity_cutoff,
+                                                                      "sequence_type": sequence_type,
+                                                                      "value": value
+                                                                      })
+
+
+class SeqMotifQuery(Terminal):
+    """Special case of a terminal for protein, DNA, or RNA sequence queries"""
+
+    def __init__(self, value: str, pattern_type: Optional[SeqMode] = "simple", sequence_type: Optional[SequenceType] = "protein"):
+        if len(value) < SEQMOTIF_SEARCH_MIN_CHARACTERS:
+            raise ValueError("The sequence motif must contain at least 2 characters")
+        else:
+            super().__init__(service=SEQMOTIF_SEARCH_SERVICE, params={"value": value,
+                                                                      "pattern_type": pattern_type,
+                                                                      "sequence_type": sequence_type})
 
 
 @dataclass(frozen=True)
 class Group(Query):
     """AND and OR combinations of queries"""
 
     operator: TAndOr
@@ -317,15 +366,15 @@
 
     def __or__(self, other: Query) -> Query:
         # Combine nodes if possible
         if self.operator == "or":
             if isinstance(other, Group):
                 if other.operator == "or":
                     return Group("or", (*self.nodes, *other.nodes))
-            elif isinstance(other, Terminal):
+            elif isinstance(other, Query):
                 return Group("or", (*self.nodes, other))
             else:
                 return NotImplemented
 
         return super().__or__(other)
 
     def _assign_ids(self, node_id=0) -> Tuple[Query, int]:
@@ -386,94 +435,95 @@
     +--------------------+---------------------+
 
     Rather than their normal bool return values, operators return Terminals.
 
     Pre-instantiated attributes are available from the
     :py:data:`rcsbsearchapi.rcsb_attributes` object. These are generally easier to use
     than constructing Attr objects by hand. A complete list of valid attributes is
-    available in the `schema <http://search.rcsb.org/rcsbsearch/v2/metadata/schema>`_.
+    available in the `schema <https://search.rcsb.org/rcsbsearch/v2/metadata/schema>`_.
 
     * The `range` dictionary requires the following keys:
      * "from" -> int
      * "to" -> int
      * "include_lower" -> bool
      * "include_upper" -> bool
     """
 
     attribute: str
+    type: Optional[str] = STRUCTURE_ATTRIBUTE_SEARCH_SERVICE  # this will be changed later, this is to allow the program to still run. Will not be optional.
 
-    def exact_match(self, value: Union[str, "Value[str]"]) -> Terminal:
+    def exact_match(self, value: Union[str, "Value[str]"]) -> AttributeQuery:
         """Exact match with the value"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "exact_match", value)
+        return AttributeQuery(self.attribute, "exact_match", value, self.type)
 
     def contains_words(
         self, value: Union[str, "Value[str]", List[str], "Value[List[str]]"]
-    ) -> Terminal:
+    ) -> AttributeQuery:
         """Match any word within the string.
 
         Words are split at whitespace. All results which match any word are returned,
         with results matching more words sorted first.
         """
         if isinstance(value, Value):
             value = value.value
         if isinstance(value, list):
             value = " ".join(value)
-        return Terminal(self.attribute, "contains_words", value)
+        return AttributeQuery(self.attribute, "contains_words", value, self.type)
 
-    def contains_phrase(self, value: Union[str, "Value[str]"]) -> Terminal:
+    def contains_phrase(self, value: Union[str, "Value[str]"]) -> AttributeQuery:
         """Match an exact phrase"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "contains_phrase", value)
+        return AttributeQuery(self.attribute, "contains_phrase", value, self.type)
 
-    def greater(self, value: TNumberLike) -> Terminal:
+    def greater(self, value: TNumberLike) -> AttributeQuery:
         """Attribute > `value`"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "greater", value)
+        return AttributeQuery(self.attribute, "greater", value, self.type)
 
-    def less(self, value: TNumberLike) -> Terminal:
+    def less(self, value: TNumberLike) -> AttributeQuery:
         """Attribute < `value`"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "less", value)
+        return AttributeQuery(self.attribute, "less", value, self.type)
 
-    def greater_or_equal(self, value: TNumberLike) -> Terminal:
+    def greater_or_equal(self, value: TNumberLike) -> AttributeQuery:
         """Attribute >= `value`"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "greater_or_equal", value)
+        return AttributeQuery(self.attribute, "greater_or_equal", value, self.type)
 
-    def less_or_equal(self, value: TNumberLike) -> Terminal:
+    def less_or_equal(self, value: TNumberLike) -> AttributeQuery:
         """Attribute <= `value`"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "less_or_equal", value)
+        return AttributeQuery(self.attribute, "less_or_equal", value, self.type)
 
-    def equals(self, value: TNumberLike) -> Terminal:
+    def equals(self, value: TNumberLike) -> AttributeQuery:
         """Attribute == `value`"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "equals", value)
+        return AttributeQuery(self.attribute, "equals", value, self.type)
 
-    def range(self, value: Dict[str, Any]) -> Terminal:
+    def range(self, value: Dict[str, Any]) -> AttributeQuery:
         """Attribute is within the specified half-open range
 
         Args:
             value: lower and upper bounds `[a, b)`
         """
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "range", value)
+        return AttributeQuery(self.attribute, "range", value, self.type)
 
-    def exists(self) -> Terminal:
+    def exists(self) -> AttributeQuery:
         """Attribute is defined for the structure"""
-        return Terminal(self.attribute, "exists")
+        return AttributeQuery(self.attribute, operator="exists")
 
     def in_(
         self,
         value: Union[
             List[str],
             List[int],
             List[float],
@@ -487,19 +537,19 @@
             "Value[List[float]]",
             "Value[List[date]]",
             "Value[Tuple[str, ...]]",
             "Value[Tuple[int, ...]]",
             "Value[Tuple[float, ...]]",
             "Value[Tuple[date, ...]]",
         ],
-    ) -> Terminal:
+    ) -> AttributeQuery:
         """Attribute is contained in the list of values"""
         if isinstance(value, Value):
             value = value.value
-        return Terminal(self.attribute, "in", value)
+        return AttributeQuery(self.attribute, operator="in", value=value)
 
     # Need ignore[override] because typeshed restricts __eq__ return value
     # https://github.com/python/mypy/issues/2783
     @overload  # type: ignore[override]
     def __eq__(self, value: "Attr") -> bool:
         ...
 
@@ -949,29 +999,33 @@
 
 class Session(Iterable[str]):
     """A single query session.
 
     Handles paging the query and parsing results
     """
 
-    url = "http://search.rcsb.org/rcsbsearch/v2/query"
+    url = RCSB_SEARCH_API_QUERY_URL
     query_id: str
     query: Query
     return_type: ReturnType
     start: int
     rows: int
+    return_content_type: List[ReturnContentType]
 
     def __init__(
-        self, query: Query, return_type: ReturnType = "entry", rows: int = 10000
+        # parameter added below for computed model inclusion
+        self, query: Query, return_type: ReturnType = "entry", rows: int = 10000, return_content_type: List[ReturnContentType] = ["experimental"]
+        # pylint: disable=dangerous-default-value
     ):
         self.query_id = Session.make_uuid()
         self.query = query.assign_ids()
         self.return_type = return_type
         self.start = 0
         self.rows = rows
+        self.return_content_type = return_content_type
 
     @staticmethod
     def make_uuid() -> str:
         "Create a new UUID to identify a query"
         return uuid.uuid4().hex
 
     @staticmethod
@@ -987,15 +1041,16 @@
 
     def _make_params(self, start=0):
         "Generate GET parameters as a dict"
         return dict(
             query=self.query.to_dict(),
             return_type=self.return_type,
             request_info=dict(query_id=self.query_id, src="ui"),  # "TODO" src deprecated?
-            request_options=dict(paginate=dict(start=start, rows=self.rows)),  # v1 -> v2: pager parameter is renamed to paginate
+            # v1 -> v2: pager parameter is renamed to paginate and results_content_type parameter added (which has a list as its value)
+            request_options=dict(paginate=dict(start=start, rows=self.rows), results_content_type=self.return_content_type),
         )
 
     def _single_query(self, start=0) -> Optional[Dict]:
         "Fires a single query"
         params = self._make_params(start)
         logging.debug(
             "Querying %s for results %s-%s", self.url, start, start + self.rows - 1
@@ -1027,15 +1082,15 @@
         yield from identifiers
 
         total = response["total_count"]
 
         while start < total:
             assert len(identifiers) == self.rows
             req_count += 1
-            if req_count == 10:
+            if req_count == REQUESTS_PER_SECOND:
                 time.sleep(1.2)  # This prevents the user from bottlenecking the server with requests.
                 req_count = 0
             response = self._single_query(start=start)
             identifiers = self._extract_identifiers(response)
             logging.debug("Got %s ids", len(identifiers))
             start += self.rows
             yield from identifiers
@@ -1064,14 +1119,16 @@
 
         return identifiers[:limit]
 
     def rcsb_query_editor_url(self) -> str:
         """URL to edit this query in the RCSB PDB query editor"""
         data = json.dumps(self._make_params(), separators=(",", ":"))
         return (
-            f"http://search.rcsb.org/query-editor.html?json={urllib.parse.quote(data)}"
+            f"https://search.rcsb.org/query-editor.html?json={urllib.parse.quote(data)}"
         )
 
     def rcsb_query_builder_url(self) -> str:
         """URL to view this query on the RCSB PDB website query builder"""
-        data = json.dumps(self._make_params(), separators=(",", ":"))
-        return f"http://www.rcsb.org/search?request={urllib.parse.quote(data)}"
+        params = self._make_params()
+        params["request_options"]["paginate"]["rows"] = 25
+        data = json.dumps(params, separators=(",", ":"))
+        return f"https://www.rcsb.org/search?request={urllib.parse.quote(data)}"
```

### Comparing `rcsbsearchapi-1.0.0/setup.py` & `rcsbsearchapi-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     name=thisPackage,
     version=version,
     description="Python package interface for the RCSB PDB search API service",
     long_description_content_type="text/markdown",
     long_description=longDescription,
     author="Dennis Piehl",
     author_email="dennis.piehl@rcsb.org",
-    url="https://github.com/rcsb/py-rcsb_api_search",
+    url="https://github.com/rcsb/py-rcsbsearchapi",
     #
     license="BSD 3-Clause",
     classifiers=[
         "Programming Language :: Python",
         # "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
```

### Comparing `rcsbsearchapi-1.0.0/tests/testschema.py` & `rcsbsearchapi-1.2.0/tests/testschema.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import logging
 import platform
 import resource
 import time
 import unittest
 
 from rcsbsearchapi import rcsb_attributes as attrs
+from rcsbsearchapi.schema import _load_json_schema, _load_chem_schema, _download_schema
+from rcsbsearchapi.const import STRUCTURE_ATTRIBUTE_SCHEMA_URL, CHEMICAL_ATTRIBUTE_SCHEMA_URL
 
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
@@ -42,22 +44,40 @@
         logger.info("Maximum resident memory size %.4f %s", rusageMax / 10 ** 6, unitS)
         endTime = time.time()
         logger.info("Completed %s at %s (%.4f seconds)", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - self.__startTime)
 
     def testSchema(self):
         ok = attrs.rcsb_id.attribute == "rcsb_id"
         self.assertTrue(ok)
-
         ok2 = attrs.rcsb_struct_symmetry.symbol.attribute == "rcsb_struct_symmetry.symbol"
         self.assertTrue(ok2)
         logger.info("Schema test results: ok : (%r), ok2: (%r)", ok, ok2)
 
+    def testSchemaVersion(self):
+        webSchema = _download_schema(STRUCTURE_ATTRIBUTE_SCHEMA_URL)
+        localSchema = _load_json_schema()
+        localVer = localSchema.get("$comment")
+        webVer = webSchema.get("$comment")
+        ok = localVer == webVer
+        logger.info("ok is %r", ok)
+        self.assertTrue(ok)
+        logger.info("Metadata schema tests results: local version (%r) and web version (%s)", localVer, webVer)
+        webSchema = _download_schema(CHEMICAL_ATTRIBUTE_SCHEMA_URL)
+        localSchema = _load_chem_schema()
+        webVer = webSchema.get("$comment")
+        localVer = localSchema.get("$comment")
+        ok = webVer == localVer
+        logger.info("ok is %r", ok)
+        self.assertTrue(ok)
+        logger.info("Chemical schema tests results: local version (%r) and web version (%s)", localVer, webVer)
+
 
 def buildSchema():
     suiteSelect = unittest.TestSuite()
     suiteSelect.addTest(SchemaTests("testSchema"))
+    suiteSelect.addTest(SchemaTests("testSchemaVersion"))
     return suiteSelect
 
 
 if __name__ == "__main__":
     mySuite = buildSchema()
     unittest.TextTestRunner(verbosity=2).run(mySuite)
```

