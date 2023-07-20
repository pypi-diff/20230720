# Comparing `tmp/otter_service-0.1.75.9.tar.gz` & `tmp/otter_service-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.1.75.9.tar", last modified: Sat Oct 15 02:01:18 2022, max compression
+gzip compressed data, was "otter_service-0.2.0.tar", last modified: Thu Jul 20 18:05:03 2023, max compression
```

## Comparing `otter_service-0.1.75.9.tar` & `otter_service-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2022-10-15 02:01:18.598477 otter_service-0.1.75.9/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.1.75.9/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8166 2022-10-15 02:01:18.598684 otter_service-0.1.75.9/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2022-07-15 16:10:04.000000 otter_service-0.1.75.9/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2021-10-24 00:07:22.000000 otter_service-0.1.75.9/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2022-10-15 02:01:18.599463 otter_service-0.1.75.9/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2022-10-15 02:01:18.591199 otter_service-0.1.75.9/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2022-10-15 02:01:18.594867 otter_service-0.1.75.9/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       25 2022-10-15 02:01:05.000000 otter_service-0.1.75.9/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1753 2022-07-14 01:10:23.000000 otter_service-0.1.75.9/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.1.75.9/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     4686 2022-10-14 00:17:13.000000 otter_service-0.1.75.9/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19906 2022-08-30 23:12:46.000000 otter_service-0.1.75.9/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2022-10-15 02:01:18.598092 otter_service-0.1.75.9/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2022-06-11 00:39:08.000000 otter_service-0.1.75.9/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.1.75.9/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2022-10-15 02:01:18.597252 otter_service-0.1.75.9/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8166 2022-10-15 02:01:18.000000 otter_service-0.1.75.9/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      499 2022-10-15 02:01:18.000000 otter_service-0.1.75.9/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2022-10-15 02:01:18.000000 otter_service-0.1.75.9/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2022-10-15 02:01:18.000000 otter_service-0.1.75.9/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2022-10-15 02:01:18.000000 otter_service-0.1.75.9/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.579800 otter_service-0.2.0/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.0/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-20 18:05:03.580074 otter_service-0.2.0/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     7704 2022-07-15 16:10:04.000000 otter_service-0.2.0/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.0/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-20 18:05:03.581045 otter_service-0.2.0/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.564402 otter_service-0.2.0/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.571563 otter_service-0.2.0/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-20 17:59:45.000000 otter_service-0.2.0/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     1753 2022-07-14 01:10:23.000000 otter_service-0.2.0/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.0/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 17:50:18.000000 otter_service-0.2.0/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19879 2023-07-20 17:58:21.000000 otter_service-0.2.0/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.575688 otter_service-0.2.0/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 17:04:07.000000 otter_service-0.2.0/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.0/src/otter_service/secrets/gke_key.yaml
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.574597 otter_service-0.2.0/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-20 18:05:03.000000 otter_service-0.2.0/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-20 18:05:03.578943 otter_service-0.2.0/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.0/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 17:37:25.000000 otter_service-0.2.0/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 17:54:37.000000 otter_service-0.2.0/tests/test_otter_nb.py
```

### Comparing `otter_service-0.1.75.9/LICENSE` & `otter_service-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/PKG-INFO` & `otter_service-0.2.0/src/otter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otter_service
-Version: 0.1.75.9
+Name: otter-service
+Version: 0.2.0
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.1.75.9/README.md` & `otter_service-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/setup.cfg` & `otter_service-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/src/otter_service/access_sops_keys.py` & `otter_service-0.2.0/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/src/otter_service/firestore-test.py` & `otter_service-0.2.0/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/src/otter_service/grade_assignment.py` & `otter_service-0.2.0/src/otter_service/grade_assignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,32 @@
     :param save_path: Where to save the archive -- for testing it is "." for normal it will /tmp
     """
     download_path = "/tmp/materials.tar.gz"
     if save_path is None:
         save_path = "."
         download_path = "./materials.tar.gz"
     r = requests.get(url, stream=True)
+
     if r.status_code == 200:
         with open(download_path, 'wb') as f:
             f.write(r.raw.read())
-    file = tarfile.open(download_path)
-    file.extractall(save_path)
-    file.close()
-    url_parts = url.split("/")
-    branch = url_parts[-1].split(".")[0]
-    file_name = os.environ["AUTOGRADER_REPO"]
-    extracted_path = f"{save_path}/{file_name}-{branch}"
-    storage_path = f"{save_path}/{file_name}"
-    if os.path.isdir(storage_path):
-        shutil.rmtree(storage_path)
-    os.rename(extracted_path, storage_path)
-    os.remove(download_path)
+        file = tarfile.open(download_path)
+        file.extractall(save_path)
+        file.close()
+        url_parts = url.split("/")
+        branch = url_parts[-1].split(".")[0]
+        file_name = os.environ["AUTOGRADER_REPO"]
+        extracted_path = f"{save_path}/{file_name}-{branch}"
+        storage_path = f"{save_path}/{file_name}"
+        if os.path.isdir(storage_path):
+            shutil.rmtree(storage_path)
+        os.rename(extracted_path, storage_path)
+        os.remove(download_path)
+    else:
+        raise Exception(f"Unable to access: {url}")
     return storage_path
 
 def remove_notebook():
     files = glob.glob('/tmp/*')
     for f in files:
         if not os.path.isdir(f):
             os.remove(f)
@@ -88,29 +91,33 @@
         process = await asyncio.create_subprocess_exec(
             *command,
             stdin=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE
         )
 
-        async with async_timeout.timeout(600):
+        # this is waiting for communication back from the process
+        # some images are quite big and take some time to build the first
+        # time through - like 20 min for otter-grader
+        async with async_timeout.timeout(2000):
             stdout, stderr = await process.communicate()
 
         for line in stderr.decode('utf-8').split('\n'):
             if line.strip() == '':
                 # Ignore empty lines
                 continue
             if 'Killed' in line:
                 # Our container was killed, so let's just skip this one
                 raise Exception(f"Container was killed -- nothing will work: {submission}")
+
         grade = stdout.decode("utf-8").strip()
         if grade is None or grade == '':
             cmd = ' '.join(command)
             raise Exception(f"Unable to determine grade coming from otter on: {submission} using this commnad: {cmd}")
-        
+
         return float(grade)
     except asyncio.TimeoutError:
         raise Exception(f'Grading timed out for {submission}')
     except Exception as e:
         raise e
     finally:
         remove_notebook()
```

### Comparing `otter_service-0.1.75.9/src/otter_service/otter_nb.py` & `otter_service-0.2.0/src/otter_service/otter_nb.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 import tornado.gen
 from tornado.web import authenticated
 from otter_service import access_sops_keys
 from otter_service.grade_assignment import grade_assignment
 import firebase_admin
 from firebase_admin import credentials, firestore
 import grpc
-from google.cloud.firestore_v1.gapic import firestore_client
-from google.cloud.firestore_v1.gapic.transports import firestore_grpc_transport
+from google.cloud.firestore_v1.client import firestore_client
+from google.cloud.firestore_v1.client import firestore_grpc_transport
 
-PREFIX = os.environ.get('JUPYTERHUB_SERVICE_PREFIX', '/services/gofer_nb/')
+PREFIX = os.environ.get('JUPYTERHUB_SERVICE_PREFIX', '/services/otter_grade/')
 
 # Use the application default credentials
 cred = credentials.ApplicationDefault()
 firebase_admin.initialize_app(cred, {
     'projectId': os.environ.get("GCP_PROJECT_ID"),
     'storageBucket': 'data8x-scratch.appspot.com/submissions'
 })
@@ -237,15 +237,15 @@
 
     # @authenticated
     async def post(self):
         notebook = None
         section = None
         assignment = None
         user = {}
-        course = "8x-default-should-be-in-notebook"
+        course = "not-set-yet"
         timestamp = get_timestamp()
         using_test_user = False
         try:
             # Accept notebook submissions, saves, then grades them
             user = self.get_current_user()
             log_info_csv("PRINT USER OBJ", course, section, assignment, str(user))
             if user is None:
```

### Comparing `otter_service-0.1.75.9/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.0/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.1.75.9/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otter-service
-Version: 0.1.75.9
+Name: otter_service
+Version: 0.2.0
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

