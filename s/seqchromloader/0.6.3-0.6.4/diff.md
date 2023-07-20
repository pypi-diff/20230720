# Comparing `tmp/seqchromloader-0.6.3.tar.gz` & `tmp/seqchromloader-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.6.3.tar", last modified: Tue Jul 11 18:48:50 2023, max compression
+gzip compressed data, was "seqchromloader-0.6.4.tar", last modified: Thu Jul 20 18:01:22 2023, max compression
```

## Comparing `seqchromloader-0.6.3.tar` & `seqchromloader-0.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.367218 seqchromloader-0.6.3/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-11 18:48:50.366933 seqchromloader-0.6.3/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.3/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.347955 seqchromloader-0.6.3/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.3/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.3/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14864 2023-07-11 18:46:36.000000 seqchromloader-0.6.3/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.3/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.365960 seqchromloader-0.6.3/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-07-11 18:48:50.000000 seqchromloader-0.6.3/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-07-11 18:48:50.367296 seqchromloader-0.6.3/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-07-11 18:47:48.000000 seqchromloader-0.6.3/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-11 18:48:50.366497 seqchromloader-0.6.3/tests/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13030 2023-06-22 19:52:40.000000 seqchromloader-0.6.3/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.768117 seqchromloader-0.6.4/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 18:01:22.767476 seqchromloader-0.6.4/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.4/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.746480 seqchromloader-0.6.4/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.4/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12749 2023-06-22 19:45:04.000000 seqchromloader-0.6.4/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14888 2023-07-20 17:54:13.000000 seqchromloader-0.6.4/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7355 2023-07-20 17:56:20.000000 seqchromloader-0.6.4/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.759014 seqchromloader-0.6.4/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-07-20 18:01:22.000000 seqchromloader-0.6.4/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-07-20 18:01:22.768308 seqchromloader-0.6.4/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-07-20 17:39:28.000000 seqchromloader-0.6.4/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-07-20 18:01:22.766298 seqchromloader-0.6.4/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    13756 2023-07-20 17:50:28.000000 seqchromloader-0.6.4/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.6.3/PKG-INFO` & `seqchromloader-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.3
+Version: 0.6.4
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.3/README.md` & `seqchromloader-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.3/seqchromloader/loader.py` & `seqchromloader-0.6.4/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.3/seqchromloader/utils.py` & `seqchromloader-0.6.4/seqchromloader/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,25 +366,25 @@
             if strand=="-":
                 target_array = target_array[::-1]
         except RuntimeError as e:
             logging.warning(e)
             logging.warning(f"RuntimeError happened when accessing {chrom}:{start}-{end}, it's probably due to at least one chromatin track bigwig doesn't have information in this region")
             raise BigWigInaccessible(chrom, start, end)
     else:
-        target_array = None
+        target_array = np.array([None])
     return target_array
 
 def extract_info(chrom, start, end, label, genome_pyfaidx, bigwigs, target, strand="+", transforms:dict=None):
     seq_array = extract_dnaOneHot(chrom, start, end, strand, genome_pyfaidx)
 
     #chromatin track
     if bigwigs is not None and len(bigwigs)>0:
         chroms_array = extract_bw(chrom, start, end, strand, bigwigs)
     else:
-        chroms_array = None
+        chroms_array = np.array([None])
     # label
     label_array = np.array(label, dtype=np.int32)[np.newaxis]
     # counts
     target_array = extract_target(chrom, start, end, strand, target)
 
     feature = {
         'seq': seq_array,
```

### Comparing `seqchromloader-0.6.3/seqchromloader/writer.py` & `seqchromloader-0.6.4/seqchromloader/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,24 +121,24 @@
         return os.path.join(outdir, f"{outprefix}_{{{begin}..{end}}}.tar.gz" if compress else f"{outprefix}_{{{begin}..{end}}}.tar")
     else:
         return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
-                                bigwig_files,
+                                bigwig_files=None,
                                 target_bam=None,
                                 target_bw=None,
                                 outdir="dataset/", 
                                 compress=True,
                                 transforms=None,
                                 DALI=False):
     # get handlers
     genome_pyfaidx = pyfaidx.Fasta(fasta)
-    bigwigs = [pyBigWig.open(bw) for bw in bigwig_files]
+    bigwigs = [pyBigWig.open(bw) for bw in bigwig_files] if bigwig_files is not None else None
     if target_bam is not None:
         target = pysam.AlignmentFile(target_bam)
     elif target_bw is not None:
         target = pyBigWig.open(target_bw)
     else:
         target = None
 
@@ -174,10 +174,11 @@
             feature_dict["chrom.npy"] = feature['chrom'].tobytes()
             feature_dict["target.npy"] = feature['target'].tobytes()
             feature_dict["label.npy"] = feature['label'].tobytes()
 
         sink.write(feature_dict)
 
     sink.close()
-    for bw in bigwigs: bw.close()
+    if bigwigs is not None:
+        for bw in bigwigs: bw.close()
 
     return filename
```

### Comparing `seqchromloader-0.6.3/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.6.4/seqchromloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.3
+Version: 0.6.4
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.3/setup.py` & `seqchromloader-0.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.6.3",
+    version="0.6.4",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.6.3/tests/test_writer_loader.py` & `seqchromloader-0.6.4/tests/test_writer_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,15 +154,34 @@
             wds.batched(2)
         )
         seq, chrom, target, label = next(iter(ds))
         self.assertEqual(seq[1,0,4].item(), 1.0)
         self.assertEqual(chrom[0,0,3].item(), 999.0)
         self.assertEqual(target[0].item(), 999.0)
         self.assertEqual(label[1].item(), 1)
-        
+
+    def test_write_chrom_target_none(self):
+        coords = pd.DataFrame({
+            'chrom': ["chr19", "chr19"],
+            'start': [0, 3],
+            'end': [5, 8],
+            'label': [0, 1],
+            'score': [".", "."],
+            'strand': ["+", "+"]
+        })
+        huge_coords = pd.concat([coords] * 5000, axis=0).reset_index()
+        dump_data_webdataset(huge_coords, 
+                    genome_fasta='data/sample.fa', 
+                    bigwig_filelist=None,
+                    outdir=self.tempdir,
+                    outprefix='test_target_none',
+                    compress=True,
+                    numProcessors=2)
+        self.assertIsFile(os.path.join(self.tempdir, "test_target_none_0.tar.gz"))
+
     def test_wds_loader(self):
         it = iter(SeqChromDatasetByWds(["data/test_0.tar.gz"], dataloader_kws={"batch_size":3}))
         seq, chrom, target, label = next(it)
 
         self.assertEqual(seq[0,0,3].item(), 1.0)
         self.assertEqual(chrom[0,0,3].item(), 4.0)
         self.assertEqual(target[0].item(), 0.0)
```

