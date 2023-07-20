# Comparing `tmp/psytricks-2.1.5.tar.gz` & `tmp/psytricks-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.5.tar", max compression
+gzip compressed data, was "psytricks-2.1.6.tar", max compression
```

## Comparing `psytricks-2.1.5.tar` & `psytricks-2.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.5/LICENSE
--rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.5/README.md
--rw-r--r--   0        0        0     1112 2023-07-17 20:45:24.275203 psytricks-2.1.5/pyproject.toml
--rw-r--r--   0        0        0       93 2023-07-17 20:45:24.279203 psytricks-2.1.5/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6146 2023-07-17 20:45:24.279203 psytricks-2.1.5/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.5/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.5/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.5/src/psytricks/mappings.py
--rw-r--r--   0        0        0    24643 2023-07-17 20:43:21.773770 psytricks-2.1.5/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 psytricks-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.6/LICENSE
+-rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.6/README.md
+-rw-r--r--   0        0        0     1112 2023-07-20 13:31:58.951332 psytricks-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-07-20 13:31:58.955332 psytricks-2.1.6/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6262 2023-07-20 13:31:58.955332 psytricks-2.1.6/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.6/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.6/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.6/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.6/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.6/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    24645 2023-07-20 13:30:58.326658 psytricks-2.1.6/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 psytricks-2.1.6/PKG-INFO
```

### Comparing `psytricks-2.1.5/LICENSE` & `psytricks-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/README.md` & `psytricks-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/pyproject.toml` & `psytricks-2.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.5"
+version = "2.1.6"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.6/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.5"
+$Version = "2.1.6"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
@@ -124,14 +124,17 @@
         -AdminAddress $AdminAddress `
         -DesktopGroupName $Group
 
     if ($null -eq $Policy) {
         throw "Error fetching permissions for Delivery Group [$Group]!"
     }
 
+    # convert into a string array (required in case of multiple usernames):
+    $UserNames = $UserNames.Split(",")
+
     if ($RemoveAccess) {
         $Data = Set-BrokerAccessPolicyRule `
             -AdminAddress $AdminAddress `
             -InputObject $Policy `
             -RemoveIncludedUsers $UserNames `
             -PassThru | `
             Select-Object -ExpandProperty IncludedUsers
```

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.6/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.6/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.6/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.6/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/cli.py` & `psytricks-2.1.6/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/decoder.py` & `psytricks-2.1.6/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/literals.py` & `psytricks-2.1.6/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/mappings.py` & `psytricks-2.1.6/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.5/src/psytricks/wrapper.py` & `psytricks-2.1.6/src/psytricks/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,35 +479,33 @@
             log.error(f"GET request [{raw_url}] didn't return any JSON: {ex}")
             raise ex
 
         ResTricksWrapper._check_response(response)
 
         return data
 
-    def send_post_request(
-        self, raw_url: str, payload: dict, no_json: bool = False
-    ) -> list:
+    def send_post_request(self, raw_url: str, payload: dict, no_json: bool = False):
         """Common method to perform a `POST` request and process the response.
 
         Parameters
         ----------
         raw_url : str
             The part of the URL that will be appended to `self.base_url`.
         payload : dict
             The parameters to pass as `JSON` payload to the POST request.
         no_json : bool
             If set to `True` the response is expected to contain no `JSON` and
             an empty list will be returned.
 
         Returns
         -------
-        list
-            The parsed `JSON` of the response, usually a list of dict. Will be
-            an empty list in case something went wrong performing the POST
-            request or processing the response (or in case the `no_json`
+        list or dict or None
+            The parsed `JSON` of the response, often a dict or a list of dict.
+            Will be an empty list in case something went wrong performing the
+            POST request or processing the response (or in case the `no_json`
             parameter was set to `True`).
         """
         try:
             response = requests.post(
                 self.base_url + raw_url, json=payload, timeout=self.timeout
             )
         except Exception as ex:  # pylint: disable-msg=broad-except
```

### Comparing `psytricks-2.1.5/PKG-INFO` & `psytricks-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.5
+Version: 2.1.6
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

