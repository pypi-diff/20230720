# Comparing `tmp/hca-import-validation-0.0.4.tar.gz` & `tmp/hca-import-validation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hca-import-validation-0.0.4.tar", last modified: Wed Nov 17 14:24:07 2021, max compression
+gzip compressed data, was "hca-import-validation-0.0.8.tar", last modified: Fri Jul  8 19:01:49 2022, max compression
```

## Comparing `hca-import-validation-0.0.4.tar` & `hca-import-validation-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 aherbst    (502) staff       (20)        0 2021-11-17 14:24:07.111699 hca-import-validation-0.0.4/
--rw-r--r--   0 aherbst    (502) staff       (20)    11357 2021-02-17 19:47:24.000000 hca-import-validation-0.0.4/LICENSE
--rw-r--r--   0 aherbst    (502) staff       (20)      418 2021-11-17 14:24:07.111853 hca-import-validation-0.0.4/PKG-INFO
--rw-r--r--   0 aherbst    (502) staff       (20)      854 2021-07-08 19:54:20.000000 hca-import-validation-0.0.4/README.md
-drwxr-xr-x   0 aherbst    (502) staff       (20)        0 2021-11-17 14:24:07.107186 hca-import-validation-0.0.4/hca/
--rw-r--r--   0 aherbst    (502) staff       (20)        0 2021-06-25 19:01:34.000000 hca-import-validation-0.0.4/hca/__init__.py
--rw-r--r--   0 aherbst    (502) staff       (20)    15521 2021-11-03 13:22:15.000000 hca-import-validation-0.0.4/hca/staging_area_validator.py
-drwxr-xr-x   0 aherbst    (502) staff       (20)        0 2021-11-17 14:24:07.111151 hca-import-validation-0.0.4/hca_import_validation.egg-info/
--rw-r--r--   0 aherbst    (502) staff       (20)      418 2021-11-17 14:24:07.000000 hca-import-validation-0.0.4/hca_import_validation.egg-info/PKG-INFO
--rw-r--r--   0 aherbst    (502) staff       (20)      312 2021-11-17 14:24:07.000000 hca-import-validation-0.0.4/hca_import_validation.egg-info/SOURCES.txt
--rw-r--r--   0 aherbst    (502) staff       (20)        1 2021-11-17 14:24:07.000000 hca-import-validation-0.0.4/hca_import_validation.egg-info/dependency_links.txt
--rw-r--r--   0 aherbst    (502) staff       (20)       96 2021-11-17 14:24:07.000000 hca-import-validation-0.0.4/hca_import_validation.egg-info/requires.txt
--rw-r--r--   0 aherbst    (502) staff       (20)        4 2021-11-17 14:24:07.000000 hca-import-validation-0.0.4/hca_import_validation.egg-info/top_level.txt
--rw-r--r--   0 aherbst    (502) staff       (20)      104 2021-10-19 19:27:13.000000 hca-import-validation-0.0.4/pyproject.toml
--rw-r--r--   0 aherbst    (502) staff       (20)      515 2021-11-17 14:24:07.112805 hca-import-validation-0.0.4/setup.cfg
+drwxr-xr-x   0 bhill      (503) staff       (20)        0 2022-07-08 19:01:49.023745 hca-import-validation-0.0.8/
+-rw-r--r--   0 bhill      (503) staff       (20)    11357 2022-06-21 15:56:57.000000 hca-import-validation-0.0.8/LICENSE
+-rw-r--r--   0 bhill      (503) staff       (20)      383 2022-07-08 19:01:49.023586 hca-import-validation-0.0.8/PKG-INFO
+-rw-r--r--   0 bhill      (503) staff       (20)     1616 2022-07-08 17:37:23.000000 hca-import-validation-0.0.8/README.md
+drwxr-xr-x   0 bhill      (503) staff       (20)        0 2022-07-08 19:01:49.022119 hca-import-validation-0.0.8/hca/
+-rw-r--r--   0 bhill      (503) staff       (20)        0 2022-06-21 15:56:57.000000 hca-import-validation-0.0.8/hca/__init__.py
+-rw-r--r--   0 bhill      (503) staff       (20)    15762 2022-07-08 17:37:23.000000 hca-import-validation-0.0.8/hca/staging_area_validator.py
+drwxr-xr-x   0 bhill      (503) staff       (20)        0 2022-07-08 19:01:49.023350 hca-import-validation-0.0.8/hca_import_validation.egg-info/
+-rw-r--r--   0 bhill      (503) staff       (20)      383 2022-07-08 19:01:49.000000 hca-import-validation-0.0.8/hca_import_validation.egg-info/PKG-INFO
+-rw-r--r--   0 bhill      (503) staff       (20)      311 2022-07-08 19:01:49.000000 hca-import-validation-0.0.8/hca_import_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 bhill      (503) staff       (20)        1 2022-07-08 19:01:49.000000 hca-import-validation-0.0.8/hca_import_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 bhill      (503) staff       (20)       96 2022-07-08 19:01:49.000000 hca-import-validation-0.0.8/hca_import_validation.egg-info/requires.txt
+-rw-r--r--   0 bhill      (503) staff       (20)        4 2022-07-08 19:01:49.000000 hca-import-validation-0.0.8/hca_import_validation.egg-info/top_level.txt
+-rw-r--r--   0 bhill      (503) staff       (20)      699 2022-07-08 17:37:23.000000 hca-import-validation-0.0.8/pyproject.toml
+-rw-r--r--   0 bhill      (503) staff       (20)       38 2022-07-08 19:01:49.023805 hca-import-validation-0.0.8/setup.cfg
+-rw-r--r--   0 bhill      (503) staff       (20)       94 2022-07-08 17:32:11.000000 hca-import-validation-0.0.8/setup.py
```

### Comparing `hca-import-validation-0.0.4/LICENSE` & `hca-import-validation-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hca-import-validation-0.0.4/README.md` & `hca-import-validation-0.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 # HCA Staging Import Validator
 
 Runs a pre-check of a staging area to identify issues that might cause the
 snapshot or indexing processes to fail.
 
+## Testing
+NB - this can take over 10 hours to run, depending on the size of the staging area. In the future, we may want to add a fake test staging area to speed up testing.
+```bash
+python validate_staging_area.py --staging-area <gs_path> --ignore-dangling-inputs
+```
+
+## PRs
+Once you have tested locally, built and pushed to TestPyPi successfully, you can submit a PR. Current reviewers are `aherbst-broad` and `danielsotirhos`.
+
 ## Building and publishing
 
 We follow the basic python packaging and distribution [guide](https://packaging.python.org/tutorials/packaging-projects/).
-These instructions assume you are working from the repository root, and that you have appropriate permissions to the 
+These instructions assume you are working from the repository root, and that you have appropriate permissions to the
 corresponding pypi project. It's encouraged that any changes to this package be tested via [testpypi](https://test.pypi.org) first.
+(NB you will need accounts on both PyPI and test.pypi.org, as well as permission to upload to this project in both.)
 
-* Install `build`: 
-```
+>**⚠ WARNING:**
+>Be sure to update the version number in the `pyproject.toml` file before uploading to PyPI!<br>
+
+* Install `build`:
+```bash
 python -m pip install --upgrade build
 ```
 * Build packages:
-```
+```bash
 python -m build
 ```
 * Install `twine`:
-```
+```bash
 python -m pip install --upgrade twine
 ```
-* Upload the package to pypi (ideally using an [API token](https://pypi.org/help/#apitoken))
+* Test the upload:
+```bash
+python -m twine upload --repository testpypi dist/*
 ```
+* Upload the package to pypi (ideally using an [API token](https://pypi.org/help/#apitoken))
+```bash
 python -m twine upload dist/*
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hca-import-validation-0.0.4/hca/staging_area_validator.py` & `hca-import-validation-0.0.8/hca/staging_area_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,54 @@
 import base64
 import json
 import logging
 import uuid
-from functools import (
-    cached_property,
-    lru_cache,
-)
-from typing import (
-    MutableMapping,
-    MutableSequence,
-    Optional,
-    Tuple,
-    TypeVar,
-)
-from urllib import (
-    parse,
-)
+from functools import cached_property, lru_cache
+from typing import MutableMapping, MutableSequence, Optional, Tuple, TypeVar
+from urllib import parse
 
 import google.cloud.storage as gcs
 import requests
-from jsonschema import (
-    FormatChecker,
-    validate,
-)
-from more_itertools import (
-    one,
-)
+from jsonschema import FormatChecker, validate
+from more_itertools import one
+from requests.adapters import HTTPAdapter, Retry
 
-T = TypeVar('T')
+T = TypeVar("T")
 JSON = MutableMapping[str, T]
 
 log = logging.getLogger(__name__)
 
 staging_area_properties_schema = {
-    '$schema': 'https://json-schema.org/draft/2019-09/schema',
-    'properties': {
-        'is_delta': {
-            'type': 'boolean'
-        }
-    },
-    'required': [
-        'is_delta'
-    ],
-    'additionalProperties': False
+    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "properties": {"is_delta": {"type": "boolean"}},
+    "required": ["is_delta"],
+    "additionalProperties": False,
 }
 
 
 class StagingAreaValidator:
-
     def main(self):
         self._run()
         exit_code = 0
         for file_name, e in self.file_errors.items():
-            log.error('Error with file: %s', file_name, exc_info=e)
+            log.error("Error with file: %s", file_name, exc_info=e)
         for file_name in self.extra_files:
-            log.warning('File is not part of a subgraph: %s', file_name)
+            log.warning("File is not part of a subgraph: %s", file_name)
         if self.file_errors:
             exit_code |= 1
-            log.error('Encountered %i files with errors',
-                      len(self.file_errors))
+            log.error("Encountered %i files with errors", len(self.file_errors))
         return exit_code
 
-    date_format = '%Y-%m-%dT%H:%M:%S.%fZ'
+    date_format = "%Y-%m-%dT%H:%M:%S.%fZ"
 
     def __init__(
-            self,
-            staging_area: str,
-            ignore_dangling_inputs: bool,
-            validate_json: bool
+        self,
+        staging_area: str,
+        ignore_dangling_inputs: bool,
+        validate_json: bool,
     ) -> None:
         super().__init__()
         self.staging_area = staging_area
         self.validate_json = validate_json
         self.ignore_dangling_inputs = ignore_dangling_inputs
 
         self.gcs = gcs.Client()
@@ -93,291 +70,318 @@
         return SchemaValidator()
 
     def _parse_gcs_url(self, gcs_url: str) -> Tuple[gcs.Bucket, str]:
         """
         Parse a GCS URL into its Bucket and path components
         """
         split_url = parse.urlsplit(gcs_url)
-        if split_url.scheme != 'gs' or not split_url.netloc:
-            print('Error: Google Cloud Storage URL must be in gs://<bucket>[/<path>] format')
+        if split_url.scheme != "gs" or not split_url.netloc:
+            print(
+                "Error: Google Cloud Storage URL must be in gs://<bucket>[/<path>] format"
+            )
             exit(1)
-        if split_url.path.endswith('/'):
+        if split_url.path.endswith("/"):
             print('Error: Google Cloud Storage URL must not end with a "/"')
             exit(1)
         if split_url.path:
-            path = split_url.path.lstrip('/') + '/'
+            path = split_url.path.lstrip("/") + "/"
         else:
-            path = ''
+            path = ""
         bucket = gcs.Bucket(self.gcs, split_url.netloc)
         return bucket, path
 
     def _run(self):
         self.file_errors.clear()
         self.validate_staging_area_properties()
         if not self.file_errors:
-            self.validate_files('links')
-            self.validate_files('metadata')
-            self.validate_files('descriptors')
-            self.validate_files('data')
+            self.validate_files("links")
+            self.validate_files("metadata")
+            self.validate_files("descriptors")
+            self.validate_files("data")
             self.check_results()
 
     def validate_staging_area_properties(self) -> None:
         """
         Verify and parse the staging area properties file.
         """
-        print('Checking staging area properties')
-        properties_file_path = self.sa_path + 'staging_area.json'
+        print("Checking staging area properties")
+        properties_file_path = self.sa_path + "staging_area.json"
         blob = self.bucket.get_blob(properties_file_path)
         assert isinstance(blob, gcs.Blob), properties_file_path
         file_json = self.download_blob_as_json(blob)
         self.validate_file_json(file_json, blob.name, staging_area_properties_schema)
-        self.is_delta = file_json['is_delta']
+        self.is_delta = file_json["is_delta"]
         assert isinstance(self.is_delta, bool), file_json
 
     def validate_files(self, path: str) -> None:
-        print(f'Checking files in {self.sa_path}{path}')
-        validate_file_fn = getattr(self, f'validate_{path}_file')
-        for blob in self.bucket.list_blobs(prefix=f'{self.sa_path}{path}'):
+        print(f"Checking files in {self.sa_path}{path}")
+        validate_file_fn = getattr(self, f"validate_{path}_file")
+        for blob in self.bucket.list_blobs(prefix=f"{self.sa_path}{path}"):
             try:
                 validate_file_fn(blob)
             except KeyboardInterrupt:
                 exit()
             except Exception as e:
-                log.error('File error: %s', blob.name)
+                log.error("File error: %s", blob.name)
                 self.file_errors[blob.name] = e
 
     def download_blob_as_json(self, blob: gcs.Blob) -> Optional[JSON]:
         file_json = json.loads(blob.download_as_bytes())
         return file_json
 
     def validate_links_file(self, blob: gcs.Blob) -> None:
         # Expected syntax: links/{bundle_uuid}_{version}_{project_uuid}.json
-        _, _, file_name = blob.name.rpartition('/')
-        assert file_name.count('_') == 2
-        assert file_name.endswith('.json')
-        _, _, project_uuid = file_name[:-5].split('_')
+        _, _, file_name = blob.name.rpartition("/")
+        assert file_name.count("_") == 2
+        assert file_name.endswith(".json")
+        _, _, project_uuid = file_name[:-5].split("_")
         file_json = self.download_blob_as_json(blob)
         self.validate_file_json(file_json, blob.name)
-        for link in file_json['links']:
-            link_type = link['link_type']
-            if link_type == 'process_link':
-                self.add_metadata_file(entity_id=link['process_id'],
-                                       entity_type=link['process_type'],
-                                       project_uuid=project_uuid,
-                                       category='process')
-                for category in ('input', 'output', 'protocol'):
-                    for entity in link[f'{category}s']:
-                        entity_type = entity[f'{category}_type']
-                        entity_id = entity[f'{category}_id']
-                        self.add_metadata_file(entity_id=entity_id,
-                                               entity_type=entity_type,
-                                               project_uuid=project_uuid,
-                                               category=category)
-            elif link_type == 'supplementary_file_link':
-                assert link['entity']['entity_type'] == 'project', link['entity']
-                assert link['entity']['entity_id'] == project_uuid, link['entity']
-                for entity in link['files']:
-                    entity_type = entity['file_type']
-                    entity_id = entity['file_id']
-                    self.add_metadata_file(entity_id=entity_id,
-                                           entity_type=entity_type,
-                                           project_uuid=project_uuid,
-                                           category='supplementary')
+        for link in file_json["links"]:
+            link_type = link["link_type"]
+            if link_type == "process_link":
+                self.add_metadata_file(
+                    entity_id=link["process_id"],
+                    entity_type=link["process_type"],
+                    project_uuid=project_uuid,
+                    category="process",
+                )
+                for category in ("input", "output", "protocol"):
+                    for entity in link[f"{category}s"]:
+                        entity_type = entity[f"{category}_type"]
+                        entity_id = entity[f"{category}_id"]
+                        self.add_metadata_file(
+                            entity_id=entity_id,
+                            entity_type=entity_type,
+                            project_uuid=project_uuid,
+                            category=category,
+                        )
+            elif link_type == "supplementary_file_link":
+                assert link["entity"]["entity_type"] == "project", link["entity"]
+                assert link["entity"]["entity_id"] == project_uuid, link["entity"]
+                for entity in link["files"]:
+                    entity_type = entity["file_type"]
+                    entity_id = entity["file_id"]
+                    self.add_metadata_file(
+                        entity_id=entity_id,
+                        entity_type=entity_type,
+                        project_uuid=project_uuid,
+                        category="supplementary",
+                    )
         if project_uuid not in self.metadata_files:
-            self.add_metadata_file(entity_id=project_uuid,
-                                   entity_type='project',
-                                   project_uuid=project_uuid,
-                                   category='project')
-
-    def add_metadata_file(self,
-                          entity_id: str,
-                          entity_type: str,
-                          project_uuid: str,
-                          category: str
-                          ) -> None:
+            self.add_metadata_file(
+                entity_id=project_uuid,
+                entity_type="project",
+                project_uuid=project_uuid,
+                category="project",
+            )
+
+    def add_metadata_file(
+        self, entity_id: str, entity_type: str, project_uuid: str, category: str
+    ) -> None:
         try:
             file = self.metadata_files[entity_id]
         except KeyError:
             self.metadata_files[entity_id] = {
-                'name': set(),
-                'entity_id': entity_id,
-                'entity_type': entity_type,
-                'metadata_versions': set(),
-                'descriptor_versions': set(),
-                'project': {project_uuid},
-                'category': {category},
-                'found_metadata': False,
+                "name": set(),
+                "entity_id": entity_id,
+                "entity_type": entity_type,
+                "metadata_versions": set(),
+                "descriptor_versions": set(),
+                "project": {project_uuid},
+                "category": {category},
+                "found_metadata": False,
             }
         else:
-            file['project'].add(project_uuid)
-            file['category'].add(category)
-        assert self.metadata_files[entity_id]['entity_type'] == entity_type
+            file["project"].add(project_uuid)
+            file["category"].add(category)
+        assert self.metadata_files[entity_id]["entity_type"] == entity_type
 
     def validate_metadata_file(self, blob: gcs.Blob) -> None:
         # Expected syntax: metadata/{metadata_type}/{metadata_id}_{version}.json
-        metadata_type, metadata_file = blob.name.split('/')[-2:]
-        assert metadata_file.count('_') == 1
-        assert metadata_file.endswith('.json')
-        metadata_id, metadata_version = metadata_file[:-5].split('_')
+        metadata_type, metadata_file = blob.name.split("/")[-2:]
+        assert metadata_file.count("_") == 1
+        assert metadata_file.endswith(".json")
+        metadata_id, metadata_version = metadata_file[:-5].split("_")
         file_json = self.download_blob_as_json(blob)
         self.validate_file_json(file_json, blob.name)
-        if provenance := file_json.get('provenance'):
-            assert metadata_id == provenance['document_id']
+        if provenance := file_json.get("provenance"):
+            assert metadata_id == provenance["document_id"]
         if metadata_file := self.metadata_files.get(metadata_id):
-            metadata_file['name'].add(blob.name)
-            metadata_file['metadata_versions'].add(metadata_version)
-            metadata_file['found_metadata'] = True
-            if metadata_type.endswith('_file'):
-                metadata_file['data_file_name'] = file_json['file_core']['file_name']
-                metadata_file['found_data_file'] = False
-            if metadata_type == 'supplementary_file' and file_json.get('provenance', {}).get('submitter_id'):
+            metadata_file["name"].add(blob.name)
+            metadata_file["metadata_versions"].add(metadata_version)
+            metadata_file["found_metadata"] = True
+            if metadata_type.endswith("_file"):
+                metadata_file["data_file_name"] = file_json["file_core"]["file_name"]
+                metadata_file["found_data_file"] = False
+            if metadata_type == "supplementary_file" and file_json.get(
+                "provenance", {}
+            ).get("submitter_id"):
                 try:
-                    self.validate_file_description(file_json.get('file_description'))
+                    self.validate_file_description(file_json.get("file_description"))
                 except Exception as e:
                     self.file_errors[blob.name] = e
-                    metadata_file['valid_stratification'] = False
-                    log.error('Invalid file_description in %s.', blob.name)
+                    metadata_file["valid_stratification"] = False
+                    log.error("Invalid file_description in %s.", blob.name)
                 else:
-                    metadata_file['valid_stratification'] = True
+                    metadata_file["valid_stratification"] = True
         else:
             self.extra_files.append(blob.name)
 
     def validate_file_description(self, file_description: str) -> None:
         if not file_description:
             return
         strata = [
             {
-                dimension: values.split(',')
-                for dimension, values in (point.split('=')
-                                          for point in stratum.split(';'))
-            } for stratum in file_description.split('\n')
+                dimension: values.split(",")
+                for dimension, values in (
+                    point.split("=") for point in stratum.split(";")
+                )
+            }
+            for stratum in file_description.split("\n")
         ]
         log.debug(strata)
         valid_keys = [
-            'genusSpecies',
-            'developmentStage',
-            'organ',
-            'libraryConstructionApproach',
+            "genusSpecies",
+            "developmentStage",
+            "organ",
+            "libraryConstructionApproach",
         ]
         for stratum in strata:
             for dimension, values in stratum.items():
                 assert dimension in valid_keys, stratum
                 assert len(values) > 0, stratum
 
     def validate_descriptors_file(self, blob: gcs.Blob) -> None:
         # Expected syntax: descriptors/{metadata_type}/{metadata_id}_{version}.json
-        metadata_type, descriptor_file = blob.name.split('/')[-2:]
-        assert descriptor_file.count('_') == 1
-        assert descriptor_file.endswith('.json')
+        metadata_type, descriptor_file = blob.name.split("/")[-2:]
+        assert descriptor_file.count("_") == 1
+        assert descriptor_file.endswith(".json")
 
-        metadata_id, descriptor_version = descriptor_file[:-5].split('_')
+        metadata_id, descriptor_version = descriptor_file[:-5].split("_")
         file_json = self.download_blob_as_json(blob)
         self.validate_file_json(file_json, blob.name)
-        file_name = file_json['file_name']
+        file_name = file_json["file_name"]
         self.names_to_id[file_name] = metadata_id
 
         if metadata_file := self.metadata_files.get(metadata_id):
-            metadata_file['crc32c'] = file_json['crc32c']
-            metadata_versions = metadata_file['metadata_versions']
-            assert descriptor_version in metadata_versions, f'Corresponding metadata version for descriptor version {descriptor_version} not found'
-            metadata_file['descriptor_versions'].add(descriptor_version)
+            metadata_file["crc32c"] = file_json["crc32c"]
+            metadata_versions = metadata_file["metadata_versions"]
+            assert (
+                descriptor_version in metadata_versions
+            ), f"Corresponding metadata version for descriptor version {descriptor_version} not found"
+            metadata_file["descriptor_versions"].add(descriptor_version)
         else:
             self.extra_files.append(blob.name)
 
     def validate_data_file(self, blob: gcs.Blob) -> None:
         # Expected syntax: data/{file_path}
-        prefix = self.sa_path + 'data/'
+        prefix = self.sa_path + "data/"
         assert blob.name.startswith(prefix)
-        file_name = blob.name[len(prefix):]
-        metadata_file = None
+        file_name = blob.name[len(prefix) :]
+        metadata_file = {}
         if metadata_id := self.names_to_id.get(file_name):
             if metadata_file := self.metadata_files.get(metadata_id):
-                metadata_file['found_data_file'] = True
-                assert metadata_file['crc32c'] == base64.b64decode(blob.crc32c).hex()
+                metadata_file["found_data_file"] = True
+                assert metadata_file["crc32c"] == base64.b64decode(blob.crc32c).hex()
         if metadata_file is None:
             self.extra_files.append(blob.name)
 
-    def validate_file_json(self,
-                           file_json: JSON,
-                           file_name: str,
-                           schema: Optional[JSON] = None
-                           ) -> None:
+    def validate_file_json(
+        self, file_json: JSON, file_name: str, schema: Optional[JSON] = None
+    ) -> None:
         if self.validate_json:
-            print(f'Validating JSON of {file_name}')
+            print(f"Validating JSON of {file_name}")
             try:
                 self.validator.validate_json(file_json, schema)
             except Exception as e:
-                log.error('File %s failed json validation.', file_name)
+                log.error("File %s failed json validation.", file_name)
                 self.file_errors[file_name] = e
 
     def check_results(self):
-        print('Checking results')
+        print("Checking results")
         for metadata_id, metadata_file in self.metadata_files.items():
             try:
                 self.check_result(metadata_file)
             except Exception as e:
-                log.error('File error: %s', metadata_file)
+                log.error("File error: %s", metadata_file)
                 self.file_errors[metadata_id] = e
         if not self.file_errors and not self.extra_files:
-            print('No errors found')
+            print("No errors found")
 
     def check_result(self, metadata_file):
-        if self.ignore_dangling_inputs and metadata_file['category'] == {'input'}:
+        if self.ignore_dangling_inputs and metadata_file["category"] == {"input"}:
             pass
         else:
-            if not metadata_file['found_metadata']:
-                if metadata_file['entity_type'] == 'project':
-                    log.warning('A metadata file was not found for project %s',
-                                one(metadata_file['project']))
+            if not metadata_file["found_metadata"]:
+                if metadata_file["entity_type"] == "project":
+                    log.warning(
+                        "A metadata file was not found for project %s",
+                        one(metadata_file["project"]),
+                    )
                 else:
-                    raise Exception('Did not find metadata file', metadata_file)
-            if self.is_delta and len(metadata_file['metadata_versions']) > 1:
-                raise Exception('Delta staging areas must not contain redundant '
-                                'versions of metadata.',
-                                metadata_file)
-            if metadata_file['entity_type'].endswith('_file'):
-                if not metadata_file['descriptor_versions'] == metadata_file['metadata_versions']:
-                    raise Exception('Did not find a matching descriptor file', metadata_file)
-                if not metadata_file['found_data_file']:
-                    raise Exception('Did not find data file', metadata_file)
+                    raise Exception("Did not find metadata file", metadata_file)
+            if self.is_delta and len(metadata_file["metadata_versions"]) > 1:
+                raise Exception(
+                    "Delta staging areas must not contain redundant "
+                    "versions of metadata.",
+                    metadata_file,
+                )
+            if metadata_file["entity_type"].endswith("_file"):
+                if (
+                    not metadata_file["descriptor_versions"]
+                    == metadata_file["metadata_versions"]
+                ):
+                    raise Exception(
+                        "Did not find a matching descriptor file", metadata_file
+                    )
+                if not metadata_file["found_data_file"]:
+                    raise Exception("Did not find data file", metadata_file)
         try:
-            stratification = metadata_file['valid_stratification']
+            stratification = metadata_file["valid_stratification"]
         except KeyError:
             pass
         else:
             if not stratification:
-                raise Exception('File has a invalid stratification value', metadata_file)
+                raise Exception(
+                    "File has a invalid stratification value", metadata_file
+                )
             else:
                 pass
 
     def validate_uuid(self, value: str) -> None:
         """
         Verify given value is a valid UUID string.
         """
         try:
             uuid.UUID(value)
         except ValueError as e:
-            raise ValueError('Invalid uuid value', value) from e
+            raise ValueError("Invalid uuid value", value) from e
 
 
 class SchemaValidator:
-
     @classmethod
-    def validate_json(cls,
-                      file_json: JSON,
-                      schema: Optional[JSON] = None
-                      ) -> None:
+    def validate_json(cls, file_json: JSON, schema: Optional[JSON] = None) -> None:
         if schema is None:
             try:
-                schema = cls._download_schema(file_json['describedBy'])
+                schema = cls._download_schema(file_json["describedBy"])
             except json.decoder.JSONDecodeError as e:
-                schema_url = file_json['describedBy']
-                raise Exception('Failed to parse schema JSON', schema_url) from e
+                schema_url = file_json["describedBy"]
+                raise Exception("Failed to parse schema JSON", schema_url) from e
         validate(file_json, schema, format_checker=FormatChecker())
 
     @classmethod
-    @lru_cache
+    # setting to maxsize=None so as not to evict old values, and maybe help avoid connectivity issues (DI-22)
+    @lru_cache(maxsize=None)
     def _download_schema(cls, schema_url: str) -> JSON:
-        log.debug('Downloading schema %s', schema_url)
-        response = requests.get(schema_url, allow_redirects=False)
+        log.debug("Downloading schema %s", schema_url)
+
+        s = requests.Session()
+        retries = Retry(
+            total=5, backoff_factor=0.2, status_forcelist=[500, 502, 503, 504]
+        )
+        s.mount("http://", HTTPAdapter(max_retries=retries))
+        s.mount("https://", HTTPAdapter(max_retries=retries))
+
+        response = s.get(schema_url, allow_redirects=False)
         response.raise_for_status()
         return response.json()
```

