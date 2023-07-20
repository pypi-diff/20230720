# Comparing `tmp/reach-4.1.0.tar.gz` & `tmp/reach-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reach-4.1.0.tar", last modified: Wed May  3 10:42:23 2023, max compression
+gzip compressed data, was "reach-4.1.1.tar", last modified: Thu Jul 20 09:36:53 2023, max compression
```

## Comparing `reach-4.1.0.tar` & `reach-4.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.660777 reach-4.1.0/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1082 2022-08-10 12:06:48.000000 reach-4.1.0/LICENSE
--rw-r--r--   0 stephantulkens   (501) staff       (20)     7217 2023-05-03 10:42:23.660612 reach-4.1.0/PKG-INFO
--rw-r--r--   0 stephantulkens   (501) staff       (20)     6277 2023-05-03 10:42:20.000000 reach-4.1.0/README.md
--rw-r--r--   0 stephantulkens   (501) staff       (20)      178 2023-04-30 19:03:35.000000 reach-4.1.0/pyproject.toml
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.657779 reach-4.1.0/reach/
--rw-r--r--   0 stephantulkens   (501) staff       (20)      290 2023-05-03 10:42:20.000000 reach-4.1.0/reach/__init__.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     2656 2023-04-30 19:01:37.000000 reach-4.1.0/reach/autoreach.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)    34095 2023-05-03 08:16:28.000000 reach-4.1.0/reach/reach.py
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.658990 reach-4.1.0/reach.egg-info/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     7217 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/PKG-INFO
--rw-r--r--   0 stephantulkens   (501) staff       (20)      365 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/SOURCES.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/dependency_links.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)       33 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/requires.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        6 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/top_level.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-04-30 18:08:45.000000 reach-4.1.0/reach.egg-info/zip-safe
--rw-r--r--   0 stephantulkens   (501) staff       (20)       38 2023-05-03 10:42:23.660819 reach-4.1.0/setup.cfg
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1310 2023-05-03 10:42:20.000000 reach-4.1.0/setup.py
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.660250 reach-4.1.0/tests/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     3292 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_auto.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1860 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_init.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)    10853 2023-05-03 08:12:10.000000 reach-4.1.0/tests/test_io.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     6300 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_similarity.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     5288 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_vectorize.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-07-20 09:36:53.589989 reach-4.1.1/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     1082 2022-08-10 12:06:48.000000 reach-4.1.1/LICENSE
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     7813 2023-07-20 09:36:53.589839 reach-4.1.1/PKG-INFO
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     6772 2023-05-07 17:42:10.000000 reach-4.1.1/README.md
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      178 2023-04-30 19:03:35.000000 reach-4.1.1/pyproject.toml
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-07-20 09:36:53.587690 reach-4.1.1/reach/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      290 2023-07-20 09:35:45.000000 reach-4.1.1/reach/__init__.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     4315 2023-05-14 11:52:31.000000 reach-4.1.1/reach/autoreach.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)    34871 2023-05-14 11:46:22.000000 reach-4.1.1/reach/reach.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-07-20 09:36:53.588986 reach-4.1.1/reach.egg-info/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     7813 2023-07-20 09:36:53.000000 reach-4.1.1/reach.egg-info/PKG-INFO
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      365 2023-07-20 09:36:53.000000 reach-4.1.1/reach.egg-info/SOURCES.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-07-20 09:36:53.000000 reach-4.1.1/reach.egg-info/dependency_links.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)       33 2023-07-20 09:36:53.000000 reach-4.1.1/reach.egg-info/requires.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        6 2023-07-20 09:36:53.000000 reach-4.1.1/reach.egg-info/top_level.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-04-30 18:08:45.000000 reach-4.1.1/reach.egg-info/zip-safe
+-rw-r--r--   0 stephantulkens   (501) staff       (20)       38 2023-07-20 09:36:53.590029 reach-4.1.1/setup.cfg
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     1409 2023-07-20 09:35:45.000000 reach-4.1.1/setup.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-07-20 09:36:53.589631 reach-4.1.1/tests/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     3292 2023-05-03 08:13:38.000000 reach-4.1.1/tests/test_auto.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     3220 2023-05-14 11:45:59.000000 reach-4.1.1/tests/test_init.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)    10853 2023-05-03 08:12:10.000000 reach-4.1.1/tests/test_io.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     6721 2023-05-14 11:47:02.000000 reach-4.1.1/tests/test_similarity.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     5288 2023-05-03 08:13:38.000000 reach-4.1.1/tests/test_vectorize.py
```

### Comparing `reach-4.1.0/LICENSE` & `reach-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reach-4.1.0/PKG-INFO` & `reach-4.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: reach
-Version: 4.1.0
+Version: 4.1.1
 Summary: A light-weight package for working with pre-trained word embeddings
 Home-page: https://github.com/stephantul/reach
 Author: Stéphan Tulkens
 Author-email: stephantul@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/stephantul/reach
 Project-URL: Issue Tracker, https://github.com/stephantul/reach/issues
 Keywords: word vectors,natural language processing,embeddings
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: auto
 License-File: LICENSE
 
 # reach
 
+[![Documentation Status](https://readthedocs.org/projects/reach/badge/?version=latest)](https://reach.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/reach.svg)](https://badge.fury.io/py/reach)
+[![Downloads](https://pepy.tech/badge/reach)](https://pepy.tech/project/reach)
+
 A light-weight package for working with pre-trained word embeddings.
 Useful for input into neural networks, or for doing compositional semantics.
 
 `reach` can read in word vectors in `word2vec` or `glove` format without
 any preprocessing.
 
 The assumption behind `reach` is a no-hassle approach to featurization. The
 vectorization and bow approaches know how to deal with OOV words, removing
 these problems from your code.
 
 `reach` also includes nearest neighbor calculation for arbitrary vectors.
 
-# Installation
+## [Documentation](https://reach.readthedocs.io/en/latest/)
+
+* [API reference](https://reach.readthedocs.io/en/latest/source/api.html)
+* Tutorial coming soon (see below for an example)
+
+## Installation
 
 If you just want `reach`:
 
 ```
 pip install reach
 ```
```

### Comparing `reach-4.1.0/README.md` & `reach-4.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 # reach
 
+[![Documentation Status](https://readthedocs.org/projects/reach/badge/?version=latest)](https://reach.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/reach.svg)](https://badge.fury.io/py/reach)
+[![Downloads](https://pepy.tech/badge/reach)](https://pepy.tech/project/reach)
+
 A light-weight package for working with pre-trained word embeddings.
 Useful for input into neural networks, or for doing compositional semantics.
 
 `reach` can read in word vectors in `word2vec` or `glove` format without
 any preprocessing.
 
 The assumption behind `reach` is a no-hassle approach to featurization. The
 vectorization and bow approaches know how to deal with OOV words, removing
 these problems from your code.
 
 `reach` also includes nearest neighbor calculation for arbitrary vectors.
 
-# Installation
+## [Documentation](https://reach.readthedocs.io/en/latest/)
+
+* [API reference](https://reach.readthedocs.io/en/latest/source/api.html)
+* Tutorial coming soon (see below for an example)
+
+## Installation
 
 If you just want `reach`:
 
 ```
 pip install reach
 ```
```

### Comparing `reach-4.1.0/reach/reach.py` & `reach-4.1.1/reach/reach.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,27 +51,17 @@
         have multiple spaces and want to keep track of them.
     unk_index : int or None, optional, default None
         The index of the UNK item. If this is None, any attempts at vectorizing
         OOV items will throw an error.
 
     Attributes
     ----------
-    items : dict
-        A mapping from items to ids.
-    indices : dict
-        A mapping from ids to items.
-    vectors : numpy array
-        The array representing the vector space.
     unk_index : int
         The integer index of your unknown glyph. This glyph will be inserted
         into your BoW space whenever an unknown item is encountered.
-    norm_vectors : numpy array
-        A normalized version of the vector space.
-    size : int
-        The dimensionality of the vector space.
     name : string
         The name of the Reach instance.
 
     """
 
     def __init__(
         self,
@@ -97,37 +87,43 @@
         self._items: Dict[Hashable, int] = {w: idx for idx, w in enumerate(items)}
         self._indices: Dict[int, Hashable] = {idx: w for w, idx in self.items.items()}
         self.vectors = np.asarray(vectors)
         self.unk_index = unk_index
         self.name = name
 
     def __len__(self) -> int:
+        """The number of the items in the vector space."""
         return len(self.items)
 
     @property
     def items(self) -> Dict[Hashable, int]:
+        """A mapping from item ids to their indices."""
         return self._items
 
     @property
     def indices(self) -> Dict[int, Hashable]:
+        """A mapping from integers to item indices."""
         return self._indices
 
     @property
     def sorted_items(self) -> Tokens:
+        """The items, sorted by index."""
         items: Tokens = [
             item for item, _ in sorted(self.items.items(), key=lambda x: x[1])
         ]
         return items
 
     @property
     def size(self) -> int:
+        """The dimensionality of the vectors"""
         return self.vectors.shape[1]
 
     @property
     def vectors(self) -> np.ndarray:
+        """The vectors themselves"""
         return self._vectors
 
     @vectors.setter
     def vectors(self, x: Matrix) -> None:
         x = np.asarray(x)
         if not np.ndim(x) == 2:
             raise ValueError(f"Your array does not have 2 dimensions: {np.ndim(x)}")
@@ -135,22 +131,39 @@
             raise ValueError(
                 f"Your array does not have the correct length, got {x.shape[0]},"
                 f" expected {len(self.items)}"
             )
         self._vectors = x
         # Make sure norm vectors is updated.
         if hasattr(self, "_norm_vectors"):
-            self._norm_vectors = self.normalize(x)
+            self._norm_vectors = self._normalize_or_copy(x)
 
     @property
     def norm_vectors(self) -> np.ndarray:
+        """
+        Vectors, but normalized to unit length.
+
+        NOTE: when all vectors are unit length, this attribute _is_ vectors.
+        """
         if not hasattr(self, "_norm_vectors"):
-            self._norm_vectors = self.normalize(self.vectors)
+            self._norm_vectors = self._normalize_or_copy(self.vectors)
         return self._norm_vectors
 
+    @staticmethod
+    def _normalize_or_copy(vectors: np.ndarray) -> np.ndarray:
+        """
+        This function returns a copy of vectors if they are unit length.
+        Otherwise, the vectors are normalized, and a new array is returned.
+        """
+        norms = np.linalg.norm(vectors, axis=1)
+        all_unit_length = np.allclose(norms[norms != 0], 1)
+        if all_unit_length:
+            return vectors
+        return Reach.normalize(vectors, norms)
+
     @classmethod
     def load(
         cls,
         vector_file: Union[File, str],
         wordlist: Optional[Tuple[str, ...]] = None,
         num_to_load: Optional[int] = None,
         truncate_embeddings: Optional[int] = None,
@@ -393,21 +406,19 @@
             The list of items to vectorize and then mean pool.
         remove_oov : bool.
             Whether to remove OOV items from the input.
             If this is False, and an unknown item is encountered, then
             the <UNK> symbol will be inserted if it is set. If it is not set,
             then the function will throw a ValueError.
         safeguard : bool.
-            There are a variety of reasons why we can't vectorize a list
-                of tokens:
+            There are a variety of reasons why we can't vectorize a list of tokens:
                 - The list might be empty after removing OOV
                 - We remove OOV but haven't set <UNK>
                 - The list of tokens is empty
-            If safeguard is False, we simply supply a zero vector instead
-                of erroring out.
+            If safeguard is False, we simply supply a zero vector instead of erroring.
 
         Returns
         -------
         vector: np.ndarray
             a vector of the correct size, which is the mean of all tokens
             in the sentence.
 
@@ -432,17 +443,17 @@
         remove_oov : bool.
             Whether to remove OOV items from the input.
             If this is False, and an unknown item is encountered, then
             the <UNK> symbol will be inserted if it is set. If it is not set,
             then the function will throw a ValueError.
         safeguard : bool.
             There are a variety of reasons why we can't vectorize a list of tokens:
-                - The list might be empty after removing OOV
-                - We remove OOV but haven't set <UNK>
-                - The list of tokens is empty
+            - The list might be empty after removing OOV
+            - We remove OOV but haven't set <UNK>
+            - The list of tokens is empty
             If safeguard is False, we simply supply a zero vector instead of erroring.
 
         Returns
         -------
         vector: np.ndarray
             a matrix with number of rows n, where n is the number of input lists, and
             columns s, which is the number of columns of a single vector.
@@ -745,43 +756,50 @@
                 word_index = np.flip(np.argsort(sims_for_word))
                 yield [
                     (self.indices[indices[idx]], sims_for_word[idx])
                     for idx in word_index
                 ]
 
     @staticmethod
-    def normalize(vectors: np.ndarray) -> np.ndarray:
+    def normalize(
+        vectors: np.ndarray, norms: Optional[np.ndarray] = None
+    ) -> np.ndarray:
         """
         Normalize a matrix of row vectors to unit length.
 
         Contains a shortcut if there are no zero vectors in the matrix.
         If there are zero vectors, we do some indexing tricks to avoid
         dividing by 0.
 
         Parameters
         ----------
         vectors : np.array
             The vectors to normalize.
+        norms: np.ndarray
+            Precomputed norms.
 
         Returns
         -------
         vectors : np.array
             The input vectors, normalized to unit length.
 
         """
         if np.ndim(vectors) == 1:
             norm = np.linalg.norm(vectors)
             if norm == 0:
                 return np.zeros_like(vectors)
             return vectors / norm
 
-        vectors = np.copy(vectors)
-        norm = np.linalg.norm(vectors, axis=1)
+        if norms is None:
+            norm = np.linalg.norm(vectors, axis=1)
+        else:
+            norm = norms
 
         if np.any(norm == 0):
+            vectors = np.copy(vectors)
             nonzero = norm > 0
             result = np.zeros_like(vectors)
             n = norm[nonzero]  # type: ignore
             p = vectors[nonzero]
             result[nonzero] = p / n[:, None]
 
             return result
@@ -962,10 +980,10 @@
 
         with open(f"{filename}_vectors.npy", "rb") as file_handle:
             vectors = np.load(file_handle)
         vectors = vectors.astype(desired_dtype)
         return cls(vectors, words, unk_index=unk_index, name=name)
 
 
-def normalize(vectors: np.ndarray) -> np.ndarray:
+def normalize(vectors: np.ndarray, norms: Optional[np.ndarray] = None) -> np.ndarray:
     """Normalize an array to unit length."""
-    return Reach.normalize(vectors)
+    return Reach.normalize(vectors, norms)
```

### Comparing `reach-4.1.0/reach.egg-info/PKG-INFO` & `reach-4.1.1/reach.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: reach
-Version: 4.1.0
+Version: 4.1.1
 Summary: A light-weight package for working with pre-trained word embeddings
 Home-page: https://github.com/stephantul/reach
 Author: Stéphan Tulkens
 Author-email: stephantul@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/stephantul/reach
 Project-URL: Issue Tracker, https://github.com/stephantul/reach/issues
 Keywords: word vectors,natural language processing,embeddings
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: auto
 License-File: LICENSE
 
 # reach
 
+[![Documentation Status](https://readthedocs.org/projects/reach/badge/?version=latest)](https://reach.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/reach.svg)](https://badge.fury.io/py/reach)
+[![Downloads](https://pepy.tech/badge/reach)](https://pepy.tech/project/reach)
+
 A light-weight package for working with pre-trained word embeddings.
 Useful for input into neural networks, or for doing compositional semantics.
 
 `reach` can read in word vectors in `word2vec` or `glove` format without
 any preprocessing.
 
 The assumption behind `reach` is a no-hassle approach to featurization. The
 vectorization and bow approaches know how to deal with OOV words, removing
 these problems from your code.
 
 `reach` also includes nearest neighbor calculation for arbitrary vectors.
 
-# Installation
+## [Documentation](https://reach.readthedocs.io/en/latest/)
+
+* [API reference](https://reach.readthedocs.io/en/latest/source/api.html)
+* Tutorial coming soon (see below for an example)
+
+## Installation
 
 If you just want `reach`:
 
 ```
 pip install reach
 ```
```

### Comparing `reach-4.1.0/setup.py` & `reach-4.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Setup file."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="reach",
-    version="4.1.0",
+    version="4.1.1",
     description="A light-weight package for working with pre-trained word embeddings",
     author="Stéphan Tulkens",
     author_email="stephantul@gmail.com",
     url="https://github.com/stephantul/reach",
     license="MIT",
     packages=find_packages(include=["reach"]),
     install_requires=["numpy", "tqdm"],
@@ -18,17 +18,19 @@
     project_urls={
         "Source Code": "https://github.com/stephantul/reach",
         "Issue Tracker": "https://github.com/stephantul/reach/issues",
     },
     classifiers=[
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords=["word vectors", "natural language processing", "embeddings"],
     zip_safe=True,
     long_description=Path("README.md").read_text(),
```

### Comparing `reach-4.1.0/tests/test_auto.py` & `reach-4.1.1/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `reach-4.1.0/tests/test_init.py` & `reach-4.1.1/tests/test_init.py`

 * *Files 23% similar despite different names*

```diff
@@ -53,7 +53,47 @@
         self.assertEqual(list(instance.sorted_items), words)
 
         with self.assertRaises(AttributeError):
             instance.indices = [0, 1, 2]  # type: ignore
 
         with self.assertRaises(AttributeError):
             instance.items = {"dog": 1}  # type: ignore
+
+    def test_init_vectors_no_norm(self) -> None:
+        words, vectors = self.data()
+        r = Reach(vectors, words)
+
+        self.assertFalse(hasattr(r, "_norm_vectors"))
+        # Initialize norm vectors
+        r.norm_vectors[0]
+        self.assertTrue(hasattr(r, "norm_vectors"))
+        self.assertFalse(r.vectors is r.norm_vectors)
+
+    def test_init_vectors_norm(self) -> None:
+        words, vectors = self.data()
+        vectors = Reach.normalize(vectors)
+
+        r = Reach(vectors, words)
+        self.assertFalse(hasattr(r, "_norm_vectors"))
+        # Initialize norm vectors
+        r.norm_vectors[0]
+        self.assertTrue(hasattr(r, "norm_vectors"))
+        self.assertTrue(r.vectors is r.norm_vectors)
+
+    def test_vectors_auto_norm_no_copy(self) -> None:
+        _, vectors = self.data()
+        result = Reach._normalize_or_copy(vectors)
+
+        self.assertTrue(np.allclose(Reach.normalize(vectors), result))
+
+    def test_vectors_auto_norm_copy(self) -> None:
+        _, vectors = self.data()
+        vectors = Reach.normalize(vectors)
+        result = Reach._normalize_or_copy(vectors)
+
+        self.assertTrue(vectors is result)
+
+    def test_vectors_auto_norm(self) -> None:
+        _, vectors = self.data()
+        result = Reach._normalize_or_copy(vectors)
+
+        self.assertTrue(np.allclose(Reach.normalize(vectors), result))
```

### Comparing `reach-4.1.0/tests/test_io.py` & `reach-4.1.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `reach-4.1.0/tests/test_similarity.py` & `reach-4.1.1/tests/test_similarity.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,22 +32,30 @@
         if norm_x == 0 or norm_y == 0:
             return 0.0
         x = x / norm_x
         y = y / norm_y
 
         return (x * y).sum()
 
-    def test_normalize(self) -> None:
+    def test_normalize_vector(self) -> None:
         x = np.arange(10)
         norm_x = Reach.normalize(x)
         norm_x_np = x / np.linalg.norm(x)
 
         self.assertTrue(np.allclose(norm_x, norm_x_np))
         self.assertTrue(np.allclose(norm_x, normalize(x)))
 
+    def test_normalize_norm(self) -> None:
+        x = np.arange(10)
+        result = Reach.normalize(x)
+        result_2 = Reach.normalize(x, np.linalg.norm(x))
+
+        self.assertTrue(np.allclose(result, result_2))
+
+    def test_normalize_array(self) -> None:
         norms = []
         X = []
         for idx in range(10):
             x = np.full(shape=(10,), fill_value=idx, dtype="float32")
             X.append(x)
             norms.append(normalize(x))
 
@@ -105,14 +113,18 @@
         result = [[x[0] for x in sublist] for sublist in instance.most_similar(words)]
         other_result = []
         for word in words:
             other_result.append([x[0] for x in instance.most_similar([word])[0]])
 
         self.assertEqual(result, other_result)
 
+    def test_batch_single_threshold(self) -> None:
+        words, vectors = self.data()
+        instance = Reach(vectors, words)
+
         result = [
             [x[0] for x in sublist]
             for sublist in instance.threshold(words, threshold=0.0)
         ]
         other_result = []
         for word in words:
             other_result.append(
@@ -154,14 +166,18 @@
         instance = Reach(vectors, words)
 
         for word, vector in zip(words, vectors):
             nn1 = instance.nearest_neighbor(vector)[0][1:]
             nn2 = instance.most_similar([word])[0]
             self.assertEqual(nn1, nn2)
 
+    def test_nearest_neighbor_threshold(self) -> None:
+        words, vectors = self.data()
+        instance = Reach(vectors, words)
+
         threshold = 0.0
         for word, vector in zip(words, vectors):
             nn1 = instance.nearest_neighbor_threshold(vector, threshold=threshold)[0][
                 1:
             ]
             nn2 = instance.threshold([word], threshold=threshold)[0]
             self.assertEqual(nn1, nn2)
@@ -175,10 +191,7 @@
 
         self.assertTrue(np.allclose(result, result2))
 
         result = instance.norm_vectors[0] @ instance.norm_vectors[1].T
         result2 = instance.vector_similarity(vectors[0], [words[1]])
 
         self.assertEqual(result, result2)
-
-        result3 = instance.vector_similarity(vectors[0], [words[1]])
-        self.assertEqual(result2, result3)
```

### Comparing `reach-4.1.0/tests/test_vectorize.py` & `reach-4.1.1/tests/test_vectorize.py`

 * *Files identical despite different names*

