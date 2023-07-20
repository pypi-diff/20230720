# Comparing `tmp/calitp_data_infra-2023.7.20.tar.gz` & `tmp/calitp_data_infra-2023.7.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2023.7.20.tar", max compression
+gzip compressed data, was "calitp_data_infra-2023.7.20.1.tar", max compression
```

## Comparing `calitp_data_infra-2023.7.20.tar` & `calitp_data_infra-2023.7.20.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-02-17 19:00:01.037081 calitp_data_infra-2023.7.20/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1200 2023-07-20 15:15:44.646986 calitp_data_infra-2023.7.20/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    26597 2023-07-20 15:15:45.570658 calitp_data_infra-2023.7.20/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      780 2023-07-20 16:18:59.803902 calitp_data_infra-2023.7.20/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.7.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-17 19:00:01.037081 calitp_data_infra-2023.7.20.1/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1200 2023-07-20 15:15:44.646986 calitp_data_infra-2023.7.20.1/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    26823 2023-07-20 17:16:14.968392 calitp_data_infra-2023.7.20.1/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      782 2023-07-20 17:13:01.037681 calitp_data_infra-2023.7.20.1/pyproject.toml
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 calitp_data_infra-2023.7.20.1/PKG-INFO
```

### Comparing `calitp_data_infra-2023.7.20/calitp_data_infra/auth.py` & `calitp_data_infra-2023.7.20.1/calitp_data_infra/auth.py`

 * *Files identical despite different names*

### Comparing `calitp_data_infra-2023.7.20/calitp_data_infra/storage.py` & `calitp_data_infra-2023.7.20.1/calitp_data_infra/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,18 @@
 def make_name_bq_safe(name: str):
     """Replace non-word characters.
     See: https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#identifiers.
     """
     return str.lower(re.sub("[^\w]", "_", name))  # noqa: W605
 
 
-AIRTABLE_BUCKET = os.environ["CALITP_BUCKET__AIRTABLE"]
-GTFS_DOWNLOAD_CONFIG_BUCKET = os.environ["CALITP_BUCKET__GTFS_DOWNLOAD_CONFIG"]
-SCHEDULE_RAW_BUCKET = os.environ["CALITP_BUCKET__GTFS_SCHEDULE_RAW"]
-RT_RAW_BUCKET = os.environ["CALITP_BUCKET__GTFS_RT_RAW"]
+AIRTABLE_BUCKET = os.getenv("CALITP_BUCKET__AIRTABLE")
+GTFS_DOWNLOAD_CONFIG_BUCKET = os.getenv("CALITP_BUCKET__GTFS_DOWNLOAD_CONFIG")
+SCHEDULE_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_SCHEDULE_RAW")
+RT_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_RT_RAW")
 
 
 PARTITIONED_ARTIFACT_METADATA_KEY = "PARTITIONED_ARTIFACT_METADATA"
 
 PartitionType = Union[str, int, pendulum.DateTime, pendulum.Date, pendulum.Time]
 
 PARTITION_SERIALIZERS: Dict[Type, Callable] = {
@@ -221,16 +221,20 @@
     class Config:
         json_encoders = {
             pendulum.DateTime: lambda dt: dt.to_iso8601_string(),
         }
 
     @property
     @abc.abstractmethod
-    def bucket(self) -> str:
-        """Bucket name"""
+    def bucket(self) -> Optional[str]:
+        """
+        Bucket name
+
+        Note that this is Optional; not all apps will have all bucket env vars set.
+        """
 
     @validator("bucket", check_fields=False, allow_reuse=True)
     def bucket_exists(cls, v):
         if not storage.Client().bucket(v).exists():
             raise ValueError(f"bucket {v} does not exist")
 
     @property
@@ -293,14 +297,15 @@
         content: bytes,
         exclude=None,
         fs: gcsfs.GCSFileSystem = None,
         client: storage.Client = None,
         retry_metadata: bool = False,
         retry_content: bool = False,
     ):
+        assert self.bucket is not None
         if (fs is None) == (client is None):
             raise TypeError("must provide a gcsfs file system OR a storage client")
 
         if fs:
             logging.info(f"saving {humanize.naturalsize(len(content))} to {self.path}")
             fs.pipe(path=self.path, value=content)
             fs.setxattrs(
@@ -588,28 +593,29 @@
     auth_query_param: Dict[str, str] = {}
 
     class Config:
         extra = "allow"
 
 
 class AirtableGTFSDataExtract(PartitionedGCSArtifact):
-    bucket: ClassVar[str] = AIRTABLE_BUCKET
+    bucket: ClassVar[Optional[str]] = AIRTABLE_BUCKET
     table: ClassVar[str] = "california_transit__gtfs_datasets"
     partition_names: ClassVar[List[str]] = ["dt", "ts"]
     ts: pendulum.DateTime
     records: List[AirtableGTFSDataRecord]
 
     @property
     def dt(self) -> pendulum.Date:
         return self.ts.date()
 
     # TODO: this is separate from the general get_latest because our
     #  airtable downloader does not set metadata yet
     @classmethod
     def get_latest(cls) -> "AirtableGTFSDataExtract":
+        assert cls.bucket is not None
         latest = get_latest_file(
             cls.bucket,
             cls.table,
             prefix_partitions={},
             # TODO: this doesn't pick up the type hint of dt since it's a property; it's fine as a string but we should fix
             partition_types={
                 name: get_type_hints(cls).get(name, str) for name in cls.partition_names
@@ -696,15 +702,15 @@
         assert self.schedule_url_for_validation is not None
         return base64.urlsafe_b64encode(
             self.schedule_url_for_validation.encode()
         ).decode()
 
 
 class GTFSDownloadConfigExtract(PartitionedGCSArtifact):
-    bucket: ClassVar[str] = GTFS_DOWNLOAD_CONFIG_BUCKET
+    bucket: ClassVar[Optional[str]] = GTFS_DOWNLOAD_CONFIG_BUCKET
     table: ClassVar[str] = "gtfs_download_configs"
     partition_names: ClassVar[List[str]] = ["dt", "ts"]
     ts: pendulum.DateTime
 
     @validator("ts", allow_reuse=True)
     def coerce_ts(cls, v):
         if isinstance(v, datetime):
@@ -742,29 +748,29 @@
 
     @property
     def base64_url(self) -> str:
         return self.config.base64_encoded_url
 
 
 class GTFSScheduleFeedExtract(GTFSFeedExtract):
-    bucket: ClassVar[str] = SCHEDULE_RAW_BUCKET
+    bucket: ClassVar[Optional[str]] = SCHEDULE_RAW_BUCKET
     table: ClassVar[str] = GTFSFeedType.schedule
     feed_type: ClassVar[GTFSFeedType] = GTFSFeedType.schedule
     partition_names: ClassVar[List[str]] = ["dt", "ts", "base64_url"]
     reconstructed: bool = False
 
     @validator("config", allow_reuse=True)
     def is_schedule_type(cls, v: GTFSDownloadConfig):
         if v.feed_type != GTFSFeedType.schedule:
             raise TypeError("a schedule extract must come from a schedule config")
         return v
 
 
 class GTFSRTFeedExtract(GTFSFeedExtract):
-    bucket: ClassVar[str] = RT_RAW_BUCKET
+    bucket: ClassVar[Optional[str]] = RT_RAW_BUCKET
     partition_names: ClassVar[List[str]] = ["dt", "hour", "ts", "base64_url"]
 
     @validator("config", allow_reuse=True)
     def is_rt_type(cls, v: GTFSDownloadConfig):
         if not v.feed_type.is_rt:
             raise TypeError("a realtime extract must come from a realtime config")
         return v
```

### Comparing `calitp_data_infra-2023.7.20/pyproject.toml` & `calitp_data_infra-2023.7.20.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp-data-infra"
-version = "2023.7.20"
+version = "2023.7.20.1"
 description = "Shared code for developing data pipelines that process Cal-ITP data."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 # Some of these are pinned oddly to play nicely with Composer
 pydantic = "~1.9"
```

### Comparing `calitp_data_infra-2023.7.20/PKG-INFO` & `calitp_data_infra-2023.7.20.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2023.7.20
+Version: 2023.7.20.1
 Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

