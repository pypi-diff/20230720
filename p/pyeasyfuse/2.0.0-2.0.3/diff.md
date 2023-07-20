# Comparing `tmp/pyeasyfuse-2.0.0.tar.gz` & `tmp/pyeasyfuse-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasyfuse-2.0.0.tar", max compression
+gzip compressed data, was "pyeasyfuse-2.0.3.tar", max compression
```

## Comparing `pyeasyfuse-2.0.0.tar` & `pyeasyfuse-2.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-07-19 19:44:41.316090 pyeasyfuse-2.0.0/LICENSE
--rwxr-xr-x   0        0        0      426 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/README.md
--rw-r--r--   0        0        0       81 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/__init__.py
--rwxr-xr-x   0        0        0     4233 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/command_line.py
--rwxr-xr-x   0        0        0    59467 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/fusionannotation.py
--rwxr-xr-x   0        0        0    10256 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/fusionreadfilter.py
--rwxr-xr-x   0        0        0     6976 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/fusiontoolparser.py
--rwxr-xr-x   0        0        0     7353 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/fusiontoolparser_helper.py
--rwxr-xr-x   0        0        0        0 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/config.py
--rwxr-xr-x   0        0        0     1016 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/count_input_reads.py
--rwxr-xr-x   0        0        0     3861 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/io_methods.py
--rwxr-xr-x   0        0        0     3678 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/qc_parser.py
--rwxr-xr-x   0        0        0     7716 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/misc/queueing.py
--rwxr-xr-x   0        0        0    35461 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/processing.py
--rwxr-xr-x   0        0        0    13646 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/read_selection.py
--rw-r--r--   0        0        0     6524 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/ref_data/GTFtoCSV.R
--rw-r--r--   0        0        0        0 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/ref_data/__init__.py
--rwxr-xr-x   0        0        0     3116 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/ref_data/gff3_to_db.py
--rwxr-xr-x   0        0        0     4233 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/ref_data/gtf2tsl.py
--rw-r--r--   0        0        0     2738 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/ref_data/reformat_genome_fasta.py
--rwxr-xr-x   0        0        0    13446 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/requantify.py
--rwxr-xr-x   0        0        0     4165 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.0/easy_fuse/resources/R/R_model_prediction.R
--rw-r--r--   0        0        0  1915516 2023-07-20 12:53:23.313192 pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full.rds
--rw-r--r--   0        0        0  2251607 2023-07-20 12:53:23.313192 pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full_rep.rds
--rw-r--r--   0        0        0   359633 2023-07-20 12:53:23.321192 pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant.rds
--rw-r--r--   0        0        0  1773782 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant_type.rds
--rwxr-xr-x   0        0        0    21424 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/summarize_data.py
--rw-r--r--   0        0        0        0 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/__init__.py
--rw-r--r--   0        0        0      621 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/fusioncatcher_1.txt
--rw-r--r--   0        0        0     2998 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/fusioncatcher_2.txt
--rw-r--r--   0        0        0     3406 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/infusion.txt
--rw-r--r--   0        0        0     3418 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/mapsplice.txt
--rw-r--r--   0        0        0      784 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/soapfuse.txt
--rw-r--r--   0        0        0    62446 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/starfusion.txt
--rw-r--r--   0        0        0     2715 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/resources/test.config.ini
--rw-r--r--   0        0        0     2274 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/test_config.py
--rw-r--r--   0        0        0     2428 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/test_fusion_annotation.py
--rw-r--r--   0        0        0    10044 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tests/test_fusion_tool_parser.py
--rwxr-xr-x   0        0        0        0 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/__init__.py
--rwxr-xr-x   0        0        0     3229 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/skewer_wrapper.py
--rwxr-xr-x   0        0        0     2540 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/soapfuse_wrapper.py
--rw-r--r--   0        0        0     2281 2023-07-20 12:53:23.329192 pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/star_custom_index.py
--rw-r--r--   0        0        0     1641 2023-07-20 16:34:47.088243 pyeasyfuse-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pyeasyfuse-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-19 19:44:41.316090 pyeasyfuse-2.0.3/LICENSE
+-rwxr-xr-x   0        0        0      426 2023-07-20 12:53:23.289191 pyeasyfuse-2.0.3/README.md
+-rw-r--r--   0        0        0       82 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/__init__.py
+-rwxr-xr-x   0        0        0     4248 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/command_line.py
+-rwxr-xr-x   0        0        0    59467 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/fusionannotation.py
+-rwxr-xr-x   0        0        0    10256 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/fusionreadfilter.py
+-rwxr-xr-x   0        0        0     6977 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/fusiontoolparser.py
+-rwxr-xr-x   0        0        0     7353 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/fusiontoolparser_helper.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/config.py
+-rwxr-xr-x   0        0        0     1016 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/count_input_reads.py
+-rwxr-xr-x   0        0        0     3861 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/io_methods.py
+-rwxr-xr-x   0        0        0     3678 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/qc_parser.py
+-rwxr-xr-x   0        0        0     7716 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/misc/queueing.py
+-rwxr-xr-x   0        0        0    35467 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/processing.py
+-rwxr-xr-x   0        0        0    13647 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/read_selection.py
+-rw-r--r--   0        0        0     6524 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/ref_data/GTFtoCSV.R
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/ref_data/__init__.py
+-rwxr-xr-x   0        0        0     3116 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/ref_data/gff3_to_db.py
+-rwxr-xr-x   0        0        0     4233 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/ref_data/gtf2tsl.py
+-rw-r--r--   0        0        0     2738 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/ref_data/reformat_genome_fasta.py
+-rwxr-xr-x   0        0        0    13447 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/requantify.py
+-rwxr-xr-x   0        0        0     4165 2023-07-20 17:24:57.988071 pyeasyfuse-2.0.3/pyeasyfuse/resources/R/R_model_prediction.R
+-rw-r--r--   0        0        0  1915516 2023-07-20 17:24:58.012071 pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full.rds
+-rw-r--r--   0        0        0  2251607 2023-07-20 17:24:58.012071 pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full_rep.rds
+-rw-r--r--   0        0        0   359633 2023-07-20 17:24:58.016071 pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant.rds
+-rw-r--r--   0        0        0  1773782 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant_type.rds
+-rwxr-xr-x   0        0        0    21428 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/summarize_data.py
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/fusioncatcher_1.txt
+-rw-r--r--   0        0        0     2998 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/fusioncatcher_2.txt
+-rw-r--r--   0        0        0     3406 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/infusion.txt
+-rw-r--r--   0        0        0     3418 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/mapsplice.txt
+-rw-r--r--   0        0        0      784 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/soapfuse.txt
+-rw-r--r--   0        0        0    62446 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/starfusion.txt
+-rw-r--r--   0        0        0     2715 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/test.config.ini
+-rw-r--r--   0        0        0     2280 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/test_config.py
+-rw-r--r--   0        0        0     2429 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/test_fusion_annotation.py
+-rw-r--r--   0        0        0    10056 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tests/test_fusion_tool_parser.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/__init__.py
+-rwxr-xr-x   0        0        0     3229 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/skewer_wrapper.py
+-rwxr-xr-x   0        0        0     2540 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/soapfuse_wrapper.py
+-rw-r--r--   0        0        0     2281 2023-07-20 17:24:58.028070 pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/star_custom_index.py
+-rw-r--r--   0        0        0     1644 2023-07-20 19:30:05.344534 pyeasyfuse-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 pyeasyfuse-2.0.3/PKG-INFO
```

### Comparing `pyeasyfuse-2.0.0/LICENSE` & `pyeasyfuse-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/command_line.py` & `pyeasyfuse-2.0.3/pyeasyfuse/command_line.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import argparse
 
-from easy_fuse.ref_data.gff3_to_db import add_gff3_to_db_args
-from easy_fuse.ref_data.gtf2tsl import add_gtf_to_tsl_args
-from easy_fuse.misc.qc_parser import add_qc_parser_args
-from easy_fuse.read_selection import add_read_selection_args
-from easy_fuse.requantify import add_requantify_args
-from easy_fuse.summarize_data import add_summarize_data_args
-from easy_fuse.fusionreadfilter import add_read_filter_args
-from easy_fuse.fusiontoolparser import add_fusion_parse_args
-from easy_fuse.fusionannotation import add_annotation_parser_args
+from pyeasyfuse.ref_data.gff3_to_db import add_gff3_to_db_args
+from pyeasyfuse.ref_data.gtf2tsl import add_gtf_to_tsl_args
+from pyeasyfuse.misc.qc_parser import add_qc_parser_args
+from pyeasyfuse.read_selection import add_read_selection_args
+from pyeasyfuse.requantify import add_requantify_args
+from pyeasyfuse.summarize_data import add_summarize_data_args
+from pyeasyfuse.fusionreadfilter import add_read_filter_args
+from pyeasyfuse.fusiontoolparser import add_fusion_parse_args
+from pyeasyfuse.fusionannotation import add_annotation_parser_args
 from logzero import logger
-import easy_fuse
-from easy_fuse.processing import add_pipeline_parser_args
-from easy_fuse.tool_wrapper.skewer_wrapper import add_skewer_args
-from easy_fuse.tool_wrapper.soapfuse_wrapper import add_soapfuse_wrapper_args
-from easy_fuse.tool_wrapper.star_custom_index import add_star_custom_index_args
+import pyeasyfuse
+from pyeasyfuse.processing import add_pipeline_parser_args
+from pyeasyfuse.tool_wrapper.skewer_wrapper import add_skewer_args
+from pyeasyfuse.tool_wrapper.soapfuse_wrapper import add_soapfuse_wrapper_args
+from pyeasyfuse.tool_wrapper.star_custom_index import add_star_custom_index_args
 
 
 epilog = "Copyright (c) 2023 TRON gGmbH (See LICENSE for licensing details)"
 
 
 def easy_fuse_cli():
     # set up logger
     parser = argparse.ArgumentParser(
-        description="EasyFuse v{}".format(easy_fuse.__version__),
+        description="EasyFuse v{}".format(pyeasyfuse.__version__),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         epilog=epilog,
     )
 
     subparsers = parser.add_subparsers(description="Commands")
 
     pipeline_parser = subparsers.add_parser(
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/fusionannotation.py` & `pyeasyfuse-2.0.3/pyeasyfuse/fusionannotation.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/fusionreadfilter.py` & `pyeasyfuse-2.0.3/pyeasyfuse/fusionreadfilter.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/fusiontoolparser.py` & `pyeasyfuse-2.0.3/pyeasyfuse/fusiontoolparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 import os
 from typing import Dict
 
 import logzero
 from logzero import logger
 
-from easy_fuse.fusiontoolparser_helper import *
+from pyeasyfuse.fusiontoolparser_helper import *
 
 
 # pylint: disable=line-too-long
 #         yes they are partially, but I do not consider this to be relevant here
 class FusionParser(object):
     """Get and parse results from previously run programs (fusion prediction, hla typing, expression estimation)"""
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/fusiontoolparser_helper.py` & `pyeasyfuse-2.0.3/pyeasyfuse/fusiontoolparser_helper.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/misc/count_input_reads.py` & `pyeasyfuse-2.0.3/pyeasyfuse/misc/count_input_reads.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/misc/io_methods.py` & `pyeasyfuse-2.0.3/pyeasyfuse/misc/io_methods.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/misc/qc_parser.py` & `pyeasyfuse-2.0.3/pyeasyfuse/misc/qc_parser.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/misc/queueing.py` & `pyeasyfuse-2.0.3/pyeasyfuse/misc/queueing.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/processing.py` & `pyeasyfuse-2.0.3/pyeasyfuse/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import os.path
 import time
 from shutil import copy
 
 import logzero
 from logzero import logger
 
-import easy_fuse
-import easy_fuse.misc.io_methods as io_methods
-from easy_fuse import __version__
-from easy_fuse.misc import queueing
-from easy_fuse.misc.config import EasyFuseConfiguration
+import pyeasyfuse
+import pyeasyfuse.misc.io_methods as io_methods
+from pyeasyfuse import __version__
+from pyeasyfuse.misc import queueing
+from pyeasyfuse.misc.config import EasyFuseConfiguration
 
 DEFAULT_CPU_MEM = "1,16"
 
 READ_FILTER_STEP = "readfilter"
 
 
 class Processing(object):
@@ -891,15 +891,15 @@
         default="",
     )
     pipeline_parser.add_argument(
         "-V",
         "--version",
         dest="version",
         action="version",
-        version="%(prog)s {version}".format(version=easy_fuse.__version__),
+        version="%(prog)s {version}".format(version=pyeasyfuse.__version__),
         help="Get version info",
     )
     pipeline_parser.set_defaults(func=pipeline_command)
 
 
 def pipeline_command(args):
     if args.jobname_suffix:
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/read_selection.py` & `pyeasyfuse-2.0.3/pyeasyfuse/read_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import sys
 import time
 
 import logzero
 import pysam  # pysam is not available for windows (where I run pylint) => pylint: disable=E0401
 from logzero import logger
 
-from easy_fuse.misc.count_input_reads import get_input_read_count_from_star
+from pyeasyfuse.misc.count_input_reads import get_input_read_count_from_star
 
 
 # pylint: disable=line-too-long
 #         yes they are partially, but I do not consider this to be relevant here
 class ReadSelection(object):
     """Select alignments belonging to putative fusions from an s/bam file"""
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/ref_data/GTFtoCSV.R` & `pyeasyfuse-2.0.3/pyeasyfuse/ref_data/GTFtoCSV.R`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/ref_data/gff3_to_db.py` & `pyeasyfuse-2.0.3/pyeasyfuse/ref_data/gff3_to_db.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/ref_data/gtf2tsl.py` & `pyeasyfuse-2.0.3/pyeasyfuse/ref_data/gtf2tsl.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/ref_data/reformat_genome_fasta.py` & `pyeasyfuse-2.0.3/pyeasyfuse/ref_data/reformat_genome_fasta.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/requantify.py` & `pyeasyfuse-2.0.3/pyeasyfuse/requantify.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @version: 20221005
 """
 import os
 
 from logzero import logger
 import pysam
 
-from easy_fuse.misc.count_input_reads import get_input_read_count_from_star
+from pyeasyfuse.misc.count_input_reads import get_input_read_count_from_star
 
 
 class Requantification(object):
     """Select alignments belonging to putative fusions from an s/bam file"""
 
     def __init__(self, bam, output, bp_distance_threshold, input_reads_stats,):
         """Parameter initialization"""
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/resources/R/R_model_prediction.R` & `pyeasyfuse-2.0.3/pyeasyfuse/resources/R/R_model_prediction.R`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full.rds` & `pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full.rds`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full_rep.rds` & `pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_full_rep.rds`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant.rds` & `pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant.rds`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant_type.rds` & `pyeasyfuse-2.0.3/pyeasyfuse/resources/model/Fusion_modeling_FFPE_train_v35.random_forest.model_full_data.EF_requant_type.rds`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/summarize_data.py` & `pyeasyfuse-2.0.3/pyeasyfuse/summarize_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 @author: BNT (URLA), TRON (PASO)
 @version: 20190118
 """
 import os
 import os.path
 import time
 
-import easy_fuse
+import pyeasyfuse
 import pkg_resources
 from logzero import logger
 import pandas as pd
-from easy_fuse.misc import queueing
-from easy_fuse.misc.count_input_reads import get_input_read_count_from_star
+from pyeasyfuse.misc import queueing
+from pyeasyfuse.misc.count_input_reads import get_input_read_count_from_star
 
 
 class FusionSummary(object):
     """Collect stats of the run and write them to file"""
 
     def __init__(
             self,
@@ -139,15 +139,15 @@
         if model_predictions and os.path.exists(ranked_fusions_file) and os.path.isfile(ranked_fusions_file):
             model_path = os.path.abspath(self.input_model_pred)
 
             # append prediction scores based on pre-calculated model
             predicted_fusions_file = os.path.join(self.output_folder, "fusions.pass.csv")
             cmd_model = "{0} --fusion_summary {1} --model_file {2} --prediction_threshold {3} --output {4}".format(
                 pkg_resources.resource_filename(
-                    easy_fuse.__name__, "resources/R/R_model_prediction.R"
+                    pyeasyfuse.__name__, "resources/R/R_model_prediction.R"
                 ),
                 ranked_fusions_file,
                 model_path,
                 self.model_pred_threshold,
                 predicted_fusions_file,
             )
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/fusioncatcher_1.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/fusioncatcher_1.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/fusioncatcher_2.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/fusioncatcher_2.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/infusion.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/infusion.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/mapsplice.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/mapsplice.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/soapfuse.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/soapfuse.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/starfusion.txt` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/starfusion.txt`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/resources/test.config.ini` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/resources/test.config.ini`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/test_config.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from configparser import NoOptionError, NoSectionError
 from unittest import TestCase
 
 import pkg_resources
 
-import easy_fuse.tests
-from easy_fuse.misc.config import EasyFuseConfiguration
+import pyeasyfuse.tests
+from pyeasyfuse.misc.config import EasyFuseConfiguration
 
 
 class TestConfig(TestCase):
     def test_config_loading(self):
         config_file = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/test.config.ini"
+            pyeasyfuse.tests.__name__, "resources/test.config.ini"
         )
         config = EasyFuseConfiguration(config_file=config_file)
         self.assertIsInstance(config, EasyFuseConfiguration)
         self.assertEqual(config.config_file, config_file)
         self.assertEqual(config.get("general", "pipeline_name"), "EasyFuse")
         self.assertEqual(config.get("general", "min_read_len_perc"), "0.75")
         self.assertEqual(config.get("general", "max_dist_proper_pair"), "200000")
@@ -28,27 +28,27 @@
         self.assertEqual(
             config.get("other_files", "infusion_cfg"),
             "/path/to/infusion_index/infusion.cfg",
         )
 
     def test_non_existing_value(self):
         config_file = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/test.config.ini"
+            pyeasyfuse.tests.__name__, "resources/test.config.ini"
         )
         config = EasyFuseConfiguration(config_file=config_file)
         with self.assertRaises(NoOptionError):
             config.get("general", "idontexist")
 
     def test_non_existing_section(self):
         config_file = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/test.config.ini"
+            pyeasyfuse.tests.__name__, "resources/test.config.ini"
         )
         config = EasyFuseConfiguration(config_file=config_file)
         with self.assertRaises(NoSectionError):
             config.get("idontexist", "pipeline_name")
 
     def test_non_existing_config_file(self):
         config_file = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/idontexist.config.ini"
+            pyeasyfuse.tests.__name__, "resources/idontexist.config.ini"
         )
         with self.assertRaises(AssertionError):
             EasyFuseConfiguration(config_file)
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/test_fusion_annotation.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/test_fusion_annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from easy_fuse.fusionannotation import FusionAnnotation
+from pyeasyfuse.fusionannotation import FusionAnnotation
 
 
 class TestFusionAnnotation(unittest.TestCase):
     def test_define_type(self):
         self.assertEqual(
             FusionAnnotation.define_type(500, "1", 200, "+", "2", 600, "-"), "trans_inv"
         )
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tests/test_fusion_tool_parser.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tests/test_fusion_tool_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import unittest
 
-import easy_fuse.tests
+import pyeasyfuse.tests
 import pkg_resources
 
-from easy_fuse.fusiontoolparser_helper import parse_fusioncatcher_results
-from easy_fuse.fusiontoolparser_helper import parse_starfusion_results
-from easy_fuse.fusiontoolparser_helper import parse_mapsplice_results
-from easy_fuse.fusiontoolparser_helper import parse_infusion_results
-from easy_fuse.fusiontoolparser_helper import parse_soapfuse_results
+from pyeasyfuse.fusiontoolparser_helper import parse_fusioncatcher_results
+from pyeasyfuse.fusiontoolparser_helper import parse_starfusion_results
+from pyeasyfuse.fusiontoolparser_helper import parse_mapsplice_results
+from pyeasyfuse.fusiontoolparser_helper import parse_infusion_results
+from pyeasyfuse.fusiontoolparser_helper import parse_soapfuse_results
 
 
 class TestFusionToolParser(unittest.TestCase):
     def setUp(self):
         self.fusion_catcher1 = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/fusioncatcher_1.txt"
+            pyeasyfuse.tests.__name__, "resources/fusioncatcher_1.txt"
         )
         self.fusion_catcher2 = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/fusioncatcher_2.txt"
+            pyeasyfuse.tests.__name__, "resources/fusioncatcher_2.txt"
         )
         self.star_fusion = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/starfusion.txt"
+            pyeasyfuse.tests.__name__, "resources/starfusion.txt"
         )
         self.mapsplice = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/mapsplice.txt"
+            pyeasyfuse.tests.__name__, "resources/mapsplice.txt"
         )
         self.infusion = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/infusion.txt"
+            pyeasyfuse.tests.__name__, "resources/infusion.txt"
         )
         self.soapfuse = pkg_resources.resource_filename(
-            easy_fuse.tests.__name__, "resources/soapfuse.txt"
+            pyeasyfuse.tests.__name__, "resources/soapfuse.txt"
         )
 
     def test_parse_fusioncatcher_results(self):
         result_dict = {
             "22:29287134:+_12:50814280:+": [
                 "EWSR1_ATF1",
                 "22:29287134:+",
```

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/skewer_wrapper.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/skewer_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/soapfuse_wrapper.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/soapfuse_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/easy_fuse/tool_wrapper/star_custom_index.py` & `pyeasyfuse-2.0.3/pyeasyfuse/tool_wrapper/star_custom_index.py`

 * *Files identical despite different names*

### Comparing `pyeasyfuse-2.0.0/pyproject.toml` & `pyeasyfuse-2.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyeasyfuse"
-version = "2.0.0"
+version = "2.0.3"
 authors = [
     "Patrick Sorn <patrick.sorn@tron-mainz.edu>",
     "Jonas Ibn-Salem <jonas.ibn-salem@tron-mainz.edu>",
     "Christoph Holsträter <christoph.holstraeter@tron-mainz.edu>",
     "David Weber <david.weber@tron-mainz.edu>",
-    "Pablo Riesgo-Ferreiro <pablo.riesgo-ferreiro@tron-mainz.edu>",
+    "Pablo Riesgo-Ferreiro <pablo.riesgoferreiro@tron-mainz.edu>",
 ]
 description = "EasyFuse is a pipeline to detect fusion transcripts from RNA-seq data with high accuracy."
 readme = "README.md"
 keywords = ["bioinformatics", "fusions", "RNA-seq", "transcriptomics"]
 license = "LICENSE"
 classifiers = [
     "Development Status :: 3 - Alpha",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Programming Language :: Python :: 3.7",
 ]
-packages = [{include = "easy_fuse"}]
+packages = [{include = "pyeasyfuse"}]
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^7.1.0"}
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*"]
 
 [tool.coverage.report]
 fail_under = 80
 
 [tool.setuptools]
-py-modules = ["easy_fuse"]
+py-modules = ["pyeasyfuse"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.8"
 numpy = "1.21.6"
 pandas = "0.24.0"
 xxhash = "1.4.3"
 biopython = "1.73"
 pysam = "0.15.2"
 gffutils = "0.10.1"
 bx-python = "0.8.2"
 logzero = "1.7.0"
 pytz = "2022.7.1"
 
 [tool.setuptools.dynamic]
-version = {attr = "easy_fuse.__version__"}
+version = {attr = "pyeasyfuse.__version__"}
 
 [tool.poetry.scripts]
-easy-fuse = "easy_fuse.command_line:easy_fuse_cli"
+easy-fuse = "pyeasyfuse.command_line:easy_fuse_cli"
```

### Comparing `pyeasyfuse-2.0.0/PKG-INFO` & `pyeasyfuse-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasyfuse
-Version: 2.0.0
+Version: 2.0.3
 Summary: EasyFuse is a pipeline to detect fusion transcripts from RNA-seq data with high accuracy.
 License: LICENSE
 Keywords: bioinformatics,fusions,RNA-seq,transcriptomics
 Author: Patrick Sorn
 Author-email: patrick.sorn@tron-mainz.edu
 Requires-Python: >=3.7,<3.8
 Classifier: Development Status :: 3 - Alpha
```

