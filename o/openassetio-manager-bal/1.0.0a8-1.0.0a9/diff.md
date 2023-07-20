# Comparing `tmp/openassetio_manager_bal-1.0.0a8-py3-none-any.whl.zip` & `tmp/openassetio_manager_bal-1.0.0a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 16277 bytes, number of entries: 9
--rw-r--r--  2.0 unx    10306 b- defN 23-May-25 16:18 openassetio_manager_bal/BasicAssetLibraryInterface.py
--rw-r--r--  2.0 unx     2977 b- defN 23-May-25 16:18 openassetio_manager_bal/__init__.py
--rw-r--r--  2.0 unx    11567 b- defN 23-May-25 16:18 openassetio_manager_bal/bal.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4016 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       80 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      881 b- defN 23-May-25 16:18 openassetio_manager_bal-1.0.0a8.dist-info/RECORD
-9 files, 41300 bytes uncompressed, 14721 bytes compressed:  64.4%
+Zip file size: 16632 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    14323 b- defN 23-Jul-20 12:48 openassetio_manager_bal/BasicAssetLibraryInterface.py
+-rw-r--r--  2.0 unx     2977 b- defN 23-Jul-20 12:48 openassetio_manager_bal/__init__.py
+-rw-r--r--  2.0 unx    11564 b- defN 23-Jul-20 12:48 openassetio_manager_bal/bal.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4016 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      881 b- defN 23-Jul-20 12:49 openassetio_manager_bal-1.0.0a9.dist-info/RECORD
+9 files, 45314 bytes uncompressed, 15076 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: openassetio_manager_bal/__init__.py
 Comment: 
 
 Filename: openassetio_manager_bal/bal.py
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/LICENSE
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/LICENSE
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/METADATA
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/METADATA
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/WHEEL
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: openassetio_manager_bal-1.0.0a8.dist-info/RECORD
+Filename: openassetio_manager_bal-1.0.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openassetio_manager_bal/BasicAssetLibraryInterface.py

```diff
@@ -16,25 +16,25 @@
 
 # Fix module-level name check, as well as OpenAssetIO methods
 # pylint: disable=invalid-name
 """
 A single-class module, providing the BasicAssetLibraryInterface class.
 """
 
-import itertools
 import os
 import time
 
 from functools import wraps
 from openassetio import constants, BatchElementError, EntityReference, TraitsData
 from openassetio.exceptions import MalformedEntityReference, PluginError
-from openassetio.managerApi import ManagerInterface
+from openassetio.managerApi import ManagerInterface, EntityReferencePagerInterface
 
 from . import bal
 
+
 __all__ = [
     "BasicAssetLibraryInterface",
 ]
 
 
 # TODO(TC): @pylint-disable
 # As we are building out the implementation vertically, we have known
@@ -45,17 +45,15 @@
 # pylint: disable=too-many-arguments, unused-argument
 
 
 def simulated_delay(func):
     @wraps(func)
     def wrapper_simulated_delay(self, *args, **kwargs):
         # pylint: disable=protected-access
-        delay_ms = self._BasicAssetLibraryInterface__settings.get(
-            bal.SETTINGS_KEY_SIMULATED_QUERY_LATENCY, 0
-        )
+        delay_ms = self.simulated_latency
         if delay_ms > 0:
             time.sleep(delay_ms / 1000.0)  # sleep takes seconds
         return func(self, *args, **kwargs)
 
     return wrapper_simulated_delay
 
 
@@ -82,14 +80,25 @@
 
     def info(self):
         return {constants.kField_EntityReferencesMatchPrefix: self.__reference_prefix}
 
     def settings(self, hostSession):
         return self.__settings.copy()
 
+    @property
+    def simulated_latency(self):
+        """
+        BAL internal convenience to get the simulated latency of API
+        methods.
+
+        This is read-only - updating the latency must be done via the
+        settings mechanism, i.e. re-`initialize` the plugin.
+        """
+        return self.__settings.get(bal.SETTINGS_KEY_SIMULATED_QUERY_LATENCY, 0)
+
     def initialize(self, managerSettings, hostSession):
         bal.validate_settings(managerSettings)
 
         # Settings updates can be partial, so make sure we keep any
         # existing path.
         existing_library_path = self.__settings.get("library_path")
         library_path = managerSettings.get("library_path", existing_library_path)
@@ -154,104 +163,168 @@
             for idx in range(len(entityReferences)):
                 errorCallback(idx, result)
             return
 
         for idx, ref in enumerate(entityReferences):
             try:
                 entity_info = bal.parse_entity_ref(ref.toString())
-            except bal.MalformedBALReference as exc:
-                result = BatchElementError(
-                    BatchElementError.ErrorCode.kMalformedEntityReference, str(exc)
-                )
-                errorCallback(idx, result)
-            else:
-                try:
-                    entity = bal.entity(entity_info, self.__library)
-                except bal.UnknownBALEntity:
-                    result = BatchElementError(
-                        BatchElementError.ErrorCode.kEntityResolutionError,
-                        f"Entity '{ref.toString()}' not found",
-                    )
-                    errorCallback(idx, result)
-                else:
-                    result = TraitsData()
-                    for trait in traitSet:
-                        trait_data = entity.traits.get(trait)
-                        if trait_data is not None:
-                            self.__add_trait_to_traits_data(trait, trait_data, result)
-
-                    successCallback(idx, result)
+                entity = bal.entity(entity_info, self.__library)
+                result = TraitsData()
+                for trait in traitSet:
+                    trait_data = entity.traits.get(trait)
+                    if trait_data is not None:
+                        self.__add_trait_to_traits_data(trait, trait_data, result)
+                successCallback(idx, result)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
     @simulated_delay
     def preflight(
         self, targetEntityRefs, traitSet, context, hostSession, successCallback, errorCallback
     ):
         # Support publishing to any valid entity reference
         for idx, ref in enumerate(targetEntityRefs):
             try:
                 bal.parse_entity_ref(ref.toString())
-            except bal.MalformedBALReference as exc:
-                result = BatchElementError(
-                    BatchElementError.ErrorCode.kMalformedEntityReference, str(exc)
-                )
-                errorCallback(idx, result)
-            else:
                 successCallback(idx, ref)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
     @simulated_delay
     def register(
         self,
         targetEntityRefs,
         entityTraitsDatas,
         context,
         hostSession,
         successCallback,
         errorCallback,
     ):
         for idx, ref in enumerate(targetEntityRefs):
             try:
                 entity_info = bal.parse_entity_ref(ref.toString())
-            except bal.MalformedBALReference as exc:
-                result = BatchElementError(
-                    BatchElementError.ErrorCode.kMalformedEntityReference, str(exc)
-                )
-                errorCallback(idx, result)
-            else:
                 traits_dict = self.__traits_data_to_dict(entityTraitsDatas[idx])
                 updated_entity_info = bal.create_or_update_entity(
                     entity_info, traits_dict, self.__library
                 )
                 successCallback(idx, self.__build_entity_ref(updated_entity_info))
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
     @simulated_delay
-    def getRelatedReferences(
-        self, entityRefs, relationshipTraitsDatas, context, hostSession, resultTraitSet=None
+    def getWithRelationship(
+        self,
+        entityReferences,
+        relationshipTraitsData,
+        resultTraitSet,
+        context,
+        hostSession,
+        successCallback,
+        errorCallback,
     ):
-        results = []
+        for idx, entity_ref in enumerate(entityReferences):
+            try:
+                entity_info = bal.parse_entity_ref(entity_ref.toString())
+                relations = bal.related_references(
+                    entity_info,
+                    self.__traits_data_to_dict(relationshipTraitsData),
+                    resultTraitSet,
+                    self.__library,
+                )
+                successCallback(idx, [self.__build_entity_ref(info) for info in relations])
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
-        # The inputs are either equal length arrays with index-wise
-        # correspondence, or, one of refs or relationships will have a
-        # single element that should be used for each entry in the
-        # other.
-        fill_value = entityRefs[0] if len(entityRefs) == 1 else relationshipTraitsDatas[0]
-
-        for entity_ref, relation_traits in itertools.zip_longest(
-            entityRefs, relationshipTraitsDatas, fillvalue=fill_value
-        ):
-            entity_info = bal.parse_entity_ref(entity_ref.toString())
-            relations = bal.related_references(
-                entity_info,
-                self.__traits_data_to_dict(relation_traits),
-                resultTraitSet,
-                self.__library,
-            )
-            # Convert the EntityInfos to entity references
-            results.append([self.__build_entity_ref(i) for i in relations])
+    @simulated_delay
+    def getWithRelationships(
+        self,
+        entityReference,
+        relationshipTraitsDatas,
+        resultTraitSet,
+        context,
+        hostSession,
+        successCallback,
+        errorCallback,
+    ):
+        for idx, relationship in enumerate(relationshipTraitsDatas):
+            try:
+                entity_info = bal.parse_entity_ref(entityReference.toString())
+                relations = bal.related_references(
+                    entity_info,
+                    self.__traits_data_to_dict(relationship),
+                    resultTraitSet,
+                    self.__library,
+                )
+                successCallback(idx, [self.__build_entity_ref(info) for info in relations])
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
-        return results
+    @simulated_delay
+    def getWithRelationshipPaged(
+        self,
+        entityReferences,
+        relationshipTraitsData,
+        resultTraitSet,
+        pageSize,
+        _context,
+        _hostSession,
+        successCallback,
+        errorCallback,
+    ):
+        for idx, entity_ref in enumerate(entityReferences):
+            try:
+                entity_info = bal.parse_entity_ref(entity_ref.toString())
+                relations = bal.related_references(
+                    entity_info,
+                    self.__traits_data_to_dict(relationshipTraitsData),
+                    resultTraitSet,
+                    self.__library,
+                )
+                successCallback(
+                    idx,
+                    BALEntityReferencePagerInterface(
+                        self.simulated_latency,
+                        pageSize,
+                        [self.__build_entity_ref(info) for info in relations],
+                    ),
+                )
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
+
+    @simulated_delay
+    def getWithRelationshipsPaged(
+        self,
+        entityReference,
+        relationshipTraitsDatas,
+        resultTraitSet,
+        pageSize,
+        _context,
+        _hostSession,
+        successCallback,
+        errorCallback,
+    ):
+        for idx, relationship in enumerate(relationshipTraitsDatas):
+            try:
+                entity_info = bal.parse_entity_ref(entityReference.toString())
+                relations = bal.related_references(
+                    entity_info,
+                    self.__traits_data_to_dict(relationship),
+                    resultTraitSet,
+                    self.__library,
+                )
+                successCallback(
+                    idx,
+                    BALEntityReferencePagerInterface(
+                        self.simulated_latency,
+                        pageSize,
+                        [self.__build_entity_ref(info) for info in relations],
+                    ),
+                )
+            except Exception as exc:  # pylint: disable=broad-except
+                self.__handle_exception(exc, idx, errorCallback)
 
     def __build_entity_ref(self, entity_info: bal.EntityInfo) -> EntityReference:
         """
         Builds an openassetio EntityReference from a BAL EntityInfo
         """
         ref_string = f"bal:///{entity_info.name}"
         return self._createEntityReference(ref_string)
@@ -274,7 +347,56 @@
         }
 
     @staticmethod
     def __add_trait_to_traits_data(trait_id: str, trait_properties: dict, traits_data: TraitsData):
         traits_data.addTrait(trait_id)
         for name, value in trait_properties.items():
             traits_data.setTraitProperty(trait_id, name, value)
+
+    @staticmethod
+    def __handle_exception(exc, idx, error_callback):
+        """
+        Calls the error_callback with an appropriate BatchElementError
+        depending on the caught exception.
+
+        Other, exceptional exceptions are re-thrown.
+        """
+        msg = str(exc)
+
+        if isinstance(exc, bal.MalformedBALReference):
+            code = BatchElementError.ErrorCode.kMalformedEntityReference
+        elif isinstance(exc, bal.UnknownBALEntity):
+            code = BatchElementError.ErrorCode.kEntityResolutionError
+        else:
+            raise exc
+
+        error_callback(idx, BatchElementError(code, msg))
+
+
+class BALEntityReferencePagerInterface(EntityReferencePagerInterface):
+    """
+    Simple implementation of a pager.
+
+    Bulk-queries all data, then splits up into cached pages ready to
+    regurgitate on demand.
+    """
+
+    def __init__(self, simulated_latency, page_size, entity_references):
+        EntityReferencePagerInterface.__init__(self)
+        self.simulated_latency = simulated_latency
+        self.__page_num = 0
+        self.__pages = []
+
+        for page_start in range(0, len(entity_references), page_size):
+            self.__pages.append(entity_references[page_start : page_start + page_size])
+
+    @simulated_delay
+    def hasNext(self, _hostSession):
+        return self.__page_num < len(self.__pages) - 1
+
+    @simulated_delay
+    def next(self, _hostSession):
+        self.__page_num += 1
+
+    @simulated_delay
+    def get(self, _hostSession):
+        return self.__pages[self.__page_num] if self.__page_num < len(self.__pages) else []
```

## openassetio_manager_bal/bal.py

```diff
@@ -334,15 +334,15 @@
 class UnknownBALEntity(RuntimeError):
     """
     An exception raised for a reference to a non-existent entity in the
     library.
     """
 
     def __init__(self, entity_info: EntityInfo):
-        super().__init__(f"Unknown BAL entity: '{entity_info.name}'")
+        super().__init__(f"Entity '{entity_info.name}' not found")
 
 
 class MalformedBALReference(RuntimeError):
     """
     An exception raised for a reference that is missing an entity name
     or other required part.
     """
```

## Comparing `openassetio_manager_bal-1.0.0a8.dist-info/LICENSE` & `openassetio_manager_bal-1.0.0a9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openassetio_manager_bal-1.0.0a8.dist-info/METADATA` & `openassetio_manager_bal-1.0.0a9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassetio-manager-bal
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A contrived "asset management system" for OpenAssetIO integration test cases.
 Author-email: Contributors to the OpenAssetIO project <openassetio-discussion@lists.aswf.io>
 Project-URL: OpenAssetIO, https://github.com/OpenAssetIO/OpenAssetIO
 Project-URL: Source, https://github.com/OpenAssetIO/OpenAssetIO-Manager-BAL
 Project-URL: Issues, https://github.com/OpenAssetIO/OpenAssetIO-Manager-BAL/issues
 Keywords: openassetio,manager
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `openassetio_manager_bal-1.0.0a8.dist-info/RECORD` & `openassetio_manager_bal-1.0.0a9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-openassetio_manager_bal/BasicAssetLibraryInterface.py,sha256=6YyQ0SJuQzxWctHGo6DgmmYqN_xg4tJlCwxJap3kScE,10306
+openassetio_manager_bal/BasicAssetLibraryInterface.py,sha256=OGx7f40mSRXakokRkQG7bo9VihxvoJ34cl9zmAaE3Gw,14323
 openassetio_manager_bal/__init__.py,sha256=qknWAey9xukBvuiZE_QhPdHLEnKCMVATRaCBJ9nYFk0,2977
-openassetio_manager_bal/bal.py,sha256=px6uNnYOeJDA3E9PTQI3yEDiP0aiSGqw5yP4ff9E_yM,11567
-openassetio_manager_bal-1.0.0a8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-openassetio_manager_bal-1.0.0a8.dist-info/METADATA,sha256=YlmBYx63kO1tb4maOAP3W9PxKYRSJeeY50MxAGkmlG0,4016
-openassetio_manager_bal-1.0.0a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openassetio_manager_bal-1.0.0a8.dist-info/entry_points.txt,sha256=fytCZqstf6QK_vvtL6GiB-WS_cVDSbYxpbu39KvH6M4,80
-openassetio_manager_bal-1.0.0a8.dist-info/top_level.txt,sha256=cENM5tr7Znp5WE3vUGZnsNPGR-KOVR9qm54_kNPbyII,24
-openassetio_manager_bal-1.0.0a8.dist-info/RECORD,,
+openassetio_manager_bal/bal.py,sha256=iv2AucQWeWMc0vpvrMHzahol8BILPbgk_Pnztj5nwZE,11564
+openassetio_manager_bal-1.0.0a9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+openassetio_manager_bal-1.0.0a9.dist-info/METADATA,sha256=6C8W8ro5tOQKVUPa1vMTvY7YZR3xI4qC9-MUaORjQMU,4016
+openassetio_manager_bal-1.0.0a9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openassetio_manager_bal-1.0.0a9.dist-info/entry_points.txt,sha256=fytCZqstf6QK_vvtL6GiB-WS_cVDSbYxpbu39KvH6M4,80
+openassetio_manager_bal-1.0.0a9.dist-info/top_level.txt,sha256=cENM5tr7Znp5WE3vUGZnsNPGR-KOVR9qm54_kNPbyII,24
+openassetio_manager_bal-1.0.0a9.dist-info/RECORD,,
```

