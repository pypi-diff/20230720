# Comparing `tmp/french_cities-0.1.0a3.tar.gz` & `tmp/french_cities-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a3.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a4.tar", max compression
```

## Comparing `french_cities-0.1.0a3.tar` & `french_cities-0.1.0a4.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1003 2023-07-20 12:31:33.351032 french_cities-0.1.0a3/french_cities/__init__.py
--rw-r--r--   0        0        0    16645 2023-07-20 11:00:48.287264 french_cities-0.1.0a3/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a3/french_cities/departement_finder.py
--rw-r--r--   0        0        0     8996 2023-07-20 08:57:54.526764 french_cities-0.1.0a3/french_cities/test.xlsx
--rw-r--r--   0        0        0    18534 2023-07-20 12:06:04.703855 french_cities-0.1.0a3/french_cities/test_sample.xlsx
--rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a3/french_cities/utils.py
--rw-r--r--   0        0        0     7719 2023-07-17 15:18:15.371670 french_cities-0.1.0a3/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-20 12:31:36.220513 french_cities-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a3/README.fr.md
--rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a3/README.md
--rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0      520 2023-07-20 15:31:44.641685 french_cities-0.1.0a4/french_cities/__init__.py
+-rw-r--r--   0        0        0    20106 2023-07-20 15:30:53.459607 french_cities-0.1.0a4/french_cities/city_finder.py
+-rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a4/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a4/french_cities/utils.py
+-rw-r--r--   0        0        0     7791 2023-07-20 14:20:02.786838 french_cities-0.1.0a4/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-20 15:31:47.476493 french_cities-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a4/README.fr.md
+-rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a4/README.md
+-rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a4/PKG-INFO
```

### Comparing `french_cities-0.1.0a3/french_cities/city_finder.py` & `french_cities-0.1.0a4/french_cities/city_finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,108 @@
 from requests_cache import CachedSession
 from requests import Session
 from rapidfuzz import fuzz
 from unidecode import unidecode
 from pynsee.geodata import get_geodata
 import geopandas as gpd
 from pyproj import Transformer
-from datetime import date
+from datetime import date, timedelta
 from typing import Union
 import numpy as np
 from pebble import ThreadPool
 from tqdm import tqdm
 
 from french_cities.vintage import set_vintage
 from french_cities.departement_finder import find_departements
 from french_cities.utils import init_pynsee
+from french_cities import LAST_INSEE_HISTO_CITIES
 
 
 logger = logging.getLogger(__name__)
 
 
+def _get_old_cities_names(
+    year: str,
+    look_for: pd.DataFrame,
+    alias: str,
+    session: Session = None,
+    last_insee_histo_cities: str = LAST_INSEE_HISTO_CITIES,
+) -> pd.DataFrame:
+    """
+    Get old city names directly from INSEE's website (hardcoded URL to update
+    annually in french_cities.__init__) and use fuzzy matching inside the same
+    departement to find best candidates.
+
+    Parameters
+    ----------
+    year : str
+        Desired vintage ("last" or castable to int)
+    look_for : pd.DataFrame
+        DataFrame cities (expected columns are "city_cleaned" & "dep") we are
+        trying to find a match to
+    alias : str
+        field to use to store the positive matches' codes into the returned
+        datafram
+    session : Session, optional
+        Requests Session to use for web queries to APIs. Note that pynsee
+        (used under the hood for geolocation recognition) uses it's own
+        session. The default is None (and will use a CachedSession with
+        **NO** expiration retrieving the INSEE's complete file)
+    last_insee_histo_cities : str, optional
+        Path to INSEE's "all cities since 1943" file.
+        Defaults to french_cities.LAST_INSEE_HISTO_CITIES
+        Currently found here:
+            https://www.insee.fr/fr/information/6800675#communes_1943
+
+    Returns
+    -------
+    match : pd.DataFrame
+        DataFrame of positive matches (ie look_for + one mor column under the
+        label `alias`)
+
+    """
+    if not session:
+        session = CachedSession(allowable_methods=("GET", "POST"))
+
+    r = session.get(last_insee_histo_cities)
+    obj = io.BytesIO(r.content)
+    df = pd.read_csv(obj)
+
+    ix = df[df.DATE_FIN.isnull() == False].index
+    df = df.loc[ix, ["NCC", "COM"]].reset_index(drop=True)
+    df = df.drop_duplicates("NCC")
+
+    df = find_departements(df, source="COM", alias="dep", type_code="insee")
+
+    # fuzzy matching df / look_for
+    match = look_for.merge(df, on="dep", how="inner")
+    match["fuzzy_match"] = match[["city_cleaned", "NCC"]].apply(
+        lambda xy: fuzz.token_set_ratio(*xy), axis=1
+    )
+
+    ix = match[match.fuzzy_match > 80].index
+    match = match.loc[ix].drop("fuzzy_match", axis=1)
+
+    # Keep matches only if there is no ambiguity
+    match = match.drop_duplicates("city_cleaned", keep=False)
+
+    try:
+        year = int(year)
+    except ValueError:
+        year = date.today().year
+    match = set_vintage(match, year, "COM")
+    match = look_for.merge(
+        match[["city_cleaned", "dep", "COM"]],
+        on=["city_cleaned", "dep"],
+        how="left",
+    )
+    match = match.rename({"COM": alias}, axis=1)
+    return match
+
+
 def _find_from_geoloc(
     epsg: int,
     df: pd.DataFrame,
     year: str = "last",
     x: str = "x",
     y: str = "y",
     field_output: str = "insee_com",
@@ -223,15 +303,17 @@
             "are necessary"
         )
         raise ValueError(msg)
 
     init_pynsee()
 
     if not session:
-        session = CachedSession(allowable_methods=("GET", "POST"))
+        session = CachedSession(
+            allowable_methods=("GET", "POST"), expire_after=timedelta(days=30)
+        )
 
     if len(necessary3 - columns) == 0 and not epsg:
         logger.warning(
             "x and y columns where found, but a valid EPSG projection was not "
             "set : geolocation will not be performed"
         )
 
@@ -335,16 +417,16 @@
                 .merge(
                     addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
                     on="full",
                 )
             )
 
         else:
-            # revert to multiple queries of BAN
-            # See issue https://github.com/BaseAdresseNationale/adresse.data.gouv.fr/issues/1575
+            # revert to multiple queries of BAN, see issue here:
+            # https://github.com/BaseAdresseNationale/adresse.data.gouv.fr/issues/1575
             logger.info(
                 f"request BAN with individual requests and {components}..."
             )
 
             def get(x):
                 r = session.get(
                     # recherche "en masse" grâce à l'API de la BAN
@@ -452,11 +534,28 @@
 
     df = df.merge(
         addresses.replace("", np.nan), how="left", on=components_kept
     )
     candidats = ["candidat_0", "best"]
     df[field_output] = combine(df, candidats)
     df = df.drop(
-        [x for x in candidats if x in set(df.columns)] + ["city_cleaned"],
+        [x for x in candidats if x in set(df.columns)],
         axis=1,
     )
+
+    # Where still no results, check directly from INSEE's website for obsolete
+    # cities (using dep & city)
+    ix = df[df[field_output].isnull()].index
+    if len(ix) > 0:
+        missing = df.loc[ix, [dep, "city_cleaned"]]
+        missing = _get_old_cities_names(
+            year, missing, "candidat_missing", session
+        )
+        df = df.merge(missing, on=[dep, "city_cleaned"], how="left")
+
+        candidats = [field_output, "candidat_missing"]
+        df[field_output] = combine(df, candidats)
+        df = df.drop("candidat_missing", axis=1)
+
+    df = df.drop("city_cleaned", axis=1)
+
     return df
```

### Comparing `french_cities-0.1.0a3/french_cities/departement_finder.py` & `french_cities-0.1.0a4/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a3/french_cities/vintage.py` & `french_cities-0.1.0a4/french_cities/vintage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Jul  7 09:17:12 2023
 """
 import pandas as pd
 from functools import partial
+from tqdm import tqdm
 
 from french_cities.utils import init_pynsee
 from pynsee.localdata import get_area_list
 from pynsee.localdata import get_ascending_area
 from pynsee.localdata import get_area_projection
 
 
@@ -131,15 +132,15 @@
        3  13204  13055
        4  13205  13055
 
     """
     date = f"{year}-01-01"
     parents = []
     func = partial(get_ascending_area, area=type_, date=date, type="commune")
-    for code in codes:
+    for code in tqdm(codes, desc="get parent from insee", leave=False):
         parents.append(
             {"CODE": code, "PARENT": func(code=code).loc[0, "code"]}
         )
 
     parents = pd.DataFrame(parents)
     return parents
```

### Comparing `french_cities-0.1.0a3/pyproject.toml` & `french_cities-0.1.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.0a3/README.fr.md` & `french_cities-0.1.0a4/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a3/README.md` & `french_cities-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a3/PKG-INFO` & `french_cities-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
```

