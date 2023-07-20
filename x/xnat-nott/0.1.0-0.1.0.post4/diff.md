# Comparing `tmp/xnat_nott-0.1.0.tar.gz` & `tmp/xnat_nott-0.1.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnat_nott-0.1.0.tar", last modified: Thu Apr 20 12:51:50 2023, max compression
+gzip compressed data, was "dist/xnat_nott-0.1.0.post4.tar", last modified: Thu Jul 20 09:22:48 2023, max compression
```

## Comparing `xnat_nott-0.1.0.tar` & `xnat_nott-0.1.0.post4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 12:51:50.405914 xnat_nott-0.1.0/
--rw-r--r--   0 martin    (1000) martin    (1000)      765 2023-04-20 12:51:50.405914 xnat_nott-0.1.0/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      346 2023-04-20 12:44:02.000000 xnat_nott-0.1.0/README.md
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-04-20 12:51:50.405914 xnat_nott-0.1.0/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3789 2023-04-20 12:46:26.000000 xnat_nott-0.1.0/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 12:51:50.405914 xnat_nott-0.1.0/xnat_nott/
--rw-r--r--   0 martin    (1000) martin    (1000)    10824 2023-04-20 12:41:08.000000 xnat_nott-0.1.0/xnat_nott/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       71 2023-04-20 12:51:49.000000 xnat_nott-0.1.0/xnat_nott/_version.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-04-20 12:51:50.405914 xnat_nott-0.1.0/xnat_nott.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)      765 2023-04-20 12:51:49.000000 xnat_nott-0.1.0/xnat_nott.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      226 2023-04-20 12:51:50.000000 xnat_nott-0.1.0/xnat_nott.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-04-20 12:51:50.000000 xnat_nott-0.1.0/xnat_nott.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       10 2023-04-20 12:51:50.000000 xnat_nott-0.1.0/xnat_nott.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       10 2023-04-20 12:51:50.000000 xnat_nott-0.1.0/xnat_nott.egg-info/top_level.txt
+drwxrwxr-x   0 bbzmsc    (1042) bbzmsc    (1045)        0 2023-07-20 09:22:48.000000 xnat_nott-0.1.0.post4/
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)    10174 2023-07-20 09:22:24.000000 xnat_nott-0.1.0.post4/LICENSE
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       33 2023-07-20 09:21:57.000000 xnat_nott-0.1.0.post4/MANIFEST.in
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)      847 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/PKG-INFO
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)      420 2023-07-20 09:20:12.000000 xnat_nott-0.1.0.post4/README.md
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       10 2023-07-20 09:20:12.000000 xnat_nott-0.1.0.post4/requirements.txt
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       38 2023-07-20 09:22:48.000000 xnat_nott-0.1.0.post4/setup.cfg
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)     3789 2023-07-20 09:20:12.000000 xnat_nott-0.1.0.post4/setup.py
+drwxrwxr-x   0 bbzmsc    (1042) bbzmsc    (1045)        0 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott/
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)    12971 2023-07-20 09:20:12.000000 xnat_nott-0.1.0.post4/xnat_nott/__init__.py
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       77 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott/_version.py
+drwxrwxr-x   0 bbzmsc    (1042) bbzmsc    (1045)        0 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)      847 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/PKG-INFO
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)      263 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/SOURCES.txt
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)        1 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/dependency_links.txt
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       10 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/requires.txt
+-rw-rw-r--   0 bbzmsc    (1042) bbzmsc    (1045)       10 2023-07-20 09:22:47.000000 xnat_nott-0.1.0.post4/xnat_nott.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xnat_nott-0.1.0/PKG-INFO` & `xnat_nott-0.1.0.post4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: xnat_nott
-Version: 0.1.0
+Version: 0.1.0.post4
 Summary: Helper functions for XNAT applications/containers
 Author: Martin Craig
 Author-email: martin.craig@nottingham.ac.uk
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # XNAT helper functions
 
 Simple set of XNAT helper functions targeted at Nottingham applications. These 
 functions were originally built in to various XNAT applications where they 
 acquired fixes and code aimed to work around XNAT oddities. It seemed best to 
 merge these into a combined set of helpers that can be re-used in different projects
 
+# To do
 
-
+Could make functions into an object but might reduce flexibility
```

### Comparing `xnat_nott-0.1.0/setup.py` & `xnat_nott-0.1.0.post4/setup.py`

 * *Files identical despite different names*

### Comparing `xnat_nott-0.1.0/xnat_nott/__init__.py` & `xnat_nott-0.1.0.post4/xnat_nott/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,63 +8,70 @@
 import json
 import logging
 import os
 import requests
 import sys
 import tempfile
 import urllib, urllib3
+import zipfile
 
 import xmltodict
 
 LOG = logging.getLogger(__name__)
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+os.environ["CURL_CA_BUNDLE"] = "" # Hack to disable CA verification
 
-def setup_logging(options):
+def setup_logging(options, **kwargs):
+    format=kwargs.get("format", "%(levelname)s: %(message)s")
     if options.debug:
-        logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+        logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format=format)
     else:
-        logging.basicConfig(stream=sys.stdout, level=logging.INFO)
+        logging.basicConfig(stream=sys.stdout, level=logging.INFO, format=format)
 
 def get_version(options):
     try:
         with open("version.txt") as f:
             options.version = f.read().strip()
     except IOError:
         options.version = "(unknown)"
 
-def convert_dicoms(dicomdir, niftidir):
+def convert_dicoms(options, dicomdir, niftidir):
+    LOG.info(f"Doing NIFTI conversion")
+    dcm2niix_args = getattr(options, "dcm2niix_args", "-d 9 -m n -f %d_%q -z y -b y")
     os.makedirs(niftidir, exist_ok=True, mode=0o777)
-    cmd = "dcm2niix -o %s %s %s" % (niftidir, "-m n -f %d_%q -z y", dicomdir)
+    cmd = f'dcm2niix -o "{niftidir}" {dcm2niix_args} "{dicomdir}"'
     LOG.info(cmd)
-    retval = os.system(cmd)
+    retval = os.system(cmd + f" 2>&1 1>{niftidir}/dcm2niix.log")
     if retval != 0:
-        LOG.warning("DICOM->NIFTI conversion failed")
-        return None
-    return niftidir
+        LOG.warning(f"DICOM->NIFTI conversion returned error status {retval}")
+    return retval
 
 def get_host_url(options):
     """
     Get the 'real' URL for XNAT, since it may be subject to redirects and these mess up POST/PUT requests
     """
+    if not getattr(options, "host", None):
+        options.host = os.environ.get("XNAT_HOST", None)
     if not options.host:
-        options.host = os.environ["XNAT_HOST"]
+        raise RuntimeError("XNAT host not specified and not in environment")
     LOG.info(f"Checking host URL: {options.host}")
-    r = requests.get(options.host, verify=False, allow_redirects=False)
+    options.host = options.host.rstrip("/")
+    r = requests.get(options.host + "/", verify=False, allow_redirects=False)
     if r.status_code in (301, 302):
         new_host = r.headers['Location']
         LOG.info(f" - Redirect detected: {new_host}")
         # Sometimes gets redirected to login page - don't want this!
         if "/app/" in new_host:
             new_host = new_host[:new_host.index("/app/")]
         options.host = new_host
     options.host = options.host.rstrip("/")
 
 def get_credentials(options):
     get_host_url(options)
-    if not options.user:
+    if not getattr(options, "user", None):
         options.user = os.environ.get("XNAT_USER", None)
     if not options.user:
         options.user = input("XNAT username: ")
     options.password = os.environ.get("XNAT_PASS", None)
     if not options.password:
         options.password = getpass.getpass()
     LOG.info(f"Using XNAT server at: {options.host} with username: {options.user}")
@@ -104,14 +111,28 @@
     project_id = project["ID"]
     LOG.debug(f"Getting subjects for prject {project_id}")
     params={"format" : "csv"}
     csvdata = xnat_get(options, f"data/projects/{project_id}/subjects/", params=params)
     subjects = list(csv.DictReader(io.StringIO(csvdata)))
     return subjects
 
+def get_subject(options, project, subject_identifier):
+    """
+    Get subject details from specified project and subject label/ID
+
+    :param subject_identifier: Case insensitive identifier, may be ID or label
+    """
+    subject_identifier = subject_identifier.lower()
+    subjects = get_subjects(options, project)
+    for s in subjects:
+        if s["ID"].lower() == subject_identifier or s["label"].lower() == subject_identifier:
+            return s
+
+    raise RuntimeError(f"Subject not found: {subject_identifier}")
+
 def get_sessions(options, project, subject):
     """
     Get session details for specified project and subject
     """
     project_id = project["ID"]
     subject_id = subject["ID"]
     LOG.debug(f"Getting sessions for project {project_id}, subject {subject_id}")
@@ -121,14 +142,28 @@
     csvdata = xnat_get(options, f"data/projects/{project_id}/subjects/{subject_id}/experiments/", params=params)
     for session in list(csv.DictReader(io.StringIO(csvdata))):
         session["subject"] = subject_id
         session["subject_label"] = subject['label']
         sessions.append(session)
     return sessions
 
+def get_session(options, project, subject, session_identifier):
+    """
+    Get session details from specified project, subject and session label/ID
+
+    :param session_identifier: Case insensitive identifier, may be ID or name
+    """
+    session_identifier = session_identifier.lower()
+    sessions = get_sessions(options, project, subject)
+    for s in sessions:
+        if s["ID"].lower() == session_identifier or s["label"].lower() == session_identifier:
+            return s
+
+    raise RuntimeError(f"Session not found: {session_identifier}")
+
 def get_all_sessions(options, project):
     """
     Get session details for all subjects in specified project
     """
     project_id = project["ID"]
     LOG.debug(f"Getting all sessions for project {project_id}")
     
@@ -178,32 +213,46 @@
     command_name, command_id, wrapper_id = command["command-name"], command["command-id"], command["wrapper-id"]
     project_id, session_id = project["ID"], session["ID"]
     LOG.info(f"Running command {command_name} on session {idx} {session_id} : {session['label']}")
 
     url = f"xapi/projects/{project_id}/commands/{command_id}/wrappers/{wrapper_id}/launch/"
     params = {"session" : session_id}
     xnat_get(options, url, params=params, method="POST")
-#        LOG.warning(f"Failed to run command on session {session_id}: {r.text} after 10 attempts")
     LOG.info("Started successfully")
 
+def get_session_dicoms(options, session, outdir):
+    session_id = session["ID"]
+    LOG.info(f"Getting DICOMs for session {session_id}")
+    data_fname = xnat_download(
+        options,
+        f"data/experiments/{session_id}/scans/ALL/resources/DICOM/files",
+        params={"format" : "zip"}
+    )
+    try:
+        with zipfile.ZipFile(data_fname, 'r') as z:
+            z.extractall(outdir)
+    finally:
+        os.remove(data_fname)
+
 def xnat_login(options):
     """
     Attempt to use the auth service to log in but fall back on HTTP basic auth if not working
     """
     url = f"{options.host}/data/services/auth"
     auth_params={"username" : options.user, "password" : options.password}
     LOG.info(f"Attempting log in: {url}")
     r = requests.put(url, verify=False, data=urllib.parse.urlencode(auth_params))
     LOG.debug(f"status: {r.status_code}")
     if r.status_code == 200:
         LOG.info(" - Logged in using auth service")
         options.cookies = {"JSESSIONID" : r.text}
         options.auth = None
     else:
-        LOG.info(f" - Failed to log in using auth service - will use basic auth instead")
+        LOG.warn(f" - Failed to log in using auth service, status {r.status_code} - will use basic auth instead")
+        LOG.warn(r.text)
         options.cookies = {}
         options.auth = (options.user, options.password)
     LOG.info("DONE login")
 
 def xnat_get(options, url, params=None, method="GET"):
     """
     Get text content from XNAT, e.g. CSV/XML data
@@ -218,27 +267,31 @@
         raise RuntimeError(f"No such HTTP method: {method}")
 
     while tries < 10:
         tries += 1
         r = method_impl(url, verify=False, cookies=options.cookies, auth=options.auth, params=params)
         if r.status_code == 200:
             break
+        if r.status_code == 401:
+            LOG.info(" - Session expired, will re-login and retry")
+            xnat_login(options)
+
     if r.status_code != 200:
         raise RuntimeError(f"Failed to execute {method} after 10 tries: {r.status_code} {r.text}")
     return r.text
 
 def xnat_download(options, url, params=None, local_fname=None):
     LOG.info(f"Downloading data from {options.host}")
     url = url.lstrip("/")
     url = f"{options.host}/{url}"
     LOG.info(f" - URL: {url}")
     r = requests.get(url, verify=False, cookies=options.cookies, auth=options.auth, params=params, stream=True)
     LOG.debug(f" - status: {r.status_code}")
     if r.status_code == 401:
-        print(" - Session expired, will re-login and retry")
+        LOG.info(" - Session expired, will re-login and retry")
         xnat_login(options)
         r = requests.get(url, verify=False, cookies=options.cookies, auth=options.auth, params=params, stream=True)
     r.raise_for_status()
 
     if not local_fname:
         local_fname = tempfile.NamedTemporaryFile(delete=False).name
     try:
```

### Comparing `xnat_nott-0.1.0/xnat_nott.egg-info/PKG-INFO` & `xnat_nott-0.1.0.post4/xnat_nott.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: xnat-nott
-Version: 0.1.0
+Version: 0.1.0.post4
 Summary: Helper functions for XNAT applications/containers
 Author: Martin Craig
 Author-email: martin.craig@nottingham.ac.uk
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # XNAT helper functions
 
 Simple set of XNAT helper functions targeted at Nottingham applications. These 
 functions were originally built in to various XNAT applications where they 
 acquired fixes and code aimed to work around XNAT oddities. It seemed best to 
 merge these into a combined set of helpers that can be re-used in different projects
 
+# To do
 
-
+Could make functions into an object but might reduce flexibility
```

