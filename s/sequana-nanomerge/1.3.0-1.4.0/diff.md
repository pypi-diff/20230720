# Comparing `tmp/sequana_nanomerge-1.3.0.tar.gz` & `tmp/sequana_nanomerge-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_nanomerge-1.3.0.tar", last modified: Mon Jun  5 10:06:44 2023, max compression
+gzip compressed data, was "dist/sequana_nanomerge-1.4.0.tar", last modified: Thu Jul 20 16:55:23 2023, max compression
```

## Comparing `sequana_nanomerge-1.3.0.tar` & `sequana_nanomerge-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8443 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5812 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8443 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14218 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/dag.png
--rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/nanomerge.rules
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8710 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8710 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14218 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7103 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13666 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/nanomerge.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-20 16:55:23.000000 sequana_nanomerge-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-07-20 16:55:16.000000 sequana_nanomerge-1.4.0/setup.py
```

### Comparing `sequana_nanomerge-1.3.0/PKG-INFO` & `sequana_nanomerge-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_nanomerge
-Version: 1.3.0
+Version: 1.4.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -154,14 +154,18 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.4.0     * sub sampling was biased in v1.3.0. Using stratified sampling to 
+                    correcly sample large file. Also set a --promethion option that
+                    auomatically sub sample 10% of the data
+                  * add summary table
         1.3.0     * handle large promethium run by using a sub sample of the 
                     sequencing summary file (--sample of pycoQC still loads the entire
                     file in memory)
         1.2.0     * handle large promethium run by using find+cat instead of just 
                     cat to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
```

### Comparing `sequana_nanomerge-1.3.0/README.rst` & `sequana_nanomerge-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,18 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.4.0     * sub sampling was biased in v1.3.0. Using stratified sampling to 
+            correcly sample large file. Also set a --promethion option that
+            auomatically sub sample 10% of the data
+          * add summary table
 1.3.0     * handle large promethium run by using a sub sample of the 
             sequencing summary file (--sample of pycoQC still loads the entire
             file in memory)
 1.2.0     * handle large promethium run by using find+cat instead of just 
             cat to cope with very large number of input files.
 1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
             runs such as promethion
```

### Comparing `sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/PKG-INFO` & `sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-nanomerge
-Version: 1.3.0
+Version: 1.4.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -154,14 +154,18 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.4.0     * sub sampling was biased in v1.3.0. Using stratified sampling to 
+                    correcly sample large file. Also set a --promethion option that
+                    auomatically sub sample 10% of the data
+                  * add summary table
         1.3.0     * handle large promethium run by using a sub sample of the 
                     sequencing summary file (--sample of pycoQC still loads the entire
                     file in memory)
         1.2.0     * handle large promethium run by using find+cat instead of just 
                     cat to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
```

### Comparing `sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/SOURCES.txt` & `sequana_nanomerge-1.4.0/sequana_nanomerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/config.yaml` & `sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/dag.png` & `sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/main.py` & `sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,36 +61,42 @@
             type=str,
             dest="samplesheet",
             required=True,
         )
 
         pipeline_group.add_argument(
             "--summary",
-            help="a summary file generated by albacore or guppy. if provided,pyqoQC is used to generate a HTML report. ",
+            help="a summary file generated by albacore or guppy. if provided, pyqoQC is used to generate a HTML report. ",
             default=None,
             type=str,
             dest="summary",
         )
 
         pipeline_group.add_argument(
             "--summary-percentage",
-            help="percentage of the sequencing summary file to process. Use this option if you have memory issue (typically with promethium runs). If unset, nanomerge will set this value automatically so that the final file to process do not exceed 16Go. This value can be cahnged with --summary-max--gb",
+            help="percentage of the sequencing summary file to process. Use this option if you have memory issue typically with promethium runs). If unset, nanomerge will set this value automatically so that the final file to process do not exceed 16Go. This value can be changed with --summary-max--gb",
             default=None,
             type=int,
             dest="summary_percentage",
         )
 
         pipeline_group.add_argument(
             "--summary-max-gb",
-            help="percentage of the sequencing summary file to process. Use :this option if you have memory issue (typically with promethium runs. ",
+            help="max size of the summary file before performing sub sampling automatically. Use this option if you have memory issue.",
             default=16,
             type=float,
             dest="summary_max_gb",
         )
 
+        pipeline_group.add_argument(
+            "--promethion",
+            action="store_true",
+            help="set summary_percentage to 10%%"
+        )
+
         self.add_argument("--run", default=False, action="store_true", help="execute the pipeline directly")
 
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
             if len(args_list) > 2:
                 msg = (
@@ -148,29 +154,34 @@
                 shutil.copy(options.summary, manager.workdir)
                 cfg.summary = Path(options.summary).name
             elif not os.path.exists(options.summary):
                 raise IOError(f"{options.summary} not found. Check your input filename")
 
             # if the sequencing summary file is large (larger than 16gb by default) we sub sample the data
             # The percentage is set automatically to have a final file of 16Gb (by default)
+
+
             if options.summary_percentage is None:
                 cfg.sub_sample_summary.percentage = options.summary_max_gb / (
                     os.stat(options.summary).st_size / 1024 / 1024 / 1024
                 )
                 cfg.sub_sample_summary.percentage = int(cfg.sub_sample_summary.percentage * 100)
                 if cfg.sub_sample_summary.percentage > 100:
                     cfg.sub_sample_summary.percentage = 100
                 if cfg.sub_sample_summary.percentage < 100:
                     size = os.stat(options.summary).st_size / 1024 / 1024 / 1024
                     logger.warning(
                         f"Input file size is {size}Gb , which is larger than {options.summary_max_gb}Gb. Will use {cfg.sub_sample_summary.percentage}% of the data"
                     )
-
             else:  # user sets the value himself, so nothing to do
                 cfg.sub_sample_summary.percentage = options.summary_percentage
+
+            # if --promethion was used, set percentage to 10 whatsover
+            if options.promethion:
+                cfg.sub_sample_summary.percentage = 10
         else:
             cfg.summary = None
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
```

### Comparing `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/schema.yaml` & `sequana_nanomerge-1.4.0/sequana_pipelines/nanomerge/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.3.0/setup.py` & `sequana_nanomerge-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # handle sequana git link
 with open("requirements.txt", encoding='utf-8') as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 1
-_MINOR               = 3
+_MINOR               = 4
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
```

