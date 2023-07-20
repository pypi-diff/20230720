# Comparing `tmp/izihawa-ipfs-api-1.0.5.tar.gz` & `tmp/izihawa-ipfs-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa-ipfs-api-1.0.5.tar", last modified: Thu Jul 20 12:18:43 2023, max compression
+gzip compressed data, was "izihawa-ipfs-api-1.0.6.tar", last modified: Thu Jul 20 13:53:57 2023, max compression
```

## Comparing `izihawa-ipfs-api-1.0.5.tar` & `izihawa-ipfs-api-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 12:18:43.898648 izihawa-ipfs-api-1.0.5/
--rw-r--r--   0 pasha      (501) staff       (20)     1063 2023-07-19 19:14:30.000000 izihawa-ipfs-api-1.0.5/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 izihawa-ipfs-api-1.0.5/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 12:18:43.898414 izihawa-ipfs-api-1.0.5/PKG-INFO
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 12:18:43.896590 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api/
--rw-r--r--   0 pasha      (501) staff       (20)     6445 2023-07-20 12:17:41.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 12:18:43.897987 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 12:18:43.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      279 2023-07-20 12:18:43.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-20 12:18:43.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       57 2023-07-20 12:18:43.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       17 2023-07-20 12:18:43.000000 izihawa-ipfs-api-1.0.5/izihawa_ipfs_api.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      479 2023-07-20 12:17:41.000000 izihawa-ipfs-api-1.0.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       56 2023-07-20 11:20:14.000000 izihawa-ipfs-api-1.0.5/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-20 12:18:43.898739 izihawa-ipfs-api-1.0.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 13:53:57.990412 izihawa-ipfs-api-1.0.6/
+-rw-r--r--   0 pasha      (501) staff       (20)     1063 2023-07-19 19:14:30.000000 izihawa-ipfs-api-1.0.6/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 izihawa-ipfs-api-1.0.6/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 13:53:57.989681 izihawa-ipfs-api-1.0.6/PKG-INFO
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 13:53:57.982809 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api/
+-rw-r--r--   0 pasha      (501) staff       (20)     6445 2023-07-20 13:41:03.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 13:53:57.988345 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 13:53:57.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      279 2023-07-20 13:53:57.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-20 13:53:57.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       57 2023-07-20 13:53:57.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       17 2023-07-20 13:53:57.000000 izihawa-ipfs-api-1.0.6/izihawa_ipfs_api.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      479 2023-07-20 13:53:35.000000 izihawa-ipfs-api-1.0.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       56 2023-07-20 11:20:14.000000 izihawa-ipfs-api-1.0.6/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-20 13:53:57.990734 izihawa-ipfs-api-1.0.6/setup.cfg
```

### Comparing `izihawa-ipfs-api-1.0.5/LICENSE` & `izihawa-ipfs-api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `izihawa-ipfs-api-1.0.5/izihawa_ipfs_api/__init__.py` & `izihawa-ipfs-api-1.0.6/izihawa_ipfs_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     async def pin(self, cid: str, progress: bool = False):
         logging.getLogger('statbox').info({
             'action': 'pin',
             'mode': 'ipfs_api_client',
             'cid': cid,
         })
         response = await self.post(f"/api/v0/dag/export?arg={cid}&progress={json.dumps(progress)}")
-        return await response.json()
+        return await response.read()
 
     async def walk_ipfs_directory(self, cid, recursive=True, size=True, resolve_type=True) -> typing.AsyncIterable[NamedCid]:
         directory_content = await self.ls(cid, size=size, resolve_type=resolve_type)
         for entry in directory_content['Objects']:
             for link in entry['Links']:
                 if link['Type'] == 2 or not resolve_type:
                     yield NamedCid(name=link['Name'], cid=link['Hash'], size=link['Size'])
```

