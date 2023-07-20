# Comparing `tmp/cdhit-reader-0.1.1.tar.gz` & `tmp/cdhit-reader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdhit-reader-0.1.1.tar", last modified: Fri Nov 25 12:30:03 2022, max compression
+gzip compressed data, was "cdhit-reader-0.2.0.tar", last modified: Thu Jul 20 08:30:22 2023, max compression
```

## Comparing `cdhit-reader-0.1.1.tar` & `cdhit-reader-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 12:30:03.678643 cdhit-reader-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1121 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (122)      126 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2022-11-25 12:30:03.678643 cdhit-reader-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 12:30:03.674643 cdhit-reader-0.1.1/cdhit_reader/
--rwxr-xr-x   0 runner    (1001) docker     (122)      602 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1431 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     6428 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_compare.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4243 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_fasta.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9816 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      479 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_testit.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       64 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 12:30:03.678643 cdhit-reader-0.1.1/cdhit_reader/test/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/test/aa.clstr
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/test/nt.clstr
--rwxr-xr-x   0 runner    (1001) docker     (122)     2850 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/cdhit_reader/test/test_clstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 12:30:03.678643 cdhit-reader-0.1.1/cdhit_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      609 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       87 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 12:30:03.000000 cdhit-reader-0.1.1/cdhit_reader.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (122)      171 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)     1275 2022-11-25 12:30:03.678643 cdhit-reader-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      217 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      411 2022-11-25 12:29:52.000000 cdhit-reader-0.1.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:30:22.872636 cdhit-reader-0.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/LICENSE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-20 08:30:22.872636 cdhit-reader-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:30:22.872636 cdhit-reader-0.2.0/cdhit_reader/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1431 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4243 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_fasta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9875 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_testit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:30:22.872636 cdhit-reader-0.2.0/cdhit_reader/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/test/aa.clstr
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/test/nt.clstr
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2850 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/cdhit_reader/test/test_clstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:30:22.872636 cdhit-reader-0.2.0/cdhit_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:30:22.000000 cdhit-reader-0.2.0/cdhit_reader.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-07-20 08:30:22.876636 cdhit-reader-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      217 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-07-20 08:30:09.000000 cdhit-reader-0.2.0/version.py
```

### Comparing `cdhit-reader-0.1.1/LICENSE.md` & `cdhit-reader-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/PKG-INFO` & `cdhit-reader-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdhit-reader
-Version: 0.1.1
+Version: 0.2.0
 Summary: CD-HIT cluster parser
 Home-page: https://github.com/telatin/cdhit-parser
 Download-URL: https://github.com/telatin/cdhit-parser
 Author: Andrea Telatin
 Author-email: andrea.telatin@gmail.com
 Maintainer: Andrea Telatin
 Maintainer-email: andrea.telatin@gmail.com
@@ -22,22 +22,24 @@
 License-File: LICENSE.md
 
 # cdhit-parser
 
 [![Python package](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml/badge.svg)](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml)
 [![Conda downloads](https://img.shields.io/conda/dn/bioconda/cdhit-reader)](https://anaconda.org/bioconda/cdhit-reader)
 [![pipy](https://img.shields.io/pypi/dm/cdhit-reader?color=blue&label=pipy%20downloads)](https://pypi.org/project/cdhit-reader/)
+![PyPI](https://img.shields.io/pypi/v/cdhit-reader)
 
 CD-HIT file reader.
 
 ## Read CD-HIT .clstr file
 
 Basic usage
 
 ```python
+from cdhit_reader import  read_cdhit
 input = "cluster.fa.clstr"
 for cluster in read_cdhit(input):
     print(f"{cluster.name} refSequence={cluster.refname} size={len(cluster)}")
 
     for member in cluster.sequences:
         print(f" {member.name} ({member.length}) identity={member.identity}% {'(Reference sequence)' if member.is_ref else ''}")
 ```
```

### Comparing `cdhit-reader-0.1.1/README.md` & `cdhit-reader-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # cdhit-parser
 
 [![Python package](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml/badge.svg)](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml)
 [![Conda downloads](https://img.shields.io/conda/dn/bioconda/cdhit-reader)](https://anaconda.org/bioconda/cdhit-reader)
 [![pipy](https://img.shields.io/pypi/dm/cdhit-reader?color=blue&label=pipy%20downloads)](https://pypi.org/project/cdhit-reader/)
+![PyPI](https://img.shields.io/pypi/v/cdhit-reader)
 
 CD-HIT file reader.
 
 ## Read CD-HIT .clstr file
 
 Basic usage
 
 ```python
+from cdhit_reader import  read_cdhit
 input = "cluster.fa.clstr"
 for cluster in read_cdhit(input):
     print(f"{cluster.name} refSequence={cluster.refname} size={len(cluster)}")
 
     for member in cluster.sequences:
         print(f" {member.name} ({member.length}) identity={member.identity}% {'(Reference sequence)' if member.is_ref else ''}")
 ```
@@ -98,8 +100,8 @@
 ## License
 
 This project is licensed under the MIT License.
 
 ## Acknowledgments
 
 This module was based on [fasta_reader](https://github.com/EBI-Metagenomics/fasta-reader-py)
-by [Danilo Horta](https://github.com/horta)
+by [Danilo Horta](https://github.com/horta)
```

### Comparing `cdhit-reader-0.1.1/cdhit_reader/__init__.py` & `cdhit-reader-0.2.0/cdhit_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/_cli.py` & `cdhit-reader-0.2.0/cdhit_reader/_cli.py`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/_compare.py` & `cdhit-reader-0.2.0/cdhit_reader/_compare.py`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/_fasta.py` & `cdhit-reader-0.2.0/cdhit_reader/_fasta.py`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/_reader.py` & `cdhit-reader-0.2.0/cdhit_reader/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,24 @@
         self.id = -1
         self.__parse()
 
     def __parse(self):
         """
         3       502nt, >IKXM6KN01CFAFI... at 1:502:1:503/+/97.81%
         """
-        pattern = re.compile(r'(?P<id>\d+)\s+(?P<size>\d+)(?P<type>aa|nt), >(?P<name>.+?)\.\.\. (?P<attr>.+)')
-        attrpatt = re.compile(r'(?P<ref>\*|at) .*?(?P<strand>[+-]?)\/?(?P<percent>\d+\.\d+)%')
+
+
+        pattern = re.compile(
+            r"(?P<id>\d+)\s+(?P<size>\d+)(?P<type>aa|nt), >(?P<name>.+?)\.\.\. (?P<attr>.+)"
+        )
+        attrpatt = re.compile(         
+            r"(?P<ref>\*|at) .*?(?P<strand>[+-]?)\/?(?P<percent>\d+\.?\d*)%"
+        )
+
+
         match = pattern.search(self.line)
 
         self.seqtype = SeqType.PROTEIN if match["type"] == "aa" else SeqType.NT
         self.strand  = Strand.NONE if self.seqtype == SeqType.PROTEIN else Strand.PLUS
         if match:
             self.name = match["name"]
             self.id = int(match["id"])
@@ -383,8 +391,8 @@
     file
         File path or IO stream.
 
     Returns
     -------
     FASTA reader.
     """
-    return FastaReader(file)
+    return FastaReader(file)
```

### Comparing `cdhit-reader-0.1.1/cdhit_reader/test/aa.clstr` & `cdhit-reader-0.2.0/cdhit_reader/test/aa.clstr`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/test/nt.clstr` & `cdhit-reader-0.2.0/cdhit_reader/test/nt.clstr`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader/test/test_clstr.py` & `cdhit-reader-0.2.0/cdhit_reader/test/test_clstr.py`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/cdhit_reader.egg-info/PKG-INFO` & `cdhit-reader-0.2.0/cdhit_reader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdhit-reader
-Version: 0.1.1
+Version: 0.2.0
 Summary: CD-HIT cluster parser
 Home-page: https://github.com/telatin/cdhit-parser
 Download-URL: https://github.com/telatin/cdhit-parser
 Author: Andrea Telatin
 Author-email: andrea.telatin@gmail.com
 Maintainer: Andrea Telatin
 Maintainer-email: andrea.telatin@gmail.com
@@ -22,22 +22,24 @@
 License-File: LICENSE.md
 
 # cdhit-parser
 
 [![Python package](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml/badge.svg)](https://github.com/telatin/cdhit-parser/actions/workflows/python-package.yml)
 [![Conda downloads](https://img.shields.io/conda/dn/bioconda/cdhit-reader)](https://anaconda.org/bioconda/cdhit-reader)
 [![pipy](https://img.shields.io/pypi/dm/cdhit-reader?color=blue&label=pipy%20downloads)](https://pypi.org/project/cdhit-reader/)
+![PyPI](https://img.shields.io/pypi/v/cdhit-reader)
 
 CD-HIT file reader.
 
 ## Read CD-HIT .clstr file
 
 Basic usage
 
 ```python
+from cdhit_reader import  read_cdhit
 input = "cluster.fa.clstr"
 for cluster in read_cdhit(input):
     print(f"{cluster.name} refSequence={cluster.refname} size={len(cluster)}")
 
     for member in cluster.sequences:
         print(f" {member.name} ({member.length}) identity={member.identity}% {'(Reference sequence)' if member.is_ref else ''}")
 ```
```

### Comparing `cdhit-reader-0.1.1/cdhit_reader.egg-info/SOURCES.txt` & `cdhit-reader-0.2.0/cdhit_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdhit-reader-0.1.1/setup.cfg` & `cdhit-reader-0.2.0/setup.cfg`

 * *Files identical despite different names*

