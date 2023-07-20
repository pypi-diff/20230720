# Comparing `tmp/seqchromloader-0.6.4.tar.gz` & `tmp/seqchromloader-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.6.4.tar", last modified: Thu Jul 20 18:01:22 2023, max compression
+gzip compressed data, was "seqchromloader-0.6.5.tar", last modified: Thu Jul 20 20:28:26 2023, max compression
```

## Comparing `seqchromloader-0.6.4.tar` & `seqchromloader-0.6.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.768117 seqchromloader-0.6.4/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 18:01:22.767476 seqchromloader-0.6.4/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.4/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.746480 seqchromloader-0.6.4/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.4/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.4/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14888 2023-07-20 17:54:13.000000 seqchromloader-0.6.4/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7355 2023-07-20 17:56:20.000000 seqchromloader-0.6.4/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.759014 seqchromloader-0.6.4/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-07-20 18:01:22.768308 seqchromloader-0.6.4/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-07-20 17:39:28.000000 seqchromloader-0.6.4/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.766298 seqchromloader-0.6.4/tests/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13756 2023-07-20 17:50:28.000000 seqchromloader-0.6.4/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 20:28:26.699423 seqchromloader-0.6.5/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 20:28:26.699165 seqchromloader-0.6.5/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.5/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 20:28:26.668444 seqchromloader-0.6.5/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.5/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.5/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14892 2023-07-20 20:24:08.000000 seqchromloader-0.6.5/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7355 2023-07-20 17:56:20.000000 seqchromloader-0.6.5/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 20:28:26.697366 seqchromloader-0.6.5/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 20:28:26.000000 seqchromloader-0.6.5/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-07-20 20:28:26.000000 seqchromloader-0.6.5/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-07-20 20:28:26.000000 seqchromloader-0.6.5/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-07-20 20:28:26.000000 seqchromloader-0.6.5/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-07-20 20:28:26.000000 seqchromloader-0.6.5/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-07-20 20:28:26.699496 seqchromloader-0.6.5/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-07-20 20:25:14.000000 seqchromloader-0.6.5/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 20:28:26.698006 seqchromloader-0.6.5/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13756 2023-07-20 17:50:28.000000 seqchromloader-0.6.5/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.6.4/PKG-INFO` & `seqchromloader-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.4
+Version: 0.6.5
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.4/README.md` & `seqchromloader-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.4/seqchromloader/loader.py` & `seqchromloader-0.6.5/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.4/seqchromloader/utils.py` & `seqchromloader-0.6.5/seqchromloader/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,25 +366,25 @@
             if strand=="-":
                 target_array = target_array[::-1]
         except RuntimeError as e:
             logging.warning(e)
             logging.warning(f"RuntimeError happened when accessing {chrom}:{start}-{end}, it's probably due to at least one chromatin track bigwig doesn't have information in this region")
             raise BigWigInaccessible(chrom, start, end)
     else:
-        target_array = np.array([None])
+        target_array = np.array([np.nan])
     return target_array
 
 def extract_info(chrom, start, end, label, genome_pyfaidx, bigwigs, target, strand="+", transforms:dict=None):
     seq_array = extract_dnaOneHot(chrom, start, end, strand, genome_pyfaidx)
 
     #chromatin track
     if bigwigs is not None and len(bigwigs)>0:
         chroms_array = extract_bw(chrom, start, end, strand, bigwigs)
     else:
-        chroms_array = np.array([None])
+        chroms_array = np.array([np.nan])
     # label
     label_array = np.array(label, dtype=np.int32)[np.newaxis]
     # counts
     target_array = extract_target(chrom, start, end, strand, target)
 
     feature = {
         'seq': seq_array,
```

### Comparing `seqchromloader-0.6.4/seqchromloader/writer.py` & `seqchromloader-0.6.5/seqchromloader/writer.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.4/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.6.5/seqchromloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.4
+Version: 0.6.5
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.4/setup.py` & `seqchromloader-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.6.4",
+    version="0.6.5",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.6.4/tests/test_writer_loader.py` & `seqchromloader-0.6.5/tests/test_writer_loader.py`

 * *Files identical despite different names*

