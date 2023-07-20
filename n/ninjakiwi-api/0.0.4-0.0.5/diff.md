# Comparing `tmp/ninjakiwi_api-0.0.4.tar.gz` & `tmp/ninjakiwi_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.4.tar", max compression
+gzip compressed data, was "ninjakiwi_api-0.0.5.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.4.tar` & `ninjakiwi_api-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.4/LICENSE
--rw-r--r--   0        0        0      229 2023-07-20 10:17:22.489408 ninjakiwi_api-0.0.4/README.md
--rw-r--r--   0        0        0       83 2023-07-19 19:59:45.011619 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     2995 2023-07-19 21:02:28.521583 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       84 2023-07-19 20:22:35.650851 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1083 2023-07-19 21:46:09.966399 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      149 2023-07-19 20:22:35.654184 ninjakiwi_api-0.0.4/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      489 2023-07-20 10:45:03.488833 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0      135 2023-07-20 10:45:23.342612 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      223 2023-07-20 10:44:10.497649 ninjakiwi_api-0.0.4/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     2830 2023-07-20 10:44:10.477649 ninjakiwi_api-0.0.4/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2756 2023-07-20 10:59:27.412142 ninjakiwi_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      526 2023-07-19 21:43:29.909004 ninjakiwi_api-0.0.4/tests/test_main.py
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0      276 2023-07-20 11:06:00.144748 ninjakiwi_api-0.0.5/README.md
+-rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.5/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0     1004 2023-07-20 12:10:12.190776 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.5/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     2902 2023-07-20 11:43:09.044143 ninjakiwi_api-0.0.5/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2756 2023-07-20 11:14:22.317483 ninjakiwi_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      666 2023-07-20 11:56:58.995664 ninjakiwi_api-0.0.5/tests/test_main.py
+-rw-r--r--   0        0        0     2431 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.5/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.4/LICENSE` & `ninjakiwi_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTD6/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from enum import Enum
 from typing import Optional
 
 __endpoint__ = "https://data.ninjakiwi.com/"
 __game__ = "btd6"
 
 
-class ChallengeFilter(str, Enum):
+class _ChallengeFilter(str, Enum):
     NEWEST = "newest"
     TRENDING = "trending"
     DAILY = "daily"
 
 
-class BossEvent(str, Enum):
+class _BossEvent(str, Enum):
     STANDARD = "standard"
     ELITE = "elite"
 
 
-class OdysseyDifficulty(str, Enum):
+class _OdysseyDifficulty(str, Enum):
     EASY = "easy"
     MEDIUM = "medium"
     HARD = "hard"
 
 
-async def btd6_url_factory(data: str, **options) -> Optional[str]:
+async def _btd6_url_factory(data: str, **options) -> Optional[str]:
     types = [
         "races",
         "bosses",
         "challenges",
         "ct",
         "odyssey",
     ]
@@ -47,39 +47,39 @@
         if bossID is not None:
             bossID_pattern = re.compile(r"^[A-Za-z0-9_-]+$")
             if not bossID_pattern.match(bossID):
                 return None
 
             type_ = options.get("type")
             teamSize = options.get("teamSize")
-            if type_ not in BossEvent.__members__ or teamSize != "1":
+            if type_ not in _BossEvent.__members__ or teamSize != "1":
                 return None
 
             return f"{base_url}/{bossID}/leaderboard/{type_}/{teamSize}"
         else:
             return base_url
 
     if data == "challenges":
         challengeFilter = options.get("challengeFilter")
-        if challengeFilter not in ChallengeFilter.__members__:
+        if challengeFilter not in _ChallengeFilter.__members__:
             return None
 
         return f"{base_url}/filter/{challengeFilter}"
 
     if data == "ct":
         ctID = options.get("ctID")
         if ctID is not None:
             return f"{base_url}/{ctID}/leaderboard/player"
         else:
             return base_url
 
     if data == "odyssey":
         odysseyID = options.get("odysseyID")
         difficulty = options.get("difficulty")
-        if odysseyID is not None and difficulty in OdysseyDifficulty.__members__:
+        if odysseyID is not None and difficulty in _OdysseyDifficulty.__members__:
             maps = options.get("maps")
             if maps is not None:
                 return f"{base_url}/{odysseyID}/{difficulty}/maps"
             else:
                 return f"{base_url}/{odysseyID}/{difficulty}"
         else:
             return base_url
```

### Comparing `ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-0.0.5/ninjakiwi_api/API/BTDB2/function.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from enum import Enum
 from typing import Optional
 
 __endpoint__ = "https://data.ninjakiwi.com/"
 __game__ = "battles2"
 
 
-class ChallengeFilter(str, Enum):
+class _ChallengeFilter(str, Enum):
     NEWEST = "newest"
     TRENDING = "trending"
     DAILY = "daily"
 
 
-async def btdb2_url_factory(data: str, **options) -> Optional[str]:
+async def _btdb2_url_factory(data: str, **options) -> Optional[str]:
     types = [
         "homs",
         "users",
     ]
 
     if data not in types:
         return None
```

### Comparing `ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-0.0.5/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.4/ninjakiwi_api/main.py` & `ninjakiwi_api-0.0.5/ninjakiwi_api/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Main module."""
 
-from typing import Callable
+from typing import Optional
 
-from .API import btd6_url_factory, btdb2_url_factory
+from ninjakiwi_api.FUNCTIONS.FETCH.model import _model
+
+from .API import _btd6_url_factory, _btdb2_url_factory
 from .FUNCTIONS import _api_fetch, _error_handler
 
 
 async def _game_to_func(game: str, data: str) -> str | None:
     games = {
-        "BTD6": btd6_url_factory,
-        "BTDB2": btdb2_url_factory,
+        "BTD6": _btd6_url_factory,
+        "BTDB2": _btdb2_url_factory,
     }
     try:
         for entry, func in games.items():
             if game == entry:
                 return await func(data)
     except (AttributeError, TypeError):
         await _error_handler(act="str", exception=f"Game {game} not found.")
         return None
 
 
-async def fetch(game: str, data: str) -> dict | None:
+async def fetch(game: str, data: str) -> Optional[_model] | None:
     """
     Asynchronously fetches data from the NinjaKiwi API based on the specified game and data type.
 
     Parameters
     ----------
     game : str
         The game for which data will be fetched. Valid options are "btd6" and "btdb2".
```

### Comparing `ninjakiwi_api-0.0.4/pyproject.toml` & `ninjakiwi_api-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.4"
+version = "0.0.5"
 homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
 description = "NinjaKiwi API (OpenDATA) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
```

### Comparing `ninjakiwi_api-0.0.4/tests/test_main.py` & `ninjakiwi_api-0.0.5/tests/test_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,26 @@
 @pytest.mark.asyncio
 async def test_fetch_btd6():
     """Sample pytest test function."""
     from ninjakiwi_api import fetch
 
     results = await fetch("BTD6", "races")
 
-    assert "success" in results
+    assert results is not None
+
+    data = await results.get_raw_data()
+
+    assert "success" in data
 
 
 @pytest.mark.asyncio
 async def test_fetch_btdb2():
     """Sample pytest test function."""
     from ninjakiwi_api import fetch
 
     results = await fetch("BTDB2", "homs")
 
-    assert "success" in results
+    assert results is not None
+
+    data = await results.get_raw_data()
+
+    assert "success" in data
```

### Comparing `ninjakiwi_api-0.0.4/PKG-INFO` & `ninjakiwi_api-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: NinjaKiwi API (OpenDATA) for Python! (My first library)
 Home-page: https://github.com/GustavoSchip/ninjakiwi_api
 License: MIT
 Keywords: NinjaKiwi,API
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Maintainer: Gustavo Schip
@@ -42,20 +42,25 @@
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tornado (>=6.2,<7.0)
 Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
 Requires-Dist: virtualenv (>=20.13.1,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
-# NinjaKiwi API
+<div align="center">
+  <h1>NinjaKiwi API</h1>
+</div>
 
+---
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/ninjakiwi_api">
     <img src="https://img.shields.io/pypi/v/ninjakiwi-api.svg"
         alt = "Release Status">
 </a>
 </p>
 
+<br>
+
 # Coming soon..
 Stay tuned guys
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.4 Summary: NinjaKiwi API
+Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.5 Summary: NinjaKiwi API
 (OpenDATA) for Python! (My first library) Home-page: https://github.com/
 GustavoSchip/ninjakiwi_api License: MIT Keywords: NinjaKiwi,API Author: Gustavo
 Schip Author-email: gustavoschip@proton.me Maintainer: Gustavo Schip
 Maintainer-email: gustavoschip@proton.me Requires-Python: >=3.11,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
@@ -22,10 +22,13 @@
 Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev" Requires-Dist: pyreadline
 (>=2.1,<3.0) Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test" Requires-
 Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "test" Requires-Dist:
 pytest-cov (>=3.0.0,<4.0.0) ; extra == "test" Requires-Dist: toml
 (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tornado (>=6.2,<7.0)
 Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev" Requires-Dist: twine
 (>=3.8.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv (>=20.13.1,<21.0.0)
-; extra == "dev" Description-Content-Type: text/markdown # NinjaKiwi API
+; extra == "dev" Description-Content-Type: text/markdown
+                          ****** NinjaKiwi API ******
+---
                                [Release_Status]
+
 # Coming soon.. Stay tuned guys
```

