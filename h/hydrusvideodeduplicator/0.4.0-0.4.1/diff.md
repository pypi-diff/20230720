# Comparing `tmp/hydrusvideodeduplicator-0.4.0.tar.gz` & `tmp/hydrusvideodeduplicator-0.4.1.tar.gz`

## Comparing `hydrusvideodeduplicator-0.4.0.tar` & `hydrusvideodeduplicator-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/docker-compose.yml
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/docker-entrypoint.sh
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/LICENSE
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/README.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/docker-compose.yml
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/docker-entrypoint.sh
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/README.md
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.4.1/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.4.0/docker-compose.yml` & `hydrusvideodeduplicator-0.4.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.4.1/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/dedup.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.4.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 import av
 from PIL import Image
 
 from ..pdqhashing.hasher.pdq_hasher import PDQHasher
 from ..pdqhashing.types.hash256 import Hash256
 
 if TYPE_CHECKING:
-    from typing import Annotated
-
-    from fractions import Fraction
     from collections.abc import Iterator
+    from fractions import Fraction
+    from typing import Annotated
 
     from .typing_utils import ValueRange
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.CRITICAL)
 
 
@@ -43,28 +42,31 @@
 
     @staticmethod
     def from_str(serialized: str) -> VpdqFeature:
         """Convert from a string back to the class - the inverse of __str__"""
         parts = serialized.split(",")
         try:
             pdq_hex, qual_str, time_str = parts  # Wrong count = ValueError
-            return VpdqFeature(Hash256.fromHexString(pdq_hex), float(qual_str), int(time_str)).assert_valid()
+            return VpdqFeature(Hash256.fromHexString(pdq_hex), float(qual_str), int(float(time_str))).assert_valid()
         except ValueError:
             raise ValueError(f"invalid {Vpdq.__name__} serialization: {serialized}")
 
     def __str__(self) -> str:
         return f"{self.pdq_hash},{self.quality},{self.frame_number}"
 
 
 class Vpdq:
     # Get the bytes of a video
     @staticmethod
     def get_video_bytes(video_file: Path | str | bytes) -> bytes:
         video = bytes()
         if isinstance(video_file, (Path, str)):
+            if not Path(video_file).is_file():
+                raise ValueError("Failed to get video file bytes. Video does not exist")
+
             try:
                 with open(str(video_file), "rb") as file:
                     video = file.read()
             except OSError as exc:
                 raise ValueError("Failed to get video file bytes. Invalid object type.") from exc
         elif isinstance(video_file, bytes):
             video = video_file
```

### Comparing `hydrusvideodeduplicator-0.4.0/.gitignore` & `hydrusvideodeduplicator-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/LICENSE` & `hydrusvideodeduplicator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/README.md` & `hydrusvideodeduplicator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/pyproject.toml` & `hydrusvideodeduplicator-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.4.0/PKG-INFO` & `hydrusvideodeduplicator-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator
 Author-email: hydrusvideodeduplicator <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

