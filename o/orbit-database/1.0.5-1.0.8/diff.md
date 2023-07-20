# Comparing `tmp/orbit_database-1.0.5.tar.gz` & `tmp/orbit_database-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database-1.0.5.tar", max compression
+gzip compressed data, was "orbit_database-1.0.8.tar", max compression
```

## Comparing `orbit_database-1.0.5.tar` & `orbit_database-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.5/LICENSE
--rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.5/README.md
--rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/README.md
--rwxr-xr-x   0        0        0     1932 2023-07-07 15:17:34.783200 orbit_database-1.0.5/orbit_database/__init__.py
--rw-r--r--   0        0        0     5978 2023-07-06 11:48:41.818031 orbit_database-1.0.5/orbit_database/audit.py
--rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/bitmap.py
--rw-r--r--   0        0        0     3653 2023-06-17 15:47:18.989970 orbit_database-1.0.5/orbit_database/catalog.py
--rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/compression.py
--rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/cursor.py
--rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/database.py
--rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/decorators.py
--rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/doc.py
--rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/exceptions.py
--rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/filterresult.py
--rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/index.py
--rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/invertedwordindex.py
--rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/manager.py
--rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/metadata.py
--rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/objectid.py
--rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/serialiser.py
--rwxr-xr-x   0        0        0    42032 2023-06-28 13:30:21.439050 orbit_database-1.0.5/orbit_database/table.py
--rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.5/orbit_database/types_.py
--rw-r--r--   0        0        0     1586 2023-07-07 15:17:34.783200 orbit_database-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 orbit_database-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2023-07-10 11:40:57.750728 orbit_database-1.0.8/LICENSE
+-rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.8/README.md
+-rw-r--r--   0        0        0    11742 2023-07-20 11:40:37.477611 orbit_database-1.0.8/orbit_database/README.md
+-rwxr-xr-x   0        0        0     1704 2023-07-20 16:45:35.159798 orbit_database-1.0.8/orbit_database/__init__.py
+-rw-r--r--   0        0        0    12072 2023-07-13 10:32:02.872543 orbit_database-1.0.8/orbit_database/audit.py
+-rwxr-xr-x   0        0        0     5871 2023-07-14 16:59:42.872426 orbit_database-1.0.8/orbit_database/bitmap.py
+-rw-r--r--   0        0        0    10583 2023-07-14 16:01:02.995067 orbit_database-1.0.8/orbit_database/catalog.py
+-rwxr-xr-x   0        0        0    12884 2023-07-14 17:23:52.638047 orbit_database-1.0.8/orbit_database/compression.py
+-rwxr-xr-x   0        0        0     2977 2023-07-12 16:54:21.028013 orbit_database-1.0.8/orbit_database/cursor.py
+-rwxr-xr-x   0        0        0    18112 2023-07-14 16:05:30.585403 orbit_database-1.0.8/orbit_database/database.py
+-rwxr-xr-x   0        0        0     9170 2023-07-14 17:25:02.376579 orbit_database-1.0.8/orbit_database/decorators.py
+-rwxr-xr-x   0        0        0    10893 2023-07-14 15:38:00.876206 orbit_database-1.0.8/orbit_database/doc.py
+-rwxr-xr-x   0        0        0     3510 2023-07-12 16:54:13.880156 orbit_database-1.0.8/orbit_database/exceptions.py
+-rwxr-xr-x   0        0        0     4418 2023-07-19 15:57:22.881621 orbit_database-1.0.8/orbit_database/filterresult.py
+-rwxr-xr-x   0        0        0    12319 2023-07-20 09:51:57.162788 orbit_database-1.0.8/orbit_database/index.py
+-rwxr-xr-x   0        0        0    23237 2023-07-20 09:50:43.468403 orbit_database-1.0.8/orbit_database/iwx.py
+-rwxr-xr-x   0        0        0     4107 2023-07-12 16:54:02.576382 orbit_database-1.0.8/orbit_database/manager.py
+-rw-r--r--   0        0        0     3155 2023-07-19 16:24:20.596560 orbit_database-1.0.8/orbit_database/matchresult.py
+-rwxr-xr-x   0        0        0    13806 2023-07-14 17:25:34.263907 orbit_database-1.0.8/orbit_database/metadata.py
+-rwxr-xr-x   0        0        0     6181 2023-07-12 16:53:21.277206 orbit_database-1.0.8/orbit_database/objectid.py
+-rwxr-xr-x   0        0        0     6222 2023-07-12 16:53:29.309046 orbit_database-1.0.8/orbit_database/serialiser.py
+-rwxr-xr-x   0        0        0    41512 2023-07-19 16:15:24.202772 orbit_database-1.0.8/orbit_database/table.py
+-rw-r--r--   0        0        0     1619 2023-07-20 16:45:35.159798 orbit_database-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 orbit_database-1.0.8/PKG-INFO
```

### Comparing `orbit_database-1.0.5/LICENSE` & `orbit_database-1.0.8/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE...!
```

### Comparing `orbit_database-1.0.5/README.md` & `orbit_database-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.5/orbit_database/__init__.py` & `orbit_database-1.0.8/orbit_database/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #####################################################################################
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 
-__version__ = "1.0.5"
+__version__ = "1.0.8"
 
 from orbit_database.manager import Manager
 from orbit_database.database import Database
 from orbit_database.table import Table
-from orbit_database.filterresult import FilterResult, MatchResult
+from orbit_database.filterresult import FilterResult
+from orbit_database.matchresult import MatchResult
 from orbit_database.index import Index
-from orbit_database.doc import Doc, JournalType
+from orbit_database.doc import Doc
 from orbit_database.compression import CompressionType
 from orbit_database.objectid import ObjectId
 from orbit_database.audit import AuditEntry
 from orbit_database.decorators import WriteTransaction, ReadTransaction, wrap_writer, wrap_reader
 from orbit_database.serialiser import Serialiser, SerialiserType
-from orbit_database.exceptions import IndexAlreadyExists, FailedToWriteMetadata, DocumentAlreadyExists, FailedToWriteData, \
-    DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex, NotDuplicateIndex, NoSuchTable, \
-    DuplicateKey, IndexWriteError, TableNotOpen, TrainingDataExists, InvalidSerialiser, InvalidId
+from orbit_database.exceptions import IndexAlreadyExists, \
+    DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex, NoSuchTable, \
+    DuplicateKey, TableNotOpen, TrainingDataExists, InvalidSerialiser, InvalidId
 from orbit_database.bitmap import Bitmap
-from orbit_database.invertedwordindex import InvertedWordIndex, Lexicon
+from orbit_database.iwx import InvertedWordIndex, Lexicon
 
 
 
 __all__ = [
     Manager,
     Database,
     Table,
@@ -35,30 +36,24 @@
     ObjectId,
     FilterResult,
     MatchResult,
     wrap_reader,
     wrap_writer,
     WriteTransaction,
     ReadTransaction,
-    JournalType,
     Serialiser,
     SerialiserType,
     IndexAlreadyExists,
-    FailedToWriteMetadata,
-    DocumentAlreadyExists,
-    FailedToWriteData,
     DocumentDoesntExist,
     InvalidId,
     InvalidKeySpecifier,
     InvalidSerialiser,
     NoSuchIndex,
-    NotDuplicateIndex,
     NoSuchTable,
     DuplicateKey,
-    IndexWriteError,
     TableNotOpen,
     TrainingDataExists,
     AuditEntry,
     Bitmap,
     InvertedWordIndex,
     Lexicon
 ]
```

### Comparing `orbit_database-1.0.5/orbit_database/database.py` & `orbit_database-1.0.8/orbit_database/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-#####################################################################################
-#
-#  Copyright (c) 2020 - Mad Penguin Consulting Ltd
-#
-#####################################################################################
-from __future__ import annotations
+"""
+██████╗  █████╗ ████████╗ █████╗ ██████╗  █████╗ ███████╗███████╗   ██████╗ ██╗   ██╗
+██╔══██╗██╔══██╗╚══██╔══╝██╔══██╗██╔══██╗██╔══██╗██╔════╝██╔════╝   ██╔══██╗╚██╗ ██╔╝
+██║  ██║███████║   ██║   ███████║██████╔╝███████║███████╗█████╗     ██████╔╝ ╚████╔╝ 
+██║  ██║██╔══██║   ██║   ██╔══██║██╔══██╗██╔══██║╚════██║██╔══╝     ██╔═══╝   ╚██╔╝  
+██████╔╝██║  ██║   ██║   ██║  ██║██████╔╝██║  ██║███████║███████╗██╗██║        ██║   
+╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═════╝ ╚═╝  ╚═╝╚══════╝╚══════╝╚═╝╚═╝        ╚═╝   
+
+The Database object models the top-level container for a collection of tables and indexes, each Database
+object maps to an LMDB database object. When you open a database there are a variety of low-level (LMDB)
+database settings that can be applied, it's worth understanding what some of them do as when you come to
+productionise your system, they will make a difference. Specifically you will want to tweak 'map_size'
+which is the maximum allowable size of your database, and possibly max_dbs if you are going to open large
+numbers of tables at the same time.
+"""
 from pathlib import Path
 from collections import UserDict
-from lmdb import Environment, Transaction as TXN, MapResizedError, NotFoundError
-from typing import Optional, Generator, Dict, Callable, ClassVar, Tuple
+from lmdb import Transaction as TXN, Environment, Transaction as MapResizedError
+from typing import Optional, Generator, Callable
+from typing_extensions import Self
 from orbit_database.doc import Doc
 from orbit_database.table import Table
 from orbit_database.audit import Auditor
 from orbit_database.serialiser import SerialiserType
 from orbit_database.compression import CompressionType
-from orbit_database.decorators import wrap_reader_yield, wrap_reader, WriteTransaction, transparent_resize
+from orbit_database.decorators import wrap_reader_yield, wrap_reader, wrap_writer, ReadTransaction, WriteTransaction, OrbitTransaction
 from orbit_database.exceptions import NoSuchTable
-from orbit_database.types_ import Config
 from orbit_database.metadata import MetaData
-from orbit_database.catalog import Catalog, CatalogEntry
+from orbit_database.catalog import Catalog
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
     import logging as log  # pragma: no cover
 
 
 class Database(UserDict):
     """
-    The Database object models the top-level container for a collection of tables and indexes, each Database
-    object maps to an LMDB database object. When you open a database there are a variety of low-level (LMDB)
-    database settings that can be applied, it's worth understanding what some of them do as when you come to
-    productionise your system, they will make a difference. Specifically you will want to tweak 'map_size'
-    which is the maximum allowable size of your database, and possibly max_dbs if you are going to open large
-    numbers of tables at the same time.
+    These class properties map directly onto LMDB and will directly affect how your database performs. If in doubt
+    run with the default settings until you get a feel for the setup you need. Mostly, the defaults should be fine.
     ---
     sync:        If False, don’t flush system buffers to disk when committing a transaction. This optimization means
                  a system crash can corrupt the database or lose the last transactions if buffers are not yet flushed
                  to disk. The risk is governed by how often the system flushes dirty buffers to disk and how often
                  sync() is called. However, if the filesystem preserves write order and writemap=False, transactions
                  exhibit ACI (atomicity, consistency, isolation) properties and only lose D (durability). I.e.
                  database integrity is maintained, but a system crash may undo the final transactions. Note that
@@ -92,47 +97,102 @@
         'create': True,
         'writemap': True,
         'metasync': False,
         'readahead': True,
         'map_async': True,
         'max_readers': 512,
         'max_dbs': 512,
-        # 'map_size': 2147483648
     }
 
     @property
-    def auditor (self):
+    def auditor (self) -> Auditor:
+        """
+        > Returns an instance to the databases auditor thread
+        """
         return self._auditor
 
+    @property
+    def index_version (self) -> int:
+        """
+        > Returns the index version number for this database (1 or 2)
+        """
+        return self._cat.version if self._cat else 0
+
+    @property
+    def isopen(self) -> bool:
+        """
+        > Returns True is the database is currently open
+        """
+        return True if hasattr(self, '_db') and self._db else False
+
+    @property
+    def map_size(self) -> int:
+        """
+        > Return the currently mapped database size
+        """
+        return self.env.info()['map_size']
+
+    @property
+    def read_transaction(self) -> ReadTransaction:
+        """
+        > Return a read-only transaction for use with "with"
+        """
+        return ReadTransaction(self)
+    
+    @property
+    def storage_allocated(self) -> int:
+        """
+        > Return the amount of storage space pre-allocated to this database
+        Assumes the underlying filesystem supports 'sparse' storage, this allocation will not 
+        reflect the amount of disk space 'actually' used. (see 'storage_used')
+        """
+        path = Path(self._path) / ("data.mdb" if self._conf.get('subdir') else "")
+        return path.stat().st_size
+    
+    @property
+    def write_transaction(self) -> WriteTransaction:
+        """
+        > Return a write-transaction for use with "with"
+        """
+        return WriteTransaction(self)
+
     def __init__(self) -> None:
         """
-        Initialise this object
+        Initialise this structure so it's ready for use
         """
         super().__init__()
         self.reset()
         
-    def reset (self):
+    def reset (self) -> None:
+        """
+        Perform a reset, used by __init__ and close(), zero all variables
+        """
         self.meta = None
         self.auto_resize = False
         self._conf = dict(self.CONFIG)
         self._auditor = None
         self._auditing = None
-        # self._index_version = 1
-        # self._catalog = None
         self._path = None
         self._cat = None
         self._db = None
         self.env = None
         self.data = {}
 
     def __getitem__(self, name: str) -> Table:
         """
-        Shortcut to self.table
+        Shortcut for the .table method, essentially this class presents as an 
+        array of tables, so if you instantiate at 'db' then you can get a table
+        reference with;
+        
+        ```
+        table_ref = db['table'] 
+        ```
 
         name - the name of the table to recover
+        > Returns a table reference
         """
         if name not in self.data:
             self.data[name] = Table(self, name)
         return self.data[name]
 
     def __repr__(self) -> str:
         """
@@ -144,21 +204,32 @@
               table_name: str,
               codec: SerialiserType=SerialiserType.NONE,
               compression_type=CompressionType.NONE,
               compression_level=None,
               integerkey: bool=False,
               auditing: bool=False,
               callback: Callable=None,
-              txn: Optional[TXN]=None,
+              txn: Optional[WriteTransaction]=None,
               cls: Optional[Doc]=Doc,
-              defer: Callable=False) -> Table:
+              defer: bool=False) -> Table:
         """
-        Returns the table associated with the supplied name
+        Recover a usable reference to the named table. If the table does not exist it
+        will be created, if it's not open it will be opened.
 
-        table_name - the name of the table to recover
+        table_name - the name of the table to provide a reference to
+        codec - the type of serialiser to use on the table
+        compression_type - the type of compression to use on the table
+        compression_level - the level of compression, only make sense with compression_type
+        integerkey - use an integer primary key rather than a string
+        auditing - whether changes to the table should be recorded in the audit table
+        callback - the default callback routine to call when changes in the table are observed
+        txn - an optional transaction wrapper
+        cls - the ORM class to be associated with objects returned from the table
+        defer - if True and the table is closed, don't try to open it
+        > Returns a Table object
         """
         if table_name not in self.data:
             cls.table = self.data[table_name] = Table(self, table_name, cls)
         if not defer:
             cls.table = self.data[table_name]
             if not self.data[table_name].isopen:
                 self.data[table_name].open(
@@ -167,78 +238,52 @@
                     compression_level=compression_level,
                     integerkey=integerkey,
                     auditing=auditing,
                     callback=callback,
                     txn=txn)
         return self.data[table_name]
 
-    @property
-    def isopen(self) -> bool:
-        """
-        Return True is the database is currently open
-        """
-        return True if hasattr(self, '_db') and self._db else False
-
-    @property
-    def map_size(self) -> int:
-        """
-        Return the currently mapped database size
-        """
-        return self.env.info()['map_size']
-
     @wrap_reader
-    def storage_used(self, txn: Optional[TXN]=None) -> Tuple[int, Dict[str, int]]:
+    def storage_used(self, txn: Optional[OrbitTransaction]=None) -> tuple[int, dict[str,int]]:
         """
         Return a tuple that represents the amount of storage space consumed by this database.
         The first entry in the tuple is the number of bytes occupied by data, the second is
         a tuple representing the size (in bytes) and name of each table in the database.
 
         txn - an optional transaction to wrap this operation
+        > Returns a tuple, [0] is total bytes, [1] is a dict of table name / bytes
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         total_bytes = 0
         results = {}
-        for name in self.tables(all=True, txn=transaction):
+        for name in self.tables(all=True, txn=txn):
             used = self.table(name).storage_used()
             total_bytes += used
             results[name] = used
         return total_bytes, results
 
-    @property
-    def storage_allocated(self):
-        """
-        Return the amount of storage space pre-allocated to this database, assuming the
-        underlying filesystem supports 'sparse' storage, this allocation will not reflect
-        the amount of disk space 'actually' used. (see 'storage_used')
-        """
-        path = Path(self._path) / ("data.mdb" if self._conf.get('subdir') else "")
-        return path.stat().st_size
-
     @wrap_reader_yield
-    def tables(self, all: bool=False, txn: Optional[TXN]=None) -> Generator[str, None, None]:
+    def tables(self, all: bool=False, txn: Optional[OrbitTransaction]=None) -> Generator[str, None, None]:
         """
         Generate a list of tables available in this database
 
         all - if True also show hidden / structural tables
         txn - an optional transaction
         """
         if self.index_version == 1:
-            transaction = txn if isinstance(txn, TXN) else txn.txn
-            with transaction.cursor(self._db) as cursor:
+            with txn.txn.cursor(self._db) as cursor:
                 while cursor.next():
                     try:
                         name = cursor.key().decode()
                     except UnicodeDecodeError:
                         continue
                     if (name[0] not in ['_', '~', '@']) or all:
                         yield name
         elif self.index_version == 2:
             if all:
-                transaction = txn if isinstance(txn, TXN) else txn.txn
-                with transaction.cursor(self._db) as cursor:
+                with txn.txn.cursor(self._db) as cursor:
                     while cursor.next():
                         try:
                             name = cursor.key().decode()
                         except UnicodeDecodeError:
                             continue
                         if name.startswith('@@'):
                             yield name
@@ -254,35 +299,15 @@
         self.env.sync(force)
 
     # @property
     # def name(self):
     #     """Return the unique name (uuid) of this database for replication"""
     #     return self.replication.uuid
 
-    @property
-    def index_version (self) -> int:
-        return self._cat.version if self._cat else 0
-
-    @property
-    def write_transaction(self) -> TXN:
-        """Return a write-transaction for this database"""
-        return WriteTransaction(self)
-
-    @property
-    def read_transaction(self) -> TXN:
-        """
-        Return a read-only transaction for use with "with"
-        """
-        try:
-            return self.env.begin()  # TODO: need multiple processes to test this
-        except MapResizedError:      # pragma: no cover
-            self.env.set_mapsize(0)  # pragma: no cover
-            return self.env.begin()  # pragma: no cover
-
-    def configure(self, config: Config) -> Database:
+    def configure(self, config: dict) -> Self:
         """
         Adjust the database configuration
         Return a reference to the current database instance
         """
         if not config:
             config = {}
         else:
@@ -299,30 +324,31 @@
                 setattr(self, f'flag_{param}', config.get(param, False))
             if param in config:
                 del config[param]
 
         self._conf = dict(self._conf, **config)
         return self
 
-    def open(self, path: str, name: str=None) -> Database:
+    def open(self, path: str, name: str=None) -> Self:
         """
         Open the database
 
         path - the location of the database files
 
         Returns a reference to the Database object
         """
         if self.isopen:
             return self
         self._path = path
         self._name = name
         self.env = Environment(path, **self._conf)
         self._cat = Catalog(getattr(self, 'flag_version', None))
         self._db = self.env.open_db()
-        with TXN(env=self.env, write=True) as txn:
+        # with TXN(env=self.env, write=True) as txn:
+        with WriteTransaction(self) as txn:
             self._cat.open(self, txn=txn)
             self.meta = MetaData(self).open(txn=txn)
         self._auditor = Auditor(self).open(self._auditing)
         return
 
     def close(self) -> None:
         """Close this database if it is open"""
@@ -345,42 +371,39 @@
     def reopen(self) -> None:
         """
         Reopen a database and all of it's tables
 
         After calling set_mapsize to resize the database, individual database handles
         are potentially invalidated, hence the save option is to reopen everything.
         """
-        @transparent_resize
-        def openup(db, txn=None):
+        @wrap_writer
+        def openup(txn=None):
             self._db = self.env.open_db()
             if self.meta:
                 self.meta.reopen(txn=txn)
 
-        # self.open(self._path)
-        openup(self)
-        for table_name, table in self.data.items():
+        openup()
+        for table in self.data.values():
             table.reopen()
 
-    def drop(self, name: str, txn: Optional[TXN]=None) -> None:
+    def drop(self, name: str, txn: Optional[WriteTransaction]=None) -> None:
         """
         Drop (delete) a database table
 
         name - name of table to drop
         txn - an optional transaction
         """
         if name not in self.data:
             raise NoSuchTable
         self.data[name].droptable(txn=txn)
         del self.data[name]
 
-    def register_norm(self, cls: Doc, nogql: Optional[Doc]=None, audit: bool=False, gpg=None):
+    def register_norm(self, cls: Doc, nogql: Optional[Doc]=None, audit: bool=False, gpg=None) -> None:
+        """
+        This is used by the ORM system to link an ORM model with a database table.
+        
+        cls - the class definition to link to
+        nogql - the noql reference to insert
+        audit - whether auditing should be enabled
+        gpg - a reference to the gpg background processor
+        """
         cls.reset(self, nogql, audit, gpg)
-
-    def drop_obsolete_indexes(self):
-        for table_name in self.tables():
-            log.warning(f'> Table > {table_name}')
-            table = self.table(table_name)
-            for index_name in table:
-                log.success(f'> Index > {index_name}')
-                index = table[index_name]
-                if not hasattr(index, 'reindexed'):
-                    log.error(f'Dead Index: {index_name}')
```

### Comparing `orbit_database-1.0.5/orbit_database/doc.py` & `orbit_database-1.0.8/orbit_database/doc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,60 @@
-#####################################################################################
-#
-#  Copyright (c) 2020 - Mad Penguin Consulting Ltd
-#
-#####################################################################################
+"""
+██████╗  ██████╗  ██████╗   ██████╗ ██╗   ██╗
+██╔══██╗██╔═══██╗██╔════╝   ██╔══██╗╚██╗ ██╔╝
+██║  ██║██║   ██║██║        ██████╔╝ ╚████╔╝ 
+██║  ██║██║   ██║██║        ██╔═══╝   ╚██╔╝  
+██████╔╝╚██████╔╝╚██████╗██╗██║        ██║   
+╚═════╝  ╚═════╝  ╚═════╝╚═╝╚═╝        ╚═╝   
+
+Records (or documents in NoSQL terminology) recovered from or stored in the database are
+always wrapped in a Doc object. It performs a number of crucial functions including;
+
+o Associating a data buffer with a key (OID)
+o Tracking updated attributes between the last read record and the current buffer
+o Tracking deleted attributes
+o Serialising and deserialising data between the database and user buffers
+o Providing a dict and object-like interfaces to interact with the data
+"""
 from __future__ import annotations
-from enum import Enum
-from typing import TYPE_CHECKING, Any, Optional, KeysView, ItemsView, ValuesView, Dict, List
+from typing import Any, Optional, KeysView, ItemsView, ValuesView, TypeVar
+from typing_extensions import Self
 from lmdb import Transaction as TXN
 from struct import pack, unpack
 from orbit_database.objectid import ObjectId
 
+Table = TypeVar('Table')
+
 try:
     from loguru import logger as log
 except ModuleNotFoundError:
     import logging as log
 
-if TYPE_CHECKING:
-    from .table import Table  # pragma: no cover
-
-
-class JournalType(Enum):
-    """
-    """
-    CREATE = 'C'
-    UPDATE = 'U'
-    APPEND = 'A'
-    DELETE = 'D'
-    ENSURE = 'E'
-    REMOVE = 'R'
-    SNAPXX = 'S'
-    DROPIX = 'I'
-
 
 class Doc(object):
     """
-    The Doc object is used to encapsulate data records before they are written to the
-    database and after they are read from the database. It performs a number of crucial
-    functions including;
-
-    o Associating a data buffer with a key (OID)
-    o Tracking updated attributes between the last read record and the current buffer
-    o Tracking deleted attributes
-    o Serialising and deserialising data between the database and user buffers
-    o Providing a dict and object-like interfaces to interact with the data
-
-    Note that this interface is 'slower' than using a raw 'dict' as in version 1, however
-    the use of 'Doc' facilitates the new 'C' extension (which should be a drop-in replacement
-    for 'Doc') which should be much faster, and this in turn facilitates the new GOBJECT
-    serialisation mechanism that should provide a 2-10x performance increase.
+    This class represents a database records (or document) and provides some very powerful features.
+    It behaves a little like an enhanced dictionary so you can access the fields within the record
+    either by using dictionary notation and supplying the field name in square brackets, or by using
+    an underscore folled by the field name. You can also initialise a Doc object from a dictionary,
+    so for example;
+    ```
+    doc = Doc({'name': 'Fred', 'age': 21})
+    print(f'{doc["name"]} is {doc._age} years old')
+    ```
+    Whereas the latter notation is much more readable, the ability access using normal dictionary
+    notation is often useful when the field name is dynamic.
     """
 
     def __init__(
             self,
-            doc: Optional[Dict]=None,
+            doc: Optional[dict]=None,
             oid: Optional[bytes|str]=None,
-            dat: Optional[Dict]=None,
-            words: Optional[List[str]]=None,
+            dat: Optional[dict]=None,
+            words: Optional[list[str]]=None,
             integerkey=False) -> None:
         """
         Instantiate a Doc object either based on a Dict or Cursor object. In the event a Cursor object
         is supplied, the (upd) field is set to cursor.value() and (oid) is set to cursor.key(). If a dict
         is supplied, (upd) is set to the value of the dict supplied, and oid is either set to the supplied
         oid or left as None by default.
 
@@ -78,231 +73,220 @@
         self.dat = dat or {}
         self.rem = []
         self.words = words or []
 
     @property
     def changed(self) -> bool:
         """
-        Return True is the Doc has changed since it was read from the database. Changes are indicated by
-        something in (rem) which signifies a field has been deleted or something in (upd) which
-        signifies something has been added or updated.
+        The object records changes so that it can report those changes to the auditing sub-system. This
+        property indicates whether the document has been changed since it was first instantiated or
+        read from the database.
+        > Returns True is the Doc has changed since it was read from the database otherwise False
         """
         return len(self.upd) != 0 or len(self.rem) != 0
+       
+    @property
+    def doc(self) -> dict:
+        """
+        > Return the current data within the buffer, typically this is initial state + changes
+        """
+        if isinstance(self.dat, dict) and isinstance(self.upd, dict):
+            return dict(self.dat, **self.upd)
+        return self.upd or self.dat
+
+    @property
+    def doc_with_id(self) -> dict:
+        """
+        > Return the current data within the buffer, typically this is initial state + changes + _id
+        """
+        if isinstance(self.dat, dict) and isinstance(self.upd, dict):
+            return dict(self.dat, **self.upd, _id=self.key)
+        return self.upd or self.dat
 
     @property
     def key(self) -> str:
         """
-        Return the current key (oid) for this document
+        > Returns the current key (oid) for this document
         """
         if not self.oid:
             return None
         try:
             return unpack('=Q', self.oid)[0] if self.integerkey else self.oid.decode()
         except UnicodeDecodeError:
             return unpack('=Q', self.oid)[0]
 
-    def journal_entry(self, jtype: JournalType, table_name: str) -> Dict[str, Dict]:
-        """Return a Journal entry for the current object"""
-        return {
-            'mod': jtype.value,
-            'table': table_name,
-            'key': self.key,
-            'upd': self.upd,
-            'rem': self.rem
-        }
-
-    def snapshot_entry(self, jtype: JournalType, table_name: str) -> Dict[str, Dict]:
-        """Return a Snapshot entry for the current object"""
-        return {  # pragma: no cover
-            'mod': jtype.value,
-            'table': table_name,
-            'key': self.key,
-            'upd': self.dat
-        }
-
-    def __getattr__(self, key: str) -> Any:
+    def __bool__(self):
         """
-        Return the data item associated with 'key' (dropping the '_' prefix)
-
-        key - data item name prefixed with an underscore
+        > Always return True for a Doc object
         """
-        if key[0] == '_':
-            key = key[1:]
-            return self.upd.get(key, self.dat.get(key))
-        return object.__getattribute__(self, key)
-        # raise AttributeError(f'unable to find key: {key}')
-
-    # def __getattribute__(self, key: str) -> Any:
-    #     if key[0] == '_' and key[1] != '_':
-    #         key = key[1:]
-    #         return self.upd.get(key, self.dat.get(key))
-    #     return object.__getattribute__(self, key)
+        return True
+    
+    def __contains__(self, key: str) -> bool:
+        """
+        Determine whether a given field name is present within the
+        current document, typically accessed as;
+        ```
+        if 'field' in doc:
+            ...
+        ```
+        > Return True if the field exists in this instance otherwise False
+        """
+        return key in self.doc
 
-    def pop (self, key: str) -> bytes:
+    def __delitem__(self, key: str):
+        """
+        Delete the field associated with the named key, typically accessed by;
+        ```
+        del doc['field']
+        ```
+        key - the field name to delete
+        """
         if key in self.upd:
-            self.upd.pop(key)
+            del self.upd[key]
         if key in self.dat:
-            ret = self.dat.pop(key)
+            del self.dat[key]
             self.rem.append(key)
-            return ret
-        return None
-
-    # def pop(self, key: str) -> None:
-    #     """Delete the named attribute"""
-    #     if key in self.upd:
-    #         del self.upd[key]
-    #     if key in self.dat:
-    #         del self.dat[key]
-    #         self.rem.append(key)
 
-    def __repr__(self) -> str:
+    def __eq__(self, doc: object):
         """
-        Return a string representation of the Doc object
+        The Equality operator for the doc object taking into account the type, oid, field contents
+        and deleted field contents.
+        > Returns True if both objects contain the same details, otherwise False
+        doc - The 'other' document to compare to (typically of type Doc)
         """
-        return f'{type(self)} with id={self.oid}'
+        return (type(self) == type(doc)) and (self.oid == doc.oid) and \
+                (self.doc == doc.doc) and (self.rem == doc.rem)
 
-    def __len__(self) -> int:
+    def __getattr__(self, key: str) -> Any:
         """
-        Return the current length of the output buffer
+        Recover a value from this structure. If the key begins with an underscore, the field
+        with matching name (after dropping the '_') will be recovered. Otherwise, the
+        appropriate attribite will be returned.
+        > Returns the data item associated with 'key' (dropping the '_' prefix)
+
+        key - item to recover, prefix with an '_' to recover field names
         """
-        return len(self.dat) + len(self.upd)
+        if key[0] == '_':
+            key = key[1:]
+            return self.upd.get(key, self.dat.get(key))
+        return object.__getattribute__(self, key)
 
     def __getitem__(self, key: str) -> Any:
         """
         Return the data item associated with 'key'
 
         key - data item name
         """
         return self.upd.get(key, self.dat.get(key))
 
-    def __delitem__(self, key: str) -> None:
+    def __len__(self) -> int:
         """
-        Delete the data item associated with key
+        > Return the length of the current buffer
+        """
+        return len(self.dat) + len(self.upd)
 
-        key - data item name
+    def __repr__(self) -> str:
         """
-        if key in self.upd:
-            del self.upd[key]
-        if key in self.dat:
-            del self.dat[key]
-            self.rem.append(key)
+        > Returns a string representation of the Doc object
+        """
+        return f'{type(self)} with id={self.oid}'
 
-    def __setattr__(self, key: str, val: Any) -> None:
+    def __setattr__(self, key: str, val: Any):
         """
-        Set the data item associated with 'key' (dropping the '_' prefix)
+        If the key is prefixed with an underscore then set the matching field
+        (after dropping the '_') to the value specified. Otherwise set the matching
+        property of this object to the value specified.
 
-        key - data item name prefixed with an underscore
+        key - field name (if prefixed with '_') or property name
         val - actual data item to associate with key
         """
         if key[0] == '_':
             k = key[1:]
             if k not in self.old:
-                # log.critical(f'setting old: {k} => {self.upd.get(k, self.dat.get(k))}')
                 self.old[k] = self.upd.get(k, self.dat.get(k))
             self.upd[k] = val
         else:
             object.__setattr__(self, key, val)
 
-    def __setitem__(self, key: str, val: Any) -> None:
+    def __setitem__(self, key: str, val: Any):
         """
-        Set the data item associated with 'key' (dropping the '_' prefix)
+        Set the named field to be the specified value.
 
         key - data item name prefixed with an underscore
         val - actual data item to associate with key
         """
         if key not in self.old:
             self.old[key] = self.upd.get(key, self.dat.get(key))
         self.upd[key] = val
 
-    def __contains__(self, key: str) -> bool:
-        """
-        Return True if the field exists in this instance.
-
-        key - the key to look for
-        """
-        return key in self.doc
-
-    def __eq__(self, o):
-        """Equal operator for a Doc object"""
-        return (type(self) == type(o)) and (self.oid == o.oid) and (self.doc == o.doc) and (self.rem == o.rem)
-
-    # def __ne__(self, o):
-    #     """Not Equal operator for a Doc object"""
-    #     print("NE>", self, self.__eq__)
-    #     return not object.__eq__(self, o)
-
-    def __bool__(self):
-        """Always return True for a Doc object"""
-        return True
-
-    def get(self, table: Table, txn: TXN) -> Optional[Doc]:
+    def get(self, table: Table, txn: OrbitTransaction) -> Optional[Self|None]:
         """
         Populate this structure by reading data from the database
 
-        db - open database handle
+        table - open table reference
         txn - active database transaction
 
-        Returns a reference to self
+        > Returns a reference to self or None if the document doesn't exist
         """
-        dat = txn.get(self.oid, db=table._db)
+        dat = txn.txn.get(self.oid, db=table._db)
         if dat:
             self.dat = table._decompressor(dat)
             return self
         return None
 
+    def items(self) -> ItemsView:
+        """
+        This is the equivalent of dict.items() the difference being we are
+        incorporating the original state of the object and subsequent changes.
+        > Returns a list of tuples where each tuple is (key, val)
+        """
+        return dict(self.dat, **self.upd).items()
+
+    def keys(self) -> KeysView:
+        """
+        This is the equivalent of dict.keys() the difference being we are
+        incorporating the original state of the object and subsequent changes.
+        > Returns a list of keys
+        """
+        return dict(self.dat, **self.upd).keys()
+
+    def pop (self, key: str) -> Optional[bytes|None]:
+        """
+        Remove the named key from the record removing it from both the origin
+        buffer and the update buffer as appropriate.
+        > Return the value removed IF it was present in the origin buffer else None
+        """
+        if key in self.upd:
+            self.upd.pop(key)
+        if key in self.dat:
+            ret = self.dat.pop(key)
+            self.rem.append(key)
+            return ret
+        return None
+
     def put(self, table: Table, append: bool=False, txn: TXN=None) -> None:
         """
-        Store the current output buffer back in the database
+        Store the current document buffer back to the database
 
-        db - open database handle
+        table - an active table reference
         append - whether to use "append" mode
         txn - active database transaction
         """
         if not self.oid:
             self.oid = str(ObjectId()).encode()
         txn.put(self.oid, table._compressor(self), append=append, db=table._db)
 
     def update(self, raw: bytes) -> None:
         """
-        Set the update buffer using a RAW string, this is used exclusively for the RAW serialiser type.
+        Set the update buffer using a RAW string, this is used exclusively by the RAW serialiser
 
         raw - bytes to assign to doc data component
         """
         self.upd = raw
 
-    def keys(self) -> KeysView:
-        """
-        Return the equivalent of dict.keys() for our current buffer
-        """
-        return dict(self.dat, **self.upd).keys()
-
-    def items(self) -> ItemsView:
-        """
-        Return the equivalent of dict.items() for our current buffer
-        """
-        return dict(self.dat, **self.upd).items()
-
     def values(self) -> ValuesView:
         """
-        Return the equivalent of dict.values() for our current buffer
+        This is the equivalent of dict.values() the difference being we are
+        incorporating the original state of the object and subsequent changes.
+        > Returns a list of values
         """
         return dict(self.dat, **self.upd).values()
-
-    @property
-    def doc(self) -> Dict[str, Any]:
-        """
-        Return the new buffer as a dictionary, i.e. the old + updates
-        """
-        if isinstance(self.dat, dict) and isinstance(self.upd, dict):
-            return dict(self.dat, **self.upd)
-        return self.upd or self.dat
-
-    @property
-    def doc_with_id(self) -> Dict[str, Any]:
-        """
-        Return the new buffer as a dictionary, i.e. the old + updates
-        """
-        if isinstance(self.dat, dict) and isinstance(self.upd, dict):
-            return dict(self.dat, **self.upd, _id=self.key)
-        return self.upd or self.dat
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orbit_database-1.0.5/orbit_database/metadata.py` & `orbit_database-1.0.8/orbit_database/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-#####################################################################################
-#
-#  Copyright (c) 2020 - Mad Penguin Consulting Ltd
-#
-#####################################################################################
-from __future__ import annotations
+"""
+███╗   ███╗███████╗████████╗ █████╗ ██████╗  █████╗ ████████╗ █████╗    ██████╗ ██╗   ██╗
+████╗ ████║██╔════╝╚══██╔══╝██╔══██╗██╔══██╗██╔══██╗╚══██╔══╝██╔══██╗   ██╔══██╗╚██╗ ██╔╝
+██╔████╔██║█████╗     ██║   ███████║██║  ██║███████║   ██║   ███████║   ██████╔╝ ╚████╔╝ 
+██║╚██╔╝██║██╔══╝     ██║   ██╔══██║██║  ██║██╔══██║   ██║   ██╔══██║   ██╔═══╝   ╚██╔╝  
+██║ ╚═╝ ██║███████╗   ██║   ██║  ██║██████╔╝██║  ██║   ██║   ██║  ██║██╗██║        ██║   
+╚═╝     ╚═╝╚══════╝   ╚═╝   ╚═╝  ╚═╝╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝╚═╝        ╚═╝   
+
+This is a legacy module mostly for handling catalog version 1 metadata access. This will
+be phased out over time once V1 databases are no longer supported.
+"""
 from struct import pack, unpack
-from typing import TYPE_CHECKING, Tuple, Generator
+from typing import Tuple, Generator, TypeVar, Optional
+from typing_extensions import Self
 from lmdb import Transaction as TXN
 from orbit_database.doc import Doc
-from orbit_database.decorators import wrap_reader_yield, wrap_reader, transparent_resize, WriteTransaction
+from orbit_database.decorators import wrap_reader_yield, wrap_reader, wrap_writer, WriteTransaction, OrbitTransaction
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
     import logging as log  # pragma: no cover
 
-if TYPE_CHECKING:
-    from .database import Database  # pragma: no cover
+Database = TypeVar("Database")
 
 
 class MetaData:
     """
     This is a wrapper for the __metadata__ table, for which there should be
     'one' per database. This contains additional information including index
     definitions and other persistent information pertaining to tables or
@@ -43,29 +48,29 @@
 
         database - the database that holds the metadata table we'll be working with
         """
         self._table = None
         self._database = database
         self.env = database.env
 
-    def open(self, txn: TXN=None):
+    def open(self, txn: Optional[OrbitTransaction]=None) -> Self:
         """
         Open the __metadata__ table and make it available for IO
+        > Returns a reference to self
         """
         if self._table:
             return self  # pragma: no cover
 
         if self._database.index_version == 1:
             metadata_name = '__metadata__'
         elif self._database.index_version == 2:
             metadata_name = '@@metadata@@'
         else:
             raise Exception(f'no index version: {self._database.index_version}')
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        self._table = self._database.table(metadata_name, txn=transaction)
+        self._table = self._database.table(metadata_name, txn=txn)
         return self
 
     def reopen(self, txn: TXN=None):
         """
         Re-Open the __metadata__ table and make it available for IO
         """
         self._table.reopen(txn=txn)
@@ -76,15 +81,15 @@
         routine primarily used when opening a table to recover the names of the indexes
         associated with that table.
 
         table_name - name of the table the index is associated with
         index_name - the name of the index to recover information on
         txn - a read or write transaction to wrap the operation
 
-        Returns a Doc object containing a 'conf' key
+        > Returns a Doc object containing a 'conf' key
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         dat = transaction.get(self.path_index(table_name, index_name), db=self._table._db)
         return Doc(self._table.deserialise(dat) if dat else None)
 
     def store_index(self, table_name: str, index_name: str, value: Doc, txn: TXN=None) -> None:
         """
@@ -113,15 +118,15 @@
     def path_index(self, table_name: str, index_name: str) -> bytes:
         """
         Build a key for the __metadata__ table to access an index definition
 
         table_name - name of the table the index is associated with
         index_name - the name of the index
 
-        Returns the assembled key in bytes format ready to be used by get/put
+        > Returns the assembled key in bytes format ready to be used by get/put
         """
         return f'_{table_name}_{index_name}'.encode()
 
     def fetch_config(self, table_name: str, txn: TXN=None) -> Doc:
         """
         Fetch the configuration dictionary from the metadata table for the named table. This
         dictionary will contain table specific settings such as the compression mechanism
@@ -190,15 +195,15 @@
         table_name - the name of the table we're fetching tags for
         tag - the name of the specific tag we want
         """
         return f'_{table_name}!{tag}'.encode()
 
     # TODO: Add journal code in here ...
 
-    @transparent_resize
+    @wrap_writer
     def remove(self, name: str, txn: TXN=None) -> None:
         """
         Remove all keys from the database for the current table. This is used by
         'droptable' to clean any latent meta data from the metadata table when
         a table is dropped.
 
         name - name of the table to remove keys from
@@ -242,28 +247,28 @@
         key - the name of the specific tag we want
         txn - a transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         raw = transaction.get(key.encode(), db=self._table._db)
         return Doc(self._table.deserialise(raw), key) if raw else None
 
-    @transparent_resize
+    @wrap_writer
     def store_key(self, key: str, val: Doc, txn: TXN=None) -> None:
         """
         Store a key in the metadata table for a given name. This is for storing database
         specific information.
 
         key - the name of the specific key to store
         val - the value to associate with the key
         txn - a transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         transaction.put(key.encode(), self._table.serialise(val.doc), db=self._table._db)
 
-    @transparent_resize
+    @wrap_writer
     def store_int(self, key: str, val: int, txn: WriteTransaction=None) -> int:
         """
         Store a key against an integer in the metadata table, returning the value stored.
 
         key - the name of the specific key to store
         val - the value to associate with the key
         txn - a transaction to wrap the operation
@@ -280,49 +285,17 @@
         key - the name of the specific key to store
         txn - a transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         raw = transaction.get(key.encode(), db=self._table._db)
         return unpack('=Q', raw)[0] if raw else None
 
-    @transparent_resize
+    @wrap_writer
     def remove_key(self, key: str, txn: TXN=None) -> None:
         """
         Remove a key, used to remove database specific information.
 
         key - the key of the information to remove
         txn - a write transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         transaction.delete(key.encode(), db=self._table._db)
-
-    # def migrateIndecies (self, txn: TXN=None):
-    #     version = self.fetch_int('index_version', txn=txn)
-    #     if not version:
-    #         log.warning('Upgrading indecies to version # 1')
-    #         rename = []
-    #         transaction = txn if isinstance(txn, TXN) else txn.txn
-    #         with transaction.cursor(self._database._db) as cursor:
-    #             while cursor.next():
-    #                 try:
-    #                     table_name = cursor.key().decode()
-    #                 except UnicodeDecodeError:
-    #                     continue
-    #                 if (table_name[0] not in ['_', '~']):
-    #                     index_key = f'_{table_name}_'
-    #                     offset = len(index_key)
-    #                     with transaction.cursor(db=self._database._db) as sub:
-    #                         sub.set_range(index_key.encode())
-    #                         name = sub.key().decode()
-    #                         while name.startswith(index_key):
-    #                             rename.append((name, f'_{table_name}|{name[offset:]}'))
-    #                             if not sub.next():
-    #                                 break
-    #                             name = sub.key().decode()
-    #         for entry in rename:
-    #             log.warning(f'Rename: {entry[0]} => {entry[1]}')
-    #             with transaction.cursor(db=self._database._db) as cursor:
-    #                 cursor.get(entry[1].encode())
-    #                 cursor.delete(entry[1].encode())
-                    
-    #                 # cursor.replace(entry[1].encode(), cursor.value())
-    #                 break
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orbit_database-1.0.5/orbit_database/table.py` & `orbit_database-1.0.8/orbit_database/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,241 +1,220 @@
-#####################################################################################
-#
-#  Copyright (c) 2020 - Mad Penguin Consulting Ltd
-#
-#####################################################################################
-from __future__ import annotations
+"""
+████████╗ █████╗ ██████╗ ██╗     ███████╗   ██████╗ ██╗   ██╗
+╚══██╔══╝██╔══██╗██╔══██╗██║     ██╔════╝   ██╔══██╗╚██╗ ██╔╝
+   ██║   ███████║██████╔╝██║     █████╗     ██████╔╝ ╚████╔╝ 
+   ██║   ██╔══██║██╔══██╗██║     ██╔══╝     ██╔═══╝   ╚██╔╝  
+   ██║   ██║  ██║██████╔╝███████╗███████╗██╗██║        ██║   
+   ╚═╝   ╚═╝  ╚═╝╚═════╝ ╚══════╝╚══════╝╚═╝╚═╝        ╚═╝   
+
+The Table module controls all aspects of tables and does most of heavy lifting
+for the library. A table object behaves like a dictionary and it's contents
+enumerate to any indexes that have been defined for the table.
+"""
 from sys import maxsize as MAXSIZE
 from collections import UserDict
-from typing import Generator, Optional, TYPE_CHECKING, Union, Callable, ClassVar
-from lmdb import Transaction as TXN, MapResizedError, NotFoundError, IncompatibleError
+from typing import Generator, Optional, Union, Callable, Type, TypeVar, Collection
+from lmdb import Transaction as TXN, NotFoundError, IncompatibleError
 from struct import pack, unpack
 from orbit_database.index import Index
-from orbit_database.doc import Doc, JournalType
+from orbit_database.doc import Doc
 from orbit_database.compression import Compression, CompressionType
 from orbit_database.serialiser import Serialiser, SerialiserType
 from orbit_database.cursor import Cursor
 from orbit_database.objectid import ObjectId
-from orbit_database.filterresult import FilterResult, MatchResult
-from orbit_database.decorators import wrap_reader, wrap_reader_yield, WriteTransaction, wrap_writer
+from orbit_database.filterresult import FilterResult
+from orbit_database.matchresult import MatchResult
+from orbit_database.decorators import wrap_reader, wrap_reader_yield, ReadTransaction, WriteTransaction, OrbitTransaction, wrap_writer
 from orbit_database.exceptions import IndexAlreadyExists, DocumentDoesntExist, InvalidKeySpecifier, NoSuchIndex
-from orbit_database.types_ import Config, OID, OIDS
 from pathlib import Path
 from operator import gt as greater, lt as less
 from json import load, dump
 
 try:
     from loguru import logger as log
 except Exception:  # pragma: no cover
     import logging as log  # pragma: no cover
 
-
 ZERO = 0
-
-
-if TYPE_CHECKING:
-    from .database import Database  # pragma: no cover
+Database = TypeVar("Database")
+Table = TypeVar("Table")
+OID = TypeVar('OID', str, bytes)
+OIDS = Collection[OID]
 
 
 class Table(UserDict, Compression, Serialiser):
     """
-    The Table class is used to wrap access to individual database tables and
-    incorporates semi-transparent compression / decompression on a per table
-    basis. Compression libraries are pluggable and implemented in the
-    Compression class.
-
-    o APPEND_MODE - when appending a record we know that the new key will be the
-                    highest value in the table so we can take advantage of LMDB's
-                    "append" mode. If you never want to use this option, set
-                    orbit-database.Table.APPEND_MODE to False.
-
-                    NOTE: compatibility issue, we've switched to our own version
-                    of "ObjectId", if you set this to True and have data that
-                    uses both BSON/ObjectId and the new ObjectId, you will have
-                    a problem. (data loss)
+    The Table class is used to wrap access to individual database tables and incorporates
+    pluggable transparent compression and pluggable transparent serialisation on a per
+    table basis. 
     """
-    APPEND_MODE = False
+    @property
+    def isopen(self) -> bool:
+        """
+        > Returns True if the table if open, otherwise False
+        """
+        return False if self._db is None else True
+
+    @property
+    def oid (self) -> ObjectId:
+        """
+        The oid is the table's unique identifier. For version #1 indexes this will be the
+        name of the table, but for version #2 this will be an "ObjectId" which relates to
+        it's primary key in the LMDB primary index.
+        
+        > Returns the 'oid' for this table
+        """
+        return self._oid
+
+    @property
+    def read_transaction(self) -> ReadTransaction:
+        """
+        Use with "with" to begin a Read-Only transaction
+        """
+        return ReadTransaction(self._database)
+
+    @property
+    def write_transaction(self) -> WriteTransaction:
+        """
+        Use with "with" to begin a Read-Write transaction
+        """
+        return WriteTransaction(self._database)
 
-    def __init__(self, database: Database, name: str, cls: ClassVar=Doc) -> None:
+    def __init__(self, database: Database, name: str, cls: Type[Doc]=Doc):
         """
-        Intantiate a table instance bases on the name of the table required. A
-        reference to the containing database is also required so the table
-        can back-reference the database environment.
+        Intantiate a table instance based on the name of the table required.
 
         database - a reference to the containing database object
         name - the name of the table to reference
+        cls - the class to use as the default return type for seek and filterresult
         """
         self.name = name
         self.env = database.env
         self._database = database
         self._cls = cls
         self._db = None
         self._oid = None
         self._meta = database.meta
         UserDict.__init__(self)
         Compression.__init__(self)
 
-    def __setitem__(self, name: str, conf: Config) -> None:
+    def __setitem__(self, name: str, conf: dict):
         """
         Create an entry for an index with the specified name
 
         name - the name of the index to create
         conf - configuration options for the index we're creating
         """
         if name in self.data:
             raise IndexAlreadyExists(name)
         self.data[name] = Index(self, name, conf)
 
     def __repr__(self) -> str:
         """
-        Generate a string representation of this object, by default we include the
-        table name and the table status, i.e. whether it is open or not.
+        > Returns a string representation of this object
         """
         return f'<{__name__}.Table instance> name="{self.name}" status={"open" if self.isopen else "closed"}'
 
-    @property
-    def oid (self) -> ObjectId:
-        return self._oid
-
-    @property
-    def isopen(self) -> bool:
-        """
-        Return True if this table is open
-        """
-        return False if self._db is None else True
-
     @wrap_reader
-    def records(self, txn: Optional[TXN]=None) -> int:
+    def records(self, txn: Optional[OrbitTransaction]=None) -> int:
         """
-        Return the number of records in this table
+        > Returns the number of records in this table
 
         txn - an transaction to wrap the operation
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        return transaction.stat(self._db).get('entries', 0)
+        return txn.txn.stat(self._db).get('entries', 0)
 
     @wrap_reader
     def stat(self, txn: Optional[TXN]=None) -> int:
         """
-        Get the stat() buffer for this table
+        > Returns the stat() buffer for this table
 
         txn - an transaction to wrap the operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         return transaction.stat(self._db)
 
-    @property
-    def read_transaction(self) -> TXN:
-        """
-        Use with "with" to begin a Read-Only transaction
-        """
-        # return ReadTransaction(self._database)
-
-        try:
-            return self.env.begin()     # TODO: Need multiple processes to test this
-        except MapResizedError:         # pragma: no cover
-            self.env.set_mapsize(0)     # pragma: no cover
-            return self.env.begin()     # pragma: no cover
-
-    @property
-    def write_transaction(self) -> TXN:
-        """Return a write transaction for this database (compatibility only)"""
-        return WriteTransaction(self._database)
-
     @wrap_reader
-    def storage_used(self, txn: Optional[TXN]=None) -> int:
+    def storage_used(self, txn: Optional[OrbitTransaction]=None) -> int:
         """
-        Return the amount of storage space used by data contained within this table
+        > Return the amount of storage space used by data contained within this table
 
         txn - optional transaction to wrap this operation
         """
-        stat = txn.stat(self._db)
+        stat = txn.txn.stat(self._db)
         return stat['psize'] * (stat['leaf_pages'] + stat['branch_pages'] + stat['overflow_pages'] + 2)
 
     @wrap_writer
     def open(
             self,
             compression_type: Optional[CompressionType]=CompressionType.NONE,
             compression_level: Optional[int]=None,
             codec: SerialiserType=SerialiserType.NONE,
             integerkey: int=False,
             compress_existing: bool=False,
             auditing: bool=False,
             callback: Callable=None,
-            txn: Optional[TXN|WriteTransaction]=None) -> Table:
+            txn: Optional[WriteTransaction]=None) -> Table:
         """
         Open this table and make it available for use, if the compression type is set to
         anything other than NONE, the following the call the table will be set to read and
         write data using the selected compression mechanism, and any data in the table will
         be compressed.
 
         compression_type - the type of compression to use
         compression_level - the compression level to set
         txn - an optional transaction to wrap this request
+        > Returns a reference to the opened table
         """
         if self.isopen:
             return self
-
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        create = False
         self._compression_type = compression_type
         self._compression_level = compression_level
         self._codec = codec
         self.integerkey = integerkey
         self._auditing = auditing
 
         if not self.name.startswith('@@') and self._database.index_version == 2:
             self._oid = name = self._database._cat.get_table_id(self.name, txn)
         else:
             self._oid = self.name
             
         try:
-            self._db = self.env.open_db(
-                # self.name.encode() if isinstance(self.name, str) else self.name,
-                self._oid.encode(),
-                create=False,
-                integerkey=integerkey,
-                txn=transaction)
+            self._db = self.env.open_db(self._oid.encode(), integerkey=integerkey, txn=txn.txn)
         except NotFoundError:
-            create = True
-            self._db = self.env.open_db(
-                # self.name.encode(),
-                self._oid.encode(),
-                integerkey=integerkey,
-                txn=transaction)
+            self._db = self.env.open_db(self._oid.encode(), integerkey=integerkey, txn=txn.txn)
         except IncompatibleError as e:
             log.error(f'{self.name} => {self._oid}:: {str(e)}')
             return self
-       
         try:
-            Serialiser.__init__(self, codec, txn=transaction)
+            Serialiser.__init__(self, codec, txn=txn)
             if not self._meta:
                 return self
-            for index_name in self.indexes(txn=transaction):
+            for index_name in self.indexes(txn=txn):
                 if index_name in self.data:
                     # means the index is open so we're doing a 're-open'
-                    self.data[index_name].open(txn=transaction)  # pragma: no cover
+                    self.data[index_name].open(txn=txn)  # pragma: no cover
                 else:
                     if self._database.index_version == 1:
-                        doc = self._meta.fetch_index(self.name, index_name, txn=transaction)
+                        doc = self._meta.fetch_index(self.name, index_name, txn=txn)
                         if not doc['conf']:
                             break  # pragma: no cover
                         self.__setitem__(index_name, doc['conf'])
                     else:
                         # log.success(f'get meta: {self.name}/{index_name} => {self._database._cat.get_metadata(self.name, index_name)}')
                         self.__setitem__(index_name, self._database._cat.get_metadata(self.name, index_name))
                     
-                    self.data[index_name].open(txn=transaction)
+                    self.data[index_name].open(txn=txn)
             if compression_type and compression_type != CompressionType.NONE:
-                do_compress = self.compression_select(compression_type, compression_level, txn=transaction)
-                Compression.open(self, txn=transaction)
-                if compress_existing and do_compress and self.records(txn=transaction):
-                    self.compress_existing_data(txn=transaction)
+                do_compress = self.compression_select(compression_type, compression_level, txn=txn)
+                Compression.open(self, txn=txn)
+                if compress_existing and do_compress and self.records(txn=txn):
+                    self.compress_existing_data(txn=txn)
             else:
-                Compression.open(self, txn=transaction)
+                Compression.open(self, txn=txn)
             if auditing:
                 self._database._auditor.watch(self.name, callback)
             
         except Exception:
             try:
                 self.close()  # pragma: no cover
             except Exception:  # pragma: no cover
@@ -244,111 +223,106 @@
 
         return self
 
     @wrap_writer
     def droptable(self, txn: Optional[TXN|WriteTransaction]=None) -> None:
         """
         Drop the current table, this will empty the table, remove all the indexes,
-        remote the table itself, and remove all associated metadat.
+        remote the table itself, and remove all associated metadata
 
         txn - a write transaction to wrap this operation
         """
         transaction = txn if isinstance(txn, TXN) else txn.txn
         for index_name in self.data:
             self.data[index_name].drop(txn=txn)
-
         transaction.drop(self._db, True)
         self._database._cat.drop(self.name, txn)
-        # if self._database.index_version == 2:
-        #     self._database._catalog.delete(self.name, txn=txn)
         self._meta.remove(self.name, txn=txn)
 
     def close(self) -> None:
         """
         Close a table by essentially losing all references to it
         """
-        # log.error(f'close table: {self.name}')
-        # if self._database._auditor:
-        #     self._database._auditor.close()
         self._db = None
         self.data.clear()
         Compression.close(self)
 
     @wrap_writer
     def reopen(
         self,
         auditing: bool=False,
-        callback: Callable=None,
+        callback: Optional[Callable]=None,
         txn: Optional[TXN|WriteTransaction]=None) -> None:
         """
         ReOpen a table, used following a change to the map size. Everything should be the
         same, we just need new database handles.
+        
+        auditing - True is auditing is to be enabled on this table for this session
+        callback - The default routine to call when some data is changed within this table
+        txn - an optional transaction to wrap this request        
         """
         self.close()
         self.env = self._database.env
         self.open(
             self._compression_type,
             self._compression_level,
             self._codec,
             self.integerkey,
             auditing = auditing,
             callback = callback,
             txn=txn)
 
     @wrap_reader_yield
-    def indexes(self, txn: Optional[TXN]=None) -> Generator[str, None, None]:
+    def indexes(self, txn: Optional[ReadTransaction]=None) -> Generator[str, None, None]:
         """
         Generate a list if indexs (names) available for this table
 
         txn - an optional transaction
         """
         if self.name.startswith('@@'):
             return []
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         if self._database.index_version == 1:
-            metadata = self._database.table('__metadata__', txn=transaction)
+            metadata = self._database.table('__metadata__', txn=txn)
             index_key = Index.index_path(self.name, '')
             offset = len(index_key)
-            with transaction.cursor(db=metadata._db) as cursor:
+            with txn.txn.cursor(db=metadata._db) as cursor:
                 cursor.set_range(index_key.encode())
                 name = cursor.key().decode()
                 while name.startswith(index_key):
                     yield name[offset:]
                     if not cursor.next():
-                        break  # pragma: no cover
+                        break
                     name = cursor.key().decode()
         elif self._database.index_version == 2:
-            for name in self._database._cat.indexes(self.name, transaction):
+            for name in self._database._cat.indexes(self.name, txn):
                 yield name
-            # catalog = self._database._catalog.get(self.name, txn=transaction)
-            # for name in catalog._indexes or []:
-            #     yield name
-
 
     @wrap_writer
     def ensure(
             self,
             index_name: str,
             func: str=None,
             duplicates: bool=False,
             force: bool=False,
             lower: bool=False,
             iwx: bool=False,
             progress: Optional[Callable]=None,
-            txn: Optional[TXN|WriteTransaction]=None) -> Index:
+            txn: Optional[WriteTransaction]=None) -> Index:
         """
         Ensure that the specified index exists, if it does by default do nothing. If the
         index does not exist, or if the 'force' flag is true, the index will be (re)created
         using the new index function.
 
         index_name - the name of the required index
         func - a description of how index keys should be generated
         duplicates - whether this is a duplicate index or not
         force - whether to re-index the index if it already exists
+        lower - whether to force keys to lower case
         iwx - true if this index is an inverted word index
+        progress - a routine to call to display progress updates
         txn - an optional transaction
 
         The "func" parameter can take one of two forms, it can either be a Python format
         string (the only option in v1) or it can be a complete python function if prefixed
         with a 'def'. So for example as a format string;
         ```
         func = '{name}'         # index by name
@@ -376,141 +350,104 @@
         [print(person.doc) for person in people.find()]
         print('--')
         [print(person.doc) for person in people.find('by_age_fs')]
         print('--')
         [print(person.doc) for person in people.find('by_age_func')]
         ```
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        if self._database.index_version == 2 and iwx:
-            if index_name not in self.data or force:
-                if index_name in self.data:
-                    self.drop(index_name, txn=transaction)
-
-                catalog = self._database._cat.ensure(self.name, index_name, iwx, transaction)
-                conf = catalog._indexes[index_name]
-                self.__setitem__(index_name, conf)
-                self.data[index_name].open(txn=transaction)
-            return self.data[index_name]
-        #
-        #   Abstract get old conf
-        #   Abstract store_index
-        #
-
-        if self._database.index_version == 1:
-            old_conf = self._meta.fetch_index(self.name, index_name, txn=transaction)
-            if not old_conf._conf:
-                old_conf = {'key': Index.index_path(self.name, index_name)}
-            else:
-                old_conf = old_conf._conf
-        else:
-            try:
-                old_conf = self._database._cat.get_metadata(self.name, index_name)
-            except NotFoundError:
-                old_conf = { 'key': str(ObjectId()) }
-
-        new_conf = {
-            'key': old_conf['key'],
-            'dupsort': duplicates,
-            'create': True,
-            'func': func,
-            'iwx': iwx,
-            'lower': lower
-        }
-        force = old_conf != new_conf or force
+        old_conf = self._database._cat.get_conf(self._database,
+            self.name, index_name, iwx, txn)
+        new_conf = dict(old_conf, **{'dupsort': duplicates, 'create': True,
+            'func': func, 'iwx': iwx, 'lower': lower })
+        force = old_conf != new_conf or force       
         if index_name not in self.data or force:
             if index_name in self.data:
-                self.drop(index_name, txn=transaction)
+                self.drop(index_name, txn=txn)
             self.__setitem__(index_name, new_conf)
-            self.data[index_name].open(txn=transaction)
+            self._database._cat.put_conf(self._database,
+                self.name, index_name, new_conf, txn)
+            self.data[index_name].open(txn=txn)
             if force:
-                if self._database.index_version == 1:
-                    self._meta.store_index(self.name, index_name, Doc({'conf': new_conf}), txn=transaction)
-                else:
-                    self._database._cat.store_index(self.name, index_name, new_conf, txn=transaction)
-                self.reindex(index_name, progress=progress, txn=transaction)
+                self.reindex(index_name, progress=progress, txn=txn)
+                
         self.data[index_name].reindexed = force
         return self.data[index_name]
-
+                    
     @wrap_writer
-    def reindex(self, index_name: str, progress: Optional[Callable]=None, txn: Optional[TXN]=None) -> None:
+    def reindex(self, index_name: str, progress: Optional[Callable]=None, txn: Optional[WriteTransaction]=None) -> None:
         """
         Reindex the named index, assuming the index exists. The index is first emptied
         and then each record is reindexed, for a large table this can take some time
         and will lock the database while in progress.
 
         index_name - the name of the index to reindex
+        progress - a routine to call to display progress updates
         txn - a write transaction to wrap the operation
         """
-        # log.warning(f'Running reindex for {index_name} in {self.name}')
         if index_name not in self.data:
             raise NoSuchIndex
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        self.data[index_name].empty(txn=transaction)
-        with transaction.cursor(self._db) as cursor:
+        self.data[index_name].empty(txn=txn)
+        with txn.txn.cursor(self._db) as cursor:
             while cursor.next():
                 if progress:
                     progress.update(1)  # pragma: no cover
-                self.data[index_name].put_cursor(cursor, txn=transaction)
+                self.data[index_name].put_cursor(cursor, txn=txn)
 
     @wrap_writer
-    def append(self, doc: Doc, txn: Optional[TXN|WriteTransaction]=None) -> Doc:
+    def append(self, doc: Doc, txn: Optional[WriteTransaction]=None) -> Doc:
         """
         Append a new record to this table
 
         doc - the data to append
         txn - an optional transaction object
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         if not doc.oid:
             if self.integerkey:
-                with transaction.cursor(db=self._db) as cursor:
+                with txn.txn.cursor(db=self._db) as cursor:
                     if not cursor.last():
                         oid = 0
                     else:
                         oid = unpack('=Q', cursor.key())[0] + 1
                     doc.oid = pack('=Q', oid)
             else:
                 doc.oid = str(ObjectId()).encode()
-        transaction.put(doc.oid, self._compressor(doc), db=self._db)
+        txn.txn.put(doc.oid, self._compressor(doc), db=self._db)
         if self._auditing:
             self._database._auditor.append(self, doc, txn)
         for index_name in self.data:
-            self.data[index_name].put(doc, txn=transaction)
+            self.data[index_name].put(doc, txn=txn)
         return doc
 
     @wrap_writer
-    def save(self, doc: Doc, txn: Optional[TXN, WriteTransaction]=None) -> None:
+    def save(self, doc: Doc, txn: Optional[WriteTransaction]=None) -> None:
         """
         Update the current record in the table
 
         doc - the record to update
         txn - an optional transaction
         """
         if not doc.oid:
             raise DocumentDoesntExist
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        old_doc = Doc(None, doc.oid).get(self, txn=transaction)
+        old_doc = Doc(None, doc.oid).get(self, txn=txn)
         if self._auditing:
             if old_doc:
                 self._database._auditor.save(self, old_doc, txn)
             else:
                 log.error(f'Audit: no old document for oid: {doc.oid}')
-        transaction.put(doc.oid, self._compressor(doc), db=self._db)
+        txn.txn.put(doc.oid, self._compressor(doc), db=self._db)
         for index_name in self.data:
-            self.data[index_name].save(old_doc, doc, txn=transaction)
-
+            self.data[index_name].save(old_doc, doc, txn=txn)
 
     @wrap_reader_yield
     def find(
             self,
             index_name: str=None,
             expression: str=None,
             limit: int = MAXSIZE,
-            txn: Optional[TXN]=None) -> Generator[Doc, None, None]:
+            txn: Optional[OrbitTransaction]=None) -> Generator[Doc, None, None]:
         """
         Find records in this table either in natural (date) order, or in index order
 
         index_name - an optional index name for ordering
         expression - the expression to filter the sort on
         limit - the maximum number of records to return
         txn - an optional transaction
@@ -518,47 +455,46 @@
         if index_name:
             if index_name not in self.data:
                 raise NoSuchIndex(index_name)
             db = self.data[index_name]._db
         else:
             db = self._db
         #
-        with txn.cursor(db) as cursor:
+        with txn.txn.cursor(db) as cursor:
             count = 0
             while count < limit and cursor.next():
                 count += 1
                 record = cursor.value()
                 if index_name:
                     key = record
-                    record = txn.get(record, db=self._db)
+                    record = txn.txn.get(record, db=self._db)
                 else:
                     key = cursor.key()
 
                 record = self._decompressor(record)
                 if callable(expression) and not expression(record):
                     continue
                 yield Doc(None, key, record)
 
     @wrap_reader
-    def get(self, oid: [bytes, str], txn: Optional[TXN, WriteTransaction]=None) -> Doc:
+    def get(self, oid: bytes|str, txn: Optional[WriteTransaction]=None) -> Doc:
         """
         Recover a single record from the database based on it's primary key
 
         oid - primary key of record to recover
         txn - an optional active transaction
         """
         try:
-            transaction = txn if isinstance(txn, TXN) else txn.txn
-            return Doc(None, pack('=Q', oid) if self.integerkey else oid).get(self, txn=transaction)
+            return Doc(None, pack('=Q', oid) if self.integerkey else oid).get(self, txn=txn)
         except Exception as e:  # pragma: no cover
             log.exception(e)  # pragma: no cover
             log.error(f'key was: {oid}')  # pragma: no cover
 
     @wrap_writer
-    def delete(self, keyspec: Union[OID, OIDS, Doc], txn: Optional[TXN]=None) -> None:
+    def delete(self, keyspec: Union[OID, OIDS, Doc], txn: Optional[WriteTransaction]=None) -> None:
         """
         Delete one or more records from the database based on a key specification that
         should reference one or more records by primary key.
 
         keyspec - we accept either a key, a list of keys or a Doc, keys may be str or bytes
         txn - an optional transaction
         """
@@ -571,82 +507,69 @@
         elif isinstance(keyspec, bytes):
             keys = [keyspec]
         elif isinstance(keyspec, int) and self.integerkey:
             keys = [keyspec]
         else:
             raise InvalidKeySpecifier(keyspec)
 
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         for key in keys:
             if isinstance(key, str):
                 key = key.encode()
-            doc = self.get(key, txn=transaction)
+            doc = self.get(key, txn=txn)
             if doc:
-                transaction.delete(doc.oid, db=self._db)
-                # if self.replicated(txn):
-                #     txn.journal.append(doc.journal_entry(JournalType.DELETE, self.name))
-
+                txn.txn.delete(doc.oid, db=self._db)
                 if self._auditing:
                     self._database._auditor.delete(self, doc, txn)
 
                 for index_name in self.data:
-                    self.data[index_name].delete(doc, txn=transaction)
+                    self.data[index_name].delete(doc, txn=txn)
             else:
                 log.error(f'unable to delete key: "{key}" from table "{self.name}"')  # pragma: no cover
 
     @wrap_writer
-    def empty(self, txn: Optional[TXN|WriteTransaction]=None) -> None:
+    def empty(self, txn: Optional[WriteTransaction]=None) -> None:
         """
         Remove all data from the current table leaving the indexing structure in-tact
 
         txn - an optional transaction
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        transaction.drop(self._db, False)
-
-        # if self.replicated(txn):
-        #     doc = Doc({
-        #         'delete': False
-        #     })
-        #     txn.journal.append(doc.journal_entry(JournalType.REMOVE, self.name))
-
+        txn.txn.drop(self._db, False)
         for index_name in self.data:
-            self.data[index_name].empty(txn=transaction)
+            self.data[index_name].empty(txn=txn)
 
     @wrap_writer
-    def drop(self, index_name: str, txn: Optional[TXN, WriteTransaction]=None) -> None:
+    def drop(self, index_name: str, txn: Optional[WriteTransaction]=None) -> None:
         """
         Drop an index from the current table
 
         index_name - the name of the index to drop
         txn - an optional transaction
         """
         if index_name not in self.data:
             raise NoSuchIndex(index_name)
 
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         index = self.data[index_name]
         del self.data[index_name]
-        index.drop(txn=transaction)
+        index.drop(txn)
         self._database._cat.drop_index(self.name, index_name, txn)
 
     @wrap_reader_yield
-    def tail(self, key: Optional[OID]=None, txn: Optional[TXN]=None) -> Generator[Doc, None, None]:
+    def tail(self, key: Optional[OID]=None, txn: Optional[ReadTransaction]=None) -> Generator[Doc, None, None]:
         """
         Generates a sequence of records starting from the key after the primary key supplied. If no
         key is supplied, all records are returned, if a misssing key is supplied, no records are
         returned. Typically use this against the last-seen key to access new keys since the last
         check.
 
         key - the key to start from
         txn - an optional transaction
 
         TODO: add index to allow tailing based on indexes
         """
-        with txn.cursor(db=self._db) as cursor:
+        with txn.txn.cursor(db=self._db) as cursor:
             if key:
                 if not isinstance(key, bytes):
                     key = key.encode()
                 #
                 #   We need this behaviour, when someone empties the table, tail needs to know
                 #   to go back to the start of the table and continue, rather then being left
                 #   on a non-existant key forever ...
@@ -657,73 +580,72 @@
                 elif not cursor.next():
                     return None
 
             for key, val in cursor.iternext(keys=True, values=True):
                 yield Doc(None, key, self._decompressor(val))
 
     @wrap_reader
-    def first(
-            self, index_name: Optional[str]=None,
+    def first(self,
+            index_name: Optional[str]=None,
             doc: Optional[Doc]=None,
-            txn: Optional[TXN]=None) -> Optional[Doc]:
+            txn: Optional[OrbitTransaction]=None) -> Optional[Doc]:
         """
         Return the first record in the table or None if there are no records
 
         index_name - the name of the index to use (defaults to primary)
         txn - an optional transaction
         """
         if index_name:
             if index_name not in self.data:
                 raise NoSuchIndex(index_name)
             db = self.data[index_name]._db
         else:
             db = self._db
-        with txn.cursor(db=db) as cursor:
+        with txn.txn.cursor(db=db) as cursor:
             if not cursor.first():
                 return None
             if index_name:
                 if doc:
                     index_entry = self.data[index_name].get(doc, txn=txn)
                 else:
                     index_entry = cursor.value()
-                doc = txn.get(index_entry, db=self._db)
+                doc = txn.txn.get(index_entry, db=self._db)
                 return Doc(None, cursor.value(), self._decompressor(doc), integerkey=self.integerkey)
             else:
                 return Doc(None, cursor.key(), self._decompressor(cursor.value()), integerkey=self.integerkey)
 
     @wrap_reader
     def last(
             self,
             index_name: Optional[str]=None,
             doc: Optional[Doc]=None,
-            txn: Optional[TXN]=None) -> Optional[Doc]:
+            txn: Optional[WriteTransaction]=None) -> Optional[Doc]:
         """
         Return the last record in the table or None if there are no records
 
         index_name - the name of the index to use (defaults to primary)
         txn - an optional transaction
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         if index_name:
             if index_name not in self.data:
                 raise NoSuchIndex(index_name)
             db = self.data[index_name]._db
         else:
             db = self._db
-        with transaction.cursor(db=db) as cursor:
+        with txn.txn.cursor(db=db) as cursor:
             if not cursor.last():
                 return None
             if index_name:
                 if doc:
                     index_entry = self.data[index_name].get_last(doc, txn=txn)
                     if not index_entry:
                         return None  # pragma: no cover
                 else:
                     index_entry = cursor.value()
-                doc = transaction.get(index_entry, db=self._db)
+                doc = txn.txn.get(index_entry, db=self._db)
                 return Doc(None, cursor.value(), self._decompressor(doc), integerkey=self.integerkey)
             else:
                 return Doc(None, cursor.key(), self._decompressor(cursor.value()), integerkey=self.integerkey)
 
     @wrap_reader_yield
     def range(
             self,
@@ -731,30 +653,29 @@
             lower: Optional[Doc]=None,
             upper: Optional[Doc]=None,
             keyonly: bool=False,
             inclusive: bool=True,
             limit: int=MAXSIZE,
             page_number: int=0,
             nodups: bool=False,
-            txn: Optional[TXN]=None) -> Generator[Doc, None, None]:
+            txn: Optional[OrbitTransaction]=None) -> Generator[Doc, None, None]:
         """
         Find all records within a range of keys, optionally including keys at each end
         and optionally returning just the keys rather than the entire record.
 
         index_name - an optional index name, if no index is supplied, use primary keys
         lower - the record at the lower end of the range
         upper - the record at the upper end of the range
         keyonly - if set to True, only returns keys rather than the entire records
         inclusive - if set to True, include the keys at each end, i.e. use <=|=> rather than <|>
         limit - maximum number of records to return
         page_number - index of the page (starts from 0) with a size `limit` to return results from
         nodups - no duplicate keys, return only unique key values and ignore duplicates
         txn - an optional transaction
         """
-        transaction = txn if isinstance(txn, TXN) else txn.txn
         if index_name:
             if index_name not in self.data:
                 raise NoSuchIndex()
             index = self.data[index_name]
             db = index._db
 
             lower_keys = index.map_key(lower) if lower else [None]
@@ -768,15 +689,15 @@
         else:
             db = self._db
             lower_keys = [lower.oid] if lower else [None]
             upper_keys = [upper.oid] if upper else [None]
 
         skip = page_number * limit
 
-        with transaction.cursor(db) as cursor:
+        with txn.txn.cursor(db) as cursor:
             for lower_key in lower_keys:
                 upper_key = upper_keys.pop(0)
                 next_record = cursor.next_nodup if nodups else cursor.next
                 cursor.set_range(lower_key) if lower_key else cursor.first()
                 if cursor.key() == lower_key and not inclusive:
                     next_record()
                 count = 0
@@ -788,27 +709,26 @@
                     else:
                         count += 1
                         if not index_name:
                             yield cursor.key().decode() if keyonly else Doc(None,
                                 cursor.key(), self._decompressor(cursor.value()))
                         else:
                             yield Cursor(index, cursor) if keyonly else Doc(
-                                None, cursor.value()).get(self, txn=transaction)
+                                None, cursor.value()).get(self, txn=txn)
                     next_record()
 
     @wrap_reader
-    def seek_one(self, index_name: str, doc: Doc, txn: Optional[TXN]=None) -> Doc:
+    def seek_one(self, index_name: str, doc: Doc, txn: Optional[OrbitTransaction]=None) -> Doc:
         """
         Find the first matching record from an index
 
         index_name - the name of the index to search
         doc - the template record to find
         txn - an optional transaction
         """
-        txn = txn if isinstance(txn, TXN) else txn.txn
         if index_name not in self.data:
             raise NoSuchIndex()
         index_entry = self.data[index_name].get(doc, txn=txn)
         return self._cls(None, index_entry).get(self, txn=txn) if index_entry else None
 
     def seek(
             self,
@@ -961,49 +881,90 @@
             index_name: str = None,
             text: str = None,
             start: Optional[int] = 0,
             limit: Optional[int] = 0,
             countonly: bool=False,
             txn: Optional[TXN]=None) -> Generator[MatchResult, None, None]:
         """
+        Provides an indexed lookup into an Inverted Word (full-text) Index.This provides a 
+        list of primary keys relating to the results of the search. Note that for large
+        datasets that may result in thousands of responses, using "limit" is advisable. A 
+        combination of start+limit can be used to provide pages result sets.
+
+        index_name - the name of the IWX index to search
+        text - the text to search for (sequence of words)
+        start - the index into the result set to start from
+        limit - the maximum number of results to return
+        countonly - if true, just return the number of matches found
+        txn - an optional transaction wrapper
+        
+        > Returns generator for "MatchResult" objects
         """
         if index_name is None or index_name not in self.data:
             raise NoSuchIndex()  # pragma: no cover
         index = self.data[index_name]
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        return index.ftx_query(text, start, limit, countonly, txn=transaction)
+        return index.ftx_query(text, start, limit, countonly, txn)
 
     @wrap_reader
     def lexicon(
             self,
             index_name: str = None,
             text: str = None,
             max: int=0,
-            txn: Optional[TXN]=None) -> Generator[(str, int), None, None]:
+            txn: Optional[TXN]=None) -> Generator[str|int, None, None]:
         """
+        Query the Lexicon for an IWX index. For a given partial string it will return a list
+        of matching words together with the number of times the word appears in a document.
+        
+        index_name - the name of the index whose Lexicon we want to query
+        text - the partial string to look up
+        max - the maximum number of results to return
+        txn - an optional transaction wrapper
+        
+        > Returns a generator for (word, count)
         """
         if index_name is None or index_name not in self.data:
             raise NoSuchIndex()  # pragma: no cover
         index = self.data[index_name]
-        transaction = txn if isinstance(txn, TXN) else txn.txn
-        return index.iwx_lexicon(text, max=max, txn=transaction)
+        return index.iwx_lexicon(text, max=max, txn=txn)
 
     def dump(self, index_name, debug=False):
         """
+        Debugging only - DO NOT USE
         """
         index = self.data[index_name]
         return index.dump(debug)
 
-    def watch(self, callback: Callable=None, txn: Optional[TXN|WriteTransaction]=None) -> None:
+    def watch(self, callback: Callable=None) -> None:
+        """
+        Set up a handler to be executed when this table is changed. This should be done once per
+        session when the table is opened.
+        
+        callback - the async function to be called when the table is changed
+        """
         self._database._auditor.watch(self.name, callback)
 
     def unwatch(self, callback: Callable=None, txn: Optional[TXN|WriteTransaction]=None) -> None:
+        """
+        Clear a table change handler entry for this table. The callback passed should be the same
+        as the handler passed to 'watch'.
+        
+        callback - the async function to be called when the table is changed
+        """
         self._database._auditor.unwatch(self.name, callback)
 
     def export_to_file (self, filename, force=False):
+        """
+        Utility routine to dump the contents of a tabel to a file in JSON format.
+        
+        filename - the name of the file to dump the table to
+        force - overwrite the file if it already exists
+        
+        > Returns the number of records dumped to the file
+        """
         path = Path(filename)
         if path.exists() and not force:
             raise FileExistsError
         with open(filename, 'w') as io:
             count = 0
             io.write('{\n')
             for result in self.filter():
@@ -1011,14 +972,22 @@
                 io.write('  "' + result.doc.key + '": ')
                 dump(result.doc.doc, io)
                 count += 1
             io.write('\n}\n')
         return count
 
     def import_from_file (self, filename):
+        """
+        Utility routine to load a table from a JSON format file, ideally one previously exported,
+        otherwise you will need to ensure the appropriate JSON format manually. 
+        
+        filename - name of the file to load
+        
+        > Returns the size of the imported file
+        """
         path = Path(filename)
         if not path.exists():
             raise FileNotFoundError
         with open(filename, 'r') as io:
             data = load(io)
             for key in data:
                 doc = Doc(dict(data[key], **{'key': key}))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orbit_database-1.0.5/pyproject.toml` & `orbit_database-1.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit_database"
-version = "1.0.5"
+version = "1.0.8"
 description = "Database library for Python based on LMDB storage engine"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -20,17 +20,18 @@
 documentation = "https://gitlab.com/madpenguin/orbit-database"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-database"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-database/-/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.10, <4"
 posix-ipc = "^1.1.1"
 lmdb = "^1.4.1"
+typing-extensions = "^4.7.1"
 
 [tool.poetry.dev-dependencies]
 pipenv = "*"
 pytest = "*"
 pytest-cov = "*"
 coverage = "*"
 ujson = "*"
```

### Comparing `orbit_database-1.0.5/PKG-INFO` & `orbit_database-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: orbit-database
-Version: 1.0.5
+Version: 1.0.8
 Summary: Database library for Python based on LMDB storage engine
 Home-page: https://gitlab.com/madpenguin/orbit-database
 Keywords: database,nosql,lmdb
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: lmdb (>=1.4.1,<2.0.0)
 Requires-Dist: posix-ipc (>=1.1.1,<2.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-database
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-database
 Description-Content-Type: text/markdown
 
 # Orbit Database - Introduction
 
 #### Welcome to the Orbit Database repository and documentation. All project documentation is included within this repository and consists of markdown files and comments within the code. These are presented in real time by the "ZeroDocs" Orbit application which renders this content to HTML in real-time.
```

