# Comparing `tmp/indiredis-0.7.1.tar.gz` & `tmp/indiredis-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indiredis-0.7.1.tar", last modified: Mon Jul  3 09:02:39 2023, max compression
+gzip compressed data, was "indiredis-0.7.2.tar", last modified: Thu Jul 20 11:45:07 2023, max compression
```

## Comparing `indiredis-0.7.1.tar` & `indiredis-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1056 2023-03-09 20:41:53.000000 indiredis-0.7.1/LICENSE
--rw-r--r--   0        0        0     3152 2023-04-09 16:31:47.000000 indiredis-0.7.1/README.md
--rw-r--r--   0        0        0    27975 2023-07-03 08:44:38.000000 indiredis-0.7.1/indiredis/__init__.py
--rw-r--r--   0        0        0     4281 2023-07-02 21:58:36.000000 indiredis-0.7.1/indiredis/__main__.py
--rw-r--r--   0        0        0    13939 2023-03-10 12:21:24.000000 indiredis-0.7.1/indiredis/indiredis/data/defaults.json
--rw-r--r--   0        0        0    64481 2023-07-02 21:57:31.000000 indiredis-0.7.1/indiredis/indiredis/data/project.json
--rw-r--r--   0        0        0     3008 2023-03-10 22:48:31.000000 indiredis-0.7.1/indiredis/indiredis/data/textblocks_json/en.json
--rw-r--r--   0        0        0     1524 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/css/w3-theme-ski.css
--rw-r--r--   0        0        0      712 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/images/logo.svg
--rw-r--r--   0        0        0      513 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/indiredis/static/images/logo_icon16.svg
--rw-r--r--   0        0        0        0 2023-03-09 20:41:53.000000 indiredis-0.7.1/indiredis/webcode/__init__.py
--rw-r--r--   0        0        0     1505 2023-03-11 17:09:55.000000 indiredis-0.7.1/indiredis/webcode/authenticate.py
--rw-r--r--   0        0        0     1846 2023-03-10 15:01:26.000000 indiredis-0.7.1/indiredis/webcode/blobs.py
--rw-r--r--   0        0        0    52167 2023-07-03 08:41:14.000000 indiredis-0.7.1/indiredis/webcode/devices.py
--rw-r--r--   0        0        0    20832 2023-07-03 08:49:15.000000 indiredis-0.7.1/indiredis/webcode/setvalues.py
--rw-r--r--   0        0        0     1000 2023-07-02 21:57:39.000000 indiredis-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 indiredis-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-03-09 20:41:53.000000 indiredis-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3152 2023-04-09 16:31:47.000000 indiredis-0.7.2/README.md
+-rw-r--r--   0        0        0    27975 2023-07-03 08:44:38.000000 indiredis-0.7.2/indiredis/__init__.py
+-rw-r--r--   0        0        0     3856 2023-07-20 11:34:03.000000 indiredis-0.7.2/indiredis/__main__.py
+-rw-r--r--   0        0        0    13939 2023-03-10 12:21:24.000000 indiredis-0.7.2/indiredis/indiredis/data/defaults.json
+-rw-r--r--   0        0        0    64481 2023-07-20 11:34:27.000000 indiredis-0.7.2/indiredis/indiredis/data/project.json
+-rw-r--r--   0        0        0     3008 2023-03-10 22:48:31.000000 indiredis-0.7.2/indiredis/indiredis/data/textblocks_json/en.json
+-rw-r--r--   0        0        0     1524 2023-03-09 20:41:53.000000 indiredis-0.7.2/indiredis/indiredis/static/css/w3-theme-ski.css
+-rw-r--r--   0        0        0      712 2023-03-09 20:41:53.000000 indiredis-0.7.2/indiredis/indiredis/static/images/logo.svg
+-rw-r--r--   0        0        0      513 2023-03-09 20:41:53.000000 indiredis-0.7.2/indiredis/indiredis/static/images/logo_icon16.svg
+-rw-r--r--   0        0        0        0 2023-03-09 20:41:53.000000 indiredis-0.7.2/indiredis/webcode/__init__.py
+-rw-r--r--   0        0        0     1505 2023-03-11 17:09:55.000000 indiredis-0.7.2/indiredis/webcode/authenticate.py
+-rw-r--r--   0        0        0     1846 2023-03-10 15:01:26.000000 indiredis-0.7.2/indiredis/webcode/blobs.py
+-rw-r--r--   0        0        0    52167 2023-07-03 08:41:14.000000 indiredis-0.7.2/indiredis/webcode/devices.py
+-rw-r--r--   0        0        0    20832 2023-07-03 08:49:15.000000 indiredis-0.7.2/indiredis/webcode/setvalues.py
+-rw-r--r--   0        0        0     1000 2023-07-20 11:33:24.000000 indiredis-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 indiredis-0.7.2/PKG-INFO
```

### Comparing `indiredis-0.7.1/LICENSE` & `indiredis-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/README.md` & `indiredis-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/__init__.py` & `indiredis-0.7.2/indiredis/__init__.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/__main__.py` & `indiredis-0.7.2/indiredis/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # any wsgi web server can serve the wsgi application produced by make_wsgi_app,
 # in this example the web server 'waitress' is used
 
 from waitress import serve
 
 from . import make_wsgi_app
 
-version = "0.7.1"
+version = "0.7.2"
 
 if __name__ == "__main__":
 
 
     parser = argparse.ArgumentParser(usage="python3 -m indiredis [options] blobdirectorypath",
         description="INDI web client communicating to indiserver and saving data to redis and to a BLOB directory.",
         epilog="The --clientonly option disables the connection to indiserver, iport and ihost will be ignored. This requires the redis database to be connected to drivers by some other process, typically using functions from package indi-mr.")
@@ -54,27 +54,16 @@
     indi_host = indi_server(host=args.ihost, port=args.iport)
     redis_host = redis_server(host=args.rhost, port=args.rport, db=0, password='', keyprefix=args.prefix,
                               to_indi_channel=args.toindipub, from_indi_channel=args.fromindipub)
 
     # create a wsgi application
     application = make_wsgi_app(redis_host, args.blobdirectorypath, url='/')
 
-<<<<<<< HEAD
-
-    # serve the application with the python waitress web server in another thread
-    webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':args.host, 'port':args.port})
-    webapp.start()
-
-    # and start the blocking function inditoredis
-    inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=args.blobdirectorypath)
-=======
     if args.clientonly:
         # blocking call which serves the application with the python waitress web server
         serve(application, host=args.host, port=args.port)
     else:
         # serve the application with the python waitress web server in another thread
         webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':args.host, 'port':args.port})
         webapp.start()
         # and start the blocking function inditoredis
         inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=args.blobdirectorypath)
-
->>>>>>> 6f1160a9d49c1389e503389f35351870101dd24e
```

### Comparing `indiredis-0.7.1/indiredis/indiredis/data/defaults.json` & `indiredis-0.7.2/indiredis/indiredis/data/defaults.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/indiredis/data/project.json` & `indiredis-0.7.2/indiredis/indiredis/data/project.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.7.2'"}*

```diff
@@ -4317,9 +4317,9 @@
         "skipolelogo": 3001,
         "url_not_found": 2080,
         "validate_error": 2010,
         "w3_css": "skis,w3_css",
         "w3_theme_ski_css": 1008
     },
     "url": "/",
-    "version": "0.7.1"
+    "version": "0.7.2"
 }
```

### Comparing `indiredis-0.7.1/indiredis/indiredis/data/textblocks_json/en.json` & `indiredis-0.7.2/indiredis/indiredis/data/textblocks_json/en.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/indiredis/static/css/w3-theme-ski.css` & `indiredis-0.7.2/indiredis/indiredis/static/css/w3-theme-ski.css`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/indiredis/static/images/logo.svg` & `indiredis-0.7.2/indiredis/indiredis/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/indiredis/static/images/logo_icon16.svg` & `indiredis-0.7.2/indiredis/indiredis/static/images/logo_icon16.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/webcode/authenticate.py` & `indiredis-0.7.2/indiredis/webcode/authenticate.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/webcode/blobs.py` & `indiredis-0.7.2/indiredis/webcode/blobs.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/webcode/devices.py` & `indiredis-0.7.2/indiredis/webcode/devices.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/indiredis/webcode/setvalues.py` & `indiredis-0.7.2/indiredis/webcode/setvalues.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.7.1/pyproject.toml` & `indiredis-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indiredis"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License","Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.7.1"
+version = "0.7.2"
 description="An INDI web client for general Instrument control. If the package is run, it provides a web service for controlling instruments. If imported, it provides functions which can be adapted to your own web server."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 dependencies = ["skipole>=5.5.2", "indi-mr>=0.4.0", "paho-mqtt>=1.5.1", "redis>=3.5.3", "waitress>=1.4.4"]
 
 [project.urls]
```

### Comparing `indiredis-0.7.1/PKG-INFO` & `indiredis-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiredis
-Version: 0.7.1
+Version: 0.7.2
 Summary: An INDI web client for general Instrument control. If the package is run, it provides a web service for controlling instruments. If imported, it provides functions which can be adapted to your own web server.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

