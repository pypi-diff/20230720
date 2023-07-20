# Comparing `tmp/izihawa-ipfs-api-1.0.3.tar.gz` & `tmp/izihawa-ipfs-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa-ipfs-api-1.0.3.tar", last modified: Wed Jul 19 20:29:41 2023, max compression
+gzip compressed data, was "izihawa-ipfs-api-1.0.4.tar", last modified: Thu Jul 20 11:20:48 2023, max compression
```

## Comparing `izihawa-ipfs-api-1.0.3.tar` & `izihawa-ipfs-api-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-19 20:29:41.466143 izihawa-ipfs-api-1.0.3/
--rw-r--r--   0 pasha      (501) staff       (20)     1063 2023-07-19 19:14:30.000000 izihawa-ipfs-api-1.0.3/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 izihawa-ipfs-api-1.0.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-19 20:29:41.465543 izihawa-ipfs-api-1.0.3/PKG-INFO
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-19 20:29:41.458708 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api/
--rw-r--r--   0 pasha      (501) staff       (20)     6426 2023-07-19 20:27:04.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-19 20:29:41.464726 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-19 20:29:41.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      279 2023-07-19 20:29:41.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-19 20:29:41.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       57 2023-07-19 20:29:41.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       17 2023-07-19 20:29:41.000000 izihawa-ipfs-api-1.0.3/izihawa_ipfs_api.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      479 2023-07-19 20:27:04.000000 izihawa-ipfs-api-1.0.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       56 2023-07-19 20:13:42.000000 izihawa-ipfs-api-1.0.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-19 20:29:41.466334 izihawa-ipfs-api-1.0.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:20:48.660304 izihawa-ipfs-api-1.0.4/
+-rw-r--r--   0 pasha      (501) staff       (20)     1063 2023-07-19 19:14:30.000000 izihawa-ipfs-api-1.0.4/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 izihawa-ipfs-api-1.0.4/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 11:20:48.660015 izihawa-ipfs-api-1.0.4/PKG-INFO
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:20:48.657990 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api/
+-rw-r--r--   0 pasha      (501) staff       (20)     6473 2023-07-20 11:20:34.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:20:48.659568 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      272 2023-07-20 11:20:48.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      279 2023-07-20 11:20:48.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-20 11:20:48.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       57 2023-07-20 11:20:48.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       17 2023-07-20 11:20:48.000000 izihawa-ipfs-api-1.0.4/izihawa_ipfs_api.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      479 2023-07-20 11:20:16.000000 izihawa-ipfs-api-1.0.4/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       56 2023-07-20 11:20:14.000000 izihawa-ipfs-api-1.0.4/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-20 11:20:48.660404 izihawa-ipfs-api-1.0.4/setup.cfg
```

### Comparing `izihawa-ipfs-api-1.0.3/LICENSE` & `izihawa-ipfs-api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `izihawa-ipfs-api-1.0.3/izihawa_ipfs_api/__init__.py` & `izihawa-ipfs-api-1.0.4/izihawa_ipfs_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,23 +151,24 @@
             'cid': cid,
         })
         response = await self.post(
             f'/api/v0/ls?arg={cid}&size={json.dumps(size)}&resolve-type={json.dumps(resolve_type)}'
         )
         return await response.json()
 
-    async def ls_stream(self, cid, size=True, resolve_type=True):
+    async def ls_stream(self, cid, size=True, resolve_type=True, timeout: int = 0):
         logging.getLogger('statbox').info({
             'action': 'ls',
             'mode': 'ipfs_api_client',
             'cid': cid,
         })
         response = await self.post(
             f'/api/v0/ls?arg={cid}&size={json.dumps(size)}&resolve-type={json.dumps(resolve_type)}&stream=true',
             response_processor=None,
+            timeout=timeout,
         )
         async for line in response.content:
             yield orjson.loads(line)
 
     async def pin(self, cid: str, progress: bool = False):
         logging.getLogger('statbox').info({
             'action': 'pin',
```

