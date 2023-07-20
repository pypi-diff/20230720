# Comparing `tmp/dupla-0.0.1.tar.gz` & `tmp/dupla-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dupla-0.0.1.tar", last modified: Tue May  9 11:59:32 2023, max compression
+gzip compressed data, was "dupla-0.0.2.tar", last modified: Thu Jul 20 12:16:40 2023, max compression
```

## Comparing `dupla-0.0.1.tar` & `dupla-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-05-09 11:59:32.921887 dupla-0.0.1/
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)    11303 2023-02-17 07:55:30.000000 dupla-0.0.1/LICENSE
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       27 2023-05-04 12:00:25.000000 dupla-0.0.1/MANIFEST.in
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3861 2023-05-09 11:59:32.921887 dupla-0.0.1/PKG-INFO
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3307 2023-05-04 12:00:25.000000 dupla-0.0.1/README.md
-drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-05-09 11:59:32.921887 dupla-0.0.1/dupla/
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      197 2023-05-04 12:00:25.000000 dupla-0.0.1/dupla/__init__.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        6 2023-05-04 12:16:18.000000 dupla-0.0.1/dupla/_version.txt
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     6713 2023-05-03 07:40:10.000000 dupla-0.0.1/dupla/base.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3427 2023-05-08 20:11:45.000000 dupla-0.0.1/dupla/dupla.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     9077 2023-05-08 20:11:45.000000 dupla-0.0.1/dupla/endpoint.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      389 2023-05-03 07:40:10.000000 dupla-0.0.1/dupla/exceptions.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      772 2023-05-03 07:40:10.000000 dupla-0.0.1/dupla/validation.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      274 2023-05-04 12:00:25.000000 dupla-0.0.1/dupla/version.py
-drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-05-09 11:59:32.921887 dupla-0.0.1/dupla.egg-info/
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3861 2023-05-09 11:59:32.000000 dupla-0.0.1/dupla.egg-info/PKG-INFO
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      403 2023-05-09 11:59:32.000000 dupla-0.0.1/dupla.egg-info/SOURCES.txt
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        1 2023-05-09 11:59:32.000000 dupla-0.0.1/dupla.egg-info/dependency_links.txt
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      166 2023-05-09 11:59:32.000000 dupla-0.0.1/dupla.egg-info/requires.txt
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        6 2023-05-09 11:59:32.000000 dupla-0.0.1/dupla.egg-info/top_level.txt
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1163 2023-05-04 12:00:25.000000 dupla-0.0.1/pyproject.toml
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       38 2023-05-09 11:59:32.921887 dupla-0.0.1/setup.cfg
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       77 2023-05-03 07:40:10.000000 dupla-0.0.1/setup.py
-drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-05-09 11:59:32.921887 dupla-0.0.1/tests/
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     5060 2023-05-08 20:11:45.000000 dupla-0.0.1/tests/test_api.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1598 2023-05-08 19:53:59.000000 dupla-0.0.1/tests/test_dupla.py
--rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1091 2023-05-04 06:42:59.000000 dupla-0.0.1/tests/test_verification.py
+drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-07-20 12:16:40.460486 dupla-0.0.2/
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)    11304 2023-07-20 09:06:57.000000 dupla-0.0.2/LICENSE
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       27 2023-06-14 19:05:04.000000 dupla-0.0.2/MANIFEST.in
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3868 2023-07-20 12:16:40.460486 dupla-0.0.2/PKG-INFO
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3314 2023-07-20 11:58:50.000000 dupla-0.0.2/README.md
+drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-07-20 12:16:40.460486 dupla-0.0.2/dupla/
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      197 2023-06-14 19:05:04.000000 dupla-0.0.2/dupla/__init__.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        6 2023-06-14 19:05:04.000000 dupla-0.0.2/dupla/_version.txt
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     6713 2023-07-20 09:06:57.000000 dupla-0.0.2/dupla/base.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3428 2023-07-20 09:06:57.000000 dupla-0.0.2/dupla/dupla.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)    10094 2023-07-20 12:16:00.000000 dupla-0.0.2/dupla/endpoint.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      627 2023-07-20 08:50:15.000000 dupla-0.0.2/dupla/exceptions.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      772 2023-07-20 09:06:57.000000 dupla-0.0.2/dupla/validation.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      275 2023-07-20 09:06:57.000000 dupla-0.0.2/dupla/version.py
+drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-07-20 12:16:40.460486 dupla-0.0.2/dupla.egg-info/
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     3868 2023-07-20 12:16:40.000000 dupla-0.0.2/dupla.egg-info/PKG-INFO
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      403 2023-07-20 12:16:40.000000 dupla-0.0.2/dupla.egg-info/SOURCES.txt
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        1 2023-07-20 12:16:40.000000 dupla-0.0.2/dupla.egg-info/dependency_links.txt
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)      183 2023-07-20 12:16:40.000000 dupla-0.0.2/dupla.egg-info/requires.txt
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)        6 2023-07-20 12:16:40.000000 dupla-0.0.2/dupla.egg-info/top_level.txt
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1253 2023-07-20 12:16:00.000000 dupla-0.0.2/pyproject.toml
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       38 2023-07-20 12:16:40.460486 dupla-0.0.2/setup.cfg
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)       77 2023-07-20 09:06:57.000000 dupla-0.0.2/setup.py
+drwxrwxr-x   0 aletyg    (1000) aletyg    (1000)        0 2023-07-20 12:16:40.460486 dupla-0.0.2/tests/
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     7329 2023-07-20 12:16:00.000000 dupla-0.0.2/tests/test_api.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1598 2023-06-14 19:05:04.000000 dupla-0.0.2/tests/test_dupla.py
+-rw-rw-r--   0 aletyg    (1000) aletyg    (1000)     1093 2023-07-20 09:06:57.000000 dupla-0.0.2/tests/test_verification.py
```

### Comparing `dupla-0.0.1/LICENSE` & `dupla-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `dupla-0.0.1/PKG-INFO` & `dupla-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dupla
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python API for making requests to DUPLA (Dataudvekslingsplatformen)
 Author-email: Valentin Rosenberg Larsen <valentin.rosenberg@gmail.com>, Alexander Tygesen <atygesen@hotmail.com>
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -64,21 +64,20 @@
     pkcs12_password="goodpassword",
     billetautomat_url="https://oces.billetautomat.skat.dk/auth/realms/oces/certificates/cert",
     jwt_token_expiration_overlap=5
 )
 
 # datetime objects are automatically converted
 # into the correct string representation
-kwargs = {
-    DuplaApiKeys.SE=["9876543210"],
+payload = {
+    DuplaApiKeys.SE=["98765432"],
     DuplaApiKeys.UDSTILLING_FRA=date.today() - timedelta(days=365),
     DuplaApiKeys.UDSTILLING_TIL=date.today()
 }
-payload = api.get_payload(**kwargs)
-data = api.get_data(payload)
+data = api.get_data(payload, format_payload=True, validate_payload=True)
 
 print(data)
 ```
 
 The fields which can be provided is given by the `api.FIELDS` dictionary,
 which is a key-value set of the API key as well as whether the key is required
 by the SKAT api. Should a key you wish to provide be missing, a consistency check of
```

### Comparing `dupla-0.0.1/README.md` & `dupla-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,20 @@
     pkcs12_password="goodpassword",
     billetautomat_url="https://oces.billetautomat.skat.dk/auth/realms/oces/certificates/cert",
     jwt_token_expiration_overlap=5
 )
 
 # datetime objects are automatically converted
 # into the correct string representation
-kwargs = {
-    DuplaApiKeys.SE=["9876543210"],
+payload = {
+    DuplaApiKeys.SE=["98765432"],
     DuplaApiKeys.UDSTILLING_FRA=date.today() - timedelta(days=365),
     DuplaApiKeys.UDSTILLING_TIL=date.today()
 }
-payload = api.get_payload(**kwargs)
-data = api.get_data(payload)
+data = api.get_data(payload, format_payload=True, validate_payload=True)
 
 print(data)
 ```
 
 The fields which can be provided is given by the `api.FIELDS` dictionary,
 which is a key-value set of the API key as well as whether the key is required
 by the SKAT api. Should a key you wish to provide be missing, a consistency check of
```

### Comparing `dupla-0.0.1/dupla/base.py` & `dupla-0.0.2/dupla/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import logging
 from datetime import datetime, timedelta
-from uuid import uuid4
 from typing import Any, Dict, Optional
-import logging
+from uuid import uuid4
 
 import requests
 import requests_pkcs12
 
 from .exceptions import DuplaApiAuthenticationException
 
 __all__ = [
```

### Comparing `dupla-0.0.1/dupla/dupla.py` & `dupla-0.0.2/dupla/dupla.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module defines the DUPLA API endpoint objects."""
 from typing import Dict
-from .endpoint import DuplaEndpointApiBase, DuplaApiKeys
+
+from .endpoint import DuplaApiKeys, DuplaEndpointApiBase
 
 __all__ = [
     "DuplaKtrApi",
     "DuplaLigApi",
     "DuplaMomsApi",
     "DuplaKtrObsApi",
     "DuplaLonsumApi",
```

### Comparing `dupla-0.0.1/dupla/endpoint.py` & `dupla-0.0.2/dupla/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
+from dataclasses import dataclass, fields
 from datetime import date, datetime
-from typing import Any, List, Dict
+from typing import Any, Dict, List
 from urllib.parse import urljoin
-from dataclasses import dataclass, fields
 
-import requests
 import backoff
+import requests
 
 from .base import DuplaApiBase
-from .exceptions import InvalidPayloadException, DuplaApiException
+from .exceptions import DuplaApiException, DuplaResponseException, InvalidPayloadException
 from .validation import convert_and_validate_iso_date
 
 logger = logging.getLogger(__file__)
 
 __all__ = ["DuplaEndpointApiBase", "DuplaApiKeys"]
 
+RESPONSE_T = Dict[str, Any]
+
 
 @dataclass
 class DuplaApiKeys:
     """Container for DUPLA API keys."""
 
     CVR: str = "VirksomhedCVRNummer"
     SE: str = "VirksomhedSENummer"
@@ -170,26 +172,46 @@
             return convert_and_validate_iso_date(value)
         if name in [DuplaApiKeys.UDSTILLING_FRA, DuplaApiKeys.UDSTILLING_TIL]:
             if isinstance(value, (date, datetime)):
                 return value.strftime("%Y-%m-%dT%H:%M:%SZ")
         return value
 
     def build_payload(self, **kwargs) -> Dict[str, Any]:
+        """Format the input values of the payload."""
         return {key: self.format_value(key, value) for key, value in kwargs.items()}
 
-    def get_data(self, payload: Dict[str, Any]) -> List[Dict[str, Any]]:
+    def get_data(
+        self,
+        payload: Dict[str, Any],
+        format_payload: bool = True,
+        validate_payload: bool = True,
+    ) -> List[RESPONSE_T]:
         """Request the server for data.
 
         Args:
             payload (dict): Payload, e.g. constructed from the `get_payload` method.
+            format_payload (bool, optional): Whether to call `build_payload` on the provided
+                payload. Otherwise the payload is provided as-is.
+                Defaults to True.
+            validate_payload (bool, optional): Whether to validate the payload.
+                Defaults to True.
 
         Returns:
             List[Dict[str, Any]]: A JSON list representing data as returned by the API.
         """
 
+        if format_payload:
+            payload = self.build_payload(**payload)
+        if validate_payload:
+            self.validate_payload(payload)
+        return self._run_payload(payload)
+
+    def _run_payload(self, payload: Dict[str, Any]) -> List[RESPONSE_T]:
+        """Execute a given payload. No conversion is done on the payload."""
+
         endpoint = self.get_endpoint()
 
         # Construct the getter with a backoff, and a modified number of max tries
         @backoff.on_exception(
             backoff.expo,
             (requests.exceptions.RequestException, DuplaApiException),
             max_tries=self.max_tries,
@@ -204,24 +226,27 @@
                 # Perform simple type check to fail fast if the server has returned
                 # something unknown.
                 data = response_json["data"]
                 if not isinstance(data, list):
                     logger.exception(
                         "Received an invalid response from DUPLA, which was not a list: %s", data
                     )
-                    raise DuplaApiException(
-                        "Invalid response from DUPLA. The data key did not contain a list."
+                    raise DuplaResponseException(
+                        "Invalid response from DUPLA. The data key did not contain a list.",
+                        response=response,
                     )
                 return data
-
+            except DuplaResponseException as e:
+                # Let the inner exception through
+                raise e
             except Exception as e:
-                logger.exception("Error occoured while processing response: %s", response.content)
-                raise DuplaApiException(
-                    "Invalid response from DUPLA. "
-                    "Response does not apply with OpenAPI specification."
+                logger.exception("Error occurred while processing response: %s", response.content)
+                raise DuplaResponseException(
+                    "An error occurred while parsing the DUPLA response.",
+                    response=response,
                 ) from e
 
         return _getter()
 
     @classmethod
     def endpoint_from_base_url(cls, url: str) -> str:
         if not cls.DEFAULT_ENDPOINT:
```

### Comparing `dupla-0.0.1/dupla/validation.py` & `dupla-0.0.2/dupla/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from datetime import date, datetime
 from typing import Union
-from datetime import datetime, date
 
 ISO_FMT = "%Y-%m-%d"  # Date format for fields requiring yyyy-mm-dd
 
 
 def convert_and_validate_iso_date(value: Union[str, date, datetime]) -> str:
     """Convert a date/datetime object to ISO.
     The value is validated to be a valid yyyy-mm-dd date string."""
```

### Comparing `dupla-0.0.1/dupla.egg-info/PKG-INFO` & `dupla-0.0.2/dupla.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dupla
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python API for making requests to DUPLA (Dataudvekslingsplatformen)
 Author-email: Valentin Rosenberg Larsen <valentin.rosenberg@gmail.com>, Alexander Tygesen <atygesen@hotmail.com>
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -64,21 +64,20 @@
     pkcs12_password="goodpassword",
     billetautomat_url="https://oces.billetautomat.skat.dk/auth/realms/oces/certificates/cert",
     jwt_token_expiration_overlap=5
 )
 
 # datetime objects are automatically converted
 # into the correct string representation
-kwargs = {
-    DuplaApiKeys.SE=["9876543210"],
+payload = {
+    DuplaApiKeys.SE=["98765432"],
     DuplaApiKeys.UDSTILLING_FRA=date.today() - timedelta(days=365),
     DuplaApiKeys.UDSTILLING_TIL=date.today()
 }
-payload = api.get_payload(**kwargs)
-data = api.get_data(payload)
+data = api.get_data(payload, format_payload=True, validate_payload=True)
 
 print(data)
 ```
 
 The fields which can be provided is given by the `api.FIELDS` dictionary,
 which is a key-value set of the API key as well as whether the key is required
 by the SKAT api. Should a key you wish to provide be missing, a consistency check of
```

### Comparing `dupla-0.0.1/pyproject.toml` & `dupla-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 test = [
   "pytest",
   "pytest-mock",
 ]
 dev = [
   "pytest",
   "pytest-mock",
-  "black",
-  "ruff",
+  "black==23.7.0",
+  "ruff==0.0.278",
   "pre-commit",
   # For publishing
   "build",
   "twine",
   "pyclean>=2.0.0",
 ]
 
@@ -51,7 +51,10 @@
 line-length = 100
 target-version = ['py38']
 
 [tool.ruff]
 line-length = 100
 exclude = ["__init__.py",
            "scripts"]
+target-version = "py38"
+extend-select = ["I", "RUF"]
+ignore = ["RUF012"]
```

### Comparing `dupla-0.0.1/tests/test_dupla.py` & `dupla-0.0.2/tests/test_dupla.py`

 * *Files identical despite different names*

### Comparing `dupla-0.0.1/tests/test_verification.py` & `dupla-0.0.2/tests/test_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import pytest
 from datetime import date, datetime
+
+import pytest
+
 from dupla import validation
 
 # Constant dates, ensures they do not change during test
 TODAY = date.today()
 TODAY_DT = datetime.now()
```

