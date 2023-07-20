# Comparing `tmp/aiobaseclient-0.2.4.tar.gz` & `tmp/aiobaseclient-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobaseclient-0.2.4.tar", last modified: Sat Apr 24 12:30:15 2021, max compression
+gzip compressed data, was "aiobaseclient-0.2.5.tar", last modified: Thu Jul 20 11:19:42 2023, max compression
```

## Comparing `aiobaseclient-0.2.4.tar` & `aiobaseclient-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2021-04-24 12:30:15.301710 aiobaseclient-0.2.4/
--rw-r--r--   0 pasha      (501) staff       (20)     1076 2021-03-29 10:25:10.000000 aiobaseclient-0.2.4/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)      353 2021-04-24 12:30:15.301964 aiobaseclient-0.2.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)       64 2021-03-29 10:25:10.000000 aiobaseclient-0.2.4/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2021-04-24 12:30:15.299726 aiobaseclient-0.2.4/aiobaseclient/
--rw-r--r--   0 pasha      (501) staff       (20)      110 2021-03-29 10:25:10.000000 aiobaseclient-0.2.4/aiobaseclient/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9204 2021-04-24 12:29:57.000000 aiobaseclient-0.2.4/aiobaseclient/base.py
--rw-r--r--   0 pasha      (501) staff       (20)      968 2021-04-05 10:46:11.000000 aiobaseclient-0.2.4/aiobaseclient/exceptions.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2021-04-24 12:30:15.301446 aiobaseclient-0.2.4/aiobaseclient.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      353 2021-04-24 12:30:15.000000 aiobaseclient-0.2.4/aiobaseclient.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      302 2021-04-24 12:30:15.000000 aiobaseclient-0.2.4/aiobaseclient.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2021-04-24 12:30:15.000000 aiobaseclient-0.2.4/aiobaseclient.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)      151 2021-04-24 12:30:15.000000 aiobaseclient-0.2.4/aiobaseclient.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       14 2021-04-24 12:30:15.000000 aiobaseclient-0.2.4/aiobaseclient.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)       89 2021-03-29 10:25:10.000000 aiobaseclient-0.2.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      653 2021-04-24 12:30:15.302632 aiobaseclient-0.2.4/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.757535 aiobaseclient-0.2.5/
+-rw-r--r--   0 pasha      (501) staff       (20)     1076 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-20 11:19:42.757727 aiobaseclient-0.2.5/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)       64 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.755326 aiobaseclient-0.2.5/aiobaseclient/
+-rw-r--r--   0 pasha      (501) staff       (20)      110 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/aiobaseclient/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9501 2023-07-20 11:14:12.000000 aiobaseclient-0.2.5/aiobaseclient/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)      968 2022-10-25 06:23:07.000000 aiobaseclient-0.2.5/aiobaseclient/exceptions.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-20 11:19:42.757146 aiobaseclient-0.2.5/aiobaseclient.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      303 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      302 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      151 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       14 2023-07-20 11:19:42.000000 aiobaseclient-0.2.5/aiobaseclient.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiobaseclient-0.2.5/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      653 2023-07-20 11:19:42.758456 aiobaseclient-0.2.5/setup.cfg
```

### Comparing `aiobaseclient-0.2.4/LICENSE` & `aiobaseclient-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobaseclient-0.2.4/aiobaseclient/base.py` & `aiobaseclient-0.2.5/aiobaseclient/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,25 @@
 
     def __init__(
         self,
         base_url: str,
         default_params: Optional[dict] = None,
         default_headers: Optional[dict] = None,
         timeout: Optional[float] = None,
-        ttl_dns_cache: Optional[float] = None,
+        use_dns_cache: bool = True,
+        ttl_dns_cache: int = 10,
         max_retries: Optional[int] = 2,
         retry_delay: Optional[float] = 0.5,
         proxy_url: Optional[str] = None,
     ):
         super().__init__()
         if base_url is None:
             raise RuntimeError(f'`base_url` must be passed for {self.__class__.__name__} constructor')
         self.base_url = base_url.rstrip('/')
+        self.use_dns_cache = use_dns_cache
         self.ttl_dns_cache = ttl_dns_cache
         self.proxy_url = proxy_url
         self.session = None
         self.default_params = CIMultiDict(filter_none(default_params or {}))
         self.default_headers = default_headers or {}
         self.timeout = timeout
         self.max_retries = max_retries
@@ -82,22 +84,24 @@
         if self.proxy_url:
             proxy_kwargs['proxy_type'],\
                 proxy_kwargs['host'],\
                 proxy_kwargs['port'],\
                 proxy_kwargs['username'],\
                 proxy_kwargs['password'] = parse_proxy_url(self.proxy_url)
             connector = ProxyConnector(
+                use_dns_cache=self.use_dns_cache,
                 ttl_dns_cache=self.ttl_dns_cache,
-                verify_ssl=False,
+                ssl=False,
                 **proxy_kwargs,
             )
         else:
             connector = aiohttp.TCPConnector(
+                use_dns_cache=self.use_dns_cache,
                 ttl_dns_cache=self.ttl_dns_cache,
-                verify_ssl=False,
+                ssl=False,
             )
         return aiohttp.ClientSession(connector=connector)
 
     async def pre_request_hook(self):
         pass
 
     async def request(
@@ -137,15 +141,15 @@
 
             response = await self.session.request(
                 method,
                 full_url,
                 params=params,
                 headers=filter_none(all_headers),
                 data=data,
-                timeout=timeout or self.timeout,
+                timeout=timeout if timeout is not None else self.timeout,
             )
             if response_processor:
                 return await response_processor(response)
             return response
         except ClientConnectorError as e:
             if isinstance(e.os_error, socket.gaierror) and (e.errno == -2 or e.errno == 111):
                 await self.session.close()
@@ -154,18 +158,20 @@
             else:
                 raise
         except (
             aiohttp.client_exceptions.ClientOSError,
             aiohttp.client_exceptions.ServerDisconnectedError,
             asyncio.TimeoutError,
             ConnectionAbortedError,
+            ConnectionResetError,
             ProxyError,
             ProxyTimeoutError,
         ) as e:
-            await self.session.close()
+            if self.session:
+                await self.session.close()
             self.session = self._create_session()
             raise TemporaryError(url=full_url, nested_error=str(e))
 
     async def delete(self, url: str = '', *args, **kwargs):
         return await self.request('delete', url, *args, **kwargs)
 
     async def get(self, url: str = '', *args, **kwargs):
@@ -189,38 +195,40 @@
     async def response_processor(self, response):
         text = await response.text()
         if response.status != 200:
             raise ExternalServiceError(response.request.url, response.status, text)
         return text
 
     async def __aenter__(self):
-        await self.start_and_wait()
+        await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.stop()
 
 
 class BaseStandardClient(BaseClient):
     def __init__(
         self,
         base_url: str,
         default_params: Optional[dict] = None,
         default_headers: Optional[dict] = None,
         timeout: Optional[float] = None,
-        ttl_dns_cache: Optional[float] = None,
+        use_dns_cache: bool = True,
+        ttl_dns_cache: int = 10,
         max_retries: Optional[int] = 2,
         retry_delay: Optional[float] = 0.5,
         proxy_url: Optional[str] = None,
     ):
         super().__init__(
             base_url=base_url,
             default_params=default_params,
             default_headers=default_headers,
             timeout=timeout,
+            use_dns_cache=use_dns_cache,
             ttl_dns_cache=ttl_dns_cache,
             max_retries=max_retries,
             retry_delay=retry_delay,
             proxy_url=proxy_url,
         )
         self.user_token = None
         self.service_token = None
```

### Comparing `aiobaseclient-0.2.4/aiobaseclient/exceptions.py` & `aiobaseclient-0.2.5/aiobaseclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiobaseclient-0.2.4/setup.cfg` & `aiobaseclient-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = 
 	Topic :: Utilities
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = aiobaseclient
 python_requires = '>=3.8'
-version = 0.2.4
+version = 0.2.5
 url = https://github.com/izihawa/aiobaseclient
 
 [options]
 packages = find:
 install_requires = 
 	aiodns >= 2.0.0
 	aiohttp >= 3.6.3
```

