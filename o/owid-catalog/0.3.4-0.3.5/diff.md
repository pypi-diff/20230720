# Comparing `tmp/owid_catalog-0.3.4.tar.gz` & `tmp/owid_catalog-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owid_catalog-0.3.4.tar", max compression
+gzip compressed data, was "owid_catalog-0.3.5.tar", max compression
```

## Comparing `owid_catalog-0.3.4.tar` & `owid_catalog-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1079 2022-11-23 20:46:48.515761 owid_catalog-0.3.4/LICENSE
--rw-r--r--   0        0        0     8089 2022-12-22 03:32:01.633675 owid_catalog-0.3.4/README.md
--rw-r--r--   0        0        0      519 2022-11-23 20:46:48.516106 owid_catalog-0.3.4/owid/catalog/__init__.py
--rw-r--r--   0        0        0    14267 2022-11-23 20:46:48.516219 owid_catalog-0.3.4/owid/catalog/catalogs.py
--rw-r--r--   0        0        0     8638 2022-12-21 03:48:04.282884 owid_catalog-0.3.4/owid/catalog/datasets.py
--rw-r--r--   0        0        0     4280 2022-11-23 20:46:48.516396 owid_catalog-0.3.4/owid/catalog/frames.py
--rw-r--r--   0        0        0     7320 2022-12-21 03:48:04.283233 owid_catalog-0.3.4/owid/catalog/meta.py
--rw-r--r--   0        0        0      449 2022-11-23 20:46:48.516547 owid_catalog-0.3.4/owid/catalog/properties.py
--rw-r--r--   0        0        0     2986 2022-11-23 20:46:48.516614 owid_catalog-0.3.4/owid/catalog/s3_utils.py
--rw-r--r--   0        0        0      532 2022-11-23 20:46:48.516720 owid_catalog-0.3.4/owid/catalog/schemas/table.json
--rw-r--r--   0        0        0      527 2022-11-23 20:46:48.516782 owid_catalog-0.3.4/owid/catalog/schemas/variable.json
--rw-r--r--   0        0        0    17641 2022-12-21 03:48:04.283786 owid_catalog-0.3.4/owid/catalog/tables.py
--rw-r--r--   0        0        0     5186 2022-12-21 03:48:04.284546 owid_catalog-0.3.4/owid/catalog/utils.py
--rw-r--r--   0        0        0     2520 2022-11-23 20:46:48.517051 owid_catalog-0.3.4/owid/catalog/variables.py
--rw-r--r--   0        0        0      968 2022-12-22 03:32:11.560593 owid_catalog-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9479 1970-01-01 00:00:00.000000 owid_catalog-0.3.4/setup.py
--rw-r--r--   0        0        0     9274 1970-01-01 00:00:00.000000 owid_catalog-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-20 11:27:12.671835 owid_catalog-0.3.5/LICENSE
+-rw-r--r--   0        0        0     8454 2023-07-20 11:50:44.727413 owid_catalog-0.3.5/README.md
+-rw-r--r--   0        0        0      581 2023-07-18 19:38:17.492847 owid_catalog-0.3.5/owid/catalog/__init__.py
+-rw-r--r--   0        0        0    14728 2023-07-14 13:30:36.646669 owid_catalog-0.3.5/owid/catalog/catalogs.py
+-rw-r--r--   0        0        0    11516 2023-07-18 19:38:17.494062 owid_catalog-0.3.5/owid/catalog/datasets.py
+-rw-r--r--   0        0        0    10211 2023-07-18 19:38:17.495131 owid_catalog-0.3.5/owid/catalog/meta.py
+-rwxr-xr-x   0        0        0      228 2023-07-14 13:37:40.053644 owid_catalog-0.3.5/owid/catalog/processing.py
+-rw-r--r--   0        0        0      449 2023-06-20 11:27:12.674116 owid_catalog-0.3.5/owid/catalog/properties.py
+-rw-r--r--   0        0        0     2991 2023-07-14 13:30:36.647732 owid_catalog-0.3.5/owid/catalog/s3_utils.py
+-rw-r--r--   0        0        0      532 2023-06-20 11:27:12.675180 owid_catalog-0.3.5/owid/catalog/schemas/table.json
+-rw-r--r--   0        0        0      527 2023-06-20 11:27:12.675302 owid_catalog-0.3.5/owid/catalog/schemas/variable.json
+-rw-r--r--   0        0        0    49494 2023-07-20 11:49:57.788681 owid_catalog-0.3.5/owid/catalog/tables.py
+-rw-r--r--   0        0        0     7183 2023-07-18 14:27:34.779483 owid_catalog-0.3.5/owid/catalog/utils.py
+-rw-r--r--   0        0        0    24659 2023-07-20 11:49:57.789173 owid_catalog-0.3.5/owid/catalog/variables.py
+-rw-r--r--   0        0        0     1100 2023-07-20 11:50:36.944956 owid_catalog-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 owid_catalog-0.3.5/PKG-INFO
```

### Comparing `owid_catalog-0.3.4/LICENSE` & `owid_catalog-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.4/README.md` & `owid_catalog-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-![build status](https://github.com/owid/owid-catalog-py/actions/workflows/python-package.yml/badge.svg)
+[![Build status](https://badge.buildkite.com/66cc67fc572120ca97b9ffff288d5d73cb33e019dd70323053.svg)](https://buildkite.com/our-world-in-data/owid-catalog-unit-tests)
 [![PyPI version](https://badge.fury.io/py/owid-catalog.svg)](https://badge.fury.io/py/owid-catalog)
-![](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)
+![](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 
 # owid-catalog
 
 _A Pythonic API for working with OWID's data catalog._
 
 Status: experimental, APIs likely to change
 
@@ -210,14 +210,21 @@
 t = Table.read_feather('/tmp/my_table.feather')
 
 t = Table.read_csv('/tmp/my_table.csv')
 ```
 
 ## Changelog
 
+- `dev`
+- `v0.3.5`
+  - Remove `catalog.frames`; use `owid-repack` package instead
+  - Relax dependency constraints
+  - Add optional `channel` argument to `DatasetMeta`
+  - Stop supporting metadata in Parquet format, load JSON sidecar instead
+  - Fix errors when creating new Table columns
 - `v0.3.4`
   - Bump `pyarrow` dependency to enable Python 3.11 support
 - `v0.3.3`
   - Add more arguments to `Table.__init__` that are often used in ETL
   - Add `Dataset.update_metadata` function for updating metadata from YAML file
   - Python 3.11 support via update of `pyarrow` dependency
 - `v0.3.2`
```

### Comparing `owid_catalog-0.3.4/owid/catalog/__init__.py` & `owid_catalog-0.3.5/owid/catalog/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 __version__ = "0.1.0"
 
-from . import utils
-from .catalogs import CHANNEL, LocalCatalog, RemoteCatalog, find, find_one
+from . import processing, utils
+from .catalogs import CHANNEL, LocalCatalog, RemoteCatalog, find, find_latest, find_one
 from .datasets import Dataset
 from .meta import DatasetMeta, License, Source, TableMeta, VariableMeta
 from .tables import Table
 from .variables import Variable
 
 __all__ = [
     "LocalCatalog",
     "RemoteCatalog",
     "find",
+    "find_latest",
     "find_one",
     "Dataset",
     "Table",
     "Variable",
     "DatasetMeta",
     "TableMeta",
     "VariableMeta",
     "Source",
     "License",
     "utils",
     "CHANNEL",
+    "processing",
 ]
```

### Comparing `owid_catalog-0.3.4/owid/catalog/catalogs.py` & `owid_catalog-0.3.5/owid/catalog/catalogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 import heapq
 import json
 import os
 import re
 import tempfile
 from pathlib import Path
-from typing import Any, Dict, Iterable, Iterator, List, Literal, Optional, Union, cast
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Union, cast
 from urllib.parse import urlparse
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import requests
 import structlog
 
 from . import s3_utils
-from .datasets import PREFERRED_FORMAT, SUPPORTED_FORMATS, Dataset, FileFormat
+from .datasets import CHANNEL, PREFERRED_FORMAT, SUPPORTED_FORMATS, Dataset, FileFormat
 from .tables import Table
 
 log = structlog.get_logger()
 
 # increment this on breaking changes to require clients to update
 OWID_CATALOG_VERSION = 3
 
@@ -32,19 +32,16 @@
 
 # S3 location for private files
 S3_OWID_URI = "s3://owid-catalog"
 
 # global copy cached after first request
 REMOTE_CATALOG: Optional["RemoteCatalog"] = None
 
-# available channels in the catalog
-CHANNEL = Literal["garden", "meadow", "grapher", "backport", "open_numbers", "examples", "explorers"]
-
 # what formats should we for our index of available datasets?
-INDEX_FORMATS: List[FileFormat] = ["feather", "parquet"]
+INDEX_FORMATS: List[FileFormat] = ["feather"]
 
 
 class CatalogMixin:
     """
     Abstract data catalog API, encapsulates finding and loading data.
     """
 
@@ -364,37 +361,56 @@
                     uri = _download_private_file(uri, tmpdir)
 
                 return Table.read(uri)
 
         raise ValueError("series is not a table spec")
 
 
-def find(
-    table: Optional[str] = None,
-    namespace: Optional[str] = None,
-    version: Optional[str] = None,
-    dataset: Optional[str] = None,
-    channels: Iterable[CHANNEL] = ("garden",),
-) -> "CatalogFrame":
+def _load_remote_catalog(channels):
     global REMOTE_CATALOG
 
     # add channel if missing and reinit remote catalog
     if REMOTE_CATALOG and not (set(channels) <= set(REMOTE_CATALOG.channels)):
         REMOTE_CATALOG = RemoteCatalog(channels=list(set(REMOTE_CATALOG.channels) | set(channels)))
 
     if not REMOTE_CATALOG:
         REMOTE_CATALOG = RemoteCatalog(channels=channels)
 
+    return REMOTE_CATALOG
+
+
+def find(
+    table: Optional[str] = None,
+    namespace: Optional[str] = None,
+    version: Optional[str] = None,
+    dataset: Optional[str] = None,
+    channels: Iterable[CHANNEL] = ("garden",),
+) -> "CatalogFrame":
+    REMOTE_CATALOG = _load_remote_catalog(channels=channels)
+
     return REMOTE_CATALOG.find(table=table, namespace=namespace, version=version, dataset=dataset)
 
 
 def find_one(*args: Optional[str], **kwargs: Optional[str]) -> Table:
     return find(*args, **kwargs).load()  # type: ignore
 
 
+def find_latest(
+    table: Optional[str] = None,
+    namespace: Optional[str] = None,
+    dataset: Optional[str] = None,
+    channels: Iterable[CHANNEL] = ("garden",),
+    version: Optional[str] = None,
+) -> Table:
+    REMOTE_CATALOG = _load_remote_catalog(channels=channels)
+
+    # If version is not specified, it will find the latest version given all other specifications.
+    return REMOTE_CATALOG.find_latest(table=table, namespace=namespace, dataset=dataset, version=version)
+
+
 def _download_private_file(uri: str, tmpdir: str) -> str:
     parsed = urlparse(uri)
     base, ext = os.path.splitext(parsed.path)
     s3_utils.download(
         S3_OWID_URI + base + ".meta.json",
         tmpdir + "/data.meta.json",
     )
```

### Comparing `owid_catalog-0.3.4/owid/catalog/datasets.py` & `owid_catalog-0.3.5/owid/catalog/datasets.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,43 +4,50 @@
 
 import hashlib
 import json
 import shutil
 import warnings
 from dataclasses import dataclass
 from glob import glob
-from os import mkdir
+from os import environ, mkdir
 from os.path import join
 from pathlib import Path
 from typing import Any, Iterator, List, Literal, Optional, Union
 
+import numpy as np
 import pandas as pd
 import yaml
 
 from . import tables, utils
 from .meta import SOURCE_EXISTS_OPTIONS, DatasetMeta, TableMeta
 from .properties import metadata_property
 
 FileFormat = Literal["csv", "feather", "parquet"]
 
 # the formats we can serialise and deserialise; in some cases they
 # will be tried in this order if we don't specify one explicitly
 SUPPORTED_FORMATS: List[FileFormat] = ["feather", "parquet", "csv"]
 
 # the formats we generate by default
-DEFAULT_FORMATS: List[FileFormat] = ["feather", "parquet"]
+DEFAULT_FORMATS: List[FileFormat] = ["feather"]
 
 # the format we use by default if we only need one
 PREFERRED_FORMAT: FileFormat = "feather"
 
 # sanity checks
 assert set(DEFAULT_FORMATS).issubset(SUPPORTED_FORMATS)
 assert PREFERRED_FORMAT in DEFAULT_FORMATS
 assert SUPPORTED_FORMATS[0] == PREFERRED_FORMAT
 
+# available channels in the catalog
+CHANNEL = Literal["garden", "meadow", "grapher", "backport", "open_numbers", "examples", "explorers"]
+
+# all pandas nullable dtypes
+NULLABLE_DTYPES = [f"{sign}{typ}{size}" for typ in ("Int", "Float") for sign in ("", "U") for size in (8, 16, 32, 64)]
+
 
 @dataclass
 class Dataset:
     """
     A dataset is a folder full of data tables, with metadata available at `index.json`.
     """
 
@@ -89,14 +96,48 @@
             to reduce binary file size. Consider using False when your dataframe is large and the repack is failing.
         """
 
         utils.validate_underscore(table.metadata.short_name, "Table's short_name")
         for col in list(table.columns) + list(table.index.names):
             utils.validate_underscore(col, "Variable's name")
 
+        # non-unique index might be causing problems down the line and is typically a mistake
+        if not table.index.is_unique:
+            # regions are the only exception where this is acceptable (though not ideal)
+            if "garden/regions/2023-01-01/regions" not in self.path:
+                warnings.warn(
+                    f"Table `{table.metadata.short_name}` from dataset `{self.metadata.short_name}` has non-unique index"
+                )
+
+        if not table.primary_key:
+            if "OWID_STRICT" in environ:
+                raise PrimaryKeyMissing(
+                    f"Table `{table.metadata.short_name}` does not have a primary_key -- please use t.set_index([col, ...], verify_integrity=True) to indicate dimensions before saving"
+                )
+            else:
+                warnings.warn(
+                    f"Table `{table.metadata.short_name}` does not have a primary_key -- please use t.set_index([col, ...], verify_integrity=True) to indicate dimensions before saving"
+                )
+
+        if not table.index.is_unique and "OWID_STRICT" in environ:
+            [(k, dups)] = table.index.value_counts().head(1).to_dict().items()
+            raise NonUniqueIndex(
+                f"Table `{table.metadata.short_name}` has duplicate values in the index -- could you have made a mistake?\n\n"
+                f"e.g. key {k} is repeated {dups} times in the index"
+            )
+
+        # check Float64 and Int64 columns for np.nan
+        for col, dtype in table.dtypes.items():
+            if dtype in NULLABLE_DTYPES:
+                # pandas nullable types like Float64 have their own pd.NA instead of np.nan
+                # make sure we don't use wrong nan, otherwise dropna and other methods won't work
+                assert (
+                    np.isnan(table[col]).sum() == 0
+                ), f"Column `{col}` is using np.nan, but it should be using pd.NA because it has type {table[col].dtype}"
+
         # copy dataset metadata to the table
         table.metadata.dataset = self.metadata
 
         for format in formats:
             if format not in SUPPORTED_FORMATS:
                 raise Exception(f"Format '{format}'' is not supported")
 
@@ -119,14 +160,23 @@
     def save(self) -> None:
         assert self.metadata.short_name, "Missing dataset short_name"
         utils.validate_underscore(self.metadata.short_name, "Dataset's short_name")
 
         if not self.metadata.namespace:
             warnings.warn(f"Dataset {self.metadata.short_name} is missing namespace")
 
+        # determine channel automatically from path
+        # NOTE: shouldn't we force channel/namespace/version/short_name to be filled from path?
+        # see https://github.com/owid/owid-catalog-py/pull/79#issue-1507959097 for discussion
+        parts = str(self.path).split("/")
+        if len(parts) >= 4:
+            channel, _, _, _ = parts[-4:]
+            if channel in CHANNEL.__args__:  # type: ignore
+                self.metadata.channel = channel
+
         self.metadata.save(self._index_file)
 
         # Update the copy of this datasets metadata in every table in the set.
         for table_name in self.table_names:
             table = self[table_name]
             table.metadata.dataset = self.metadata
             table._save_metadata(join(self.path, table.metadata.checked_name + ".meta.json"))
@@ -142,15 +192,15 @@
             - "append": append new source to existing ones
             - "fail": raise an exception if source already exists
         """
         self.metadata.update_from_yaml(metadata_path, if_source_exists=if_source_exists)
 
         with open(metadata_path) as istream:
             metadata = yaml.safe_load(istream)
-            for table_name in metadata["tables"].keys():
+            for table_name in metadata.get("tables", {}).keys():
                 table = self[table_name]
                 table.update_metadata_from_yaml(metadata_path, table_name)
                 table._save_metadata(join(self.path, table.metadata.checked_name + ".meta.json"))
 
     def index(self, catalog_path: Path = Path("/")) -> pd.DataFrame:
         """
         Return a DataFrame describing the contents of this dataset, one row per table.
@@ -185,14 +235,17 @@
 
         return pd.DataFrame.from_records(rows)
 
     @property
     def _index_file(self) -> str:
         return join(self.path, "index.json")
 
+    def __bool__(self) -> bool:
+        return True
+
     def __len__(self) -> int:
         return len(self.table_names)
 
     def __iter__(self) -> Iterator[tables.Table]:
         for name in self.table_names:
             yield self[name]
 
@@ -241,7 +294,15 @@
     with open(filename, "rb") as istream:
         chunk = istream.read(chunk_size)
         while chunk:
             checksum.update(chunk)
             chunk = istream.read(chunk_size)
 
     return checksum
+
+
+class PrimaryKeyMissing(Exception):
+    pass
+
+
+class NonUniqueIndex(Exception):
+    pass
```

### Comparing `owid_catalog-0.3.4/owid/catalog/meta.py` & `owid_catalog-0.3.5/owid/catalog/meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 
 import json
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, TypeVar, Union
 
-import yaml
+import pandas as pd
 from dataclasses_json import dataclass_json
 
 T = TypeVar("T")
 
 
 def pruned_json(cls: T) -> T:
     orig = cls.to_dict  # type: ignore
@@ -31,15 +31,15 @@
 
 @pruned_json
 @dataclass_json
 @dataclass
 class Source:
     """Notes on importing sources to grapher:
     - Field `source.description` gets mapped to `Internal notes`, but we rather use it for `additional_info`
-    - The most important fields are `published_by`, `publisher_source` and `additional_info`
+    - The most important fields are `published_by` and `additional_info`
     - In admin for dataset (i.e. /admin/datasets/1234) only the first source of a dataset is shown and
         can be edited. The other ones are not visible.
     """
 
     name: Optional[str] = None
     description: Optional[str] = None
     url: Optional[str] = None
@@ -48,15 +48,14 @@
     date_accessed: Optional[str] = None
     publication_date: Optional[str] = None
     publication_year: Optional[int] = None
     # specific fields for grapher
     # NOTE: it's not clear how to map description & name to fields in grapher, so
     # we're keeping both for the time being. We might consolidate them in the future
     published_by: Optional[str] = None
-    publisher_source: Optional[str] = None
 
     def to_dict(self) -> Dict[str, Any]:
         ...
 
     def update(self, **kwargs: Dict[str, Any]) -> None:
         for key, value in kwargs.items():
             if value is not None:
@@ -73,14 +72,17 @@
     def to_dict(self) -> Dict[str, Any]:
         ...
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "License":
         ...
 
+    def __bool__(self):
+        return bool(self.name or self.url)
+
 
 @pruned_json
 @dataclass_json
 @dataclass
 class VariableMeta:
     """Allowed fields for `display` attribute used for grapher:
         name
@@ -101,35 +103,48 @@
     description: Optional[str] = None
     sources: List[Source] = field(default_factory=list)
     licenses: List[License] = field(default_factory=list)
     unit: Optional[str] = None
     short_unit: Optional[str] = None
     display: Optional[Dict[str, Any]] = None
     additional_info: Optional[Dict[str, Any]] = None
+    processing_log: List[Dict[str, Any]] = field(default_factory=list)
 
     def to_dict(self) -> Dict[str, Any]:
         ...
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "VariableMeta":
         ...
 
+    def _repr_html_(self):
+        # Render a nice display of the table metadata
+        record = self.to_dict()
+        return """
+             <h2 style="margin-bottom: 0em"><pre>{}</pre></h2>
+             <p style="font-variant: small-caps; font-family: sans-serif; font-size: 1.5em; color: grey; margin-top: -0.2em; margin-bottom: 0.2em">variable meta</p>
+             {}
+        """.format(
+            getattr(self, "_name", None), to_html(record)
+        )
+
 
 @pruned_json
 @dataclass_json
 @dataclass
 class DatasetMeta:
     """
     The metadata for this entire dataset kept in JSON (e.g. mydataset/index.json).
 
     The number of fields is limited, but should handle everything that we get from
     Walden. There is a lot more opportunity to store more metadata at the table and
     the variable level.
     """
 
+    channel: Optional[str] = None
     namespace: Optional[str] = None
     # NOTE: short_name should be underscore and validate in setter, however this
     # is nontrivial to do with `dataclass_json` (see https://github.com/lidatong/dataclasses-json/issues/176)
     short_name: Optional[str] = None
     title: Optional[str] = None
     description: Optional[str] = None
     sources: List[Source] = field(default_factory=list)
@@ -145,16 +160,18 @@
         """Imply version from publication_date or publication_year if not given
         in __init__."""
         if self.version is None:
             if len(self.sources) == 1:
                 (source,) = self.sources
                 if source.publication_date:
                     self.version = str(source.publication_date)
-                else:
+                elif source.publication_year:
                     self.version = str(source.publication_year)
+                else:
+                    self.version = None
 
     def save(self, filename: Union[str, Path]) -> None:
         filename = Path(filename).as_posix()
         with open(filename, "w") as ostream:
             json.dump(self.to_dict(), ostream, indent=2, default=str)
 
     @classmethod
@@ -165,20 +182,28 @@
     def to_dict(self) -> Dict[str, Any]:
         ...
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "DatasetMeta":
         ...
 
+    def _params_yaml(self) -> dict:
+        """Parameters passed to YAML for dynamic interpolation."""
+        params = {}
+        if self.version and self.version != "latest":
+            params["YEAR"] = pd.to_datetime(self.version).year
+        return params
+
     def update_from_yaml(self, path: Union[Path, str], if_source_exists: SOURCE_EXISTS_OPTIONS = "fail") -> None:
         """The main reason for wanting to do this is to manually override what goes into Grapher before an export."""
-        with open(path) as istream:
-            annot = yaml.safe_load(istream)
+        from owid.catalog import utils
 
-        dataset_sources = annot["dataset"].get("sources", []) or []
+        annot = utils.dynamic_yaml_load(path, self._params_yaml())
+
+        dataset_sources = annot.get("dataset", {}).get("sources", []) or []
 
         # update sources of dataset, if there are no sources in the new dataset, don't update existing ones
         if if_source_exists == "replace" and dataset_sources:
             self.sources = []
 
         new_sources = []
         for source_annot in dataset_sources:
@@ -192,18 +217,27 @@
             # otherwise append it
             else:
                 new_sources.append(Source(**source_annot))
 
         self.sources.extend(new_sources)
 
         # update dataset
-        for k, v in annot["dataset"].items():
+        for k, v in annot.get("dataset", {}).items():
             if k != "sources":
                 setattr(self, k, v)
 
+    @property
+    def uri(self) -> str:
+        """Return unique URI for this dataset if"""
+        assert self.channel, "DatasetMeta.channel is not set"
+        assert self.namespace, "DatasetMeta.namespace is not set"
+        assert self.version, "DatasetMeta.version is not set"
+        assert self.short_name, "DatasetMeta.short_name is not set"
+        return f"{self.channel}/{self.namespace}/{self.version}/{self.short_name}"
+
 
 @pruned_json
 @dataclass_json
 @dataclass
 class TableMeta:
     # data about this table
     short_name: Optional[str] = None
@@ -223,7 +257,47 @@
 
     def to_dict(self) -> Dict[str, Any]:
         ...
 
     @staticmethod
     def from_dict(dict: Dict[str, Any]) -> "TableMeta":
         ...
+
+    def _repr_html_(self):
+        # Render a nice display of the table metadata
+        record = self.to_dict()
+        short_name = record.pop("short_name")
+        return """
+             <h2 style="margin-bottom: 0em"><pre>{}</pre></h2>
+             <p style="font-variant: small-caps; font-family: sans-serif; font-size: 1.5em; color: grey; margin-top: -0.2em; margin-bottom: 0.2em">table meta</p>
+             {}
+        """.format(
+            short_name, to_html(record)
+        )
+
+
+def to_html(record: Any) -> Optional[str]:
+    if isinstance(record, dict):
+        rows = []
+        for k, v in record.items():
+            if not v:
+                continue
+            v_str = to_html(v)
+            rows.append(
+                """<tr><th style="text-align: right; font-family: sans-serif; vertical-align: top; padding: 0.2em 1em;"><strong>{}</strong></th><td style="text-align: left; padding: 0.2em 1em;">{}</td></tr>""".format(
+                    k, v_str
+                )
+            )
+        return '<table style="margin: 0em"><tbody>{}</tbody></table>'.format("".join(rows))
+
+    elif isinstance(record, list):
+        record = list(filter(None, record))
+        if not record:
+            return None
+
+        rows = []
+        for item in record:
+            rows.append("<li>{}</li>".format(to_html(item)))
+        return '<ul style="text-align: left; margin-top: 0em; margin-bottom: 0em">{}</ul>'.format("".join(rows))
+
+    else:
+        return str(record)
```

### Comparing `owid_catalog-0.3.4/owid/catalog/s3_utils.py` & `owid_catalog-0.3.5/owid/catalog/s3_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 import logging
 import os
 from os import path
 from typing import Any, Tuple
 from urllib.parse import urlparse
 
-import boto3
 from botocore.exceptions import ClientError
 
 SPACES_ENDPOINT = "https://nyc3.digitaloceanspaces.com"
 S3_BASE = "s3://walden.nyc3.digitaloceanspaces.com"
 HTTPS_BASE = "https://walden.nyc3.digitaloceanspaces.com"
 AWS_PROFILE = os.environ.get("AWS_PROFILE", "default")
 
@@ -68,14 +67,16 @@
 
     if not quiet:
         logging.info("DOWNLOADED", f"{s3_url} -> {filename}")
 
 
 def connect() -> Any:
     "Return a connection to Walden's DigitalOcean space."
+    import boto3
+
     check_for_default_profile()
 
     session = boto3.Session(profile_name=AWS_PROFILE)
     client = session.client(
         service_name="s3",
         endpoint_url=SPACES_ENDPOINT,
     )
```

### Comparing `owid_catalog-0.3.4/owid/catalog/schemas/table.json` & `owid_catalog-0.3.5/owid/catalog/schemas/table.json`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.4/owid/catalog/schemas/variable.json` & `owid_catalog-0.3.5/owid/catalog/schemas/variable.json`

 * *Files identical despite different names*

### Comparing `owid_catalog-0.3.4/owid/catalog/utils.py` & `owid_catalog-0.3.5/owid/catalog/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,60 @@
+import datetime as dt
 import re
-from typing import List, Literal, Optional, overload
+from pathlib import Path
+from typing import List, Literal, Optional, Union, overload
 
+import dynamic_yaml
 import numpy as np
 import pandas as pd
+import pytz
 from unidecode import unidecode
 
 from .tables import Table
 from .variables import Variable
 
 
 @overload
-def underscore(name: str, validate: bool = True) -> str:
+def underscore(name: str, validate: bool = True, camel_to_snake: bool = False) -> str:
     ...
 
 
 @overload
-def underscore(name: None, validate: bool = True) -> None:
+def underscore(name: None, validate: bool = True, camel_to_snake: bool = False) -> None:
     ...
 
 
-def underscore(name: Optional[str], validate: bool = True) -> Optional[str]:
+def underscore(name: Optional[str], validate: bool = True, camel_to_snake: bool = False) -> Optional[str]:
     """Convert arbitrary string to under_score. This was fine tuned on WDI bank column names.
     This function might evolve in the future, so make sure to have your use cases in tests
     or rather underscore your columns yourself.
+
+    Parameters
+    ----------
+    name : str
+        String to format.
+    validate: bool, optional
+        Whether to validate that the string is under_score. Defaults to True.
+    camel_to_snake: bool, optional
+        Whether to convert camelCase to snake_case. Defaults to False.
+
+    Returns
+    -------
+    str:
+        String using snake_case formatting.
     """
     if name is None:
         return None
 
     orig_name = name
 
+    # camelCase to snake_case
+    if camel_to_snake:
+        name = _camel_to_snake(name)
+
     name = (
         name.replace(" ", "_")
         .replace("-", "_")
         .replace("—", "_")
         .replace("–", "_")
         .replace(",", "_")
         .replace(".", "_")
@@ -95,14 +117,37 @@
     # make sure it's under_score now, if not then raise NameError
     if validate:
         validate_underscore(name, f"`{orig_name}`")
 
     return name
 
 
+def _camel_to_snake(name: str) -> str:
+    """Convert string camelCase to snake_case.
+
+    Reference: https://stackoverflow.com/a/1176023/5056599 CC BY-SA 4.0
+
+    Example:
+    >>> _camel_to_snake('camelCase')
+    'camel_case'
+
+    Parameters
+    ----------
+    name : str
+        String using camelCase formatting.
+
+    Returns
+    -------
+    str:
+        String using snake_case formatting.
+    """
+    name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", name).lower()
+
+
 def _resolve_collisions(
     orig_cols: pd.Index,
     new_cols: pd.Index,
     collision: Literal["raise", "rename", "ignore"],
 ) -> pd.Index:
     new_cols = new_cols.copy()
     vc = new_cols.value_counts()
@@ -126,33 +171,46 @@
     return new_cols
 
 
 def underscore_table(
     t: Table,
     collision: Literal["raise", "rename", "ignore"] = "raise",
     inplace: bool = False,
+    camel_to_snake: bool = False,
 ) -> Table:
     """Convert column and index names to underscore. In extremely rare cases
     two columns might have the same underscored version. Use `collision` param
-    to control whether to raise an error or append numbered suffix."""
+    to control whether to raise an error or append numbered suffix.
+
+    Parameters
+    ----------
+    t : Table
+        Table to underscore.
+    collision : Literal["raise", "rename", "ignore"], optional
+        How to handle collisions, by default "raise".
+    inplace : bool, optional
+        Whether to modify the table in place, by default False.
+    camel_to_snake : bool, optional
+        Whether to convert strings camelCase to snake_case, by default False.
+    """
     orig_cols = t.columns
 
     # underscore columns and resolve collisions
-    new_cols = pd.Index([underscore(c) for c in t.columns])
+    new_cols = pd.Index([underscore(c, camel_to_snake=camel_to_snake) for c in t.columns])
     new_cols = _resolve_collisions(orig_cols, new_cols, collision)
 
     columns_map = {c_old: c_new for c_old, c_new in zip(orig_cols, new_cols)}
     if inplace:
         t.rename(columns=columns_map, inplace=True)
     else:
         t = t.rename(columns=columns_map)
 
-    t.index.names = [underscore(e) for e in t.index.names]
+    t.index.names = [underscore(e, camel_to_snake=camel_to_snake) for e in t.index.names]
     t.metadata.primary_key = t.primary_key
-    t.metadata.short_name = underscore(t.metadata.short_name)
+    t.metadata.short_name = underscore(t.metadata.short_name, camel_to_snake=camel_to_snake)
 
     # put original names as titles into metadata by default
     for c_old, c_new in columns_map.items():
         if t[c_new].metadata.title is None:
             t[c_new].metadata.title = c_old
 
     return t
@@ -167,7 +225,19 @@
 def concat_variables(variables: List[Variable]) -> Table:
     """Concatenate variables into a single table keeping all metadata."""
     t = Table(pd.concat(variables, axis=1))
     for v in variables:
         if v.name:
             t._fields[v.name] = v.metadata
     return t
+
+
+def dynamic_yaml_load(path: Union[Path, str], params: dict = {}) -> dict:
+    with open(path) as istream:
+        yd = dynamic_yaml.load(istream)
+
+    yd.update(params)
+
+    # additional parameters
+    yd["TODAY"] = dt.datetime.now().astimezone(pytz.timezone("Europe/London")).strftime("%-d %B %Y")
+
+    return yd
```

### Comparing `owid_catalog-0.3.4/pyproject.toml` & `owid_catalog-0.3.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 [tool.poetry]
 name = "owid-catalog"
-version = "0.3.4"
+version = "0.3.5"
 description = "Core data types used by OWID for managing data."
 authors = ["Our World In Data <tech@ourworldindata.org>"]
 license = "MIT"
 packages = [{ include = "owid" }]
 readme = "README.md"
 repository = "https://github.com/owid/owid-grapher-py"
 homepage = "https://github.com/owid/owid-grapher-py"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^1.3.3"
-jsonschema = "^3.2.0"
-pandas-stubs = "^1.2.0"
-dataclasses-json = "^0.5.6"
-pyarrow = "^10.0.1"
-ipdb = "^0.13.9"
-pytest-cov = "^2.12.1"
-requests = "^2.26.0"
-boto3 = "^1.21.13"
-Unidecode = "^1.3.4"
-PyYAML = "^5.4.1"
-structlog = "^21.5.0"
+python = ">=3.8.1"
+pandas = ">=1.3.3,<2.0"
+jsonschema = ">=3.2.0"
+pandas-stubs = ">=1.2.0"
+dataclasses-json = ">=0.5.6"
+pyarrow = ">=10.0.1"
+ipdb = ">=0.13.9"
+pytest-cov = ">=2.12.1"
+requests = ">=2.26.0"
+boto3 = ">=1.21.13"
+Unidecode = ">=1.3.4"
+PyYAML = ">=5.4.1"
+structlog = ">=21.5.0"
+owid-repack = ">=0.1.1"
+dynamic-yaml = "^1.3.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-black = "^22.3"
-flake8 = "^3.9.2"
-watchdog = "^2.1.5"
-argh = "^0.26.2"
-isort = "^5.10.1"
-pyright = "^1.1.278"
+pytest = ">=6.2.5"
+black = ">=22.3"
+flake8 = ">=3.9.2"
+watchdog = ">=2.1.5"
+argh = ">=0.26.2"
+isort = ">=5.10.1"
+pyright = ">=1.1.278"
+
+[tool.poetry.group.dev.dependencies]
+isort = ">=5.12.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 120
```

### Comparing `owid_catalog-0.3.4/setup.py` & `owid_catalog-0.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,308 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: owid-catalog
+Version: 0.3.5
+Summary: Core data types used by OWID for managing data.
+Home-page: https://github.com/owid/owid-grapher-py
+License: MIT
+Author: Our World In Data
+Author-email: tech@ourworldindata.org
+Requires-Python: >=3.8.1
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: Unidecode (>=1.3.4)
+Requires-Dist: boto3 (>=1.21.13)
+Requires-Dist: dataclasses-json (>=0.5.6)
+Requires-Dist: dynamic-yaml (>=1.3.4,<2.0.0)
+Requires-Dist: ipdb (>=0.13.9)
+Requires-Dist: jsonschema (>=3.2.0)
+Requires-Dist: owid-repack (>=0.1.1)
+Requires-Dist: pandas (>=1.3.3,<2.0)
+Requires-Dist: pandas-stubs (>=1.2.0)
+Requires-Dist: pyarrow (>=10.0.1)
+Requires-Dist: pytest-cov (>=2.12.1)
+Requires-Dist: requests (>=2.26.0)
+Requires-Dist: structlog (>=21.5.0)
+Project-URL: Repository, https://github.com/owid/owid-grapher-py
+Description-Content-Type: text/markdown
 
-packages = \
-['owid', 'owid.catalog']
+[![Build status](https://badge.buildkite.com/66cc67fc572120ca97b9ffff288d5d73cb33e019dd70323053.svg)](https://buildkite.com/our-world-in-data/owid-catalog-unit-tests)
+[![PyPI version](https://badge.fury.io/py/owid-catalog.svg)](https://badge.fury.io/py/owid-catalog)
+![](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 
-package_data = \
-{'': ['*'], 'owid.catalog': ['schemas/*']}
+# owid-catalog
 
-install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
- 'Unidecode>=1.3.4,<2.0.0',
- 'boto3>=1.21.13,<2.0.0',
- 'dataclasses-json>=0.5.6,<0.6.0',
- 'ipdb>=0.13.9,<0.14.0',
- 'jsonschema>=3.2.0,<4.0.0',
- 'pandas-stubs>=1.2.0,<2.0.0',
- 'pandas>=1.3.3,<2.0.0',
- 'pyarrow>=10.0.1,<11.0.0',
- 'pytest-cov>=2.12.1,<3.0.0',
- 'requests>=2.26.0,<3.0.0',
- 'structlog>=21.5.0,<22.0.0']
-
-setup_kwargs = {
-    'name': 'owid-catalog',
-    'version': '0.3.4',
-    'description': 'Core data types used by OWID for managing data.',
-    'long_description': '![build status](https://github.com/owid/owid-catalog-py/actions/workflows/python-package.yml/badge.svg)\n[![PyPI version](https://badge.fury.io/py/owid-catalog.svg)](https://badge.fury.io/py/owid-catalog)\n![](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)\n\n# owid-catalog\n\n_A Pythonic API for working with OWID\'s data catalog._\n\nStatus: experimental, APIs likely to change\n\n## Overview\n\nOur World In Data is building a new data catalog, with the goal of our datasets being reproducible and transparent to the general public. That project is our [etl](https://github.com/owid/etl), which going forward will contain the recipes for all the datasets we republish.\n\nThis library allows you to query our data catalog programmatically, and get back data in the form of Pandas data frames, perfect for data pipelines or Jupyter notebook explorations.\n\n```mermaid\ngraph TB\n\netl -->|reads| walden[upstream datasets]\netl -->|generates| s3[data catalog]\ncatalog[owid-catalog-py] -->|queries| s3\n```\n\nWe would love feedback on how we can make this library and overall data catalog better. Feel free to send us an email at info@ourworldindata.org, or start a [discussion](https://github.com/owid/etl/discussions) on Github.\n\n## Quickstart\n\nInstall with `pip install owid-catalog`. Then you can begin exploring the experimental data catalog:\n\n```python\nfrom owid import catalog\n\n# look for Covid-19 data, return a data frame of matches\ncatalog.find(\'covid\')\n\n# load Covid-19 data from the Our World In Data namespace as a data frame\ndf = catalog.find(\'covid\', namespace=\'owid\').load()\n\n# load data from other than the default `garden` channel\nlung_cancer_tables = catalog.find(\'lung_cancer_deaths_per_100000_men\', channels=[\'open_numbers\'])\ndf = lung_cancer_tables.iloc[0].load()\n```\n\n## Development\n\nYou need Python 3.8+, `poetry` and `make` installed. Clone the repo, then you can simply run:\n\n```\n# run all unit tests and CI checks\nmake test\n\n# watch for changes, then run all checks\nmake watch\n```\n\n## Data types\n\n### Catalog\n\nA catalog is an arbitrarily deep folder structure containing datasets inside. It can be local on disk, or remote.\n\n#### Load the remote catalog\n\n```python\n# find the default OWID catalog and fetch the catalog index over HTTPS\ncat = RemoteCatalog()\n\n# get a list of matching tables in different datasets\nmatches = cat.find(\'population\')\n\n# fetch a data frame for a specific match over HTTPS\nt = cat.find_one(\'population\', namespace=\'gapminder\')\n\n# load other channels than `garden`\ncat = RemoteCatalog(channels=(\'garden\', \'meadow\', \'open_numbers\'))\n```\n\n### Datasets\n\nA dataset is a folder of tables containing metadata about the overall collection.\n\n- Metadata about the dataset lives in `index.json`\n- All tables in the folder must share a common format (CSV or Feather)\n\n#### Create a new dataset\n\n```python\n# make a folder and an empty index.json file\nds = Dataset.create(\'/tmp/my_data\')\n```\n\n```python\n# choose CSV instead of feather for files\nds = Dataset.create(\'/tmp/my_data\', format=\'csv\')\n```\n\n#### Add a table to a dataset\n\n```python\n# serialize a table using the table\'s name and the dataset\'s default format (feather)\n# (e.g. /tmp/my_data/my_table.feather)\nds.add(table)\n```\n\n#### Remove a table from a dataset\n\n```python\nds.remove(\'table_name\')\n```\n\n#### Access a table\n\n```python\n# load a table including metadata into memory\nt = ds[\'my_table\']\n```\n\n#### List tables\n\n```python\n# the length is the number of datasets discovered on disk\nassert len(ds) > 0\n```\n\n```python\n# iterate over the tables discovered on disk\nfor table in ds:\n    do_something(table)\n```\n\n#### Add metadata\n\n```python\n# you need to manually save your changes\nds.title = "Very Important Dataset"\nds.description = "This dataset is a composite of blah blah blah..."\nds.save()\n```\n\n#### Copy a dataset\n\n```python\n# copying a dataset copies all its files to a new location\nds_new = ds.copy(\'/tmp/new_data_path\')\n\n# copying a dataset is identical to copying its folder, so this works too\nshutil.copytree(\'/tmp/old_data\', \'/tmp/new_data_path\')\nds_new = Dataset(\'/tmp/new_data_path\')\n```\n\n### Tables\n\nTables are essentially pandas DataFrames but with metadata. All operations on them occur in-memory, except for loading from and saving to disk. On disk, they are represented by tabular file (feather or CSV) and a JSON metadata file.\n\nColumns of `Table` have attribute `VariableMeta`, including their type, description, and unit. Be carful when manipulating them, not all operations are currently supported. Supported are: adding a column, renaming columns. Not supported: direct assignment to `t.columns = ...` or to index names `t.columns.index = ...`.\n\n#### Make a new table\n\n```python\n# same API as DataFrames\nt = Table({\n    \'gdp\': [1, 2, 3],\n    \'country\': [\'AU\', \'SE\', \'CH\']\n}).set_index(\'country\')\n```\n\n#### Add metadata about the whole table\n\n```python\nt.title = \'Very important data\'\n```\n\n#### Add metadata about a field\n\n```python\nt.gdp.description = \'GDP measured in 2011 international $\'\nt.sources = [\n    Source(title=\'World Bank\', url=\'https://www.worldbank.org/en/home\')\n]\n```\n\n#### Add metadata about all fields at once\n\n```python\n# sources and licenses are actually stored a the field level\nt.sources = [\n    Source(title=\'World Bank\', url=\'https://www.worldbank.org/en/home\')\n]\nt.licenses = [\n    License(\'CC-BY-SA-4.0\', url=\'https://creativecommons.org/licenses/by-nc/4.0/\')\n]\n```\n\n#### Save a table to disk\n\n```python\n# save to /tmp/my_table.feather + /tmp/my_table.meta.json\nt.to_feather(\'/tmp/my_table.feather\')\n\n# save to /tmp/my_table.csv + /tmp/my_table.meta.json\nt.to_csv(\'/tmp/my_table.csv\')\n```\n\n#### Load a table from disk\n\nThese work like normal pandas DataFrames, but if there is also a `my_table.meta.json` file, then metadata will also get read. Otherwise it will be assumed that the data has no metadata:\n\n```python\nt = Table.read_feather(\'/tmp/my_table.feather\')\n\nt = Table.read_csv(\'/tmp/my_table.csv\')\n```\n\n## Changelog\n\n- `v0.3.4`\n  - Bump `pyarrow` dependency to enable Python 3.11 support\n- `v0.3.3`\n  - Add more arguments to `Table.__init__` that are often used in ETL\n  - Add `Dataset.update_metadata` function for updating metadata from YAML file\n  - Python 3.11 support via update of `pyarrow` dependency\n- `v0.3.2`\n  - Fix a bug in `Catalog.__getitem__()`\n  - Replace `mypy` type checker by `pyright`\n- `v0.3.1`\n  - Sort imports with `isort`\n  - Change black line length to 120\n  - Add `grapher` channel\n  - Support path-based indexing into catalogs\n- `v0.3.0`\n  - Update `OWID_CATALOG_VERSION` to 3\n  - Support multiple formats per table\n  - Support reading and writing `parquet` files with embedded metadata\n  - Optional `repack` argument when adding tables to dataset\n  - Underscore `|`\n  - Get `version` field from `DatasetMeta` init\n  - Resolve collisions of `underscore_table` function\n  - Convert `version` to `str` and load json `dimensions`\n- `v0.2.9`\n  - Allow multiple channels in `catalog.find` function\n- `v0.2.8`\n  - Update `OWID_CATALOG_VERSION` to 2\n- `v0.2.7`\n  - Split datasets into channels (`garden`, `meadow`, `open_numbers`, ...) and make garden default one\n  - Add `.find_latest` method to Catalog\n- `v0.2.6`\n  - Add flag `is_public` for public/private datasets\n  - Enforce snake_case for table, dataset and variable short names\n  - Add fields `published_by` and `published_at` to Source\n  - Added a list of supported and unsupported operations on columns\n  - Updated `pyarrow`\n- `v0.2.5`\n  - Fix ability to load remote CSV tables\n- `v0.2.4`\n  - Update the default catalog URL to use a CDN\n- `v0.2.3`\n  - Fix methods for finding and loading data from a `LocalCatalog`\n- `v0.2.2`\n  - Repack frames to compact dtypes on `Table.to_feather()`\n- `v0.2.1`\n  - Fix key typo used in version check\n- `v0.2.0`\n  - Copy dataset metadata into tables, to make tables more traceable\n  - Add API versioning, and a requirement to update if your version of this library is too old\n- `v0.1.1`\n  - Add support for Python 3.8\n- `v0.1.0`\n  - Initial release, including searching and fetching data from a remote catalog\n',
-    'author': 'Our World In Data',
-    'author_email': 'tech@ourworldindata.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/owid/owid-grapher-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+_A Pythonic API for working with OWID's data catalog._
 
+Status: experimental, APIs likely to change
+
+## Overview
+
+Our World In Data is building a new data catalog, with the goal of our datasets being reproducible and transparent to the general public. That project is our [etl](https://github.com/owid/etl), which going forward will contain the recipes for all the datasets we republish.
+
+This library allows you to query our data catalog programmatically, and get back data in the form of Pandas data frames, perfect for data pipelines or Jupyter notebook explorations.
+
+```mermaid
+graph TB
+
+etl -->|reads| walden[upstream datasets]
+etl -->|generates| s3[data catalog]
+catalog[owid-catalog-py] -->|queries| s3
+```
+
+We would love feedback on how we can make this library and overall data catalog better. Feel free to send us an email at info@ourworldindata.org, or start a [discussion](https://github.com/owid/etl/discussions) on Github.
+
+## Quickstart
+
+Install with `pip install owid-catalog`. Then you can begin exploring the experimental data catalog:
+
+```python
+from owid import catalog
+
+# look for Covid-19 data, return a data frame of matches
+catalog.find('covid')
+
+# load Covid-19 data from the Our World In Data namespace as a data frame
+df = catalog.find('covid', namespace='owid').load()
+
+# load data from other than the default `garden` channel
+lung_cancer_tables = catalog.find('lung_cancer_deaths_per_100000_men', channels=['open_numbers'])
+df = lung_cancer_tables.iloc[0].load()
+```
+
+## Development
+
+You need Python 3.8+, `poetry` and `make` installed. Clone the repo, then you can simply run:
+
+```
+# run all unit tests and CI checks
+make test
+
+# watch for changes, then run all checks
+make watch
+```
+
+## Data types
+
+### Catalog
+
+A catalog is an arbitrarily deep folder structure containing datasets inside. It can be local on disk, or remote.
+
+#### Load the remote catalog
+
+```python
+# find the default OWID catalog and fetch the catalog index over HTTPS
+cat = RemoteCatalog()
+
+# get a list of matching tables in different datasets
+matches = cat.find('population')
+
+# fetch a data frame for a specific match over HTTPS
+t = cat.find_one('population', namespace='gapminder')
+
+# load other channels than `garden`
+cat = RemoteCatalog(channels=('garden', 'meadow', 'open_numbers'))
+```
+
+### Datasets
+
+A dataset is a folder of tables containing metadata about the overall collection.
+
+- Metadata about the dataset lives in `index.json`
+- All tables in the folder must share a common format (CSV or Feather)
+
+#### Create a new dataset
+
+```python
+# make a folder and an empty index.json file
+ds = Dataset.create('/tmp/my_data')
+```
+
+```python
+# choose CSV instead of feather for files
+ds = Dataset.create('/tmp/my_data', format='csv')
+```
+
+#### Add a table to a dataset
+
+```python
+# serialize a table using the table's name and the dataset's default format (feather)
+# (e.g. /tmp/my_data/my_table.feather)
+ds.add(table)
+```
+
+#### Remove a table from a dataset
+
+```python
+ds.remove('table_name')
+```
+
+#### Access a table
+
+```python
+# load a table including metadata into memory
+t = ds['my_table']
+```
+
+#### List tables
+
+```python
+# the length is the number of datasets discovered on disk
+assert len(ds) > 0
+```
+
+```python
+# iterate over the tables discovered on disk
+for table in ds:
+    do_something(table)
+```
+
+#### Add metadata
+
+```python
+# you need to manually save your changes
+ds.title = "Very Important Dataset"
+ds.description = "This dataset is a composite of blah blah blah..."
+ds.save()
+```
+
+#### Copy a dataset
+
+```python
+# copying a dataset copies all its files to a new location
+ds_new = ds.copy('/tmp/new_data_path')
+
+# copying a dataset is identical to copying its folder, so this works too
+shutil.copytree('/tmp/old_data', '/tmp/new_data_path')
+ds_new = Dataset('/tmp/new_data_path')
+```
+
+### Tables
+
+Tables are essentially pandas DataFrames but with metadata. All operations on them occur in-memory, except for loading from and saving to disk. On disk, they are represented by tabular file (feather or CSV) and a JSON metadata file.
+
+Columns of `Table` have attribute `VariableMeta`, including their type, description, and unit. Be carful when manipulating them, not all operations are currently supported. Supported are: adding a column, renaming columns. Not supported: direct assignment to `t.columns = ...` or to index names `t.columns.index = ...`.
+
+#### Make a new table
+
+```python
+# same API as DataFrames
+t = Table({
+    'gdp': [1, 2, 3],
+    'country': ['AU', 'SE', 'CH']
+}).set_index('country')
+```
+
+#### Add metadata about the whole table
+
+```python
+t.title = 'Very important data'
+```
+
+#### Add metadata about a field
+
+```python
+t.gdp.description = 'GDP measured in 2011 international $'
+t.sources = [
+    Source(title='World Bank', url='https://www.worldbank.org/en/home')
+]
+```
+
+#### Add metadata about all fields at once
+
+```python
+# sources and licenses are actually stored a the field level
+t.sources = [
+    Source(title='World Bank', url='https://www.worldbank.org/en/home')
+]
+t.licenses = [
+    License('CC-BY-SA-4.0', url='https://creativecommons.org/licenses/by-nc/4.0/')
+]
+```
+
+#### Save a table to disk
+
+```python
+# save to /tmp/my_table.feather + /tmp/my_table.meta.json
+t.to_feather('/tmp/my_table.feather')
+
+# save to /tmp/my_table.csv + /tmp/my_table.meta.json
+t.to_csv('/tmp/my_table.csv')
+```
+
+#### Load a table from disk
+
+These work like normal pandas DataFrames, but if there is also a `my_table.meta.json` file, then metadata will also get read. Otherwise it will be assumed that the data has no metadata:
+
+```python
+t = Table.read_feather('/tmp/my_table.feather')
+
+t = Table.read_csv('/tmp/my_table.csv')
+```
+
+## Changelog
+
+- `dev`
+- `v0.3.5`
+  - Remove `catalog.frames`; use `owid-repack` package instead
+  - Relax dependency constraints
+  - Add optional `channel` argument to `DatasetMeta`
+  - Stop supporting metadata in Parquet format, load JSON sidecar instead
+  - Fix errors when creating new Table columns
+- `v0.3.4`
+  - Bump `pyarrow` dependency to enable Python 3.11 support
+- `v0.3.3`
+  - Add more arguments to `Table.__init__` that are often used in ETL
+  - Add `Dataset.update_metadata` function for updating metadata from YAML file
+  - Python 3.11 support via update of `pyarrow` dependency
+- `v0.3.2`
+  - Fix a bug in `Catalog.__getitem__()`
+  - Replace `mypy` type checker by `pyright`
+- `v0.3.1`
+  - Sort imports with `isort`
+  - Change black line length to 120
+  - Add `grapher` channel
+  - Support path-based indexing into catalogs
+- `v0.3.0`
+  - Update `OWID_CATALOG_VERSION` to 3
+  - Support multiple formats per table
+  - Support reading and writing `parquet` files with embedded metadata
+  - Optional `repack` argument when adding tables to dataset
+  - Underscore `|`
+  - Get `version` field from `DatasetMeta` init
+  - Resolve collisions of `underscore_table` function
+  - Convert `version` to `str` and load json `dimensions`
+- `v0.2.9`
+  - Allow multiple channels in `catalog.find` function
+- `v0.2.8`
+  - Update `OWID_CATALOG_VERSION` to 2
+- `v0.2.7`
+  - Split datasets into channels (`garden`, `meadow`, `open_numbers`, ...) and make garden default one
+  - Add `.find_latest` method to Catalog
+- `v0.2.6`
+  - Add flag `is_public` for public/private datasets
+  - Enforce snake_case for table, dataset and variable short names
+  - Add fields `published_by` and `published_at` to Source
+  - Added a list of supported and unsupported operations on columns
+  - Updated `pyarrow`
+- `v0.2.5`
+  - Fix ability to load remote CSV tables
+- `v0.2.4`
+  - Update the default catalog URL to use a CDN
+- `v0.2.3`
+  - Fix methods for finding and loading data from a `LocalCatalog`
+- `v0.2.2`
+  - Repack frames to compact dtypes on `Table.to_feather()`
+- `v0.2.1`
+  - Fix key typo used in version check
+- `v0.2.0`
+  - Copy dataset metadata into tables, to make tables more traceable
+  - Add API versioning, and a requirement to update if your version of this library is too old
+- `v0.1.1`
+  - Add support for Python 3.8
+- `v0.1.0`
+  - Initial release, including searching and fetching data from a remote catalog
 
-setup(**setup_kwargs)
```

