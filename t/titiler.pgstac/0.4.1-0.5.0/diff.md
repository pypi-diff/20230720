# Comparing `tmp/titiler.pgstac-0.4.1.tar.gz` & `tmp/titiler.pgstac-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-0.4.1.tar", last modified: Wed Jun 21 08:30:16 2023, max compression
+gzip compressed data, was "titiler.pgstac-0.5.0.tar", last modified: Thu Jul 20 10:46:30 2023, max compression
```

## Comparing `titiler.pgstac-0.4.1.tar` & `titiler.pgstac-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1097 2023-06-21 08:29:39.269532 titiler.pgstac-0.4.1/LICENSE
--rw-r--r--   0        0        0     4451 2023-06-21 08:29:39.269532 titiler.pgstac-0.4.1/README.md
--rw-r--r--   0        0        0     2618 2023-06-21 08:29:39.393534 titiler.pgstac-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/__init__.py
--rw-r--r--   0        0        0      874 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/db.py
--rw-r--r--   0        0        0     3936 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/dependencies.py
--rw-r--r--   0        0        0    37672 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/factory.py
--rw-r--r--   0        0        0       91 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/logger.py
--rw-r--r--   0        0        0     3877 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/main.py
--rw-r--r--   0        0        0     6797 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/model.py
--rw-r--r--   0        0        0    12695 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/mosaic.py
--rw-r--r--   0        0        0     2642 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/reader.py
--rw-r--r--   0        0        0     3518 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/settings.py
--rw-r--r--   0        0        0      834 2023-06-21 08:29:39.397534 titiler.pgstac-0.4.1/titiler/pgstac/utils.py
--rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 titiler.pgstac-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-20 10:45:45.444031 titiler.pgstac-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4459 2023-07-20 10:45:45.444031 titiler.pgstac-0.5.0/README.md
+-rw-r--r--   0        0        0     2558 2023-07-20 10:45:45.552033 titiler.pgstac-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/__init__.py
+-rw-r--r--   0        0        0      874 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/db.py
+-rw-r--r--   0        0        0     5129 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/dependencies.py
+-rw-r--r--   0        0        0    37947 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/factory.py
+-rw-r--r--   0        0        0       91 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/logger.py
+-rw-r--r--   0        0        0     7780 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/main.py
+-rw-r--r--   0        0        0     5913 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/model.py
+-rw-r--r--   0        0        0    13737 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/mosaic.py
+-rw-r--r--   0        0        0     3037 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/reader.py
+-rw-r--r--   0        0        0     3542 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/settings.py
+-rw-r--r--   0        0        0    10268 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/templates/index.html
+-rw-r--r--   0        0        0      834 2023-07-20 10:45:45.556033 titiler.pgstac-0.5.0/titiler/pgstac/utils.py
+-rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 titiler.pgstac-0.5.0/PKG-INFO
```

### Comparing `titiler.pgstac-0.4.1/LICENSE` & `titiler.pgstac-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.1/README.md` & `titiler.pgstac-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/10407788/132182694-52cd3d02-5b80-4bb0-9102-b98272fae0f9.png"/>
+  <img width="500" src="https://github.com/stac-utils/titiler-pgstac/assets/10407788/24a64ea9-fede-4ee8-ab8d-625c9e94db44"/>
   <p align="center">Connect PgSTAC and TiTiler.</p>
 </p>
 
 <p align="center">
   <a href="https://github.com/stac-utils/titiler-pgstac/actions?query=workflow%3ACI" target="_blank">
       <img src="https://github.com/developmentseed/titiler/workflows/CI/badge.svg" alt="Test">
   </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
- [https://user-images.githubusercontent.com/10407788/132182694-52cd3d02-5b80-
-                          4bb0-9102-b98272fae0f9.png]
+ [https://github.com/stac-utils/titiler-pgstac/assets/10407788/24a64ea9-fede-
+                            4ee8-ab8d-625c9e94db44]
                           Connect PgSTAC and TiTiler.
                  [Test] [Coverage] [Package_version] [License]
 --- **Documentation**: https://stac-utils.github.io/titiler-pgstac/ **Source
 Code**: https://github.com/stac-utils/titiler-pgstac --- `TiTiler.PgSTAC` is a
 [titiler](https://github.com/developmentseed/titiler) extension which connect
 to [pgstac](https://github.com/stac-utils/pgstac) STAC database in order to
 create dynamic **mosaics** based on [`Search Query`](https://github.com/
```

### Comparing `titiler.pgstac-0.4.1/pyproject.toml` & `titiler.pgstac-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,21 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
-    "titiler.core>=0.11.7,<0.12",
-    "titiler.mosaic>=0.11.7,<0.12",
-    "geojson-pydantic",
-    "stac-pydantic==2.0.*",
-    "fastapi>=0.87,<0.95",
-    "starlette>=0.21.0,<0.25",
+    "titiler.core>=0.12.0,<0.13",
+    "titiler.mosaic>=0.12.0,<0.13",
+    "geojson-pydantic~=0.6",
+    "pydantic~=1.0",
 ]
 dynamic = []
-version = "0.4.1"
+version = "0.5.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 psycopg = [
     "psycopg[pool]",
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/db.py` & `titiler.pgstac-0.5.0/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/factory.py` & `titiler.pgstac-0.5.0/titiler/pgstac/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Custom MosaicTiler Factory for PgSTAC Mosaic Backend."""
 
 import os
 import re
+import sys
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
@@ -20,42 +21,49 @@
 import rasterio
 from cogeo_mosaic.backends import BaseBackend
 from cogeo_mosaic.errors import MosaicNotFoundError
 from fastapi import Body, Depends, HTTPException, Path, Query
 from geojson_pydantic import Feature, FeatureCollection
 from psycopg import sql
 from psycopg.rows import class_row
-from rio_tiler.constants import MAX_THREADS
-from rio_tiler.models import BandStatistics
-from rio_tiler.utils import get_array_statistics
+from pydantic import conint
+from rio_tiler.constants import MAX_THREADS, WGS84_CRS
+from rio_tiler.mosaic.methods.base import MosaicMethodBase
 from starlette.datastructures import QueryParams
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response
 
 from titiler.core.dependencies import (
     AssetsBidxExprParams,
+    CoordCRSParams,
     DefaultDependency,
     HistogramParams,
     StatisticsParams,
 )
 from titiler.core.factory import BaseTilerFactory, img_endpoint_params
 from titiler.core.models.mapbox import TileJSON
 from titiler.core.models.responses import MultiBaseStatisticsGeoJSON
 from titiler.core.resources.enums import ImageType, MediaType, OptionalHeader
 from titiler.core.resources.responses import GeoJSONResponse, XMLResponse
-from titiler.mosaic.resources.enums import PixelSelectionMethod
+from titiler.mosaic.factory import PixelSelectionParams
 from titiler.pgstac import model
 from titiler.pgstac.dependencies import (
     BackendParams,
     PathParams,
     PgSTACParams,
     SearchParams,
+    TileParams,
 )
 from titiler.pgstac.mosaic import PGSTACBackend
 
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import Annotated
+
 
 def _first_value(values: List[Any], default: Any = None):
     """Return the first not None value."""
     return next(filter(lambda x: x is not None, values), default)
 
 
 @dataclass
@@ -71,14 +79,16 @@
     histogram_dependency: Type[DefaultDependency] = HistogramParams
 
     # Search dependency
     search_dependency: Callable[
         ..., Tuple[model.PgSTACSearch, model.Metadata]
     ] = SearchParams
 
+    pixel_selection_dependency: Callable[..., MosaicMethodBase] = PixelSelectionParams
+
     backend_dependency: Type[DefaultDependency] = BackendParams
 
     # Add/Remove some endpoints
     add_statistics: bool = False
 
     add_viewer: bool = False
 
@@ -86,18 +96,20 @@
 
     def register_routes(self) -> None:
         """This Method register routes to the router."""
         self._search_routes()
         if self.add_mosaic_list:
             self._search_list_routes()
 
+        # NOTE: `assets` route HAVE TO be registered before `tiles` routes
+        self._assets_routes()
+
         self._tiles_routes()
         self._tilejson_routes()
         self._wmts_routes()
-        self._assets_routes()
 
         if self.add_statistics:
             self._statistics_routes()
 
         if self.add_viewer:
             self._map_routes()
 
@@ -111,102 +123,104 @@
         @self.router.get(
             "/{searchid}/tiles/{z}/{x}/{y}@{scale}x", **img_endpoint_params
         )
         @self.router.get(
             "/{searchid}/tiles/{z}/{x}/{y}@{scale}x.{format}", **img_endpoint_params
         )
         @self.router.get(
-            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}", **img_endpoint_params
+            "/{searchid}/tiles/{tileMatrixSetId}/{z}/{x}/{y}", **img_endpoint_params
         )
         @self.router.get(
-            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}.{format}",
+            "/{searchid}/tiles/{tileMatrixSetId}/{z}/{x}/{y}.{format}",
             **img_endpoint_params,
         )
         @self.router.get(
-            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}@{scale}x",
+            "/{searchid}/tiles/{tileMatrixSetId}/{z}/{x}/{y}@{scale}x",
             **img_endpoint_params,
         )
         @self.router.get(
-            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}@{scale}x.{format}",
+            "/{searchid}/tiles/{tileMatrixSetId}/{z}/{x}/{y}@{scale}x.{format}",
             **img_endpoint_params,
         )
         def tile(
             searchid=Depends(self.path_dependency),
-            z: int = Path(..., ge=0, le=30, description="Tile's zoom level"),
-            x: int = Path(..., description="Tile's column"),
-            y: int = Path(..., description="Tile's row"),
-            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
-                self.default_tms,
-                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
-            ),
-            scale: int = Query(
-                1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
-            ),
-            format: ImageType = Query(
-                None, description="Output image type. Default is auto."
-            ),
+            tile=Depends(TileParams),
+            tileMatrixSetId: Annotated[  # type: ignore
+                Literal[tuple(self.supported_tms.list())],
+                f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
+            ] = self.default_tms,
+            scale: Annotated[  # type: ignore
+                Optional[conint(gt=0, le=4)],
+                "Tile size scale. 1=256x256, 2=512x512...",
+            ] = None,
+            format: Annotated[
+                ImageType,
+                "Default will be automatically defined if the output image needs a mask (png) or not (jpeg).",
+            ] = None,
             layer_params=Depends(self.layer_dependency),
             dataset_params=Depends(self.dataset_dependency),
-            pixel_selection: PixelSelectionMethod = Query(
-                PixelSelectionMethod.first, description="Pixel selection method."
-            ),
-            buffer: Optional[float] = Query(
-                None,
-                gt=0,
-                alias="buffer",
-                title="Tile buffer.",
-                description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
-            ),
+            pixel_selection=Depends(self.pixel_selection_dependency),
+            buffer: Annotated[
+                Optional[float],
+                Query(
+                    gt=0,
+                    title="Tile buffer.",
+                    description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
+                ),
+            ] = None,
             post_process=Depends(self.process_dependency),
             rescale=Depends(self.rescale_dependency),
-            color_formula: Optional[str] = Query(
-                None,
-                title="Color Formula",
-                description="rio-color formula (info: https://github.com/mapbox/rio-color)",
-            ),
+            color_formula: Annotated[
+                Optional[str],
+                Query(
+                    title="Color Formula",
+                    description="rio-color formula (info: https://github.com/mapbox/rio-color)",
+                ),
+            ] = None,
             colormap=Depends(self.colormap_dependency),
             render_params=Depends(self.render_dependency),
             pgstac_params: PgSTACParams = Depends(),
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
             env=Depends(self.environment_dependency),
         ):
             """Create map tile."""
-            headers: Dict[str, str] = {}
-
-            tms = self.supported_tms.get(TileMatrixSetId)
-
             threads = int(os.getenv("MOSAIC_CONCURRENCY", MAX_THREADS))
 
+            scale = scale or 1
+
             strict_zoom = str(os.getenv("MOSAIC_STRICT_ZOOM", False)).lower() in [
                 "true",
                 "yes",
             ]
 
+            tms = self.supported_tms.get(tileMatrixSetId)
             with rasterio.Env(**env):
                 with self.reader(
                     searchid,
                     tms=tms,
                     reader_options={**reader_params},
                     **backend_params,
                 ) as src_dst:
 
-                    if strict_zoom and (z < src_dst.minzoom or z > src_dst.maxzoom):
+                    if strict_zoom and (
+                        tile.z < src_dst.minzoom or tile.z > src_dst.maxzoom
+                    ):
                         raise HTTPException(
                             400,
-                            f"Invalid ZOOM level {z}. Should be between {src_dst.minzoom} and {src_dst.maxzoom}",
+                            f"Invalid ZOOM level {tile.z}. Should be between {src_dst.minzoom} and {src_dst.maxzoom}",
                         )
 
                     image, assets = src_dst.tile(
-                        x,
-                        y,
-                        z,
+                        tile.x,
+                        tile.y,
+                        tile.z,
                         tilesize=scale * 256,
                         buffer=buffer,
-                        pixel_selection=pixel_selection.method(),
+                        pixel_selection=pixel_selection,
                         threads=threads,
                         **layer_params,
                         **dataset_params,
                         **pgstac_params,
                     )
 
             if post_process:
@@ -226,14 +240,15 @@
 
             content = image.render(
                 img_format=format.driver,
                 **format.profile,
                 **render_params,
             )
 
+            headers: Dict[str, str] = {}
             if OptionalHeader.x_assets in self.optional_headers:
                 ids = [x["id"] for x in assets]
                 headers["X-Assets"] = ",".join(ids)
 
             return Response(content, media_type=format.mediatype, headers=headers)
 
     def _tilejson_routes(self) -> None:
@@ -242,62 +257,71 @@
         @self.router.get(
             "/{searchid}/tilejson.json",
             response_model=TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
         )
         @self.router.get(
-            "/{searchid}/{TileMatrixSetId}/tilejson.json",
+            "/{searchid}/{tileMatrixSetId}/tilejson.json",
             response_model=TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
         )
         def tilejson(
             request: Request,
             searchid=Depends(self.path_dependency),
-            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
-                self.default_tms,
-                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
-            ),
-            tile_format: Optional[ImageType] = Query(
-                None, description="Output image type. Default is auto."
-            ),
-            tile_scale: int = Query(
-                1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
-            ),
-            minzoom: Optional[int] = Query(
-                None, description="Overwrite default minzoom."
-            ),
-            maxzoom: Optional[int] = Query(
-                None, description="Overwrite default maxzoom."
-            ),
-            layer_params=Depends(self.layer_dependency),  # noqa
-            dataset_params=Depends(self.dataset_dependency),  # noqa
-            pixel_selection: PixelSelectionMethod = Query(
-                PixelSelectionMethod.first, description="Pixel selection method."
-            ),  # noqa
-            buffer: Optional[float] = Query(
-                None,
-                gt=0,
-                alias="buffer",
-                title="Tile buffer.",
-                description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
-            ),  # noqa
-            post_process=Depends(self.process_dependency),  # noqa
-            rescale=Depends(self.rescale_dependency),  # noqa
-            color_formula: Optional[str] = Query(
-                None,
-                title="Color Formula",
-                description="rio-color formula (info: https://github.com/mapbox/rio-color)",
-            ),  # noqa
-            colormap=Depends(self.colormap_dependency),  # noqa
-            render_params=Depends(self.render_dependency),  # noqa
-            pgstac_params: PgSTACParams = Depends(),  # noqa
-            backend_params=Depends(self.backend_dependency),  # noqa
-            reader_params=Depends(self.reader_dependency),  # noqa
+            tileMatrixSetId: Annotated[  # type: ignore
+                Literal[tuple(self.supported_tms.list())],
+                f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
+            ] = self.default_tms,
+            tile_format: Annotated[
+                Optional[ImageType],
+                Query(
+                    description="Default will be automatically defined if the output image needs a mask (png) or not (jpeg).",
+                ),
+            ] = None,
+            tile_scale: Annotated[
+                Optional[int],
+                Query(
+                    gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
+                ),
+            ] = None,
+            minzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default minzoom."),
+            ] = None,
+            maxzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default maxzoom."),
+            ] = None,
+            layer_params=Depends(self.layer_dependency),
+            dataset_params=Depends(self.dataset_dependency),
+            pixel_selection=Depends(self.pixel_selection_dependency),
+            buffer: Annotated[
+                Optional[float],
+                Query(
+                    gt=0,
+                    title="Tile buffer.",
+                    description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
+                ),
+            ] = None,
+            post_process=Depends(self.process_dependency),
+            rescale=Depends(self.rescale_dependency),
+            color_formula: Annotated[
+                Optional[str],
+                Query(
+                    title="Color Formula",
+                    description="rio-color formula (info: https://github.com/mapbox/rio-color)",
+                ),
+            ] = None,
+            colormap=Depends(self.colormap_dependency),
+            render_params=Depends(self.render_dependency),
+            pgstac_params: PgSTACParams = Depends(),
+            backend_params=Depends(self.backend_dependency),
+            reader_params=Depends(self.reader_dependency),
         ):
             """Return TileJSON document for a SearchId."""
             with request.app.state.dbpool.connection() as conn:
                 with conn.cursor(row_factory=class_row(model.Search)) as cursor:
                     cursor.execute(
                         "SELECT * FROM searches WHERE hash=%s;",
                         (searchid,),
@@ -307,17 +331,18 @@
                         raise MosaicNotFoundError(f"SearchId `{searchid}` not found")
 
             route_params = {
                 "searchid": search_info.id,
                 "z": "{z}",
                 "x": "{x}",
                 "y": "{y}",
-                "scale": tile_scale,
-                "TileMatrixSetId": TileMatrixSetId,
+                "tileMatrixSetId": tileMatrixSetId,
             }
+            if tile_scale:
+                route_params["scale"] = tile_scale
             if tile_format:
                 route_params["format"] = tile_format.value
 
             tiles_url = self.url_for(request, "tile", **route_params)
 
             qs_key_to_remove = [
                 "tilematrixsetid",
@@ -330,15 +355,15 @@
                 (key, value)
                 for (key, value) in request.query_params._list
                 if key.lower() not in qs_key_to_remove
             ]
             if qs:
                 tiles_url += f"?{urlencode(qs)}"
 
-            tms = self.supported_tms.get(TileMatrixSetId)
+            tms = self.supported_tms.get(tileMatrixSetId)
             minzoom = _first_value([minzoom, search_info.metadata.minzoom], tms.minzoom)
             maxzoom = _first_value([maxzoom, search_info.metadata.maxzoom], tms.maxzoom)
             bounds = _first_value(
                 [search_info.input_search.get("bbox"), search_info.metadata.bounds],
                 tms.bbox,
             )
             return {
@@ -350,69 +375,78 @@
             }
 
     def _map_routes(self):  # noqa: C901
         """Register /map endpoint."""
 
         @self.router.get("/{searchid}/map", response_class=HTMLResponse)
         @self.router.get(
-            "/{searchid}/{TileMatrixSetId}/map", response_class=HTMLResponse
+            "/{searchid}/{tileMatrixSetId}/map", response_class=HTMLResponse
         )
         def map_viewer(
             request: Request,
             searchid=Depends(self.path_dependency),
-            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
-                self.default_tms,
-                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
-            ),
-            tile_format: Optional[ImageType] = Query(
-                None, description="Output image type. Default is auto."
-            ),  # noqa
-            tile_scale: int = Query(
-                1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
-            ),  # noqa
-            minzoom: Optional[int] = Query(
-                None, description="Overwrite default minzoom."
-            ),  # noqa
-            maxzoom: Optional[int] = Query(
-                None, description="Overwrite default maxzoom."
-            ),  # noqa
-            layer_params=Depends(self.layer_dependency),  # noqa
-            dataset_params=Depends(self.dataset_dependency),  # noqa
-            pixel_selection: PixelSelectionMethod = Query(
-                PixelSelectionMethod.first, description="Pixel selection method."
-            ),  # noqa
-            buffer: Optional[float] = Query(
-                None,
-                gt=0,
-                alias="buffer",
-                title="Tile buffer.",
-                description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
-            ),  # noqa
-            post_process=Depends(self.process_dependency),  # noqa
-            rescale=Depends(self.rescale_dependency),  # noqa
-            color_formula: Optional[str] = Query(
-                None,
-                title="Color Formula",
-                description="rio-color formula (info: https://github.com/mapbox/rio-color)",
-            ),  # noqa
-            colormap=Depends(self.colormap_dependency),  # noqa
-            render_params=Depends(self.render_dependency),  # noqa
-            pgstac_params: PgSTACParams = Depends(),  # noqa
-            backend_params=Depends(self.backend_dependency),  # noqa
-            reader_params=Depends(self.reader_dependency),  # noqa
-            env=Depends(self.environment_dependency),  # noqa
+            tileMatrixSetId: Annotated[
+                Literal[tuple(self.supported_tms.list())],
+                f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
+            ] = self.default_tms,
+            tile_format: Annotated[
+                Optional[ImageType],
+                Query(
+                    description="Default will be automatically defined if the output image needs a mask (png) or not (jpeg).",
+                ),
+            ] = None,
+            tile_scale: Annotated[
+                Optional[int],
+                Query(
+                    gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
+                ),
+            ] = None,
+            minzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default minzoom."),
+            ] = None,
+            maxzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default maxzoom."),
+            ] = None,
+            layer_params=Depends(self.layer_dependency),
+            dataset_params=Depends(self.dataset_dependency),
+            pixel_selection=Depends(self.pixel_selection_dependency),
+            buffer: Annotated[
+                Optional[float],
+                Query(
+                    gt=0,
+                    title="Tile buffer.",
+                    description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
+                ),
+            ] = None,
+            post_process=Depends(self.process_dependency),
+            rescale=Depends(self.rescale_dependency),
+            color_formula: Annotated[
+                Optional[str],
+                Query(
+                    title="Color Formula",
+                    description="rio-color formula (info: https://github.com/mapbox/rio-color)",
+                ),
+            ] = None,
+            colormap=Depends(self.colormap_dependency),
+            render_params=Depends(self.render_dependency),
+            pgstac_params: PgSTACParams = Depends(),
+            backend_params=Depends(self.backend_dependency),
+            reader_params=Depends(self.reader_dependency),
+            env=Depends(self.environment_dependency),
         ):
             """Return a simple map viewer."""
             tilejson_url = self.url_for(
-                request, "tilejson", searchid=searchid, TileMatrixSetId=TileMatrixSetId
+                request, "tilejson", searchid=searchid, tileMatrixSetId=tileMatrixSetId
             )
             if request.query_params._list:
                 tilejson_url += f"?{urlencode(request.query_params._list)}"
 
-            tms = self.supported_tms.get(TileMatrixSetId)
+            tms = self.supported_tms.get(tileMatrixSetId)
             return self.templates.TemplateResponse(
                 name="map.html",
                 context={
                     "request": request,
                     "tilejson_endpoint": tilejson_url,
                     "tms": tms,
                     "resolutions": [tms._resolution(matrix) for matrix in tms],
@@ -421,62 +455,69 @@
             )
 
     def _wmts_routes(self):  # noqa: C901
         """Add wmts endpoint."""
 
         @self.router.get("/{searchid}/WMTSCapabilities.xml", response_class=XMLResponse)
         @self.router.get(
-            "/{searchid}/{TileMatrixSetId}/WMTSCapabilities.xml",
+            "/{searchid}/{tileMatrixSetId}/WMTSCapabilities.xml",
             response_class=XMLResponse,
         )
         def wmts(
             request: Request,
             searchid=Depends(self.path_dependency),
-            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(
-                self.default_tms,
-                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
-            ),  # noqa
+            tileMatrixSetId: Annotated[
+                Literal[tuple(self.supported_tms.list())],
+                f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
+            ] = self.default_tms,
             src_path=Depends(self.path_dependency),
-            tile_format: ImageType = Query(
-                ImageType.png, description="Output image type. Default is png."
-            ),
-            tile_scale: int = Query(
-                1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
-            ),
-            minzoom: Optional[int] = Query(
-                None, description="Overwrite default minzoom."
-            ),
-            maxzoom: Optional[int] = Query(
-                None, description="Overwrite default maxzoom."
-            ),
-            layer_params=Depends(self.layer_dependency),  # noqa
-            dataset_params=Depends(self.dataset_dependency),  # noqa
-            pixel_selection: PixelSelectionMethod = Query(
-                PixelSelectionMethod.first, description="Pixel selection method."
-            ),  # noqa
-            buffer: Optional[float] = Query(
-                None,
-                gt=0,
-                alias="buffer",
-                title="Tile buffer.",
-                description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
-            ),  # noqa
-            post_process=Depends(self.process_dependency),  # noqa
-            rescale=Depends(self.rescale_dependency),  # noqa
-            color_formula: Optional[str] = Query(
-                None,
-                title="Color Formula",
-                description="rio-color formula (info: https://github.com/mapbox/rio-color)",
-            ),  # noqa
-            colormap=Depends(self.colormap_dependency),  # noqa
-            render_params=Depends(self.render_dependency),  # noqa
-            pgstac_params: PgSTACParams = Depends(),  # noqa
-            backend_params=Depends(self.backend_dependency),  # noqa
-            reader_params=Depends(self.reader_dependency),  # noqa
-            env=Depends(self.environment_dependency),  # noqa
+            tile_format: Annotated[
+                ImageType,
+                Query(description="Output image type. Default is png."),
+            ] = ImageType.png,
+            tile_scale: Annotated[
+                int,
+                Query(
+                    gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
+                ),
+            ] = 1,
+            minzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default minzoom."),
+            ] = None,
+            maxzoom: Annotated[
+                Optional[int],
+                Query(description="Overwrite default maxzoom."),
+            ] = None,
+            layer_params=Depends(self.layer_dependency),
+            dataset_params=Depends(self.dataset_dependency),
+            pixel_selection=Depends(self.pixel_selection_dependency),
+            buffer: Annotated[
+                Optional[float],
+                Query(
+                    gt=0,
+                    title="Tile buffer.",
+                    description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
+                ),
+            ] = None,
+            post_process=Depends(self.process_dependency),
+            rescale=Depends(self.rescale_dependency),
+            color_formula: Annotated[
+                Optional[str],
+                Query(
+                    title="Color Formula",
+                    description="rio-color formula (info: https://github.com/mapbox/rio-color)",
+                ),
+            ] = None,
+            colormap=Depends(self.colormap_dependency),
+            render_params=Depends(self.render_dependency),
+            pgstac_params: PgSTACParams = Depends(),
+            backend_params=Depends(self.backend_dependency),
+            reader_params=Depends(self.reader_dependency),
+            env=Depends(self.environment_dependency),
         ):
             """OGC WMTS endpoint."""
             with request.app.state.dbpool.connection() as conn:
                 with conn.cursor(row_factory=class_row(model.Search)) as cursor:
                     cursor.execute(
                         "SELECT * FROM searches WHERE hash=%s;",
                         (searchid,),
@@ -488,15 +529,15 @@
             route_params = {
                 "searchid": searchid,
                 "z": "{TileMatrix}",
                 "x": "{TileCol}",
                 "y": "{TileRow}",
                 "scale": tile_scale,
                 "format": tile_format.value,
-                "TileMatrixSetId": TileMatrixSetId,
+                "tileMatrixSetId": tileMatrixSetId,
             }
             tiles_url = self.url_for(request, "tile", **route_params)
 
             qs_key_to_remove = [
                 "tilematrixsetid",
                 "tile_format",
                 "tile_scale",
@@ -509,30 +550,30 @@
                 (key, value)
                 for (key, value) in request.query_params._list
                 if key.lower() not in qs_key_to_remove
             ]
             if qs:
                 tiles_url += f"?{urlencode(qs)}"
 
-            tms = self.supported_tms.get(TileMatrixSetId)
+            tms = self.supported_tms.get(tileMatrixSetId)
             minzoom = _first_value([minzoom, search_info.metadata.minzoom], tms.minzoom)
             maxzoom = _first_value([maxzoom, search_info.metadata.maxzoom], tms.maxzoom)
             bounds = _first_value(
                 [search_info.input_search.get("bbox"), search_info.metadata.bounds],
                 tms.bbox,
             )
 
             tileMatrix = []
             for zoom in range(minzoom, maxzoom + 1):  # type: ignore
                 matrix = tms.matrix(zoom)
                 tm = f"""
                         <TileMatrix>
-                            <ows:Identifier>{matrix.identifier}</ows:Identifier>
+                            <ows:Identifier>{matrix.id}</ows:Identifier>
                             <ScaleDenominator>{matrix.scaleDenominator}</ScaleDenominator>
-                            <TopLeftCorner>{matrix.topLeftCorner[0]} {matrix.topLeftCorner[1]}</TopLeftCorner>
+                            <TopLeftCorner>{matrix.pointOfOrigin[0]} {matrix.pointOfOrigin[1]}</TopLeftCorner>
                             <TileWidth>{matrix.tileWidth}</TileWidth>
                             <TileHeight>{matrix.tileHeight}</TileHeight>
                             <MatrixWidth>{matrix.matrixWidth}</MatrixWidth>
                             <MatrixHeight>{matrix.matrixHeight}</MatrixHeight>
                         </TileMatrix>"""
                 tileMatrix.append(tm)
 
@@ -551,77 +592,69 @@
                 media_type=MediaType.xml.value,
             )
 
     def _assets_routes(self):
         """Register assets routes."""
 
         @self.router.get(
-            "/{searchid}/{z}/{x}/{y}/assets",
-            responses={200: {"description": "Return list of assets"}},
-            deprecated=True,
-        )
-        @self.router.get(
-            "/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}/assets",
-            responses={200: {"description": "Return list of assets"}},
-            response_model=List[Dict],
-            deprecated=True,
-        )
-        @self.router.get(
             "/{searchid}/tiles/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
         )
         @self.router.get(
-            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}/assets",
+            "/{searchid}/tiles/{tileMatrixSetId}/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
             response_model=List[Dict],
         )
         def assets_for_tile(
             searchid=Depends(self.path_dependency),
-            z: int = Path(..., ge=0, le=30, description="Tiles's zoom level"),
-            x: int = Path(..., description="Tiles's column"),
-            y: int = Path(..., description="Tiles's row"),
-            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
-                self.default_tms,
-                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
-            ),
+            tile=Depends(TileParams),
+            tileMatrixSetId: Annotated[
+                Literal[tuple(self.supported_tms.list())],
+                f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
+            ] = self.default_tms,
             pgstac_params: PgSTACParams = Depends(),
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
         ):
             """Return a list of assets which overlap a given tile"""
-            tms = self.supported_tms.get(TileMatrixSetId)
-
+            tms = self.supported_tms.get(tileMatrixSetId)
             with self.reader(
                 searchid,
                 tms=tms,
                 reader_options={**reader_params},
                 **backend_params,
             ) as src_dst:
-                return src_dst.assets_for_tile(x, y, z, **pgstac_params)
+                return src_dst.assets_for_tile(tile.x, tile.y, tile.z, **pgstac_params)
 
         @self.router.get(
             "/{searchid}/{lon},{lat}/assets",
             responses={200: {"description": "Return list of assets"}},
             response_model=List[Dict],
         )
         def assets_for_point(
+            lon: Annotated[float, Path(description="Longitude")],
+            lat: Annotated[float, Path(description="Latitude")],
             searchid=Depends(self.path_dependency),
-            lon: float = Path(..., description="Longitude"),
-            lat: float = Path(..., description="Latitude"),
+            coord_crs=Depends(CoordCRSParams),
             pgstac_params: PgSTACParams = Depends(),
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
         ):
             """Return a list of assets for a given point."""
             with self.reader(
                 searchid,
                 reader_options={**reader_params},
                 **backend_params,
             ) as src_dst:
-                return src_dst.assets_for_point(lon, lat, **pgstac_params)
+                return src_dst.assets_for_point(
+                    lon,
+                    lat,
+                    coord_crs=coord_crs or WGS84_CRS,
+                    **pgstac_params,
+                )
 
     def _search_routes(self) -> None:
         """register search routes."""
 
         @self.router.post(
             "/register",
             responses={200: {"description": "Register a Search."}},
@@ -703,29 +736,35 @@
             "/list",
             responses={200: {"description": "List Mosaics in PgSTAC."}},
             response_model=model.Infos,
             response_model_exclude_none=True,
         )
         def list_mosaic(
             request: Request,
-            limit: int = Query(
-                10,
-                ge=1,
-                le=1000,
-                description="Page size limit",
-            ),
-            offset: int = Query(
-                0,
-                ge=0,
-                description="Page offset",
-            ),
-            sortby: Optional[str] = Query(
-                None,
-                description="Sort the response items by a property (ascending (default) or descending).",
-            ),
+            limit: Annotated[
+                int,
+                Query(
+                    ge=1,
+                    le=1000,
+                    description="Page size limit",
+                ),
+            ] = 10,
+            offset: Annotated[
+                int,
+                Query(
+                    ge=0,
+                    description="Page offset",
+                ),
+            ] = 0,
+            sortby: Annotated[
+                Optional[str],
+                Query(
+                    description="Sort the response items by a property (ascending (default) or descending).",
+                ),
+            ] = None,
         ):
             """List a Search query."""
             # Default filter to only return `metadata->type == 'mosaic'`
             mosaic_filter = sql.SQL("metadata->>'type' = 'mosaic'")
 
             # additional metadata property filter passed in query-parameters
             # <propname>=val - filter for a metadata property. Multiple property filters are ANDed together.
@@ -868,24 +907,26 @@
                 200: {
                     "content": {"application/json": {}},
                     "description": "Return statistics for geojson features.",
                 }
             },
         )
         def geojson_statistics(
-            geojson: Union[FeatureCollection, Feature] = Body(
-                ..., description="GeoJSON Feature or FeatureCollection."
-            ),
+            geojson: Annotated[
+                Union[FeatureCollection, Feature],
+                Body(description="GeoJSON Feature or FeatureCollection."),
+            ],
             searchid=Depends(self.path_dependency),
+            coord_crs=Depends(CoordCRSParams),
             layer_params=Depends(self.layer_dependency),
             dataset_params=Depends(self.dataset_dependency),
-            pixel_selection: PixelSelectionMethod = Query(
-                PixelSelectionMethod.first, description="Pixel selection method."
-            ),
-            max_size: int = Query(1024, description="Maximum image size to read onto."),
+            pixel_selection=Depends(self.pixel_selection_dependency),
+            max_size: Annotated[
+                int, Query(description="Maximum image size to read onto.")
+            ] = 1024,
             stats_params=Depends(self.stats_dependency),
             histogram_params=Depends(self.histogram_dependency),
             pgstac_params: PgSTACParams = Depends(),
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
             env=Depends(self.environment_dependency),
         ):
@@ -901,34 +942,24 @@
                     searchid,
                     reader_options={**reader_params},
                     **backend_params,
                 ) as src_dst:
                     for feature in fc:
                         data, _ = src_dst.feature(
                             feature.dict(exclude_none=True),
-                            pixel_selection=pixel_selection.method(),
+                            shape_crs=coord_crs or WGS84_CRS,
+                            pixel_selection=pixel_selection,
                             threads=threads,
                             max_size=max_size,
                             **layer_params,
                             **dataset_params,
                             **pgstac_params,
                         )
 
-                        stats = get_array_statistics(
-                            data.as_masked(),
-                            **stats_params,
-                            **histogram_params,
+                        stats = data.statistics(
+                            **stats_params, hist_options={**histogram_params}
                         )
 
                         feature.properties = feature.properties or {}
-                        feature.properties.update(
-                            {
-                                "statistics": {
-                                    f"{data.band_names[ix]}": BandStatistics(
-                                        **stats[ix]
-                                    )
-                                    for ix in range(len(stats))
-                                }
-                            }
-                        )
+                        feature.properties.update({"statistics": stats})
 
             return fc.features[0] if isinstance(geojson, Feature) else fc
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/model.py` & `titiler.pgstac-0.5.0/titiler/pgstac/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,36 @@
 """
 Titiler.pgstac models.
 
 Note: This is mostly a copy of https://github.com/stac-utils/stac-fastapi/blob/master/stac_fastapi/pgstac/stac_fastapi/pgstac/types/search.py
 """
 
-import operator
 from datetime import datetime
-from enum import Enum, auto
-from types import DynamicClassAttribute
-from typing import Any, Callable, Dict, List, Optional, Union
-
-from geojson_pydantic.geometries import (
-    LineString,
-    MultiLineString,
-    MultiPoint,
-    MultiPolygon,
-    Point,
-    Polygon,
-)
+from typing import Any, Dict, List, Literal, Optional
+
+from geojson_pydantic.geometries import Geometry
+from geojson_pydantic.types import BBox
 from pydantic import BaseModel, Field, root_validator, validator
-from stac_pydantic.shared import BBox
-from stac_pydantic.utils import AutoValueEnum
 
 from titiler.core.resources.enums import MediaType
 
+# ref: https://github.com/stac-api-extensions/query
+# TODO: add "startsWith", "endsWith", "contains", "in"
+Operator = Literal["eq", "neq", "lt", "lte", "gt", "gte"]
 
-class FilterLang(str, Enum):
-    """filter language.
-
-    ref: https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#get-query-parameters-and-post-json-fields
-    """
-
-    cql_json = "cql-json"
-    cql_text = "cql-text"
-    cql2_json = "cql2-json"
-
-
-class Operator(str, AutoValueEnum):
-    """Defines the set of operators supported by the API."""
-
-    eq = auto()
-    ne = auto()
-    lt = auto()
-    lte = auto()
-    gt = auto()
-    gte = auto()
-    # TODO: These are defined in the spec but aren't currently implemented by the api
-    # startsWith = auto()
-    # endsWith = auto()
-    # contains = auto()
-    # in = auto()
-
-    @DynamicClassAttribute
-    def operator(self) -> Callable[[Any, Any], bool]:
-        """Return python operator."""
-        return getattr(operator, self._value_)
+# ref: https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#get-query-parameters-and-post-json-fields
+FilterLang = Literal["cql-json", "cql-text", "cql2-json"]
 
-
-class SearchType(str, Enum):
-    """Search type."""
-
-    mosaic = "mosaic"
-    search = "search"
+SearchType = Literal["mosaic", "search"]
 
 
 class Metadata(BaseModel):
     """Metadata Model."""
 
-    type: SearchType = SearchType.mosaic
+    type: SearchType = "mosaic"
 
     # WGS84 bounds
     bounds: Optional[BBox]
 
     # Min/Max zoom for WebMercatorQuad TMS
     minzoom: Optional[int]
     maxzoom: Optional[int]
@@ -96,32 +55,29 @@
     #     }
     # }
     defaults: Optional[Dict[str, Any]]
 
     class Config:
         """Config for model."""
 
-        use_enum_values = True
         extra = "allow"
 
 
 class PgSTACSearch(BaseModel):
     """Search Query model.
 
     Notes/Diff with standard model:
         - 'fields' is not in the Model because it's defined at the tiler level
         - we don't set limit
     """
 
     collections: Optional[List[str]] = None
     ids: Optional[List[str]] = None
     bbox: Optional[BBox]
-    intersects: Optional[
-        Union[Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon]
-    ]
+    intersects: Optional[Geometry]
     query: Optional[Dict[str, Dict[Operator, Any]]]
     filter: Optional[Dict]
     datetime: Optional[str] = None
     sortby: Any
     filter_lang: Optional[FilterLang] = Field(None, alias="filter-lang")
 
     class Config:
@@ -198,15 +154,15 @@
     usecount: int
     metadata: Metadata
 
     @validator("metadata", pre=True)
     def validate_metadata(cls, v):
         """Set SearchType.search when not present in metadata."""
         if "type" not in v:
-            v["type"] = SearchType.search.name
+            v["type"] = "search"
 
         return v
 
 
 class Link(BaseModel):
     """Link model.
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/mosaic.py` & `titiler.pgstac-0.5.0/titiler/pgstac/mosaic.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cogeo_mosaic.mosaic import MosaicJSON
 from geojson_pydantic import Point, Polygon
 from geojson_pydantic.geometries import Geometry, parse_geometry_obj
 from morecantile import TileMatrixSet
 from psycopg import errors as pgErrors
 from psycopg_pool import ConnectionPool
 from rasterio.crs import CRS
-from rasterio.warp import transform_geom
+from rasterio.warp import transform, transform_bounds, transform_geom
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidAssetName, PointOutsideBounds
 from rio_tiler.io import Reader
 from rio_tiler.io.base import BaseReader, MultiBaseReader
 from rio_tiler.models import ImageData
 from rio_tiler.mosaic import mosaic_reader
 from rio_tiler.tasks import multi_values
@@ -83,23 +83,35 @@
             asset (str): STAC asset name.
 
         Returns:
             str: STAC asset href.
 
         """
         if asset not in self.assets:
-            raise InvalidAssetName(f"{asset} is not valid")
+            raise InvalidAssetName(
+                f"{asset} is not valid. Should be one of {self.assets}"
+            )
 
-        info = AssetInfo(url=self.input["assets"][asset]["href"])
-        if "file:header_size" in self.input["assets"][asset]:
-            info["env"] = {
-                "GDAL_INGESTED_BYTES_AT_OPEN": self.input["assets"][asset][
-                    "file:header_size"
-                ]
-            }
+        asset_info = self.input["assets"][asset]
+        info = AssetInfo(
+            url=asset_info["href"],
+            env={},
+        )
+
+        if header_size := asset_info.get("file:header_size"):
+            info["env"]["GDAL_INGESTED_BYTES_AT_OPEN"] = header_size
+
+        if bands := asset_info.get("raster:bands"):
+            stats = [
+                (b["statistics"]["minimum"], b["statistics"]["maximum"])
+                for b in bands
+                if {"minimum", "maximum"}.issubset(b.get("statistics", {}))
+            ]
+            if len(stats) == len(bands):
+                info["dataset_statistics"] = stats
 
         return info
 
 
 @attr.s
 class PGSTACBackend(BaseBackend):
     """PgSTAC Mosaic Backend."""
@@ -115,32 +127,32 @@
     minzoom: int = attr.ib()
     maxzoom: int = attr.ib()
 
     # Use Custom STAC reader (outside init)
     reader: Type[CustomSTACReader] = attr.ib(init=False, default=CustomSTACReader)
     reader_options: Dict = attr.ib(factory=dict)
 
-    geographic_crs: CRS = attr.ib(default=WGS84_CRS)
-
     # default values for bounds
     bounds: BBox = attr.ib(default=(-180, -90, 180, 90))
+
     crs: CRS = attr.ib(default=WGS84_CRS)
+    geographic_crs: CRS = attr.ib(default=WGS84_CRS)
 
     # The reader is read-only (outside init)
     mosaic_def: MosaicJSON = attr.ib(init=False)
 
     _backend_name = "PgSTAC"
 
     def __attrs_post_init__(self) -> None:
         """Post Init."""
         # Construct a FAKE mosaicJSON
         # mosaic_def has to be defined.
         # we set `tiles` to an empty list.
         self.mosaic_def = MosaicJSON(
-            mosaicjson="0.0.2",
+            mosaicjson="0.0.3",
             name=self.input,
             bounds=self.bounds,
             minzoom=self.minzoom,
             maxzoom=self.maxzoom,
             tiles=[],
         )
 
@@ -165,32 +177,54 @@
         pass
 
     def assets_for_tile(self, x: int, y: int, z: int, **kwargs: Any) -> List[Dict]:
         """Retrieve assets for tile."""
         bbox = self.tms.bounds(morecantile.Tile(x, y, z))
         return self.get_assets(Polygon.from_bounds(*bbox), **kwargs)
 
-    def assets_for_point(self, lng: float, lat: float, **kwargs: Any) -> List[Dict]:
+    def assets_for_point(
+        self,
+        lng: float,
+        lat: float,
+        coord_crs: CRS = WGS84_CRS,
+        **kwargs: Any,
+    ) -> List[Dict]:
         """Retrieve assets for point."""
         # Point search is currently broken within PgSTAC
         # in order to return the correct result we need to make sure exitwhenfull and skipcovered options
         # are set to `False`
         # ref: https://github.com/stac-utils/pgstac/pull/52
         kwargs.update(**{"exitwhenfull": False, "skipcovered": False})
+
+        if coord_crs != WGS84_CRS:
+            xs, ys = transform(coord_crs, WGS84_CRS, [lng], [lat])
+            lng, lat = xs[0], ys[0]
+
         return self.get_assets(Point(type="Point", coordinates=(lng, lat)), **kwargs)
 
     def assets_for_bbox(
         self,
         xmin: float,
         ymin: float,
         xmax: float,
         ymax: float,
+        coord_crs: CRS = WGS84_CRS,
         **kwargs: Any,
     ) -> List[Dict]:
         """Retrieve assets for bbox."""
+        if coord_crs != WGS84_CRS:
+            xmin, ymin, xmax, ymax = transform_bounds(
+                coord_crs,
+                WGS84_CRS,
+                xmin,
+                ymin,
+                xmax,
+                ymax,
+            )
+
         return self.get_assets(Polygon.from_bounds(xmin, ymin, xmax, ymax), **kwargs)
 
     @cached(  # type: ignore
         TTLCache(maxsize=cache_config.maxsize, ttl=cache_config.ttl),
         key=lambda self, geom, **kwargs: hashkey(self.input, str(geom), **kwargs),
     )
     @retry(
@@ -296,26 +330,28 @@
 
         return mosaic_reader(mosaic_assets, _reader, tile_x, tile_y, tile_z, **kwargs)
 
     def point(
         self,
         lon: float,
         lat: float,
+        coord_crs: CRS = WGS84_CRS,
         reverse: bool = False,
         scan_limit: Optional[int] = None,
         items_limit: Optional[int] = None,
         time_limit: Optional[int] = None,
         exitwhenfull: Optional[bool] = None,
         skipcovered: Optional[bool] = None,
         **kwargs: Any,
     ) -> List:
         """Get Point value from multiple observation."""
         mosaic_assets = self.assets_for_point(
             lon,
             lat,
+            coord_crs=coord_crs,
             scan_limit=scan_limit,
             items_limit=items_limit,
             time_limit=time_limit,
             exitwhenfull=exitwhenfull,
             skipcovered=skipcovered,
         )
         if not mosaic_assets:
@@ -324,18 +360,19 @@
         if reverse:
             mosaic_assets = list(reversed(mosaic_assets))
 
         def _reader(
             item: Dict[str, Any],
             lon: float,
             lat: float,
+            coord_crs=coord_crs,
             **kwargs: Any,
         ) -> Dict:
             with self.reader(item, **self.reader_options) as src_dst:
-                return src_dst.point(lon, lat, **kwargs)
+                return src_dst.point(lon, lat, coord_crs=coord_crs, **kwargs)
 
         if "allowed_exceptions" not in kwargs:
             kwargs.update({"allowed_exceptions": (PointOutsideBounds,)})
 
         return list(multi_values(mosaic_assets, _reader, lon, lat, **kwargs).items())
 
     def feature(
@@ -352,15 +389,15 @@
         skipcovered: Optional[bool] = None,
         **kwargs: Any,
     ) -> Tuple[ImageData, List[str]]:
         """Create an Image from multiple items for a GeoJSON feature."""
         if "geometry" in shape:
             shape = shape["geometry"]
 
-        # PgSTAC except geometry in WGS84
+        # PgSTAC needs geometry in WGS84
         shape_wgs84 = shape
         if shape_crs != WGS84_CRS:
             shape_wgs84 = transform_geom(shape_crs, WGS84_CRS, shape)
 
         mosaic_assets = self.get_assets(
             parse_geometry_obj(shape_wgs84),
             scan_limit=scan_limit,
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/reader.py` & `titiler.pgstac-0.5.0/titiler/pgstac/reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,27 +63,35 @@
         return self.tms.minzoom
 
     @maxzoom.default
     def _maxzoom(self):
         return self.tms.maxzoom
 
     def _get_asset_info(self, asset: str) -> AssetInfo:
-        """Validate asset names and return asset's url.
-
-        Args:
-            asset (str): STAC asset name.
-
-        Returns:
-            str: STAC asset href.
-
-        """
+        """Validate asset names and return asset's info."""
         if asset not in self.assets:
-            raise InvalidAssetName(f"{asset} is not valid")
+            raise InvalidAssetName(
+                f"{asset} is not valid. Should be one of {self.assets}"
+            )
 
         asset_info = self.input.assets[asset]
-        info = AssetInfo(url=asset_info.get_absolute_href())
+        extras = asset_info.extra_fields
+
+        info = AssetInfo(
+            url=asset_info.get_absolute_href(),
+            metadata=extras,
+        )
 
         if "file:header_size" in asset_info.extra_fields:
             h = asset_info.extra_fields["file:header_size"]
             info["env"] = {"GDAL_INGESTED_BYTES_AT_OPEN": h}
 
+        if bands := extras.get("raster:bands"):
+            stats = [
+                (b["statistics"]["minimum"], b["statistics"]["maximum"])
+                for b in bands
+                if {"minimum", "maximum"}.issubset(b.get("statistics", {}))
+            ]
+            if len(stats) == len(bands):
+                info["dataset_statistics"] = stats
+
         return info
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/settings.py` & `titiler.pgstac-0.5.0/titiler/pgstac/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class ApiSettings(BaseSettings):
     """API settings"""
 
     name: str = "titiler-pgstac"
     cors_origins: str = "*"
     cachecontrol: str = "public, max-age=3600"
+    root_path: str = ""
     debug: bool = False
 
     @validator("cors_origins")
     def parse_cors_origin(cls, v):
         """Parse CORS origins."""
         return [origin.strip() for origin in v.split(",")]
```

### Comparing `titiler.pgstac-0.4.1/titiler/pgstac/utils.py` & `titiler.pgstac-0.5.0/titiler/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.4.1/PKG-INFO` & `titiler.pgstac-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.4.1
+Version: 0.5.0
 Summary: Connect PgSTAC and TiTiler.
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,pgSTAC
 Author-email: Vincent Sarago <vincent@developmentseed.com>,David Bitner <david@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Project-URL: Documentation, https://stac-utils.github.io/titiler-pgstac/
 Project-URL: Homepage, https://stac-utils.github.io/titiler-pgstac/
 Project-URL: Issues, https://github.com/stac-utils/titiler-pgstac/issues
 Project-URL: Source, https://github.com/stac-utils/titiler-pgstac
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/10407788/132182694-52cd3d02-5b80-4bb0-9102-b98272fae0f9.png"/>
+  <img width="500" src="https://github.com/stac-utils/titiler-pgstac/assets/10407788/24a64ea9-fede-4ee8-ab8d-625c9e94db44"/>
   <p align="center">Connect PgSTAC and TiTiler.</p>
 </p>
 
 <p align="center">
   <a href="https://github.com/stac-utils/titiler-pgstac/actions?query=workflow%3ACI" target="_blank">
       <img src="https://github.com/developmentseed/titiler/workflows/CI/badge.svg" alt="Test">
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.4.1 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.5.0 Summary: Connect
 PgSTAC and TiTiler. Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile
 server,pgSTAC Author-email: Vincent Sarago
 developmentseed.com>,David Bitner
 developmentseed.com> Requires-Python: >=3.8 Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -11,16 +11,16 @@
 Provides-Extra: dev Provides-Extra: psycopg Provides-Extra: psycopg-binary
 Provides-Extra: psycopg-c Provides-Extra: test Project-URL: Changelog, https://
 stac-utils.github.io/titiler-pgstac/release-notes/ Project-URL: Documentation,
 https://stac-utils.github.io/titiler-pgstac/ Project-URL: Homepage, https://
 stac-utils.github.io/titiler-pgstac/ Project-URL: Issues, https://github.com/
 stac-utils/titiler-pgstac/issues Project-URL: Source, https://github.com/stac-
 utils/titiler-pgstac Description-Content-Type: text/markdown
- [https://user-images.githubusercontent.com/10407788/132182694-52cd3d02-5b80-
-                          4bb0-9102-b98272fae0f9.png]
+ [https://github.com/stac-utils/titiler-pgstac/assets/10407788/24a64ea9-fede-
+                            4ee8-ab8d-625c9e94db44]
                           Connect PgSTAC and TiTiler.
                  [Test] [Coverage] [Package_version] [License]
 --- **Documentation**: https://stac-utils.github.io/titiler-pgstac/ **Source
 Code**: https://github.com/stac-utils/titiler-pgstac --- `TiTiler.PgSTAC` is a
 [titiler](https://github.com/developmentseed/titiler) extension which connect
 to [pgstac](https://github.com/stac-utils/pgstac) STAC database in order to
 create dynamic **mosaics** based on [`Search Query`](https://github.com/
```

