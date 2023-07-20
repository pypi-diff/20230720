# Comparing `tmp/french_cities-0.1.0a1.tar.gz` & `tmp/french_cities-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a1.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a2.tar", max compression
```

## Comparing `french_cities-0.1.0a1.tar` & `french_cities-0.1.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      349 2023-07-17 15:20:01.154915 french_cities-0.1.0a1/french_cities/__init__.py
--rw-r--r--   0        0        0    13454 2023-07-17 16:30:05.265571 french_cities-0.1.0a1/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a1/french_cities/departement_finder.py
--rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a1/french_cities/utils.py
--rw-r--r--   0        0        0     7719 2023-07-17 15:18:15.371670 french_cities-0.1.0a1/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-18 13:30:56.742912 french_cities-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     8605 2023-07-18 13:25:53.965112 french_cities-0.1.0a1/README.fr.md
--rw-r--r--   0        0        0     7223 2023-07-18 13:24:45.904682 french_cities-0.1.0a1/README.md
--rw-r--r--   0        0        0    16802 1970-01-01 00:00:00.000000 french_cities-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-07-20 12:05:49.356617 french_cities-0.1.0a2/french_cities/__init__.py
+-rw-r--r--   0        0        0    16645 2023-07-20 11:00:48.287264 french_cities-0.1.0a2/french_cities/city_finder.py
+-rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a2/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a2/french_cities/utils.py
+-rw-r--r--   0        0        0     7719 2023-07-17 15:18:15.371670 french_cities-0.1.0a2/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-20 11:44:07.438358 french_cities-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a2/README.fr.md
+-rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a2/README.md
+-rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a2/PKG-INFO
```

### Comparing `french_cities-0.1.0a1/french_cities/city_finder.py` & `french_cities-0.1.0a2/french_cities/city_finder.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from unidecode import unidecode
 from pynsee.geodata import get_geodata
 import geopandas as gpd
 from pyproj import Transformer
 from datetime import date
 from typing import Union
 import numpy as np
+from pebble import ThreadPool
+from tqdm import tqdm
 
 from french_cities.vintage import set_vintage
 from french_cities.departement_finder import find_departements
 from french_cities.utils import init_pynsee
 
 
 logger = logging.getLogger(__name__)
@@ -247,32 +249,34 @@
             .str.replace(
                 r" \(.*\)$", "", regex=True
             )  # Neuville-Housset (La) -> Neuville-Housset
             .str.upper()
             .apply(unidecode)  # A voir si on conserve
             .str.split(r"\W+")
             .str.join(" ")
+            .str.strip(" ")
+            .str.replace(r" ?CEDEX$", "", regex=True)  # LOOS CEDEX -> LOOS
         )
 
     # Control which configuration can be used
     # Note that the order is relevant here, as this will determine the result's
     # preference
-    to_test_ok = []
-    to_test = [
-        (postcode, "city_cleaned"),
-        (address, postcode, "city_cleaned"),
-        (dep, "city_cleaned"),
-    ]
-    for test_cols in to_test:
+    to_test_ok = {}
+    to_test = {
+        (postcode, "city_cleaned"): "municipality",
+        (address, postcode, "city_cleaned"): None,
+        (dep, "city_cleaned"): "municipality",
+    }
+    for test_cols, type_ban_search in to_test.items():
         try:
             df.loc[:, test_cols]
         except KeyError:
             pass
         else:
-            to_test_ok.append(test_cols)
+            to_test_ok[test_cols] = type_ban_search
 
     components_kept = list(
         {field for test_cols in to_test_ok for field in test_cols}
     )
 
     addresses = df.loc[:, components_kept].drop_duplicates().fillna("")
 
@@ -282,51 +286,124 @@
         addresses = find_departements(
             addresses, postcode, dep, postcode, session
         )
 
     for k, components in enumerate(to_test_ok):
 
         def list_map(df, columns):
+            # contatenation of multiple columns
             "https://stackoverflow.com/questions/39291499#answer-62135779"
             return pd.Series(
                 map(" ".join, df[list(columns)].values.tolist()),
                 index=df.index,
             )
 
         if "full" in set(addresses.columns):
             addresses = addresses.drop("full", axis=1)
         addresses = addresses.join(
             list_map(addresses.copy(), components).to_frame("full")
         )
         addresses = addresses.drop_duplicates(keep="first")
 
-        logger.info(f"request BAN with {components}...")
-        r = session.post(
-            # recherche "en masse" grâce à l'API de la BAN
-            "https://api-adresse.data.gouv.fr/search/csv/",
-            files=[
-                ("data", addresses.to_csv(index=False)),
-                ("result_columns", (None, "full")),
-                ("result_columns", (None, "result_score")),
-                ("result_columns", (None, "result_city")),
-                ("result_columns", (None, "result_citycode")),
-            ],
-        )
+        if to_test_ok[components] is None:
+            # safe to use the CSV geocoder
+            logger.info(f"request BAN with CSV geocoder and {components}...")
+            r = session.post(
+                # recherche "en masse" grâce à l'API de la BAN
+                "https://api-adresse.data.gouv.fr/search/csv/",
+                files=[
+                    ("data", addresses.to_csv(index=False)),
+                    ("type", (None, "municipality")),
+                    ("result_columns", (None, "full")),
+                    ("result_columns", (None, "result_score")),
+                    ("result_columns", (None, "result_city")),
+                    ("result_columns", (None, "result_citycode")),
+                ],
+            )
 
-        logger.info("résultat obtenu")
+            logger.info("résultat obtenu")
 
-        results_api = (
-            pd.read_csv(io.BytesIO(r.content), dtype={"result_citycode": str})
-            .drop_duplicates()
-            .loc[:, ["full", "result_score", "result_city", "result_citycode"]]
-            .merge(
-                addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
-                on="full",
+            results_api = (
+                pd.read_csv(
+                    io.BytesIO(r.content),
+                    dtype={"dep": str, "result_citycode": str},
+                )
+                .drop_duplicates()
+                .loc[
+                    :,
+                    ["full", "result_score", "result_city", "result_citycode"],
+                ]
+                .merge(
+                    addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
+                    on="full",
+                )
+            )
+
+        else:
+            # revert to multiple queries of BAN
+            # See issue https://github.com/BaseAdresseNationale/adresse.data.gouv.fr/issues/1575
+            logger.info(
+                f"request BAN with individual requests and {components}..."
+            )
+
+            def get(x):
+                r = session.get(
+                    # recherche "en masse" grâce à l'API de la BAN
+                    "https://api-adresse.data.gouv.fr/search/",
+                    params={
+                        "q": x,
+                        "type": to_test_ok[components],
+                        "autocomplete": 0,
+                        "limit": 1,
+                    },
+                ).json()
+                features = r["features"]
+                query = r["query"]
+                for dict_ in features:
+                    dict_["properties"].update({"full": query})
+
+                return features
+
+            # Without multithreading:
+            # results_api = gpd.GeoDataFrame.from_features(
+            #     np.array(addresses.full.apply(get).tolist()).flatten()
+            #     )
+
+            args = addresses.full.tolist()
+            results = []
+            with tqdm(
+                total=len(args), desc="Queuing download", leave=False
+            ) as pbar:
+                with ThreadPool(10) as pool:
+                    future = pool.map(get, args)
+                    results_iterator = future.result()
+                    while True:
+                        try:
+                            results.append(next(results_iterator))
+                        except StopIteration:
+                            break
+                        finally:
+                            pbar.update(1)
+
+            results_api = (
+                gpd.GeoDataFrame.from_features(np.array(results).flatten())
+                .loc[:, ["full", "score", "city", "citycode"]]
+                .rename(
+                    {
+                        "score": "result_score",
+                        "city": "result_city",
+                        "citycode": "result_citycode",
+                    },
+                    axis=1,
+                )
+                .merge(
+                    addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
+                    on="full",
+                )
             )
-        )
 
         # Control results : same department
         results_api = find_departements(
             results_api, "result_citycode", "result_dep", "insee", session
         )
         ix = results_api[results_api.dep == results_api.result_dep].index
         results_api = results_api.loc[ix]
@@ -356,14 +433,15 @@
 
         results_api = results_api.loc[ix, ["full", "result_citycode"]].rename(
             {"result_citycode": f"candidat_{k+1}"}, axis=1
         )
         addresses = addresses.merge(results_api, on="full", how="left")
 
     def combine(df: pd.DataFrame, columns: list) -> pd.Series:
+        columns = [x for x in columns if x in set(df.columns)]
         first, *next_ = columns
         s = df[first]
         for field in next_:
             s = s.combine_first(df[field])
         return s
 
     candidats = [f"candidat_{k+1}" for k in range(len(to_test_ok))]
@@ -373,9 +451,12 @@
     addresses = addresses.drop_duplicates()
 
     df = df.merge(
         addresses.replace("", np.nan), how="left", on=components_kept
     )
     candidats = ["candidat_0", "best"]
     df[field_output] = combine(df, candidats)
-    df = df.drop(candidats + ["city_cleaned"], axis=1)
+    df = df.drop(
+        [x for x in candidats if x in set(df.columns)] + ["city_cleaned"],
+        axis=1,
+    )
     return df
```

### Comparing `french_cities-0.1.0a1/french_cities/departement_finder.py` & `french_cities-0.1.0a2/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a1/french_cities/vintage.py` & `french_cities-0.1.0a2/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a1/pyproject.toml` & `french_cities-0.1.0a2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
@@ -20,19 +20,21 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tgrandje/french-cities/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests-cache = "^1.1.0"
 unidecode = "^1.3.6"
-pynsee = { git = "https://github.com/tgrandje/pynsee"}
 python-dotenv = "^1.0.0"
 pandas = "^2.0.3"
 geopandas = "^0.13.2"
 rapidfuzz = "^3.1.1"
+pynsee = "^0.1.4"
+pebble = "^5.0.3"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 spyder = "^5.4.3"
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `french_cities-0.1.0a1/README.fr.md` & `french_cities-0.1.0a2/README.fr.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 
 
 # Installation
 
 `pip install french-cities`
 
 Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
-Dans l'immédiat, vous pouvez installer la branche provisoire à l'aide de la 
-commande suivante :
-`pip install git+https://github.com/tgrandje/pynsee@feat/add_proj_support`
+Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
+désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
+github :
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
 
 # Configuration
 
 ## Ajout des clefs API INSEE
 `french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être 
 fonctionnel. Jusqu'à quatre clefs peuvent être spécifiées à l'aide de variables
 d'environnement :
 * insee_key
 * insee_secret, 
 * http_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 * https_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 
-Merci de se référer à la documentation de `pynsee` pour plus d'information 
-sur les clefs API et la configuration.
+Merci de se référer à [la documentation de `pynsee`](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+pour plus d'information sur les clefs API et la configuration.
 
 ## Gestion des sessions web
 `pynsee` utilise son propre gestionnaire de session web. 
 Ainsi, les objets Session passés en argument à `french-cities` ne seront
 **PAS** partagés avec `pynsee`. Cela explique la possibilité de passer une 
 session en argument alors même que des proxy professionnels peuvent être 
 spécifiés par variables d'environnement (pour `pynsee`).
@@ -42,15 +46,15 @@
 des communes à partir de leurs noms en s'appuyant sur la BAN (Base Adresse 
 Nationale) ou sur le service de géocodage Nominatim.
 
 La différence est que `french-cities` est optimisé pour travailler avec des données
 fournies sous la forme de Series ou DataFrames pandas. Ce package gérera mieux
 de gros volumes de données que ne le feraient des appels multiples à des API.
 
-### Retrieve departements' codes
+### Trouver les départements
 `french-cities` peut retrouver un code département à partir de codes postaux ou 
 de codes communes officiels (COG/INSEE).
 
 Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
 Adresse Nationale) et devrait fournir des résultats corrects.
 
 Travailler à partir de codes communes officiels peut entraîner des résultats
@@ -79,15 +83,15 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `find_departements`, merci 
 d'utiliser la commande suivante :
 `help(find_departements)`.
 
-### Retrieve cities' codes
+### Trouver les codes communes
 `french-cities` peut retrouver le code commune à partir de champs multiples.
 Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
 une certaine limite).
 
 Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
 de priorité) :
 * 'x' et 'y' (dans ce cas, un code EPSG doit être explicitement donné);
@@ -158,15 +162,15 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `find_city`, merci 
 d'utiliser la commande suivante :
 `help(find_city)`.
 
-### Set vintage to cities' codes
+### Projection de codes communes dans un millésime donné
 `french-cities` peut tenter de "projeter" un dataframe dans un millésime donné,
 la date initiale demeurant inconnue (voire inexistante, les cas de fichiers
 "multi-millésimés" étant fréquents dans la vie réelle).
 
 Des erreurs peuvent survenir, notamment pour les communes restaurées (dans la 
 mesure où la date initiale de la donnée est inconnue ou inexistante).
```

### Comparing `french_cities-0.1.0a1/README.md` & `french_cities-0.1.0a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,35 @@
 
 
 # Installation
 
 `pip install french-cities`
 
 Note that at this instant, `pynsee` doesn't support communal projection.
-Please use this command to install the correct branch:
-`pip install git+https://github.com/tgrandje/pynsee@feat/add_proj_support`
+After installing `french-cities` from pypi, please uninstall pynsee and replace
+it with the current master:
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
+
 
 
 # Configuration
 
 ## Setting INSEE's API keys
 `french-cities` uses `pynsee` under the hood. For it to work, you need to set
 the credentials up. You can set up to four environment variables:
 * insee_key
 * insee_secret, 
 * http_proxy (if accessing web behind a corporate proxy)
 * https_proxy (if accessing web behind a corporate proxy)
 
-Please refer to `pynsee`'s documentation to help configure the API's access.
+Please refer to [`pynsee`'s documentation](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+to help configure the API's access.
 
 ## Session management
 Note that `pynsee` uses it's own web session. Every Session object you will pass
 to `french-cities` will **NOT** be shared with `pynsee`. This explains the
 possibility to pass a session as an argument to `french-cities` functions,
 even if you had to configure the corporate proxy through environment variables
 for `pynsee`.
```

### Comparing `french_cities-0.1.0a1/PKG-INFO` & `french_cities-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: geopandas (>=0.13.2,<0.14.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: pynsee @ git+https://github.com/tgrandje/pynsee
+Requires-Dist: pebble (>=5.0.3,<6.0.0)
+Requires-Dist: pynsee (>=0.1.4,<0.2.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/tgrandje/french-cities/issues
 Project-URL: Documentation, https://github.com/tgrandje/french-cities/
 Project-URL: Repository, https://github.com/tgrandje/french-cities/
 Description-Content-Type: text/markdown
 
 # french-cities
@@ -35,29 +37,35 @@
 
 
 # Installation
 
 `pip install french-cities`
 
 Note that at this instant, `pynsee` doesn't support communal projection.
-Please use this command to install the correct branch:
-`pip install git+https://github.com/tgrandje/pynsee@feat/add_proj_support`
+After installing `french-cities` from pypi, please uninstall pynsee and replace
+it with the current master:
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
+
 
 
 # Configuration
 
 ## Setting INSEE's API keys
 `french-cities` uses `pynsee` under the hood. For it to work, you need to set
 the credentials up. You can set up to four environment variables:
 * insee_key
 * insee_secret, 
 * http_proxy (if accessing web behind a corporate proxy)
 * https_proxy (if accessing web behind a corporate proxy)
 
-Please refer to `pynsee`'s documentation to help configure the API's access.
+Please refer to [`pynsee`'s documentation](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+to help configure the API's access.
 
 ## Session management
 Note that `pynsee` uses it's own web session. Every Session object you will pass
 to `french-cities` will **NOT** be shared with `pynsee`. This explains the
 possibility to pass a session as an argument to `french-cities` functions,
 even if you had to configure the corporate proxy through environment variables
 for `pynsee`.
@@ -250,31 +258,35 @@
 
 
 # Installation
 
 `pip install french-cities`
 
 Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
-Dans l'immédiat, vous pouvez installer la branche provisoire à l'aide de la 
-commande suivante :
-`pip install git+https://github.com/tgrandje/pynsee@feat/add_proj_support`
+Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
+désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
+github :
+```
+pip uninstall pynsee
+pip install git+https://github.com/InseeFrLab/pynsee
+```
 
 # Configuration
 
 ## Ajout des clefs API INSEE
 `french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être 
 fonctionnel. Jusqu'à quatre clefs peuvent être spécifiées à l'aide de variables
 d'environnement :
 * insee_key
 * insee_secret, 
 * http_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 * https_proxy (le cas échéant, pour accès web derrière un proxy professionnel)
 
-Merci de se référer à la documentation de `pynsee` pour plus d'information 
-sur les clefs API et la configuration.
+Merci de se référer à [la documentation de `pynsee`](https://pynsee.readthedocs.io/en/latest/api_subscription.html)
+pour plus d'information sur les clefs API et la configuration.
 
 ## Gestion des sessions web
 `pynsee` utilise son propre gestionnaire de session web. 
 Ainsi, les objets Session passés en argument à `french-cities` ne seront
 **PAS** partagés avec `pynsee`. Cela explique la possibilité de passer une 
 session en argument alors même que des proxy professionnels peuvent être 
 spécifiés par variables d'environnement (pour `pynsee`).
@@ -288,15 +300,15 @@
 des communes à partir de leurs noms en s'appuyant sur la BAN (Base Adresse 
 Nationale) ou sur le service de géocodage Nominatim.
 
 La différence est que `french-cities` est optimisé pour travailler avec des données
 fournies sous la forme de Series ou DataFrames pandas. Ce package gérera mieux
 de gros volumes de données que ne le feraient des appels multiples à des API.
 
-### Retrieve departements' codes
+### Trouver les départements
 `french-cities` peut retrouver un code département à partir de codes postaux ou 
 de codes communes officiels (COG/INSEE).
 
 Travailler à partir de codes postaux entraînera l'utilisation de la BAN (Base
 Adresse Nationale) et devrait fournir des résultats corrects.
 
 Travailler à partir de codes communes officiels peut entraîner des résultats
@@ -325,15 +337,15 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `find_departements`, merci 
 d'utiliser la commande suivante :
 `help(find_departements)`.
 
-### Retrieve cities' codes
+### Trouver les codes communes
 `french-cities` peut retrouver le code commune à partir de champs multiples.
 Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
 une certaine limite).
 
 Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
 de priorité) :
 * 'x' et 'y' (dans ce cas, un code EPSG doit être explicitement donné);
@@ -404,15 +416,15 @@
 print(df)
 ```
 
 Pour une documentation complète sur la fonction `find_city`, merci 
 d'utiliser la commande suivante :
 `help(find_city)`.
 
-### Set vintage to cities' codes
+### Projection de codes communes dans un millésime donné
 `french-cities` peut tenter de "projeter" un dataframe dans un millésime donné,
 la date initiale demeurant inconnue (voire inexistante, les cas de fichiers
 "multi-millésimés" étant fréquents dans la vie réelle).
 
 Des erreurs peuvent survenir, notamment pour les communes restaurées (dans la 
 mesure où la date initiale de la donnée est inconnue ou inexistante).
```

