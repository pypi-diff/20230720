# Comparing `tmp/seqdata-0.1.1.tar.gz` & `tmp/seqdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqdata-0.1.1.tar", max compression
+gzip compressed data, was "seqdata-0.1.2.tar", max compression
```

## Comparing `seqdata-0.1.1.tar` & `seqdata-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      861 2023-06-23 20:14:19.000000 seqdata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1355 2023-06-23 18:57:24.000000 seqdata-0.1.1/seqdata/__init__.py
--rw-r--r--   0        0        0     2412 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/_dataload/_SequenceDataset.py
--rw-r--r--   0        0        0      981 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/_deprecated.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.1.1/seqdata/_io/__init__.py
--rw-r--r--   0        0        0    10816 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/bed_ops.py
--rw-r--r--   0        0        0     4943 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/read.py
--rw-r--r--   0        0        0      206 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/__init__.py
--rw-r--r--   0        0        0    11173 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/bam.py
--rw-r--r--   0        0        0    10022 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/fasta.py
--rw-r--r--   0        0        0     6152 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/readers/table.py
--rw-r--r--   0        0        0    13505 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/vcf.py
--rw-r--r--   0        0        0     9706 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/wig.py
--rw-r--r--   0        0        0     2705 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/utils.py
--rw-r--r--   0        0        0     9375 2023-06-21 22:49:16.000000 seqdata-0.1.1/seqdata/torch.py
--rw-r--r--   0        0        0     2281 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/types.py
--rw-r--r--   0        0        0    12620 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/xarray/seqdata.py
--rw-r--r--   0        0        0      901 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/xarray/utils.py
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 seqdata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1463 2023-07-20 19:56:15.000000 seqdata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1355 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_deprecated.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.1.2/seqdata/_io/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-18 16:37:11.000000 seqdata-0.1.2/seqdata/_io/bed_ops.py
+-rw-r--r--   0        0        0    14002 2023-07-18 16:22:45.000000 seqdata-0.1.2/seqdata/_io/read.py
+-rw-r--r--   0        0        0      206 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/__init__.py
+-rw-r--r--   0        0        0    11173 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/bam.py
+-rw-r--r--   0        0        0    10022 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/fasta.py
+-rw-r--r--   0        0        0     6152 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/table.py
+-rw-r--r--   0        0        0    13505 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/vcf.py
+-rw-r--r--   0        0        0     9706 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/_io/readers/wig.py
+-rw-r--r--   0        0        0    22161 2023-07-17 22:57:09.000000 seqdata-0.1.2/seqdata/_io/readers.py
+-rw-r--r--   0        0        0     2705 2023-07-17 22:58:07.000000 seqdata-0.1.2/seqdata/_io/utils.py
+-rw-r--r--   0        0        0     9375 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/torch.py
+-rw-r--r--   0        0        0     2281 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/types.py
+-rw-r--r--   0        0        0    15925 2023-07-18 16:36:35.000000 seqdata-0.1.2/seqdata/xarray/seqdata.py
+-rw-r--r--   0        0        0      901 2023-07-17 22:57:20.000000 seqdata-0.1.2/seqdata/xarray/utils.py
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 seqdata-0.1.2/PKG-INFO
```

### Comparing `seqdata-0.1.1/seqdata/__init__.py` & `seqdata-0.1.2/seqdata/__init__.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_deprecated.py` & `seqdata-0.1.2/seqdata/_deprecated.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/bed_ops.py` & `seqdata-0.1.2/seqdata/_io/bed_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 def add_bed_to_sdata(
     sdata: xr.Dataset,
     bed: pd.DataFrame,
     col_prefix: Optional[str] = None,
     sequence_dim: Optional[str] = None,
 ):
+    """Add a BED-like DataFrame to a Dataset."""
     if col_prefix is not None:
         bed.columns = [col_prefix + c for c in bed.columns]
     if sequence_dim is not None:
         bed.index.name = sequence_dim
     return sdata.merge(bed.to_xarray())
```

### Comparing `seqdata-0.1.1/seqdata/_io/readers/bam.py` & `seqdata-0.1.2/seqdata/_io/readers/bam.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/readers/fasta.py` & `seqdata-0.1.2/seqdata/_io/readers/fasta.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/readers/table.py` & `seqdata-0.1.2/seqdata/_io/readers/table.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/readers/vcf.py` & `seqdata-0.1.2/seqdata/_io/readers/vcf.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/readers/wig.py` & `seqdata-0.1.2/seqdata/_io/readers/wig.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/_io/utils.py` & `seqdata-0.1.2/seqdata/_io/utils.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/torch.py` & `seqdata-0.1.2/seqdata/torch.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/types.py` & `seqdata-0.1.2/seqdata/types.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/seqdata/xarray/seqdata.py` & `seqdata-0.1.2/seqdata/xarray/seqdata.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,14 +50,58 @@
     chunk_store: Optional[Union[MutableMapping, PathType]] = None,
     storage_options: Optional[Dict[str, str]] = None,
     decode_timedelta: Optional[bool] = None,
     use_cftime: Optional[bool] = None,
     zarr_version: Optional[int] = None,
     **kwargs,
 ):
+    """Open a SeqData object from disk.
+
+    Parameters
+    ----------
+    store : str, Path
+        Path to the SeqData object.
+    group : str, optional
+        Name of the group to open, by default None
+    synchronizer : None, optional
+        Synchronizer to use, by default None
+    chunks : {None, True, False, int, dict, tuple}, optional
+        Chunking scheme to use, by default "auto"
+    decode_cf : bool, optional
+        Whether to decode CF conventions, by default True
+    mask_and_scale : bool, optional
+        Whether to mask and scale data, by default False
+    decode_times : bool, optional
+        Whether to decode times, by default True
+    concat_characters : bool, optional
+        Whether to concatenate characters, by default False
+    decode_coords : bool, optional
+        Whether to decode coordinates, by default True
+    drop_variables : {None, str, iterable}, optional
+        Variables to drop, by default None
+    consolidated : bool, optional
+        Whether to consolidate metadata, by default None
+    overwrite_encoded_chunks : bool, optional
+        Whether to overwrite encoded chunks, by default False
+    chunk_store : {None, MutableMapping, str, Path}, optional
+        Chunk store to use, by default None
+    storage_options : dict, optional
+        Storage options to use, by default None
+    decode_timedelta : bool, optional
+        Whether to decode timedeltas, by default None
+    use_cftime : bool, optional
+        Whether to use cftime, by default None
+    zarr_version : int, optional
+        Zarr version to use, by default None
+    
+    Returns
+    -------
+    xr.Dataset
+        SeqData object
+    """
     ds = xr.open_zarr(
         store=store,
         group=group,
         synchronizer=synchronizer,
         chunks=chunks,  # type: ignore
         decode_cf=decode_cf,
         mask_and_scale=mask_and_scale,
@@ -76,28 +120,67 @@
     )
     return ds
 
 
 def to_zarr(
     sdata: xr.Dataset,
     store: PathType,
-    load_first = False,
     chunk_store: Optional[Union[MutableMapping, PathType]] = None,
     mode: Optional[Literal["w", "w-", "a", "r+"]] = None,
     synchronizer: Optional[Any] = None,
     group: Optional[str] = None,
     encoding: Optional[Dict] = None,
     compute=True,
     consolidated: Optional[bool] = None,
     append_dim: Optional[Hashable] = None,
     region: Optional[Dict] = None,
     safe_chunks=True,
     storage_options: Optional[Dict] = None,
     zarr_version: Optional[int] = None,
 ):
+    """Write a xarray object to disk as a Zarr store.
+
+    Makes use of the `to_zarr` method of xarray objects, but modifies 
+    the encoding for cases where the chunking is not uniform.
+
+    Parameters
+    ----------
+    sdata : xr.Dataset
+        SeqData object to write to disk.
+    store : str, Path
+        Path to the SeqData object.
+    chunk_store : {None, MutableMapping, str, Path}, optional
+        Chunk store to use, by default None
+    mode : {None, "w", "w-", "a", "r+"}, optional
+        Mode to use, by default None
+    synchronizer : None, optional
+        Synchronizer to use, by default None
+    group : str, optional
+        Name of the group to open, by default None
+    encoding : dict, optional
+        Encoding to use, by default None
+    compute : bool, optional
+        Whether to compute, by default True
+    consolidated : bool, optional
+        Whether to consolidate metadata, by default None
+    append_dim : {None, str}, optional
+        Name of the append dimension, by default None
+    region : dict, optional
+        Region to use, by default None
+    safe_chunks : bool, optional
+        Whether to use safe chunks, by default True
+    storage_options : dict, optional
+        Storage options to use, by default None
+    zarr_version : int, optional
+        Zarr version to use, by default None
+
+    Returns
+    -------
+    None
+    """
     sdata = sdata.reset_encoding()
 
     for arr in sdata.data_vars.values():
         if "_FillValue" in arr.attrs:
             del arr.attrs["_FillValue"]
 
         # rechunk non-uniform chunking
@@ -138,15 +221,18 @@
     *readers: FlatReader,
     path: PathType,
     fixed_length: bool,
     sequence_dim: Optional[str] = None,
     length_dim: Optional[str] = None,
     overwrite=False,
 ) -> xr.Dataset:
-    """Save a SeqData to disk and open it (without loading it into memory).
+    """Composable function to create a SeqData object from flat files.
+    
+    Saves a SeqData to disk and open it (without loading it into memory).
+    TODO: Tutorials coming soon.
 
     Parameters
     ----------
     path : str, Path
         Path to save this SeqData to.
     fixed_length : bool
         `True`: assume the all sequences have the same length and will infer it
@@ -188,15 +274,18 @@
     bed: Union[PathType, pd.DataFrame],
     max_jitter=0,
     sequence_dim: Optional[str] = None,
     length_dim: Optional[str] = None,
     splice=False,
     overwrite=False,
 ) -> xr.Dataset:
-    """Save a SeqData to disk and open it (without loading it into memory).
+    """Composable function to create a SeqData object from region based files.
+    
+    Saves a SeqData to disk and open it (without loading it into memory).
+    TODO: Tutorials coming soon.
 
     Parameters
     ----------
     path : str, Path
         Path to save this SeqData to.
     fixed_length : int, bool, optional
         `int`: use regions of this length centered around those in the BED file.
@@ -335,14 +424,15 @@
     sdata: xr.Dataset,
     obs: Union[xr.Dataset, pd.DataFrame],
     on: Optional[str] = None,
     left_on: Optional[str] = None,
     right_on: Optional[str] = None,
     how: Literal["inner", "left", "right", "outer", "exact"] = "inner",
 ):
+    """Merge observations into a SeqData object along sequence axis."""
     if on is None and (left_on is None or right_on is None):
         raise ValueError
     if on is not None and (left_on is not None or right_on is not None):
         raise ValueError
 
     if on is None:
         assert left_on is not None
```

### Comparing `seqdata-0.1.1/seqdata/xarray/utils.py` & `seqdata-0.1.2/seqdata/xarray/utils.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.1/PKG-INFO` & `seqdata-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: seqdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Annotated sequence data
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
 Provides-Extra: torch
+Requires-Dist: Sphinx[docs] (>=6.2.1,<7.0.0) ; extra == "docs"
 Requires-Dist: cyvcf2 (>=0.30.18,<0.31.0)
 Requires-Dist: dask (>=2023.3.2,<2024.0.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: myst-parser[docs] (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
+Requires-Dist: nbsphinx[docs] (>=0.9.2,<0.10.0) ; extra == "docs"
 Requires-Dist: numcodecs (>=0.11.0,<0.12.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pandera (>=0.14.5,<0.15.0)
+Requires-Dist: pandoc[docs] (>=2.3,<3.0) ; extra == "docs"
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyBigWig (>=0.3.22,<0.4.0)
 Requires-Dist: pybedtools (>=0.9.0,<0.10.0)
 Requires-Dist: pyranges (>=0.0.120,<0.0.121)
 Requires-Dist: pysam (>=0.21.0,<0.22.0)
-Requires-Dist: seqpro (==0.1.1)
-Requires-Dist: torch[torch] (>=1.12.0,<2.0.0) ; extra == "torch"
+Requires-Dist: seqpro (>=0.1.1,<0.2.0)
+Requires-Dist: sphinx-autobuild[docs] (==2021.3.14) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.21.1,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme[docs] (>=1.2.2,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-apidoc[docs] (>=0.3.0,<0.4.0) ; extra == "docs"
+Requires-Dist: torch[torch] (>=1.12.0) ; extra == "torch"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xarray (==2023.4.0)
 Requires-Dist: zarr (>=2.14.2,<3.0.0)
```

