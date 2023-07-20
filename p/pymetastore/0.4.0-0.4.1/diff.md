# Comparing `tmp/pymetastore-0.4.0.tar.gz` & `tmp/pymetastore-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetastore-0.4.0.tar", last modified: Mon Jul 10 21:56:27 2023, max compression
+gzip compressed data, was "pymetastore-0.4.1.tar", last modified: Thu Jul 20 16:09:42 2023, max compression
```

## Comparing `pymetastore-0.4.0.tar` & `pymetastore-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.4.0/LICENSE
--rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.4.0/pymetastore/__init__.py
--rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote
--rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.4.0/pymetastore/hive_metastore/__init__.py
--rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.4.0/pymetastore/hive_metastore/constants.py
--rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.4.0/pymetastore/hive_metastore/ttypes.py
--rw-r--r--   0        0        0    21240 2023-07-10 21:52:23.632268 pymetastore-0.4.0/pymetastore/htypes.py
--rw-r--r--   0        0        0    26176 2023-07-10 21:52:23.632813 pymetastore-0.4.0/pymetastore/metastore.py
--rw-r--r--   0        0        0     3381 2023-07-10 21:52:23.633402 pymetastore-0.4.0/pymetastore/stats.py
--rw-r--r--   0        0        0     1393 2023-07-10 21:56:27.253183 pymetastore-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    26646 2023-07-10 21:52:23.633742 pymetastore-0.4.0/tests/integration/test_metastore.py
--rw-r--r--   0        0        0    19596 2023-06-29 00:42:02.587038 pymetastore-0.4.0/tests/unit/test_htypes.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 pymetastore-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-22 19:20:51.055689 pymetastore-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1064 2023-06-26 15:39:01.814661 pymetastore-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 19:20:51.056280 pymetastore-0.4.1/pymetastore/__init__.py
+-rwxr-xr-x   0        0        0    62034 2023-06-22 19:20:51.056609 pymetastore-0.4.1/pymetastore/hive_metastore/ThriftHiveMetastore-remote
+-rw-r--r--   0        0        0  1715657 2023-06-22 19:20:51.059532 pymetastore-0.4.1/pymetastore/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0       57 2023-06-22 19:20:51.059681 pymetastore-0.4.1/pymetastore/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     1387 2023-06-22 19:20:51.059785 pymetastore-0.4.1/pymetastore/hive_metastore/constants.py
+-rw-r--r--   0        0        0   839918 2023-06-22 19:20:51.061341 pymetastore-0.4.1/pymetastore/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0    21240 2023-07-10 21:52:23.632268 pymetastore-0.4.1/pymetastore/htypes.py
+-rw-r--r--   0        0        0    26019 2023-07-20 16:01:38.039462 pymetastore-0.4.1/pymetastore/metastore.py
+-rw-r--r--   0        0        0     3381 2023-07-10 21:52:23.633402 pymetastore-0.4.1/pymetastore/stats.py
+-rw-r--r--   0        0        0     1780 2023-07-20 16:09:42.484534 pymetastore-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    33917 2023-07-20 16:01:38.039800 pymetastore-0.4.1/tests/integration/test_metastore.py
+-rw-r--r--   0        0        0    19724 2023-07-20 16:01:38.041120 pymetastore-0.4.1/tests/unit/test_htypes.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 pymetastore-0.4.1/PKG-INFO
```

### Comparing `pymetastore-0.4.0/LICENSE` & `pymetastore-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/README.md` & `pymetastore-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore-remote` & `pymetastore-0.4.1/pymetastore/hive_metastore/ThriftHiveMetastore-remote`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/hive_metastore/ThriftHiveMetastore.py` & `pymetastore-0.4.1/pymetastore/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/hive_metastore/constants.py` & `pymetastore-0.4.1/pymetastore/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/hive_metastore/ttypes.py` & `pymetastore-0.4.1/pymetastore/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/htypes.py` & `pymetastore-0.4.1/pymetastore/htypes.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pymetastore/metastore.py` & `pymetastore-0.4.1/pymetastore/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,16 +328,16 @@
         is_skewed = partition.sd.skewedInfo is not None
         location = "" if partition.sd.location is None else partition.sd.location
         serde_parameters = (
             {}
             if partition.sd.serdeInfo.parameters is None
             else partition.sd.serdeInfo.parameters
         )
-        catName = "" if partition.catName is None else partition.catName
-        writeId = -1 if partition.writeId is None else partition.writeId
+        cat_name = "" if partition.catName is None else partition.catName
+        write_id = -1 if partition.writeId is None else partition.writeId
         last_access_time = (
             -1 if partition.lastAccessTime is None else partition.lastAccessTime
         )
         partition_parameters = (
             {} if partition.parameters is None else partition.parameters
         )
         create_time = -1 if partition.createTime is None else partition.createTime
@@ -346,16 +346,16 @@
         partition_table_name = partition.tableName
 
         assert isinstance(sort_cols, list)
         assert isinstance(bucket_cols, list)
         assert isinstance(num_buckets, int)
         assert isinstance(location, str)
         assert isinstance(serde_parameters, dict)
-        assert isinstance(catName, str)
-        assert isinstance(writeId, int)
+        assert isinstance(cat_name, str)
+        assert isinstance(write_id, int)
         assert isinstance(last_access_time, int)
         assert isinstance(partition_parameters, dict)
         assert isinstance(create_time, int)
         assert isinstance(values, list)
         assert isinstance(db_name, str)
         assert isinstance(partition_table_name, str)
 
@@ -376,16 +376,16 @@
             db_name,
             partition_table_name,
             values,
             partition_parameters,
             create_time,
             last_access_time,
             sd,
-            catName,
-            writeId,
+            cat_name,
+            write_id,
         )
 
         return result_partition
 
     def get_table(self, database_name: str, table_name: str) -> HTable:
         table: Table = self.client.get_table(database_name, table_name)
 
@@ -397,50 +397,46 @@
                 t_part_columns: List[FieldSchema] = table.partitionKeys
                 for column in t_part_columns:
                     if column is not None:
                         if isinstance(column, FieldSchema):
                             if column.type is not None:
                                 type_parser = TypeParser(column.type)
                             else:
-                                raise TypeError(f"Expected type to be str, got None")
+                                raise TypeError("Expected type to be str, got None")
                             if column.comment is not None:
                                 comment = column.comment
                             else:
                                 comment = ""
                             if column.name is not None:
                                 name = column.name
                             else:
-                                raise TypeError(f"Expected name to be str, got None")
+                                raise TypeError("Expected name to be str, got None")
                             partition_columns.append(
                                 HColumn(name, type_parser.parse_type(), comment)
                             )
 
         if table.sd is not None:
             if table.sd.cols is not None:
                 if isinstance(table.sd.cols, list):
                     t_columns: List[FieldSchema] = table.sd.cols
                     for column in t_columns:
                         if column is not None:
                             if isinstance(column, FieldSchema):
                                 if column.type is not None:
                                     type_parser = TypeParser(column.type)
                                 else:
-                                    raise TypeError(
-                                        f"Expected type to be str, got None"
-                                    )
+                                    raise TypeError("Expected type to be str, got None")
                                 if column.comment is not None:
                                     comment = column.comment
                                 else:
                                     comment = ""
                                 if column.name is not None:
                                     name = column.name
                                 else:
-                                    raise TypeError(
-                                        f"Expected name to be str, got None"
-                                    )
+                                    raise TypeError("Expected name to be str, got None")
                                 columns.append(
                                     HColumn(name, type_parser.parse_type(), comment)
                                 )
 
             if table.sd.serdeInfo is not None:
                 if isinstance(table.sd.serdeInfo, SerDeInfo):
                     if table.sd.serdeInfo.serializationLib is not None:
@@ -455,35 +451,35 @@
                             f"Expected serdeInfo to be str, got {type(table.sd.serdeInfo)}"
                         )
                 else:
                     raise TypeError(
                         f"Expected serdeInfo to be SerDeInfo, got {type(table.sd.serdeInfo)}"
                     )
             else:
-                raise TypeError(f"Expected serdeInfo to be SerDeInfo, got None")
+                raise TypeError("Expected serdeInfo to be SerDeInfo, got None")
 
             if table.sd.inputFormat is not None:
                 if isinstance(table.sd.inputFormat, str):
                     input_format = table.sd.inputFormat
                 else:
                     raise TypeError(
                         f"Expected inputFormat to be str, got {type(table.sd.inputFormat)}"
                     )
             else:
-                raise TypeError(f"Expected inputFormat to be str, got None")
+                raise TypeError("Expected inputFormat to be str, got None")
 
             if table.sd.outputFormat is not None:
                 if isinstance(table.sd.outputFormat, str):
                     output_format = table.sd.outputFormat
                 else:
                     raise TypeError(
                         f"Expected outputFormat to be str, got {type(table.sd.outputFormat)}"
                     )
             else:
-                raise TypeError(f"Expected outputFormat to be str, got None")
+                raise TypeError("Expected outputFormat to be str, got None")
 
             storage_format = StorageFormat(serde, input_format, output_format)
 
             bucket_property = None
             if table.sd.bucketCols is not None:
                 sort_cols = []
                 if table.sd.sortCols is not None:
```

### Comparing `pymetastore-0.4.0/pymetastore/stats.py` & `pymetastore-0.4.1/pymetastore/stats.py`

 * *Files identical despite different names*

### Comparing `pymetastore-0.4.0/pyproject.toml` & `pymetastore-0.4.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 [project]
 name = "pymetastore"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Python client for the Thrift interface to Hive Metastore"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
     { name = "Kostas Pardalis" },
 ]
 dependencies = [
     "thrift>=0.16.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
+keywords = [
+    "data",
+    "data catalog",
+    "data discovery",
+    "data engineering",
+    "data governance",
+    "data infrastructure",
+    "data integration",
+    "data pipelines",
+    "hcatalog",
+    "hive",
+    "hive metastore",
+    "metadata",
+    "metastore",
+    "thrift",
+    "python",
+    "recap",
+]
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+repository = "https://github.com/recap-cloud/pymetastore"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
```

### Comparing `pymetastore-0.4.0/tests/integration/test_metastore.py` & `pymetastore-0.4.1/tests/integration/test_metastore.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,34 +29,71 @@
     HDatabase,
     HPartition,
     HStorage,
     HTable,
     HiveBucketProperty,
     StorageFormat,
 )
-from pymetastore.stats import *
+from pymetastore.stats import (
+    BinaryTypeStats,
+    BooleanTypeStats,
+    DateTypeStats,
+    DecimalTypeStats,
+    DoubleTypeStats,
+    LongTypeStats,
+    StringTypeStats,
+)
 
 
 @pytest.fixture(scope="module")
 def hive_client():
+    """
+    Create a connection to the Hive Metastore.
+
+    This function opens a connection to the Hive Metastore on a specified host and port.
+    The host and port can be defined in environment variables HMS_HOST and HMS_PORT.
+    If not defined, it defaults to "localhost" and 9083, respectively.
+
+    The function uses a context manager (via the `yield` keyword) to ensure that the
+    transport connection is properly closed after use.
+
+    Yields:
+        client: A handle to the Hive Metastore client.
+
+    Raises:
+        TTransportException: If a connection to the Hive Metastore cannot be established.
+    """
     host = os.environ.get("HMS_HOST", "localhost")
     port = int(os.environ.get("HMS_PORT", 9083))
     transport = TSocket.TSocket(host, port)
     transport = TTransport.TBufferedTransport(transport)
     protocol = TBinaryProtocol.TBinaryProtocol(transport)
     client = Client(protocol)
     transport.open()
 
     yield client
 
     transport.close()
 
 
 @pytest.fixture(scope="module", autouse=True)
+# pylint: disable=redefined-outer-name
+# pylint: disable=too-many-locals
+# pylint: disable=invalid-name
 def setup_data(hive_client):
+    """
+    Set up initial data for testing the core functionality of pymetastore.
+
+    This function creates a test database, several test tables, and partitions for
+    these tables in the Hive metastore. It tests various data types, including
+    primitive types, parameterized types, and table statistics.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+    """
     db = ttypes.Database(
         name="test_db",
         description="This is a test database",
         locationUri="/tmp/test_db.db",
         parameters={},
         ownerName="owner",
     )
@@ -295,36 +332,88 @@
             stats_obj_decimal,
             stats_obj_date,
         ],
     )
     hive_client.update_table_column_statistics(col_stats)
 
 
+# pylint: disable=redefined-outer-name
 def test_list_databases(hive_client):
+    """
+    Test the functionality of listing all databases.
+
+    This function retrieves all databases and checks that the database "test_db" is present.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If "test_db" is not found in the list of databases.
+    """
     assert "test_db" in HMS(hive_client).list_databases()
 
 
+# pylint: disable=redefined-outer-name
 def test_get_database(hive_client):
+    """
+    Test the functionality of retrieving database metadata.
+
+    This function retrieves the database "test_db" and checks that the properties
+    of the database match the expected values.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the properties of the fetched database do not match the expected values.
+    """
     hms = HMS(hive_client)
     database = hms.get_database("test_db")
     assert isinstance(database, HDatabase)
     assert database.name == "test_db"
     assert database.location == "file:/tmp/test_db.db"
     assert database.owner_name == "owner"
 
 
+# pylint: disable=redefined-outer-name
 def test_list_tables(hive_client):
+    """
+    Test the functionality of listing all tables in a database.
+
+    This function retrieves all tables from the database "test_db" and checks
+    that the table "test_table" is present.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If "test_table" is not found in the list of tables in "test_db".
+    """
     hms = HMS(hive_client)
     tables = hms.list_tables("test_db")
     assert isinstance(tables, list)
     assert "test_table" in tables
 
 
 @pytest.mark.xfail(reason="'table_type' is coming back MANAGED_TABLE.")
+# pylint: disable=redefined-outer-name
 def test_get_table(hive_client):
+    """
+    Test the functionality of retrieving table metadata.
+
+    This function retrieves the table "test_table" from the database "test_db" and
+    checks that the properties of the table match the expected values. This includes
+    checks on the table name, owner, location, columns, and table type.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the properties of the fetched table do not match the expected values.
+    """
     hms = HMS(hive_client)
     table = hms.get_table("test_db", "test_table")
     assert isinstance(table, HTable)
     assert table.database_name == "test_db"
     assert table.name == "test_table"
     assert table.owner == "owner"
     assert table.storage.location == "file:/tmp/test_db/test_table"
@@ -343,15 +432,29 @@
     # https://github.com/apache/hive/blob/14a1f70607db5ae6cf71b6d4343f308a5167581c/standalone-metastore/metastore-server/src/main/java/org/apache/hadoop/hive/metastore/client/builder/TableBuilder.java#L69C43-L69C43
     # Something similar happens also when you choose a "VIRTUAL_VIEW" table type, where
     # the metastore overrides the storage descriptor removing in the location the file::
     # prefix.
     assert table.table_type == "EXTERNAL_TABLE"
 
 
+# pylint: disable=redefined-outer-name
 def test_get_table_columns(hive_client):
+    """
+    Test the functionality of retrieving table columns, including those defined for partitioning.
+
+    This function retrieves the table "test_table" from the database "test_db" and
+    fetches the column and partition column definitions. It then checks that the types
+    and properties of the columns are correctly recognized and are of the expected types.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the column types or properties do not match the expected values.
+    """
     hms = HMS(hive_client)
     table = hms.get_table("test_db", "test_table")
     columns = table.columns
     partition_columns = table.partition_columns
 
     assert columns[0].name == "col1"
     assert isinstance(columns[0].type, HType)
@@ -371,35 +474,76 @@
     assert isinstance(partition_columns[0].type, HType)
     assert isinstance(partition_columns[0].type, HPrimitiveType)
     assert partition_columns[0].type.name == "STRING"
     assert partition_columns[0].type.category == HTypeCategory.PRIMITIVE
     assert partition_columns[0].comment == ""
 
 
+# pylint: disable=redefined-outer-name
 def test_list_columns(hive_client):
+    """
+    Test the functionality of listing all column names of a table.
+
+    This function retrieves all column names from the table "test_table" in the database
+    "test_db". It then checks that the names of the returned columns are as expected.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the names of the fetched columns do not match the expected values.
+    """
     hms = HMS(hive_client)
     columns = hms.list_columns("test_db", "test_table")
 
     assert isinstance(columns, list)
     assert len(columns) == 2
     assert columns[0] == "col1"
     assert columns[1] == "col2"
 
 
+# pylint: disable=redefined-outer-name
 def test_list_partitions(hive_client):
+    """
+    Test the functionality of listing all partitions of a table.
+
+    This function retrieves all partition names from the table "test_table" in the database
+    "test_db". It then checks that all expected partitions are found.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If not all expected partitions are found.
+    """
     hms = HMS(hive_client)
     partitions = hms.list_partitions("test_db", "test_table")
 
     assert isinstance(partitions, list)
     assert len(partitions) == 5
     for i in range(1, 6):
         assert f"partition={i}" in partitions
 
 
+# pylint: disable=redefined-outer-name
 def test_get_partitions(hive_client):
+    """
+    Test the functionality of retrieving all partitions of a table.
+
+    This function retrieves all partitions from the table "test_table" in the database
+    "test_db". It then checks that the properties of each returned partition are as
+    expected and that all expected partitions are found.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the properties of the fetched partitions do not match the
+        expected values, or if not all expected partitions are found.
+    """
     hms = HMS(hive_client)
     partitions = hms.get_partitions("test_db", "test_table")
     expected_storage = HStorage(
         storage_format=StorageFormat(
             serde="org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe",
             input_format="org.apache.hadoop.mapred.TextInputFormat",
             output_format="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
@@ -431,15 +575,29 @@
         assert partition.cat_name == "hive"
         assert isinstance(partition.parameters, dict)
         assert partition.write_id == -1
 
     assert missing_partitions == set()
 
 
+# pylint: disable=redefined-outer-name
 def test_get_partition(hive_client):
+    """
+    Test the functionality of retrieving a single partition.
+
+    This function retrieves a specific partition "partition=1" from the table
+    "test_table" in the database "test_db". It then checks that the properties
+    of the returned partition are as expected.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the properties of the fetched partition do not match the expected values.
+    """
     hms = HMS(hive_client)
     partition = hms.get_partition("test_db", "test_table", "partition=1")
     expected_storage = HStorage(
         storage_format=StorageFormat(
             serde="org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe",
             input_format="org.apache.hadoop.mapred.TextInputFormat",
             output_format="org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
@@ -463,15 +621,30 @@
     assert partition.create_time != 0
     assert partition.last_access_time == 0
     assert partition.cat_name == "hive"
     assert isinstance(partition.parameters, dict)
     assert partition.write_id == -1
 
 
+# pylint: disable=redefined-outer-name
+# pylint: disable=too-many-statements
 def test_primitive_types(hive_client):
+    """
+    Test the functionality of handling primitive types.
+
+    This function retrieves the table "test_table2" from the database "test_db" and
+    fetches the column definitions. It then checks that the types and properties
+    of the columns are correctly recognized and are of the expected primitive types.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the column types or properties do not match the expected values.
+    """
     hms = HMS(hive_client)
 
     table = hms.get_table("test_db", "test_table2")
     columns = table.columns
 
     assert len(columns) == 13
 
@@ -563,15 +736,30 @@
     assert isinstance(columns[12].type, HType)
     assert isinstance(columns[12].type, HPrimitiveType)
     assert columns[12].type.name == "BINARY"
     assert columns[12].type.category == HTypeCategory.PRIMITIVE
     assert columns[12].comment == "c15"
 
 
+# pylint: disable=redefined-outer-name
+# pylint: disable=too-many-statements
 def test_parameterized_types(hive_client):
+    """
+    Test the functionality of handling parameterized types.
+
+    This function retrieves the table "test_table3" from the database "test_db" and
+    fetches the column definitions. It then checks that the types and properties
+    of the columns are correctly recognized and are of the expected types.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the column types or properties do not match the expected values.
+    """
     hms = HMS(hive_client)
     table = hms.get_table("test_db", "test_table3")
     columns = table.columns
 
     assert len(columns) == 7
 
     assert columns[0].name == "col16"
@@ -650,15 +838,29 @@
     assert isinstance(columns[6].type.types[0], HPrimitiveType)
     assert columns[6].type.types[0].name == "INT"
     assert isinstance(columns[6].type.types[1], HType)
     assert isinstance(columns[6].type.types[1], HPrimitiveType)
     assert columns[6].type.types[1].name == "STRING"
 
 
+# pylint: disable=redefined-outer-name
 def test_table_stats(hive_client):
+    """
+    Test the table statistics fetching functionality of the HMS class.
+
+    This function retrieves the table "test_table4" from the database "test_db" and
+    then fetches the statistics for seven columns of different types. The function
+    checks that the returned statistics are correct and of the expected types.
+
+    Args:
+        hive_client: A handle to the Hive metastore client.
+
+    Raises:
+        AssertionError: If the fetched statistics are not as expected.
+    """
     hms = HMS(hive_client)
     table = hms.get_table("test_db", "test_table4")
 
     statistics = hms.get_table_stats(
         table,
         [
             HColumn("col4", HPrimitiveType(PrimitiveCategory.BOOLEAN)),
```

### Comparing `pymetastore-0.4.0/tests/unit/test_htypes.py` & `pymetastore-0.4.1/tests/unit/test_htypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     ex = HType("int", PrimitiveCategory.INT)
     assert str(ex) == "HType(name=int, category=PrimitiveCategory.INT)"
     assert repr(ex) == "HType('int', PrimitiveCategory.INT)"
     clone = eval(repr(ex))
     assert clone == ex
 
 
+# pylint: disable=line-too-long
 def test_hmap_type_str_repr_and_eq():
     typ = HMapType(
         HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT)
     )
     assert isinstance(typ, HMapType)
     assert (
         str(typ)
@@ -509,27 +510,29 @@
         == "HMapType(HPrimitiveType(PrimitiveCategory.STRING), HPrimitiveType(PrimitiveCategory.INT))"
     )
 
     clone = eval(repr(typ))
     assert clone == typ
 
 
+# pylint: disable=line-too-long
 def test_hlist_type_str_repr_and_eq():
     _type = HListType(HPrimitiveType(PrimitiveCategory.INT))
     assert isinstance(_type, HListType)
     assert (
         str(_type)
         == "HListType(name=LIST, category=HTypeCategory.LIST), element_type=HPrimitiveType(name=INT, category=HTypeCategory.PRIMITIVE))"
     )
     assert repr(_type) == "HListType(HPrimitiveType(PrimitiveCategory.INT))"
 
     clone = eval(repr(_type))
     assert clone == _type
 
 
+# pylint: disable=line-too-long
 def test_hunion_type_str_repr_and_eq():
     _type = HUnionType(
         [
             HPrimitiveType(PrimitiveCategory.INT),
             HPrimitiveType(PrimitiveCategory.STRING),
         ]
     )
@@ -573,14 +576,15 @@
     assert str(_type) == "HDecimalType(precision=10, scale=2)"
     assert repr(_type) == "HDecimalType(10, 2)"
 
     clone = eval(repr(_type))
     assert clone == _type
 
 
+# pylint: disable=line-too-long
 def test_hstruct_type_str_repr_and_eq():
     _type = HStructType(
         ["name", "age"],
         [
             HPrimitiveType(PrimitiveCategory.STRING),
             HPrimitiveType(PrimitiveCategory.INT),
         ],
```

### Comparing `pymetastore-0.4.0/PKG-INFO` & `pymetastore-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pymetastore
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python client for the Thrift interface to Hive Metastore
+Keywords: data data catalog data discovery data engineering data governance data infrastructure data integration data pipelines hcatalog hive hive metastore metadata metastore thrift python recap
 Author: Kostas Pardalis
 Author-Email: Chris Riccomini <criccomini@apache.org>
 License: MIT
+Project-URL: Repository, https://github.com/recap-cloud/pymetastore
 Requires-Python: >=3.8
 Requires-Dist: thrift>=0.16.0
 Description-Content-Type: text/markdown
 
 # pymetastore 🐝 🐍
 
 `pymetastore` is a Python client for Hive Metastore.
```

