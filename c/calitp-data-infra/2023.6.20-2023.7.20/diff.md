# Comparing `tmp/calitp_data_infra-2023.6.20.tar.gz` & `tmp/calitp_data_infra-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2023.6.20.tar", max compression
+gzip compressed data, was "calitp_data_infra-2023.7.20.tar", max compression
```

## Comparing `calitp_data_infra-2023.6.20.tar` & `calitp_data_infra-2023.7.20.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-14 15:20:22.416689 calitp_data_infra-2023.6.20/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-14 15:20:22.416792 calitp_data_infra-2023.6.20/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    24488 2023-06-20 15:44:59.472390 calitp_data_infra-2023.6.20/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      752 2023-06-20 15:54:29.473732 calitp_data_infra-2023.6.20/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.6.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-17 19:00:01.037081 calitp_data_infra-2023.7.20/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1200 2023-07-20 15:15:44.646986 calitp_data_infra-2023.7.20/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    26597 2023-07-20 15:15:45.570658 calitp_data_infra-2023.7.20/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      780 2023-07-20 16:18:59.803902 calitp_data_infra-2023.7.20/pyproject.toml
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.7.20/PKG-INFO
```

### Comparing `calitp_data_infra-2023.6.20/calitp_data_infra/auth.py` & `calitp_data_infra-2023.7.20/calitp_data_infra/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Mapping
 
-from google.cloud import secretmanager
+from google.cloud import secretmanager  # type: ignore
 
 project = "projects/cal-itp-data-infra"
 
 
 def get_secret_by_name(
     name: str,
     client=secretmanager.SecretManagerServiceClient(),
@@ -21,15 +21,17 @@
     secret_values = {}
 
     # once we get on at least 2.0.0 of secret manager, we can filter server-side
     for secret in client.list_secrets(parent=project):
         if label in secret.labels:
             version = f"{secret.name}/versions/latest"
             response = client.access_secret_version(version)
-            secret_values[secret.name.split("/")[-1]] = response.payload.data.decode("UTF-8").strip()
+            secret_values[secret.name.split("/")[-1]] = response.payload.data.decode(
+                "UTF-8"
+            ).strip()
 
     return secret_values
 
 
 if __name__ == "__main__":
     print("loading secrets...")
     get_secret_by_name("BEAR_TRANSIT_KEY")
```

### Comparing `calitp_data_infra-2023.6.20/calitp_data_infra/storage.py` & `calitp_data_infra-2023.7.20/calitp_data_infra/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,40 @@
 import os
 import re
 import sys
 from abc import ABC
 from datetime import datetime
 from enum import Enum
 from typing import (
+    Callable,
     ClassVar,
     Dict,
     List,
     Mapping,
     Optional,
     Tuple,
     Type,
     Union,
     get_type_hints,
 )
 
 import backoff
-import gcsfs
+import gcsfs  # type: ignore
 import humanize
 import pendulum
-from calitp_data.config import get_bucket, require_pipeline
-from calitp_data.storage import get_fs
-from google.cloud import storage
-from google.cloud.storage import Blob
+from calitp_data.config import get_bucket, require_pipeline  # type: ignore
+from calitp_data.storage import get_fs  # type: ignore
+from google.cloud import storage  # type: ignore
 from pydantic import (
     BaseModel,
+    ConstrainedStr,
     Extra,
     Field,
     HttpUrl,
     ValidationError,
-    constr,
     validator,
 )
 from pydantic.class_validators import root_validator
 from pydantic.tools import parse_obj_as
 from requests import Request, Session
 from typing_extensions import Annotated, Literal
 
@@ -110,45 +110,48 @@
 def make_name_bq_safe(name: str):
     """Replace non-word characters.
     See: https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#identifiers.
     """
     return str.lower(re.sub("[^\w]", "_", name))  # noqa: W605
 
 
-AIRTABLE_BUCKET = os.getenv("CALITP_BUCKET__AIRTABLE")
-GTFS_DOWNLOAD_CONFIG_BUCKET = os.getenv("CALITP_BUCKET__GTFS_DOWNLOAD_CONFIG")
-SCHEDULE_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_SCHEDULE_RAW")
-RT_RAW_BUCKET = os.getenv("CALITP_BUCKET__GTFS_RT_RAW")
+AIRTABLE_BUCKET = os.environ["CALITP_BUCKET__AIRTABLE"]
+GTFS_DOWNLOAD_CONFIG_BUCKET = os.environ["CALITP_BUCKET__GTFS_DOWNLOAD_CONFIG"]
+SCHEDULE_RAW_BUCKET = os.environ["CALITP_BUCKET__GTFS_SCHEDULE_RAW"]
+RT_RAW_BUCKET = os.environ["CALITP_BUCKET__GTFS_RT_RAW"]
 
 
 PARTITIONED_ARTIFACT_METADATA_KEY = "PARTITIONED_ARTIFACT_METADATA"
 
 PartitionType = Union[str, int, pendulum.DateTime, pendulum.Date, pendulum.Time]
 
-PARTITION_SERIALIZERS = {
+PARTITION_SERIALIZERS: Dict[Type, Callable] = {
     str: str,
     int: str,
     pendulum.Date: lambda d: d.to_date_string(),
     pendulum.DateTime: lambda dt: dt.to_iso8601_string(),
 }
 
-PARTITION_DESERIALIZERS = {
+PARTITION_DESERIALIZERS: Dict[Type, Callable] = {
     str: str,
     int: int,
     pendulum.Date: lambda s: pendulum.parse(s, exact=True),
     pendulum.DateTime: lambda s: pendulum.parse(s, exact=True),
 }
 
 
-def partition_map(path) -> Dict[str, PartitionType]:
+def partition_map(path) -> Dict[str, str]:
     return {key: value for key, value in re.findall(r"/(\w+)=([\w\-:=+.]+)(?=/)", path)}
 
 
 def serialize_partitions(partitions: Dict[str, PartitionType]) -> List[str]:
-    return [f"{name}={PARTITION_SERIALIZERS[type(value)](value)}" for name, value in partitions.items()]
+    return [
+        f"{name}={PARTITION_SERIALIZERS[type(value)](value)}"
+        for name, value in partitions.items()
+    ]
 
 
 class GTFSFeedType(str, Enum):
     schedule = "schedule"
     service_alerts = "service_alerts"
     trip_updates = "trip_updates"
     vehicle_positions = "vehicle_positions"
@@ -162,19 +165,21 @@
             GTFSFeedType.trip_updates,
             GTFSFeedType.vehicle_positions,
         ):
             return True
         raise RuntimeError(f"managed to end up with an invalid enum type of {self}")
 
 
-def upload_from_string(blob: storage.Blob, data, content_type, client):
+def upload_from_string(
+    blob: storage.Blob, data: bytes, content_type: str, client: storage.Client
+):
     blob.upload_from_string(
-        data,
-        content_type,
-        client,
+        data=data,
+        content_type=content_type,
+        client=client,
     )
 
 
 # Is there a better pattern for making this retry optional by the caller?
 @backoff.on_exception(
     backoff.expo,
     base=5,
@@ -197,21 +202,25 @@
     exception=(Exception,),
     max_tries=3,
 )
 def set_metadata_with_retry(*args, **kwargs):
     return set_metadata(*args, **kwargs)
 
 
+class StringNoWhitespace(ConstrainedStr):
+    strip_whitespace = True
+
+
 class PartitionedGCSArtifact(BaseModel, abc.ABC):
     """
     This class is designed to be subclassed to model "extracts", i.e. a particular
     download of a given data source.
     """
 
-    filename: constr(strip_whitespace=True)
+    filename: StringNoWhitespace
 
     class Config:
         json_encoders = {
             pendulum.DateTime: lambda dt: dt.to_iso8601_string(),
         }
 
     @property
@@ -235,29 +244,39 @@
         """
         Defines the partitions into which this artifact is organized.
         The order does matter!
         """
 
     @property
     def serialized_partitions(self) -> List[str]:
-        return serialize_partitions({name: getattr(self, name) for name in self.partition_names})
+        return serialize_partitions(
+            {name: getattr(self, name) for name in self.partition_names}
+        )
 
     @property
     def partition_types(self) -> Dict[str, Type[PartitionType]]:
         return {}
 
     @root_validator(allow_reuse=True)
     def check_partitions(cls, values):
         # TODO: this isn't great but some partition_names are properties
         if isinstance(cls.partition_names, property):
             return values
-        cls_properties = [name for name in dir(cls) if isinstance(getattr(cls, name), property)]
-        missing = [name for name in cls.partition_names if name not in values and name not in cls_properties]
+        cls_properties = [
+            name for name in dir(cls) if isinstance(getattr(cls, name), property)
+        ]
+        missing = [
+            name
+            for name in cls.partition_names
+            if name not in values and name not in cls_properties
+        ]
         if missing:
-            raise ValueError(f"all partition names must exist as fields or properties; missing {missing}")
+            raise ValueError(
+                f"all partition names must exist as fields or properties; missing {missing}"
+            )
         return values
 
     @property
     def name(self):
         return os.path.join(
             self.table,
             *self.serialized_partitions,
@@ -287,77 +306,104 @@
             fs.setxattrs(
                 path=self.path,
                 # This syntax seems silly but it's so we pass the _value_ of PARTITIONED_ARTIFACT_METADATA_KEY
                 **{PARTITIONED_ARTIFACT_METADATA_KEY: self.json(exclude=exclude)},
             )
 
         if client:
-            logging.info(f"saving {humanize.naturalsize(len(content))} to {self.bucket} {self.name}")
+            logging.info(
+                f"saving {humanize.naturalsize(len(content))} to {self.bucket} {self.name}"
+            )
             blob = storage.Blob(
                 name=self.name,
                 bucket=client.bucket(self.bucket.replace("gs://", "")),
             )
 
-            upload_from_string_func = upload_from_string_with_retry if retry_content else upload_from_string
-            upload_from_string_func(
-                blob=blob,
-                data=content,
-                content_type="application/octet-stream",
-                client=client,
-            )
-
-            set_metadata_func = set_metadata_with_retry if retry_metadata else set_metadata
-            set_metadata_func(
-                blob=blob,
-                model=self,
-                exclude=exclude,
-            )
+            if retry_content:
+                upload_from_string_with_retry(
+                    blob=blob,
+                    data=content,
+                    content_type="application/octet-stream",
+                    client=client,
+                )
+            else:
+                upload_from_string(
+                    blob=blob,
+                    data=content,
+                    content_type="application/octet-stream",
+                    client=client,
+                )
+
+            if retry_metadata:
+                set_metadata_with_retry(
+                    blob=blob,
+                    model=self,
+                    exclude=exclude,
+                )
+            else:
+                set_metadata(
+                    blob=blob,
+                    model=self,
+                    exclude=exclude,
+                )
 
 
 # TODO: this should really use a typevar
+# This contains several assignment ignores because they are actually ClassVars.
+# Maybe the underlying abstract property definition is an anti-pattern.
 def fetch_all_in_partition(
     cls: Type[PartitionedGCSArtifact],
     partitions: Dict[str, PartitionType],
-    bucket: str = None,
-    table: str = None,
+    bucket: Optional[str] = None,
+    table: Optional[str] = None,
     verbose=False,
-) -> Tuple[List[PartitionedGCSArtifact], List[Blob], List[Blob]]:
+) -> Tuple[List[PartitionedGCSArtifact], List[storage.Blob], List[storage.Blob]]:
     if not bucket:
-        bucket = cls.bucket
+        bucket = cls.bucket  # type: ignore[assignment]
 
         if not isinstance(bucket, str):
-            raise TypeError(f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}")
+            raise TypeError(
+                f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}"
+            )
 
     if not table:
-        table = cls.table
+        table = cls.table  # type: ignore[assignment]
 
         if not isinstance(table, str):
-            raise TypeError(f"must either pass table, or the table must resolve to a string; got {type(table)}")
+            raise TypeError(
+                f"must either pass table, or the table must resolve to a string; got {type(table)}"
+            )
 
     prefix = "/".join(
         [
             table,
             *serialize_partitions(partitions),
             "",
         ]
     )
     if verbose:
         print(f"listing all files in {bucket}/{prefix}")
     client = storage.Client()
     # once Airflow is upgraded to Python 3.9, can use:
     # files = client.list_blobs(bucket.removeprefix("gs://"), prefix=prefix, delimiter=None)
-    files = client.list_blobs(re.sub(r"^gs://", "", bucket), prefix=prefix, delimiter=None)
+    files = client.list_blobs(
+        re.sub(r"^gs://", "", bucket), prefix=prefix, delimiter=None
+    )
 
     parsed: List[PartitionedGCSArtifact] = []
-    blobs_with_missing_metadata: List[Blob] = []
-    blobs_with_invalid_metadata: List[Blob] = []
+    blobs_with_missing_metadata: List[storage.Blob] = []
+    blobs_with_invalid_metadata: List[storage.Blob] = []
 
     for file in files:
         try:
-            parsed.append(parse_obj_as(cls, json.loads(file.metadata[PARTITIONED_ARTIFACT_METADATA_KEY])))
+            parsed.append(
+                parse_obj_as(
+                    cls, json.loads(file.metadata[PARTITIONED_ARTIFACT_METADATA_KEY])
+                )
+            )
         except (TypeError, KeyError):
             logging.exception(f"metadata missing on {bucket}/{file.name}")
             blobs_with_missing_metadata.append(file)
         except ValidationError:
             logging.exception(f"invalid metadata found on {bucket}/{file.name}")
             blobs_with_invalid_metadata.append(file)
 
@@ -413,15 +459,17 @@
 
     @property
     def partition(self) -> Dict[str, str]:
         return partition_map(self.name + "/")
 
     def children(self, fs) -> List["GCSObjectInfo"]:
         # TODO: this should work with a discriminated type but idk why it's not
-        return parse_obj_as(GCSObjectInfoList, [fs.info(child) for child in fs.ls(self.name)]).__root__
+        return parse_obj_as(
+            GCSObjectInfoList, [fs.info(child) for child in fs.ls(self.name)]
+        ).__root__
 
 
 GCSObjectInfo = Annotated[
     Union[GCSFileInfo, GCSDirectoryInfo],
     Field(discriminator="type"),
 ]
 
@@ -434,75 +482,99 @@
     table: str,
     prefix_partitions: Dict[str, PartitionType],
     partition_types: Dict[str, Type[PartitionType]],
 ) -> GCSFileInfo:
     fs = get_fs()
     fs.invalidate_cache()
 
-    prefix_info = fs.info("/".join([bucket, table, *serialize_partitions(prefix_partitions), ""]))
+    prefix_info = fs.info(
+        "/".join([bucket, table, *serialize_partitions(prefix_partitions), ""])
+    )
     directory = GCSDirectoryInfo(**prefix_info)
 
     for key, typ in partition_types.items():
-        directory = sorted(
+        next_dir = sorted(
             directory.children(fs),
             key=lambda o: PARTITION_DESERIALIZERS[typ](o.partition[key]),
             reverse=True,
         )[0]
+        # ensure we always get directories
+        assert isinstance(next_dir, GCSDirectoryInfo)
+        directory = next_dir
 
     children = directory.children(fs)
     # This is just a convention for us for now; we could also label files with metadata if desired
+    # Note: this assumes that there is only 1 file in the final "directory"; this is probably an anti-pattern
     if len(children) != 1:
-        raise ValueError(f"found {len(directory.children(fs))} files rather than 1 in the directory {directory.name}")
+        raise ValueError(
+            f"found {len(directory.children(fs))} files rather than 1 in the directory {directory.name}"
+        )
 
     ret = children[0]
 
     # is there a way to have pydantic check this?
     if not isinstance(ret, GCSFileInfo):
-        raise ValueError(f"encountered unexpected type {type(ret)} rather than GCSFileInfo")
+        raise ValueError(
+            f"encountered unexpected type {type(ret)} rather than GCSFileInfo"
+        )
 
     return ret
 
 
+# This contains several assignment ignores because they are actually ClassVars.
+# Maybe the underlying abstract property definition is an anti-pattern.
 def get_latest(
     cls: Type[PartitionedGCSArtifact],
-    bucket: str = None,
-    table: str = None,
-    partition_names: List[str] = None,
+    bucket: Optional[str] = None,
+    table: Optional[str] = None,
+    partition_names: Optional[List[str]] = None,
 ) -> PartitionedGCSArtifact:
     if not bucket:
-        bucket = cls.bucket
+        bucket = cls.bucket  # type: ignore[assignment]
 
         if not isinstance(bucket, str):
-            raise TypeError(f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}")
+            raise TypeError(
+                f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}"
+            )
 
     if not table:
-        table = cls.table
+        table = cls.table  # type: ignore[assignment]
 
         if not isinstance(table, str):
-            raise TypeError(f"must either pass table, or the table must resolve to a string; got {type(table)}")
+            raise TypeError(
+                f"must either pass table, or the table must resolve to a string; got {type(table)}"
+            )
 
     if not partition_names:
-        partition_names = cls.partition_names
+        partition_names = cls.partition_names  # type: ignore[assignment]
 
         if not isinstance(partition_names, list):
             raise TypeError(
                 f"must either pass partition names, or the partition names must resolve to a list; got {type(partition_names)}"
             )
 
     latest = get_latest_file(
         bucket,
         table,
         prefix_partitions={},
         # TODO: this doesn't pick up the type hint of dt since it's a property; it's fine as a string but we should fix
-        partition_types={name: get_type_hints(cls).get(name, str) for name in partition_names},
+        partition_types={
+            name: get_type_hints(cls).get(name, str) for name in partition_names
+        },
     )
 
     logging.info(f"identified {latest.name} as the most recent extract of {cls}")
 
-    return cls(**json.loads(get_fs().getxattr(path=f"gs://{latest.name}", attr=PARTITIONED_ARTIFACT_METADATA_KEY)))
+    return cls(
+        **json.loads(
+            get_fs().getxattr(
+                path=f"gs://{latest.name}", attr=PARTITIONED_ARTIFACT_METADATA_KEY
+            )
+        )
+    )
 
 
 class AirtableGTFSDataRecord(BaseModel):
     id: str
     name: str
     uri: Optional[str]
     pipeline_url: Optional[str]
@@ -535,26 +607,33 @@
     @classmethod
     def get_latest(cls) -> "AirtableGTFSDataExtract":
         latest = get_latest_file(
             cls.bucket,
             cls.table,
             prefix_partitions={},
             # TODO: this doesn't pick up the type hint of dt since it's a property; it's fine as a string but we should fix
-            partition_types={name: get_type_hints(cls).get(name, str) for name in cls.partition_names},
+            partition_types={
+                name: get_type_hints(cls).get(name, str) for name in cls.partition_names
+            },
         )
 
-        logging.info(f"identified {latest.name} as the most recent extract of gtfs datasets")
+        logging.info(
+            f"identified {latest.name} as the most recent extract of gtfs datasets"
+        )
 
         with get_fs().open(latest.name, "rb") as f:
             content = gzip.decompress(f.read())
 
         return AirtableGTFSDataExtract(
             filename=latest.filename,
             ts=pendulum.parse(latest.partition["ts"], exact=True),
-            records=[AirtableGTFSDataRecord(**json.loads(row)) for row in content.decode().splitlines()],
+            records=[
+                AirtableGTFSDataRecord(**json.loads(row))
+                for row in content.decode().splitlines()
+            ],
         )
 
 
 # forbid here as we want to be super careful/strict
 class GTFSDownloadConfig(BaseModel, extra=Extra.forbid):
     extracted_at: Optional[pendulum.DateTime]
     name: Optional[str]
@@ -588,15 +667,17 @@
         return v
 
     def build_request(self, auth_dict: Mapping[str, str]) -> Request:
         params = {k: auth_dict[v] for k, v in self.auth_query_params.items()}
         headers = {k: auth_dict[v] for k, v in self.auth_headers.items()}
 
         # some web servers require user agents or they will throw a 4XX error
-        headers["User-Agent"] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.12; rv:55.0) Gecko/20100101 Firefox/55.0"
+        headers[
+            "User-Agent"
+        ] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.12; rv:55.0) Gecko/20100101 Firefox/55.0"
 
         # inspired by: https://stackoverflow.com/questions/18869074/create-url-without-request-execution
         return Request(
             "GET",
             url=self.url,
             params=params,
             headers=headers,
@@ -608,15 +689,18 @@
         # we care about replacing slashes for GCS object names
         # can use: https://www.base64url.com/ to test encoding/decoding
         # convert in bigquery: https://cloud.google.com/bigquery/docs/reference/standard-sql/string_functions#from_base64
         return base64.urlsafe_b64encode(self.url.encode()).decode()
 
     @property
     def base64_validation_url(self) -> str:
-        return base64.urlsafe_b64encode(self.schedule_url_for_validation.encode()).decode()
+        assert self.schedule_url_for_validation is not None
+        return base64.urlsafe_b64encode(
+            self.schedule_url_for_validation.encode()
+        ).decode()
 
 
 class GTFSDownloadConfigExtract(PartitionedGCSArtifact):
     bucket: ClassVar[str] = GTFS_DOWNLOAD_CONFIG_BUCKET
     table: ClassVar[str] = "gtfs_download_configs"
     partition_names: ClassVar[List[str]] = ["dt", "ts"]
     ts: pendulum.DateTime
@@ -660,15 +744,15 @@
     def base64_url(self) -> str:
         return self.config.base64_encoded_url
 
 
 class GTFSScheduleFeedExtract(GTFSFeedExtract):
     bucket: ClassVar[str] = SCHEDULE_RAW_BUCKET
     table: ClassVar[str] = GTFSFeedType.schedule
-    feed_type: ClassVar[str] = GTFSFeedType.schedule
+    feed_type: ClassVar[GTFSFeedType] = GTFSFeedType.schedule
     partition_names: ClassVar[List[str]] = ["dt", "ts", "base64_url"]
     reconstructed: bool = False
 
     @validator("config", allow_reuse=True)
     def is_schedule_type(cls, v: GTFSDownloadConfig):
         if v.feed_type != GTFSFeedType.schedule:
             raise TypeError("a schedule extract must come from a schedule config")
@@ -706,30 +790,36 @@
     **request_kwargs,
 ) -> Tuple[GTFSFeedExtract, bytes]:
     s = Session()
     r = s.prepare_request(config.build_request(auth_dict))
     resp = s.send(r, **request_kwargs)
     resp.raise_for_status()
 
-    disposition_header = resp.headers.get("content-disposition", resp.headers.get("Content-Disposition"))
+    disposition_header = resp.headers.get(
+        "content-disposition", resp.headers.get("Content-Disposition")
+    )
 
     if disposition_header:
         if disposition_header.startswith("filename="):
             # sorry; cgi won't parse unless it's prefixed with the disposition type
             disposition_header = f"attachment; {disposition_header}"
         _, params = cgi.parse_header(disposition_header)
         disposition_filename = params.get("filename")
     else:
         disposition_filename = None
 
     filename = (
-        disposition_filename or (os.path.basename(resp.url) if resp.url.endswith(".zip") else None) or default_filename
+        disposition_filename
+        or (os.path.basename(resp.url) if resp.url.endswith(".zip") else None)
+        or default_filename
     )
 
-    extract_class = GTFSRTFeedExtract if config.feed_type.is_rt else GTFSScheduleFeedExtract
+    extract_class = (
+        GTFSRTFeedExtract if config.feed_type.is_rt else GTFSScheduleFeedExtract
+    )
     extract = extract_class(
         filename=filename,
         config=config,
         response_code=resp.status_code,
         response_headers=resp.headers,
         ts=ts,
     )
@@ -741,24 +831,28 @@
     # just some useful testing stuff
     latest = AirtableGTFSDataExtract.get_latest()
     print(latest.path, len(latest.records))
     extract = get_latest(GTFSDownloadConfigExtract)
     fs = get_fs()
     with fs.open(extract.path, "rb") as f:
         content = gzip.decompress(f.read())
-    records = [GTFSDownloadConfig(**json.loads(row)) for row in content.decode().splitlines()]
+    records = [
+        GTFSDownloadConfig(**json.loads(row)) for row in content.decode().splitlines()
+    ]
     download_feed(records[0], auth_dict={}, ts=pendulum.now(), timeout=1)
     print("downloaded a thing!")
     sys.exit(0)
 
     # use Etc/UTC instead of UTC
     # Etc/UTC is what the pods get as a timezone... and it serializes to 2022-08-18T00:00:00+00:00
     # whereas UTC serializes to 2022-08-18T00:00:00Z
     # this should probably be checked in the partitioned artifact?
-    yesterday_noon = pendulum.yesterday("Etc/UTC").replace(minute=0, second=0, microsecond=0)
+    yesterday_noon = pendulum.yesterday("Etc/UTC").replace(
+        minute=0, second=0, microsecond=0
+    )
     vp_files, _, _ = fetch_all_in_partition(
         cls=GTFSRTFeedExtract,
         fs=get_fs(),
         partitions={
             "dt": yesterday_noon.date(),
             "hour": yesterday_noon,
         },
```

### Comparing `calitp_data_infra-2023.6.20/pyproject.toml` & `calitp_data_infra-2023.7.20/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp-data-infra"
-version = "2023.06.20"
+version = "2023.7.20"
 description = "Shared code for developing data pipelines that process Cal-ITP data."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 # Some of these are pinned oddly to play nicely with Composer
 pydantic = "~1.9"
@@ -17,14 +17,15 @@
 calitp-data = "2023.2.15.1"
 google-cloud-secret-manager = "~1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.0"
 hypothesis = "^6.68.0"
+types-requests = "^2.31.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `calitp_data_infra-2023.6.20/PKG-INFO` & `calitp_data_infra-2023.7.20/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2023.6.20
+Version: 2023.7.20
 Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

