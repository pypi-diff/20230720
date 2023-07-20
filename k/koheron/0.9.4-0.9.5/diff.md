# Comparing `tmp/koheron-0.9.4.tar.gz` & `tmp/koheron-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/koheron-0.9.4.tar", last modified: Wed Sep 14 16:36:22 2016, max compression
+gzip compressed data, was "dist/koheron-0.9.5.tar", last modified: Sat Sep 17 20:31:06 2016, max compression
```

## Comparing `koheron-0.9.4.tar` & `koheron-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-14 16:36:22.000000 koheron-0.9.4/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      202 2016-09-14 16:34:01.000000 koheron-0.9.4/koheron/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2294 2016-09-14 16:34:01.000000 koheron-0.9.4/koheron/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2918 2016-09-14 16:34:01.000000 koheron-0.9.4/koheron/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9924 2016-09-14 16:34:01.000000 koheron-0.9.4/koheron/koheron.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2016-09-14 16:34:01.000000 koheron-0.9.4/koheron/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2016-09-14 16:36:22.000000 koheron-0.9.4/koheron.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2016-09-14 16:34:01.000000 koheron-0.9.4/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2016-09-14 16:36:22.000000 koheron-0.9.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2016-09-14 16:36:22.000000 koheron-0.9.4/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-17 20:31:06.000000 koheron-0.9.5/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2016-09-17 20:28:35.000000 koheron-0.9.5/koheron/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2016-09-17 20:28:35.000000 koheron-0.9.5/koheron/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2918 2016-09-17 20:28:35.000000 koheron-0.9.5/koheron/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11106 2016-09-17 20:28:35.000000 koheron-0.9.5/koheron/koheron.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2016-09-17 20:28:35.000000 koheron-0.9.5/koheron/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2016-09-17 20:31:06.000000 koheron-0.9.5/koheron.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2016-09-17 20:28:35.000000 koheron-0.9.5/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2016-09-17 20:31:06.000000 koheron-0.9.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2016-09-17 20:31:06.000000 koheron-0.9.5/setup.cfg
```

### Comparing `koheron-0.9.4/koheron/cli.py` & `koheron-0.9.5/koheron/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,15 +56,35 @@
     client = KoheronClient(host=conn_type.host, unixsock=conn_type.unixsock)
     if device is None:
         click.echo(client.commands)
     else:
         device_idx = client.devices_idx[device]
         click.echo(client.commands[device_idx])
 
+# Commands that call the HTTP API:
+
+@cli.command()
+@click.pass_obj
+def live(conn_type):
+    """Get name and version of live instrument"""
+    from .koheron import live_instrument
+    name, version = live_instrument(conn_type.host)
+    click.echo('{}-{}'.format(name, version))
+
+@cli.command()
+@click.pass_obj
+@click.argument('instrument_zip')
+@click.option('--run', is_flag=True)
+def upload(conn_type, instrument_zip, run):
+    """Upload instrument.zip"""
+    from .koheron import upload_instrument
+    upload_instrument(conn_type.host, instrument_zip, run=run)
+
 @cli.command()
 @click.pass_obj
-@click.argument('instrument_name')
-@click.option('--always_restart', is_flag=True)
-def install(conn_type, instrument_name, always_restart):
-    """Install a given instrument."""
-    from .koheron import install_instrument
-    install_instrument(conn_type.host, instrument_name, always_restart=always_restart)
+@click.argument('instrument_name', required=False)
+@click.argument('instrument_version', required=False)
+@click.option('--restart', is_flag=True)
+def run(conn_type, instrument_name, instrument_version, restart):
+    """Run a given instrument."""
+    from .koheron import run_instrument
+    run_instrument(conn_type.host, instrument_name, instrument_version, restart=restart)
```

### Comparing `koheron-0.9.4/koheron/common.py` & `koheron-0.9.5/koheron/common.py`

 * *Files identical despite different names*

### Comparing `koheron-0.9.4/koheron/koheron.py` & `koheron-0.9.5/koheron/koheron.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,43 +11,77 @@
 
 ConnectionError = requests.ConnectionError
 
 # --------------------------------------------
 # HTTP API
 # --------------------------------------------
 
-def upload_instrument(host, filename):
-	with open(filename, 'rb') as fileobj:
-		url = 'http://{}/api/instruments/upload'.format(host)
-		r = requests.post(url, files={filename: fileobj})
-
-def install_instrument(host, instrument_name, always_restart=False, verbose=False):
-    if not always_restart:
-        # Don't restart the instrument if already launched
-        current_instrument = requests.get('http://{}/api/instruments/live'.format(host)).json()
-        if current_instrument['name'] == instrument_name:
-            return
-
-    instruments = requests.get('http://{}/api/instruments/local'.format(host)).json()
-    if instruments:
-        for name, shas in instruments.items():
-            if name == instrument_name and len(shas) > 0:
-                r = requests.get('http://{}/api/instruments/run/{}/{}'.format(host, name, shas[0]))
-                if verbose:
-                    print(r.text)
-                return
-    raise ValueError("Instrument " + instrument_name + " not found")
+def live_instrument(host):
+    live_instrument = requests.get('http://{}/api/instruments/live'.format(host)).json()
+    name = live_instrument['name']
+    version = live_instrument['sha']
+    return name, version
+
+def get_name_version(filename):
+    # filename = 'name-version.zip'
+    tokens = filename.split('.')[0].split('-')
+    name = '-'.join(tokens[:-1])
+    version = tokens[-1]
+    return name, version
+
+def upload_instrument(host, filename, run=False):
+    with open(filename, 'rb') as fileobj:
+        url = 'http://{}/api/instruments/upload'.format(host)
+        r = requests.post(url, files={filename: fileobj})
+    if run:
+        name, version = get_name_version(filename)
+        r = requests.get('http://{}/api/instruments/run/{}/{}'.format(host, name, version))
+
+def run_instrument(host, name=None, version=None, restart=False):
+    instrument_running = False
+    instrument_in_store = False
+
+    live_name, live_version = live_instrument(host)
+    name_ok = (live_name == name)
+    version_ok = ((version is None) or (live_version == version))
+    
+    if (name is None) or (name_ok and version_ok): # Instrument already running
+        name, version = live_name, live_version
+        instrument_running = True
+
+    if not instrument_running: # Find the instrument in the local store:
+        instruments = requests.get('http://{}/api/instruments/local'.format(host)).json()
+        versions = instruments.get(name)
+        if versions is None:
+            raise ValueError('Instrument %s not found' % name)
+
+        if version is None:
+            # Use the first version found by default
+            version = versions[0]
+        if version in versions:
+            instrument_in_store = True
+        else:
+            raise ValueError('Did not found version {} for instrument {}'.format(version, name))
+
+    if instrument_in_store or (instrument_running and restart):
+        r = requests.get('http://{}/api/instruments/run/{}/{}'.format(host, name, version))
+
+def connect(host, *args, **kwargs):
+    run_instrument(host, *args, **kwargs)
+    client = KoheronClient(host)
+    return client
 
 def load_instrument(host, instrument='blink', always_restart=False):
-    install_instrument(host, instrument, always_restart=always_restart)
+    print('Warning: load_instrument() is deprecated, use connect() instead')
+    run_instrument(host, instrument, restart=always_restart)
     client = KoheronClient(host)
     return client
 
 # --------------------------------------------
-# command decorator
+# Command decorator
 # --------------------------------------------
 
 def command(classname=None, funcname=None):
     def real_command(func):
         def wrapper(self, *args):
             device_name = classname or self.__class__.__name__
             cmd_name = funcname or func.__name__
```

### Comparing `koheron-0.9.4/setup.py` & `koheron-0.9.5/setup.py`

 * *Files identical despite different names*

