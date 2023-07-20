# Comparing `tmp/recordlinkage-0.8.1-py2.py3-none-any.whl.zip` & `tmp/recordlinkage-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,36 @@
-Zip file size: 887858 bytes, number of entries: 32
--rw-r--r--  2.0 unx      409 b- defN 16-Nov-29 09:54 recordlinkage/__init__.py
--rw-r--r--  2.0 unx      471 b- defN 17-Jan-27 10:52 recordlinkage/_version.py
--rw-r--r--  2.0 unx    21647 b- defN 17-Jan-13 15:34 recordlinkage/classifiers.py
--rw-r--r--  2.0 unx    28202 b- defN 17-Jan-22 16:02 recordlinkage/comparing.py
--rw-r--r--  2.0 unx    16795 b- defN 17-Jan-09 22:10 recordlinkage/indexing.py
--rw-r--r--  2.0 unx     6092 b- defN 17-Jan-09 22:10 recordlinkage/measures.py
+Zip file size: 887307 bytes, number of entries: 34
+-rw-r--r--  2.0 unx      532 b- defN 17-Jun-21 11:14 recordlinkage/__init__.py
+-rw-r--r--  2.0 unx      471 b- defN 17-Jun-21 11:18 recordlinkage/_version.py
+-rw-r--r--  2.0 unx     4667 b- defN 17-Jun-21 11:14 recordlinkage/base.py
+-rw-r--r--  2.0 unx    21647 b- defN 17-Feb-05 19:15 recordlinkage/classifiers.py
+-rw-r--r--  2.0 unx    28202 b- defN 17-Feb-05 17:53 recordlinkage/comparing.py
+-rw-r--r--  2.0 unx    31683 b- defN 17-Jun-21 11:14 recordlinkage/indexing.py
+-rw-r--r--  2.0 unx     7704 b- defN 17-Jun-21 11:14 recordlinkage/measures.py
+-rw-r--r--  2.0 unx     2202 b- defN 17-Jun-21 11:14 recordlinkage/rl_logging.py
 -rw-r--r--  2.0 unx     2438 b- defN 17-Jan-09 22:10 recordlinkage/types.py
--rw-r--r--  2.0 unx     1816 b- defN 17-Jan-21 21:28 recordlinkage/utils.py
+-rw-r--r--  2.0 unx     1033 b- defN 17-Jun-21 11:10 recordlinkage/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Nov-29 09:54 recordlinkage/algorithms/__init__.py
 -rw-r--r--  2.0 unx      469 b- defN 16-Nov-29 09:54 recordlinkage/algorithms/distance.py
 -rw-r--r--  2.0 unx     7123 b- defN 16-Nov-29 09:54 recordlinkage/algorithms/em.py
+-rw-r--r--  2.0 unx     2714 b- defN 17-Jun-21 11:14 recordlinkage/algorithms/indexing.py
 -rw-r--r--  2.0 unx     1996 b- defN 16-Nov-29 09:54 recordlinkage/algorithms/numeric.py
--rw-r--r--  2.0 unx     3911 b- defN 17-Jan-21 21:27 recordlinkage/algorithms/string.py
--rw-r--r--  2.0 unx        0 b- defN 16-Nov-29 09:54 recordlinkage/compat/__init__.py
--rw-r--r--  2.0 unx    30098 b- defN 16-Nov-29 09:54 recordlinkage/compat/six.py
--rw-r--r--  2.0 unx     9115 b- defN 17-Jan-22 20:16 recordlinkage/datasets/__init__.py
--rw-r--r--  2.0 unx     2113 b- defN 17-Jan-12 13:15 recordlinkage/datasets/random.py
+-rw-r--r--  2.0 unx     3911 b- defN 17-Feb-05 17:53 recordlinkage/algorithms/string.py
+-rw-r--r--  2.0 unx       92 b- defN 17-Apr-17 17:12 recordlinkage/datasets/__init__.py
+-rw-r--r--  2.0 unx     9114 b- defN 17-Apr-17 17:12 recordlinkage/datasets/external.py
+-rw-r--r--  2.0 unx     2294 b- defN 17-Apr-17 17:12 recordlinkage/datasets/generate.py
 -rw-r--r--  2.0 unx   102415 b- defN 16-Nov-29 09:54 recordlinkage/datasets/febrl/dataset1.csv
 -rw-r--r--  2.0 unx   514835 b- defN 16-Nov-29 09:54 recordlinkage/datasets/febrl/dataset2.csv
 -rw-r--r--  2.0 unx   514019 b- defN 16-Nov-29 09:54 recordlinkage/datasets/febrl/dataset3.csv
 -rw-r--r--  2.0 unx   519618 b- defN 16-Nov-29 09:54 recordlinkage/datasets/febrl/dataset4a.csv
 -rw-r--r--  2.0 unx   515463 b- defN 16-Nov-29 09:54 recordlinkage/datasets/febrl/dataset4b.csv
 -rw-r--r--  2.0 unx      272 b- defN 16-Nov-29 12:43 recordlinkage/datasets/krebsregister/frequencies.csv
 -rw-r--r--  2.0 unx       98 b- defN 16-Nov-29 09:54 recordlinkage/standardise/__init__.py
--rw-r--r--  2.0 unx     4498 b- defN 17-Jan-13 15:34 recordlinkage/standardise/cleaning.py
--rw-r--r--  2.0 unx     2335 b- defN 17-Jan-21 21:27 recordlinkage/standardise/encoding.py
--rw-r--r--  2.0 unx     5637 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      656 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/metadata.json
--rw-r--r--  2.0 unx       14 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     6108 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx     2904 b- defN 17-Jan-27 10:52 recordlinkage-0.8.1.dist-info/RECORD
-32 files, 2321677 bytes uncompressed, 883196 bytes compressed:  62.0%
+-rw-r--r--  2.0 unx     4498 b- defN 17-Feb-05 17:53 recordlinkage/standardise/cleaning.py
+-rw-r--r--  2.0 unx     2335 b- defN 17-Feb-05 17:53 recordlinkage/standardise/encoding.py
+-rw-r--r--  2.0 unx     5795 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      656 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/metadata.json
+-rw-r--r--  2.0 unx       14 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      110 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     6266 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     3081 b- defN 17-Jun-21 11:18 recordlinkage-0.9.0.dist-info/RECORD
+34 files, 2317767 bytes uncompressed, 882371 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: recordlinkage/__init__.py
 Comment: 
 
 Filename: recordlinkage/_version.py
 Comment: 
 
+Filename: recordlinkage/base.py
+Comment: 
+
 Filename: recordlinkage/classifiers.py
 Comment: 
 
 Filename: recordlinkage/comparing.py
 Comment: 
 
 Filename: recordlinkage/indexing.py
 Comment: 
 
 Filename: recordlinkage/measures.py
 Comment: 
 
+Filename: recordlinkage/rl_logging.py
+Comment: 
+
 Filename: recordlinkage/types.py
 Comment: 
 
 Filename: recordlinkage/utils.py
 Comment: 
 
 Filename: recordlinkage/algorithms/__init__.py
@@ -27,30 +33,30 @@
 
 Filename: recordlinkage/algorithms/distance.py
 Comment: 
 
 Filename: recordlinkage/algorithms/em.py
 Comment: 
 
-Filename: recordlinkage/algorithms/numeric.py
+Filename: recordlinkage/algorithms/indexing.py
 Comment: 
 
-Filename: recordlinkage/algorithms/string.py
+Filename: recordlinkage/algorithms/numeric.py
 Comment: 
 
-Filename: recordlinkage/compat/__init__.py
+Filename: recordlinkage/algorithms/string.py
 Comment: 
 
-Filename: recordlinkage/compat/six.py
+Filename: recordlinkage/datasets/__init__.py
 Comment: 
 
-Filename: recordlinkage/datasets/__init__.py
+Filename: recordlinkage/datasets/external.py
 Comment: 
 
-Filename: recordlinkage/datasets/random.py
+Filename: recordlinkage/datasets/generate.py
 Comment: 
 
 Filename: recordlinkage/datasets/febrl/dataset1.csv
 Comment: 
 
 Filename: recordlinkage/datasets/febrl/dataset2.csv
 Comment: 
@@ -72,26 +78,26 @@
 
 Filename: recordlinkage/standardise/cleaning.py
 Comment: 
 
 Filename: recordlinkage/standardise/encoding.py
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/DESCRIPTION.rst
+Filename: recordlinkage-0.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/metadata.json
+Filename: recordlinkage-0.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/top_level.txt
+Filename: recordlinkage-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/WHEEL
+Filename: recordlinkage-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/METADATA
+Filename: recordlinkage-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: recordlinkage-0.8.1.dist-info/RECORD
+Filename: recordlinkage-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## recordlinkage/__init__.py

```diff
@@ -1,13 +1,17 @@
 
+# pylint: disable=wildcard-import,g-bad-import-order,g-import-not-at-top
+
 from recordlinkage.indexing import *
 from recordlinkage.comparing import *
 from recordlinkage.classifiers import *
 from recordlinkage.measures import *
 
+from recordlinkage import rl_logging as logging
+
 # # import standardise
 # from recordlinkage.standardise.cleaning import *
 # from recordlinkage.standardise.encoding import *
 
 from recordlinkage._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
```

## recordlinkage/_version.py

```diff
@@ -7,15 +7,15 @@
 import json
 import sys
 
 version_json = '''
 {
  "dirty": false,
  "error": null,
- "full-revisionid": "d8c92f6bfdaa8e48b67221eeda298c94de4ae2db",
- "version": "0.8.1"
+ "full-revisionid": "2b4d1ac5f148b9569738b9b5a9943166b3fbb798",
+ "version": "0.9.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## recordlinkage/indexing.py

```diff
@@ -1,16 +1,32 @@
 from __future__ import division
 
+import warnings
 from functools import wraps
 
 import pandas
 import numpy
 
-from recordlinkage.utils import IndexError, merge_dicts, max_number_of_pairs
+from recordlinkage.base import BaseIndexator
+from recordlinkage.utils import IndexError
+from recordlinkage.utils import merge_dicts
+from recordlinkage.utils import max_number_of_pairs
 from recordlinkage.algorithms.string import qgram_similarity
+from recordlinkage.utils import listify
+from recordlinkage.measures import reduction_ratio
+from recordlinkage.measures import max_pairs
+from recordlinkage.algorithms.indexing import \
+    random_pairs_with_replacement
+from recordlinkage.algorithms.indexing import \
+    random_pairs_without_replacement_small_frames
+from recordlinkage.algorithms.indexing import \
+    random_pairs_without_replacement_large_frames
+
+from recordlinkage import rl_logging as logging
+
 
 
 def check_index_names(func):
     # decorator to prevent index name conflicts. Used in functions like
     # blocking and SNI. Also useful for user defined functions.
 
     @wraps(func)
@@ -179,15 +195,16 @@
 @check_index_names
 def _sortedneighbourhood(
         df_a, df_b, column, window=3, sorting_key_values=None,
         block_on=[], block_left_on=[], block_right_on=[]):
 
     # Check if window is an odd number
     if not isinstance(window, int) or (window < 0) or not bool(window % 2):
-        raise ValueError('The given window length is not a positive and odd integer.')
+        raise ValueError(
+            'The given window length is not a positive and odd integer.')
 
     block_on = [block_on] if type(block_on) != list else block_on
     block_left_on = [block_left_on] if type(
         block_left_on) != list else block_left_on
     block_right_on = [block_right_on] if type(
         block_right_on) != list else block_right_on
 
@@ -208,23 +225,23 @@
         ))
 
     sorting_key_factors = numpy.arange(len(sorting_key_values))
 
     data_dict_A = {kl: df_a[kl] for kl in keys_left}
     data_dict_B = {kl: df_b[kl] for kl in keys_right}
 
+    sorted_index = pandas.Series(
+        index=sorting_key_values, data=sorting_key_factors)
     sorted_df_A = pandas.DataFrame(
         merge_dicts(
             data_dict_A,
-            {column: df_a[column].replace(
-                sorting_key_values, sorting_key_factors),
+            {column: df_a[column].map(sorted_index),
              df_a.index.name: df_a.index.values}))
     sorted_df_B = pandas.DataFrame(
-        {column: df_b[column].replace(
-            sorting_key_values, sorting_key_factors),
+        {column: df_b[column].map(sorted_index),
             df_b.index.name: df_b.index.values})
 
     pairs_concat = None
 
     # Internal window size
     _window = int((window - 1) / 2)
 
@@ -282,14 +299,19 @@
 class PairsCore(object):
     """Core class for making record pairs.
 
     """
 
     def __init__(self, df_a, df_b=None, chunks=None, verify_integrity=True):
 
+        warnings.warn(
+            "indexing api changed, see the documentation for the new format",
+            DeprecationWarning
+        )
+
         self.df_a = df_a
         self.df_b = df_b
         self.chunks = chunks
 
         self.deduplication = True if df_b is None else False
 
         if verify_integrity:
@@ -575,7 +597,425 @@
 
         return self.index(_eye)
 
     @property
     def reduction(self):
 
         return 1 - self.n_pairs / self.maximum_number_of_pairs
+
+
+##############################################################################
+#
+# This section contains the indexing classes for the new indexing API.
+#
+
+
+class FullIndex(BaseIndexator):
+    """FullIndex()
+    Class to generate a 'full' index.
+
+    A full index is an index with all possible combinations of record pairs.
+    In case of linking, this indexation method generates the cartesian product
+    of both DataFrame's. In case of deduplicating DataFrame A, this indexation
+    method are the pairs defined by the upper triangular matrix of the A x A.
+
+    Note
+    ----
+    This indexation method can be slow for large DataFrame's. The number of
+    comparisons scales quadratic.
+    Also, not all classifiers work well with large numbers of record pairs
+    were most of the pairs are distinct.
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        super(FullIndex, self).__init__(*args, **kwargs)
+
+    def _link_index(self, df_a, df_b):
+
+        n_max = max_pairs((df_a, df_b))
+
+        if n_max > 1e7:
+            logging.warn(
+                "The number of record pairs is large. Consider a different "
+                "indexation algorithm for better performance. "
+            )
+
+        return pandas.MultiIndex.from_product(
+            [df_a.index.values, df_b.index.values],
+            names=[df_a.index.name, df_b.index.name]
+        )
+
+    def _dedup_index(self, df_a):
+
+        n_max = max_pairs((df_a))
+
+        if n_max > 1e7:
+            logging.warn(
+                "The number of record pairs is large. Consider a different "
+                "indexation algorithm for better performance. "
+            )
+
+        levels = [df_a.index.values, df_a.index.values]
+        labels = numpy.triu_indices(len(df_a.index), k=1)
+        names = [df_a.index.name, df_a.index.name]
+
+        return pandas.MultiIndex(
+            levels=levels,
+            labels=labels,
+            names=names,
+            verify_integrity=False
+        )
+
+
+class BlockIndex(BaseIndexator):
+    """BlockIndex(on=None, left_on=None, right_on=None)
+    Make candidate record pairs that agree on one or more variables.
+
+    Returns all record pairs that agree on the given variable(s). This method
+    is known as *blocking*. Blocking is an effective way to make a subset of
+    the record space (A * B).
+
+    Parameters
+    ----------
+    on : label, optional
+        A column name or a list of column names. These columns are used to
+        block on.
+    left_on : label, optional
+        A column name or a list of column names of dataframe A. These
+        columns are used to block on. This argument is ignored when argument
+        'on' is given.
+    right_on : label, optional
+        A column name or a list of column names of dataframe B. These
+        columns are used to block on. This argument is ignored when argument
+        'on' is given.
+
+    Examples
+    --------
+    In the following example, the record pairs are made for two historical
+    datasets with census data. The datasets are named ``census_data_1980``
+    and ``census_data_1990``.
+
+    >>> indexer = recordlinkage.BlockIndex(on='first_name')
+    >>> indexer.index(census_data_1980, census_data_1990)
+
+    """
+
+    def __init__(self, on=None, left_on=None, right_on=None,
+                 *args, **kwargs):
+        super(BlockIndex, self).__init__(*args, **kwargs)
+
+        # variables to block on
+        self.on = on
+        self.left_on = left_on
+        self.right_on = right_on
+
+    def _link_index(self, df_a, df_b):
+        # Index name conflicts do not occur. They are handled in the
+        # decorator.
+
+        left_on = listify(self.left_on)
+        right_on = listify(self.right_on)
+
+        if self.on:
+            left_on, right_on = listify(self.on), listify(self.on)
+
+        if not left_on or not right_on:
+            raise ValueError("no column labels given")
+
+        if len(left_on) != len(right_on):
+            raise ValueError(
+                "length of left and right keys needs to be the same"
+            )
+
+        blocking_keys = ["blocking_key_%d" % i for i, v in enumerate(left_on)]
+
+        # make a dataset for the data on the left
+        data_left = df_a[left_on].dropna(axis=0, how='any', inplace=False)
+        data_left.columns = blocking_keys
+        data_left['index_x'] = data_left.index
+
+        # make a dataset for the data on the right
+        data_right = df_b[right_on].dropna(axis=0, how='any', inplace=False)
+        data_right.columns = blocking_keys
+        data_right['index_y'] = data_right.index
+
+        # merge the dataframes
+        pairs = data_left.merge(
+            data_right, how='inner', on=blocking_keys
+        ).set_index(['index_x', 'index_y'])
+
+        return pairs.index.rename([df_a.index.name, df_b.index.name])
+
+
+class SortedNeighbourhoodIndex(BaseIndexator):
+    """SortedNeighbourhoodIndex(on=None, left_on=None, right_on=None, window=3, sorting_key_values=None, block_on=[], block_left_on=[], block_right_on=[])
+    Make candidate record pairs with the SortedNeighbourhood algorithm.
+
+    This algorithm returns record pairs that agree on the sorting key, but
+    also records pairs in their neighbourhood. A large window size results in
+    more record pairs. A window size of 1 returns the blocking index.
+
+    The Sorted Neighbourhood Index method is a great method when there is
+    relatively large amount of spelling mistakes. Blocking will fail in that
+    situation because it excludes to many records on minor spelling mistakes.
+
+    Parameters
+    ----------
+    on: label
+        Specify the on to make a sorted index
+    window: int, optional
+        The width of the window, default is 3
+    sorting_key_values: array, optional
+        A list of sorting key values (optional).
+    block_on: label
+        Additional columns to use standard blocking on
+    block_left_on: label
+        Additional columns of the left dataframe to use standard blocking
+        on.
+    block_right_on: label
+        Additional columns of the right dataframe to use standard
+        blocking on
+
+
+    Examples
+    --------
+    In the following example, the record pairs are made for two historical
+    datasets with census data. The datasets are named ``census_data_1980``
+    and ``census_data_1990``.
+
+    >>> indexer = recordlinkage.SortedNeighbourhoodIndex(on='first_name', w=9)
+    >>> indexer.index(census_data_1980, census_data_1990)
+
+    """
+
+    def __init__(self, on=None, left_on=None, right_on=None, window=3,
+                 sorting_key_values=None, block_on=[], block_left_on=[],
+                 block_right_on=[], *args, **kwargs):
+        super(SortedNeighbourhoodIndex, self).__init__(*args, **kwargs)
+
+        # variables to block on
+        self.on = on
+        self.left_on = left_on
+        self.right_on = right_on
+        self.window = window
+        self.sorting_key_values = sorting_key_values
+        self.block_on = block_on
+        self.block_left_on = block_left_on
+        self.block_right_on = block_right_on
+
+    def _get_sorting_key_values(self, array1, array2):
+        """return the sorting key values as a series"""
+
+        concat_arrays = numpy.concatenate([array1, array2])
+        unique_values = numpy.unique(concat_arrays)
+
+        return numpy.sort(unique_values)
+
+    def _link_index(self, df_a, df_b):
+
+        # Index name conflicts do not occur. They are handled in the
+        # decorator.
+
+        left_on = listify(self.left_on)
+        right_on = listify(self.right_on)
+
+        if self.on:
+            left_on = listify(self.on)
+            right_on = listify(self.on)
+
+        if not left_on or not right_on:
+            raise ValueError("no column labels given")
+
+        if len(left_on) != len(right_on):
+            raise ValueError(
+                "length of left and right keys needs to be the same"
+            )
+
+        window = self.window
+
+        # Check if window is an odd number
+        if not isinstance(window, int) or (window < 0) or not bool(window % 2):
+            raise ValueError(
+                'window is not a positive and odd integer')
+
+        # # sorting key is single column
+        # if isinstance(self.on, (tuple, list, dict)):
+        #     raise ValueError(
+        #         "sorting key is not a label")
+
+        # make blocking keys correct
+
+        block_left_on = listify(self.block_left_on)
+        block_right_on = listify(self.block_right_on)
+
+        if self.block_on:
+            block_left_on = listify(self.block_on)
+            block_right_on = listify(self.block_on)
+
+        # drop missing values and columns without relevant information
+        data_left = df_a[listify(left_on) + block_left_on].dropna(
+            axis=0, how='any', inplace=False
+        )
+        data_left.columns = ['sorting_key'] + ["blocking_key_%d" %
+                                               i for i, v in enumerate(block_left_on)]
+        data_left['index_x'] = data_left.index
+
+        data_right = df_b[listify(right_on) + block_right_on].dropna(
+            axis=0, how='any', inplace=False
+        )
+        data_right.columns = ['sorting_key'] + ["blocking_key_%d" %
+                                                i for i, v in enumerate(block_right_on)]
+        data_right['index_y'] = data_right.index
+
+        # sorting_key_values is the terminology in Data Matching [Christen,
+        # 2012]
+        if self.sorting_key_values is None:
+
+            self.sorting_key_values = self._get_sorting_key_values(
+                data_left['sorting_key'].values,
+                data_right['sorting_key'].values
+            )
+
+        sorting_key_factors = pandas.Series(
+            numpy.arange(len(self.sorting_key_values)),
+            index=self.sorting_key_values)
+
+        data_left['sorting_key'] = data_left[
+            'sorting_key'].map(sorting_key_factors)
+        data_right['sorting_key'] = data_right[
+            'sorting_key'].map(sorting_key_factors)
+
+        # Internal window size
+        _window = int((window - 1) / 2)
+
+        def merge_lagged(x, y, w):
+            """Merge two dataframes with a lag on in the sorting key."""
+
+            y = y.copy()
+            y['sorting_key'] = y['sorting_key'] + w
+
+            return x.merge(y, how='inner')
+
+        pairs_concat = [merge_lagged(data_left, data_right, w)
+                        for w in range(-_window, _window + 1)]
+
+        pairs = pandas.concat(pairs_concat, axis=0).set_index(
+            ['index_x', 'index_y']
+        ).index.rename([df_a.index.name, df_b.index.name])
+
+        return pairs
+
+
+class RandomIndex(BaseIndexator):
+    """RandomIndex(n, replace=True, random_state=None)
+    Class to generate random pairs of records.
+
+    This class returns random pairs of records with or without replacement.
+    Use the random_state parameter to seed the algorithm and reproduce
+    results. This way to make record pairs is useful for the training of
+    unsupervised learning models for record linkage.
+
+    Parameters
+    ----------
+    n : int
+        The number of record pairs to return. In case replace=False, the
+        integer n should be bounded by 0 < n <= n_max where n_max is the
+        maximum number of pairs possible.
+    replace : bool, optional
+        Whether the sample of record pairs is with or without replacement.
+        Default: True
+    random_state : int or numpy.random.RandomState, optional
+        Seed for the random number generator (if int), or numpy RandomState
+        object.
+
+    """
+
+    def __init__(self, n, replace=True, random_state=None, *args, **kwargs):
+        super(RandomIndex, self).__init__(*args, **kwargs)
+
+        self.n = n
+        self.replace = replace
+        self.random_state = random_state
+
+    def _link_index(self, df_a, df_b):
+
+        shape = (len(df_a), len(df_b))
+        n_max = max_pairs(shape)
+
+        if not isinstance(self.n, int):
+            raise ValueError('n must be an integer')
+
+        # with replacement
+        if self.replace:
+
+            if n_max == 0:
+                raise ValueError(
+                    "one of the dataframes is empty")
+
+            pairs = random_pairs_with_replacement(
+                self.n, shape, self.random_state)
+
+        # without replacement
+        else:
+
+            if self.n <= 0 or self.n > n_max:
+                raise ValueError(
+                    "n must be a integer satisfying 0<n<=%s" % n_max)
+
+            # large dataframes
+            if n_max < 1e6:
+                pairs = random_pairs_without_replacement_small_frames(
+                    self.n, shape, self.random_state)
+            # small dataframes
+            else:
+                pairs = random_pairs_without_replacement_large_frames(
+                    self.n, shape, self.random_state)
+
+        levels = [df_a.index.values, df_b.index.values]
+        labels = pairs
+        names = [df_a.index.name, df_b.index.name]
+
+        return pandas.MultiIndex(
+            levels=levels,
+            labels=labels,
+            names=names,
+            verify_integrity=False
+        )
+
+    def _dedup_index(self, df_a):
+
+        shape = (len(df_a),)
+
+        # with replacement
+        if self.replace:
+            pairs = random_pairs_with_replacement(
+                self.n, shape, self.random_state)
+
+        # without replacement
+        else:
+
+            n_max = max_pairs(shape)
+
+            if not isinstance(self.n, int) or self.n <= 0 or self.n > n_max:
+                raise ValueError(
+                    "n must be a integer satisfying 0<n<=%s" % n_max)
+
+            # large dataframes
+            if n_max < 1e6:
+                pairs = random_pairs_without_replacement_small_frames(
+                    self.n, shape, self.random_state)
+            # small dataframes
+            else:
+                pairs = random_pairs_without_replacement_large_frames(
+                    self.n, shape, self.random_state)
+
+        levels = [df_a.index.values, df_a.index.values]
+        labels = pairs
+        names = [df_a.index.name, df_a.index.name]
+
+        return pandas.MultiIndex(
+            levels=levels,
+            labels=labels,
+            names=names,
+            verify_integrity=False
+        )
```

## recordlinkage/measures.py

```diff
@@ -1,12 +1,82 @@
 # measures.py
 
 from __future__ import division
 
 import numpy
+import pandas
+
+
+def reduction_ratio(n, x):
+    """Compute the reduction ratio.
+
+    The reduction ratio is 1 minus the ratio candidate matches and the maximum
+    number of pairs possible.
+
+    Parameters
+    ----------
+    n: int, pandas.MultiIndex
+        The number of candidate record pairs or the pandas.MultiIndex with
+        record pairs.
+    x: a list of pandas.DataFrame objects
+        The data used to make the candidate record pairs.
+
+    Returns
+    -------
+    float
+        The reduction ratio.
+
+    """
+
+    n_max = max_pairs(x)
+
+    if isinstance(n, pandas.MultiIndex):
+        n = len(n)
+
+    if n > n_max:
+        raise ValueError("n has to be smaller of equal n_max")
+
+    return 1 - n / n_max
+
+
+def recall_score(candidate_links, true_matches):
+
+    return len(true_matches.intersection(candidate_links)) / len(true_matches)
+
+
+def _get_len(x):
+    """Return int or len(x)"""
+
+    return x if isinstance(x, int) else len(x)
+
+
+def _max_pairs_deduplication(x):
+    """Compute the maximum number of record pairs in case of deduplication."""
+
+    return int(x * (x - 1) / 2)
+
+
+def _max_pairs_linkage(x):
+    """Get the maximum number of record pairs in case of linking."""
+    return numpy.prod(x)
+
+
+def max_pairs(shape):
+    """Compute the maximum number of record pairs possible."""
+
+    if not isinstance(shape, (tuple, list)):
+        n = _max_pairs_deduplication(_get_len(shape))
+
+    elif (isinstance(shape, (tuple, list)) and len(shape) == 1):
+        n = _max_pairs_deduplication(_get_len(shape[0]))
+
+    else:
+        n = _max_pairs_linkage([_get_len(xi) for xi in shape])
+
+    return n
 
 
 def true_positives(true_match_index, matches_index):
     """Count the number of True Positives.
 
     Return the number of correctly classified links, also called the number of
     True Positives (TP).
```

## recordlinkage/utils.py

```diff
@@ -1,13 +1,9 @@
-import sys
-
 import numpy
 
-from recordlinkage.types import is_list_like, is_numpy_like
-
 
 # Errors and Exception handlers
 class IndexError(Exception):
     """ Error class for errors related to indexing. """
     pass
 
 # Checks and conversions
@@ -26,62 +22,25 @@
 
 def unique(x):
     """Convert a list in a unique list."""
 
     return list(set(x))
 
 
-def _resample(frame, index, level_i):
-    """
-    Resample a pandas.Series or pandas.DataFrame with one level of a
-    MultiIndex.
-    """
-
-    data = frame.loc[index.get_level_values(level_i)]
-    data.index = index
-
-    return data
-
-
 def merge_dicts(*dict_args):
     '''
     Given any number of dicts, shallow copy and merge into a new dict,
     precedence goes to key value pairs in latter dicts.
     '''
     result = {}
     for dictionary in dict_args:
         result.update(dictionary)
     return result
 
 
-def split_or_pass(v):
-    """
-    Make a tuple of a single value or return the tuple.
-
-    Example
-    -------
-    >>> v1, v2 = split_or_tuple(3)
-    v1 is 3 and v2 and 3
-    >>> v1, v2 = split_or_tuple((3,4))
-    v1 is 3 and v2 and 4
-
-    """
-
-    if isinstance(v, (tuple, list)):
-
-        if len(v) != 2:
-            raise ValueError(
-                'The number of elements in the list of tuple has to be 2. ')
-
-        return tuple(v)
-
-    else:
-        return (v, v)
-
-
 def max_number_of_pairs(*args):
     """Compute the maximum number of pairs."""
 
     if not args:
         raise ValueError('expected at least one dataframe')
 
     if len(args) == 1:
```

## recordlinkage/datasets/__init__.py

```diff
@@ -1,259 +1,2 @@
-
-import os
-import zipfile
-
-import pandas
-
-from six import BytesIO
-from six.moves.urllib.request import urlopen
-
-
-def load_krebsregister(block=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10], missing_values=None, shuffle=True):
-    """Dataset 'Krebsregister'
-
-    This dataset of comparison patterns was obtained in a epidemiological
-    cancer study in Germany. The comparison patterns were created by the
-    Institute for Medical Biostatistics, Epidemiology and Informatics (IMBEI)
-    and the University Medical Center of Johannes Gutenberg University
-    (Mainz, Germany). The dataset is available for research online.
-
-        "The records represent individual data including first and family
-        name, sex, date of birth and postal code, which were collected
-        through iterative insertions in the course of several years. The
-        comparison patterns in this data set are based on a sample of
-        100.000 records dating from 2005 to 2008. Data pairs were
-        classified as "match" or "non-match" during  an extensive manual
-        review where several documentarists were involved.  The resulting
-        classification formed the basis for assessing the quality of the
-        registry's own record linkage procedure.
-
-        In order to limit the amount of patterns a blocking procedure was
-        applied, which selects only record pairs that meet specific
-        agreement conditions. The results of the following six blocking
-        iterations were merged together:
-
-        1. Phonetic equality of first name and family name, equality of date of birth.
-        2. Phonetic equality of first name, equality of day of birth.
-        3. Phonetic equality of first name, equality of month of birth.
-        4. Phonetic equality of first name, equality of year of birth.
-        5. Equality of complete date of birth.
-        6. Phonetic equality of family name, equality of sex.
-
-        This procedure resulted in 5.749.132 record pairs, of which
-        20.931 are matches. The data set is split into 10 blocks of
-        (approximately) equal size and ratio of matches to non-matches."
-
-    Parameters
-    ----------
-    block : int, list
-        An integer or a list with integers between 1 and 10. The blocks are
-        the blocks explained in the description.
-    missing_values : object, int, float
-        The value of the missing values. Default NaN.
-    shuffle : bool
-        Shuffle the record pairs. Default True.
-
-    Returns
-    -------
-    (pandas.DataFrame, pandas.MultiIndex)
-        A data frame with comparison vectors and a multi index with the
-        indices of the matches.
-
-    """
-
-    # If the data is not found, download it.
-    for i in range(1, 11):
-
-        filepath = os.path.join(os.path.dirname(__file__),
-                                'krebsregister', 'block_{}.zip'.format(i))
-
-        if not os.path.exists(filepath):
-            _download_krebsregister()
-            break
-
-    if isinstance(block, (list, tuple)):
-
-        data = pandas.concat([_krebsregister_block(bl) for bl in block])
-    else:
-
-        data = _krebsregister_block(block)
-
-    if shuffle:
-        data = data.sample(frac=1, random_state=535)
-
-    match_index = data.index[data['is_match']]
-    del data['is_match']
-
-    if pandas.notnull(missing_values):
-        data.fillna(missing_values, inplace=True)
-
-    return data, match_index
-
-
-def _download_krebsregister():
-
-    zip_file_url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00210/donation.zip"
-
-    try:
-        print("Start downloading the data.")
-        r = urlopen(zip_file_url).read()
-
-        # unzip the content and put it in the krebsregister folder
-        z = zipfile.ZipFile(BytesIO(r))
-        z.extractall(os.path.join(os.path.dirname(__file__), 'krebsregister'))
-
-        print("Data download succesfull.")
-
-    except Exception as e:
-        print("Issue with downloading the data:", e)
-
-
-def _krebsregister_block(block):
-
-    if block not in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
-        raise ValueError(
-            "Argument 'block' has to be integer in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] or list of integers.")
-
-    fp_i = os.path.join(os.path.dirname(__file__),
-                        'krebsregister', 'block_{}.zip'.format(block))
-
-    data_block = pandas.read_csv(
-        fp_i,
-        index_col=['id_1', 'id_2'],
-        na_values='?',
-        compression='zip')
-
-    data_block.columns = [
-        'cmp_firstname1', 'cmp_firstname2', 'cmp_lastname1', 'cmp_lastname2',
-        'cmp_sex', 'cmp_birthday', 'cmp_birthmonth', 'cmp_birthyear',
-        'cmp_zipcode', 'is_match']
-    data_block.index.names = ['id1', 'id2']
-
-    return data_block
-
-
-def load_febrl1():
-    """FEBRL dataset 1
-
-    The Freely Extensible Biomedical Record Linkage (Febrl) package was
-    distributed with a dataset generator and four datasets generated with the
-    generator. This functions returns the first Febrl dataset as a pandas
-    DataFrame.
-
-            *"This data set contains 1000 records (500 original and 500
-            duplicates, with exactly one duplicate per original record."*
-
-    Returns
-    -------
-    pandas.DataFrame
-        A pandas DataFrame with Febrl dataset1.csv.
-
-    """
-
-    return _load_febrl_data('dataset1.csv')
-
-
-def load_febrl2():
-    """FEBRL dataset 2
-
-    The Freely Extensible Biomedical Record Linkage (Febrl) package was
-    distributed with a dataset generator and four datasets generated with the
-    generator. This functions returns the second Febrl dataset as a pandas
-    DataFrame.
-
-            *"This data set contains 5000 records (4000 originals and 1000
-            duplicates), with a maximum of 5 duplicates based on one original
-            record (and a poisson distribution of duplicate records).
-            Distribution of duplicates:
-            19 originals records have 5 duplicate records
-            47 originals records have 4 duplicate records
-            107 originals records have 3 duplicate records
-            141 originals records have 2 duplicate records
-            114 originals records have 1 duplicate record
-            572 originals records have no duplicate record"*
-
-    Returns
-    -------
-    pandas.DataFrame
-        A pandas DataFrame with Febrl dataset2.csv.
-
-    """
-
-    return _load_febrl_data('dataset2.csv')
-
-
-def load_febrl3():
-    """FEBRL dataset 3
-
-    The Freely Extensible Biomedical Record Linkage (Febrl) package was
-    distributed with a dataset generator and four datasets generated with the
-    generator. This functions returns the third Febrl dataset as a pandas
-    DataFrame.
-
-            *"This data set contains 5000 records (2000 originals and 3000
-            duplicates), with a maximum of 5 duplicates based on one original
-            record (and a Zipf distribution of duplicate records).
-            Distribution of duplicates:
-            168 originals records have 5 duplicate records
-            161 originals records have 4 duplicate records
-            212 originals records have 3 duplicate records
-            256 originals records have 2 duplicate records
-            368 originals records have 1 duplicate record
-            1835 originals records have no duplicate record"*
-
-    Returns
-    -------
-    pandas.DataFrame
-        A pandas DataFrame with Febrl dataset3.csv.
-
-    """
-
-    return _load_febrl_data('dataset3.csv')
-
-
-def load_febrl4():
-    """FEBRL dataset 4
-
-    The Freely Extensible Biomedical Record Linkage (Febrl) package was
-    distributed with a dataset generator and four datasets generated with the
-    generator. This  functions returns the fourth Febrl dataset as a pandas
-    DataFrame.
-
-            *"Generated as one data set with 10000 records (5000 originals and
-            5000  duplicates, with one duplicate per original), the originals
-            have been split from the duplicates, into dataset4a.csv
-            (containing the 5000 original records) and dataset4b.csv
-            (containing the 5000 duplicate records) These two data sets can be
-            used for testing linkage procedures."*
-
-
-    Returns
-    -------
-    (pandas.DataFrame, pandas.DataFrame)
-        A pandas DataFrame with Febrl dataset4a.csv and a pandas dataframe
-        with Febrl dataset4b.csv.
-
-    """
-
-    return _load_febrl_data('dataset4a.csv'), _load_febrl_data('dataset4b.csv')
-
-
-def _load_febrl_data(filename):
-    # Internal function for loading febrl data
-
-    filepath = os.path.join(os.path.dirname(__file__), 'febrl', filename)
-
-    febrl_data = pandas.read_csv(filepath,
-                                 index_col="rec_id",
-                                 sep=",",
-                                 engine='c',
-                                 skipinitialspace=True,
-                                 encoding='utf-8',
-                                 dtype={
-                                     "street_number": object,
-                                     "date_of_birth": object,
-                                     "soc_sec_id": object,
-                                     "postcode": object
-                                 })
-
-    return febrl_data
+from recordlinkage.datasets.external import *
+from recordlinkage.datasets.generate import *
```

## Comparing `recordlinkage/datasets/random.py` & `recordlinkage/datasets/generate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import pandas as pd
 import numpy as np
 
 
-def binary_comparisons(n, n_match, m=[0.9] * 8, u=[0.1] * 8,
-                       random_state=None):
+def binary_vectors(n, n_match, m=[0.9] * 8, u=[0.1] * 8,
+                   random_state=None):
     """Generate random binary comparison vectors
 
-    This function is used to generate random comparison vectors. The outcome
-    of each comparison is restricted to 0 and 1.
+    This function is used to generate random comparison vectors. The result of
+    each comparison is a binary value (0 or 1).
 
     Parameters
     ----------
     n : int
-        The number of comparison vectors.
+        The total number of comparison vectors.
     n_match : int
-        The number of matches.
+        The number of matching record pairs.
     m : list, default [0.9] * 8, optional
-        The probability of an agreeing comparison given the pairs is a match.
+        A list of m probabilities of each partially identifying variable. The
+        m probability is the probability that an identifier in matching
+        record pairs agrees.
     u : list, default [0.9] * 8, optional
-        The probability of an agreeing comparison given the records in the
-        pair do not belong to the same entity.
+        A list of u probabilities of each partially identifying variable. The
+        u probability is the probability that an identifier in non-matching
+        record pairs agrees.
     random_state : int or numpy.random.RandomState, optional
-        Seed for the random number generator (if int), or numpy RandomState
-        object.
+        Seed for the random number generator with an integer or numpy
+        RandomState object.
 
     Returns
     -------
-    dict
-        The dicitionary with your classifier parameters.
+    pandas.DataFrame
+        A dataframe with comparison vectors.
 
 
     """
 
     if len(m) != len(u):
         raise ValueError("the length of 'm' is not equal the length of 'u'")
```

## Comparing `recordlinkage-0.8.1.dist-info/DESCRIPTION.rst` & `recordlinkage-0.9.0.dist-info/DESCRIPTION.rst`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,26 @@
 Load your data into pandas DataFrames. 
 
 .. code:: python
 
     df_a = pandas.DataFrame(YOUR_FIRST_DATASET)
     df_b = pandas.DataFrame(YOUR_SECOND_DATASET)
 
-Comparing all record can be computationally intensive. Therefore, we make
-smart set of candidate links with one of the built-in indexing techniques like
+Comparing all record can be computationally intensive. Therefore, we make 
+set of candidate links with one of the built-in indexing techniques like
 **blocking**. In this example, only pairs of records that agree on the surname
-are included.
+are returned.
 
 .. code:: python
 
-    index = recordlinkage.Pairs(df_a, df_b)
-    candidate_links = index.block('surname')
+    block_class = recordlinkage.BlockIndex('surname')
+    candidate_links = block_class.index(df_a, df_b)
+
+**Older versions of Python Record Linkage Toolkit use a different syntax for
+indexing.** `More info about migrating is found here.<#migrating>`_
 
 For each candidate link, compare the records with one of the
 comparison or similarity algorithms in the Compare class.
 
 .. code:: python
 
     c = recordlinkage.Compare(candidate_links, df_a, df_b)
```

## Comparing `recordlinkage-0.8.1.dist-info/metadata.json` & `recordlinkage-0.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.0'"}*

```diff
@@ -31,9 +31,9 @@
                 "scikit-learn (>=0.17.1)",
                 "scipy (>=0.17.1)",
                 "six (>=1.10.0)"
             ]
         }
     ],
     "summary": "A record linkage toolkit for linking and deduplication",
-    "version": "0.8.1"
+    "version": "0.9.0"
 }
```

## Comparing `recordlinkage-0.8.1.dist-info/METADATA` & `recordlinkage-0.9.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: recordlinkage
-Version: 0.8.1
+Version: 0.9.0
 Summary: A record linkage toolkit for linking and deduplication
 Home-page: http://recordlinkage.readthedocs.io/
 Author: Jonathan de Bruin
 Author-email: jonathandebruinhome@gmail.com
 License: GPL-3.0
 Platform: any
 Requires-Dist: jellyfish (>=0.5.4)
@@ -52,23 +52,26 @@
 Load your data into pandas DataFrames. 
 
 .. code:: python
 
     df_a = pandas.DataFrame(YOUR_FIRST_DATASET)
     df_b = pandas.DataFrame(YOUR_SECOND_DATASET)
 
-Comparing all record can be computationally intensive. Therefore, we make
-smart set of candidate links with one of the built-in indexing techniques like
+Comparing all record can be computationally intensive. Therefore, we make 
+set of candidate links with one of the built-in indexing techniques like
 **blocking**. In this example, only pairs of records that agree on the surname
-are included.
+are returned.
 
 .. code:: python
 
-    index = recordlinkage.Pairs(df_a, df_b)
-    candidate_links = index.block('surname')
+    block_class = recordlinkage.BlockIndex('surname')
+    candidate_links = block_class.index(df_a, df_b)
+
+**Older versions of Python Record Linkage Toolkit use a different syntax for
+indexing.** `More info about migrating is found here.<#migrating>`_
 
 For each candidate link, compare the records with one of the
 comparison or similarity algorithms in the Compare class.
 
 .. code:: python
 
     c = recordlinkage.Compare(candidate_links, df_a, df_b)
```

## Comparing `recordlinkage-0.8.1.dist-info/RECORD` & `recordlinkage-0.9.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-recordlinkage/__init__.py,sha256=ecKtRaYgHn5-4AF_NTFcT9JbBgt8MlMNW7HHS4MKJyQ,409
-recordlinkage/_version.py,sha256=eIIM9cfYh7FBkhghp44KAvrJ_SqhHYI0ImieGZCdv58,471
+recordlinkage/__init__.py,sha256=ruMFPM2qVHhqPmrU9lCJnGTGn1tXA6jZYo3ea_Qj1kI,532
+recordlinkage/_version.py,sha256=Im_LDPXd05rKmTiTM5lHxqROruIdbt9US_iJ3d6EDMk,471
+recordlinkage/base.py,sha256=sza8xKsmixMipHnrwA-gu9LKb0M7eazbxed0AaOOmIQ,4667
 recordlinkage/classifiers.py,sha256=O3kDWQgzjCLdJEue5VfNQDO-3gOYq_-uUe4mB8BImSE,21647
 recordlinkage/comparing.py,sha256=x5w-Efl5gps2r3RZ3Ht-RE5CvMc238cxsM8Tc9pb25c,28202
-recordlinkage/indexing.py,sha256=OZ182liBSeHfn2t5tdpVdlQ-hMJLfIypD_M68jyS6pk,16795
-recordlinkage/measures.py,sha256=JDZ97zmq5sRoA75kjxl25edqQSE7kxYu8GwKDLAJCP4,6092
+recordlinkage/indexing.py,sha256=B80arYcVgIiEd9DmsUoWlF6zugI0sOZa-hcPSN-OkHo,31683
+recordlinkage/measures.py,sha256=OhfJVHZv1BefTpvApLf3EkdSd6LSs4sJTRpu6VB4mec,7704
+recordlinkage/rl_logging.py,sha256=cxoeSiotRtF3TMGP9MNzeNn3qLZeD9It70oTYDO7hZY,2202
 recordlinkage/types.py,sha256=kYfslDsYh0BKCa1xwTBApRKPuBv07eSR3q8o0nWbJRc,2438
-recordlinkage/utils.py,sha256=YpxpvelGFAWwSdrPmp-o0Fh-Nkyrd3HyTau6Iy0xbkw,1816
+recordlinkage/utils.py,sha256=NpHLlRxGGyZFcRSo7pzTOgo5aRmtV_myPuM-8pqAkkM,1033
 recordlinkage/algorithms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 recordlinkage/algorithms/distance.py,sha256=oNEV77eD9FIj6_6l56H4TP7siPZGeEVVPfcIRh7R1kY,469
 recordlinkage/algorithms/em.py,sha256=NdKsv4RSjSEbTWmvL8gxd_0rf1SS7GUU_fdVgmNQIfU,7123
+recordlinkage/algorithms/indexing.py,sha256=99Ob6A5SZfHJR4ERJFY20UTKkHnezIv0VPr3AJjACKc,2714
 recordlinkage/algorithms/numeric.py,sha256=VCMLhE8S15Zr6wqzA90OpM5PzldrpOBiXBiQTO0Axfo,1996
 recordlinkage/algorithms/string.py,sha256=S4x3NyYOrsjSp_4FzIOXS8VMNRwTRLtNt4wSL6jQFso,3911
-recordlinkage/compat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-recordlinkage/compat/six.py,sha256=A6hdJZVjI3t_geebZ9BzUvwRrIXo0lfwzQlM2LcKyas,30098
-recordlinkage/datasets/__init__.py,sha256=iqDJectdrzM_SFFoa4Pk6H2pFx6Xr8DmZSayRJjYq30,9115
-recordlinkage/datasets/random.py,sha256=cQZ2Kvonp_bcSTzpUnQvIwGtYgD1w8ucT76Q1_frVJY,2113
+recordlinkage/datasets/__init__.py,sha256=5OGzm6v9dX8OtHbmDYnqXRE4xHlPQo1gSNC671CPjSo,92
+recordlinkage/datasets/external.py,sha256=aBTlsf-B16_J8kKoLsZswFzJJDDoTzOtfpkX3vnyGt8,9114
+recordlinkage/datasets/generate.py,sha256=jieAwLLoitsWA3z1YJUT8bdEx7YgFcBj-2GePgIJ6aI,2294
 recordlinkage/datasets/febrl/dataset1.csv,sha256=Y3rPnbmTp3zEnUecfFO3OadIYV8nKgUP-XPoA4sbnLY,102415
 recordlinkage/datasets/febrl/dataset2.csv,sha256=DIbv4JEHafuxP7jG-gGn7tzZpTqKuJZbKUb4fc18QZU,514835
 recordlinkage/datasets/febrl/dataset3.csv,sha256=DmZzMEWK6I3T1rnKs5r052KaL--YqBDQ6l8V5IIgvb8,514019
 recordlinkage/datasets/febrl/dataset4a.csv,sha256=B8fLPwqNiBgOgDF_KmBJne5OgySkTDgFn05_7QqLRIg,519618
 recordlinkage/datasets/febrl/dataset4b.csv,sha256=Lu12yZ-iI3vj7AE6EjQnkm1BWKvLOo9lh01sfxNYzyw,515463
 recordlinkage/datasets/krebsregister/frequencies.csv,sha256=Ssq8jr2CFInHB-680EdHaGH5bTnbbW_reuRlByKoEbI,272
 recordlinkage/standardise/__init__.py,sha256=hwUYd5AhUUW5JCqmYwPby7137X21DnstCpBLQd4EqQA,98
 recordlinkage/standardise/cleaning.py,sha256=yxV3d6JmwfBcVXnAnF-ZZEKxrpjGCNbRzJ4ln4sspZU,4498
 recordlinkage/standardise/encoding.py,sha256=slcARE88dWRPVITiy937XuyRUeHpAeWwcxMQC0NpN9Y,2335
-recordlinkage-0.8.1.dist-info/DESCRIPTION.rst,sha256=LB7KpcGGK6KXGZjH7lYNQeFEmkG_NTHb1Wdu3vO5Yao,5637
-recordlinkage-0.8.1.dist-info/METADATA,sha256=UJGxFllIujXPnVwn0fZOtvV6bAn-F5htz3sB4eeU1bo,6108
-recordlinkage-0.8.1.dist-info/RECORD,,
-recordlinkage-0.8.1.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
-recordlinkage-0.8.1.dist-info/metadata.json,sha256=myLhNxpNLSqjzSL95jjcnGnQYNf2fhjyTbETg_mhtjI,656
-recordlinkage-0.8.1.dist-info/top_level.txt,sha256=jEXUwwnoL0tD3deiffOINdTjo9xseF_jIOsji-c-joo,14
+recordlinkage-0.9.0.dist-info/DESCRIPTION.rst,sha256=axRHZs2ZWx4NTN0h1V0Jvtvt-hmERRXSaYFOt9L8Arg,5795
+recordlinkage-0.9.0.dist-info/METADATA,sha256=bC2rm3SQRbceRkMaJXtNISw5Z-PbvXIy_j0PW6-0Wqs,6266
+recordlinkage-0.9.0.dist-info/RECORD,,
+recordlinkage-0.9.0.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
+recordlinkage-0.9.0.dist-info/metadata.json,sha256=AhZzQxK9efGi_31AnZDe_-me_fXRS5pg2elRf3J2RUI,656
+recordlinkage-0.9.0.dist-info/top_level.txt,sha256=jEXUwwnoL0tD3deiffOINdTjo9xseF_jIOsji-c-joo,14
```

