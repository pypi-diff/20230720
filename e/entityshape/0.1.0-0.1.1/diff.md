# Comparing `tmp/entityshape-0.1.0.tar.gz` & `tmp/entityshape-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entityshape-0.1.0.tar", max compression
+gzip compressed data, was "entityshape-0.1.1.tar", max compression
```

## Comparing `entityshape-0.1.0.tar` & `entityshape-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.1.0/LICENSE
--rw-r--r--   0        0        0     3914 2023-06-25 14:47:24.433237 entityshape-0.1.0/README.md
--rw-r--r--   0        0        0     2040 2023-06-25 15:16:53.263700 entityshape-0.1.0/entityshape/__init__.py
--rw-r--r--   0        0        0      538 2023-06-24 12:30:09.051783 entityshape-0.1.0/entityshape/enums.py
--rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/__init__.py
--rw-r--r--   0        0        0      183 2023-06-24 12:27:51.347797 entityshape-0.1.0/entityshape/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14398 2023-06-24 12:27:51.351131 entityshape-0.1.0/entityshape/models/__pycache__/compareshape.cpython-311.pyc
--rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.1.0/entityshape/models/__pycache__/conditions.cpython-311.pyc
--rw-r--r--   0        0        0      812 2023-06-24 12:27:51.451131 entityshape-0.1.0/entityshape/models/__pycache__/property_value.cpython-311.pyc
--rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.1.0/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
--rw-r--r--   0        0        0    11008 2023-06-25 14:39:11.690780 entityshape-0.1.0/entityshape/models/__pycache__/result.cpython-311.pyc
--rw-r--r--   0        0        0    17190 2023-06-24 12:27:51.461131 entityshape-0.1.0/entityshape/models/__pycache__/shape.cpython-311.pyc
--rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.1.0/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
--rw-r--r--   0        0        0      967 2023-06-24 12:43:06.050877 entityshape-0.1.0/entityshape/models/__pycache__/statement_value.cpython-311.pyc
--rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/compareshape.py
--rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/property_value.py
--rw-r--r--   0        0        0     7004 2023-06-25 14:39:11.244107 entityshape-0.1.0/entityshape/models/result.py
--rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/shape.py
--rw-r--r--   0        0        0      377 2023-06-24 12:41:01.799816 entityshape-0.1.0/entityshape/models/statement_value.py
--rw-r--r--   0        0        0     3138 2023-06-25 15:24:27.303751 entityshape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 entityshape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4134 2023-07-20 18:03:06.774013 entityshape-0.1.1/README.md
+-rw-r--r--   0        0        0     2353 2023-07-20 16:57:55.423286 entityshape-0.1.1/entityshape/__init__.py
+-rw-r--r--   0        0        0      538 2023-06-24 12:30:09.051783 entityshape-0.1.1/entityshape/enums.py
+-rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.1.1/entityshape/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.1.1/entityshape/models/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-24 12:27:51.347797 entityshape-0.1.1/entityshape/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14398 2023-06-24 12:27:51.351131 entityshape-0.1.1/entityshape/models/__pycache__/compareshape.cpython-311.pyc
+-rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.1.1/entityshape/models/__pycache__/conditions.cpython-311.pyc
+-rw-r--r--   0        0        0      812 2023-06-24 12:27:51.451131 entityshape-0.1.1/entityshape/models/__pycache__/property_value.cpython-311.pyc
+-rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.1.1/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
+-rw-r--r--   0        0        0    12886 2023-07-20 17:04:52.278385 entityshape-0.1.1/entityshape/models/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0      797 2023-07-20 17:04:52.408386 entityshape-0.1.1/entityshape/models/__pycache__/result_property.cpython-311.pyc
+-rw-r--r--   0        0        0    17190 2023-06-24 12:27:51.461131 entityshape-0.1.1/entityshape/models/__pycache__/shape.cpython-311.pyc
+-rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.1.1/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
+-rw-r--r--   0        0        0      967 2023-06-24 12:43:06.050877 entityshape-0.1.1/entityshape/models/__pycache__/statement_value.cpython-311.pyc
+-rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.1.1/entityshape/models/compareshape.py
+-rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.1.1/entityshape/models/property_value.py
+-rw-r--r--   0        0        0     8659 2023-07-20 17:04:51.741711 entityshape-0.1.1/entityshape/models/result.py
+-rw-r--r--   0        0        0      172 2023-07-20 17:01:32.216014 entityshape-0.1.1/entityshape/models/result_property.py
+-rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.1.1/entityshape/models/shape.py
+-rw-r--r--   0        0        0      377 2023-06-24 12:41:01.799816 entityshape-0.1.1/entityshape/models/statement_value.py
+-rw-r--r--   0        0        0     3169 2023-07-20 17:56:24.007189 entityshape-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 entityshape-0.1.1/PKG-INFO
```

### Comparing `entityshape-0.1.0/LICENSE` & `entityshape-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/README.md` & `entityshape-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 The shape and compareshape classes currently only support:
 * cardinality (too many or not enough values)
 * whether the property is allowed or not
 * whether the value of a statement on a given property is correct/incorrect
 
 It is still a bit unclear if and how the qualifier validation works.
 
+Only Wikidata is supported currently when fetching labels for the result.
+If you need support for other Wikibase installations, [comment here](https://github.com/dpriskorn/entityshape/issues/15).
+
 # Installation
 Get it from pypi
 
 `$ pip install pyentityshape`
 
 # Usage
 
@@ -29,18 +32,18 @@
 [campsites](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-campsites-in-sweden.ipynb) 
 [shelters](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-shelters-in-sweden.ipynb)
 
 ## CLI
 Example:
 ```
 e = EntityShape(eid="E1", lang="en", qid="Q1")
-result = e.get_result()
+result = e.validate_and_get_result()
 # Get human readable result
 print(result)
-"Valid: False\nproperties_without_enough_correct_statements: {'P31'}"
+"Valid: False\nProperties_without_enough_correct_statements: instance of (P31)"
 # Access the data
 print(result.properties_without_enough_correct_statements)
 "{'P31'}"
 ```
 
 ## Validation
 The is_valid method on the Result object mimics all red warnings displayed by https://www.wikidata.org/wiki/User:Teester/EntityShape.js 
@@ -49,15 +52,15 @@
 1.  properties with too many statements found
 2.   incorrect statements found
 3.   some required properties are missing
 4.   properties without enough correct statements found
 5.   statements with properties that are not allowed found
 
 ## Known working schemas
-This library currently only supports a subset of all features in the ShEx specifikation.
+This library currently only supports a subset of all features in the ShEx specification.
 
 The following Entity Schemas are known to work:
 * [hiking path](https://www.wikidata.org/w/index.php?title=EntitySchema:E375&oldid=1833851062)
 * [shelter](https://www.wikidata.org/w/index.php?title=EntitySchema:E398&oldid=1923235264)
 
 # Background
 This library is the glue between libraries like [Wikibase
```

### Comparing `entityshape-0.1.0/entityshape/__init__.py` & `entityshape-0.1.1/entityshape/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Any, Dict, Optional
 
 from pydantic import BaseModel
 
 from entityshape.exceptions import ApiError, EidError, LangError, QidError
 from entityshape.models.compareshape import CompareShape
 from entityshape.models.result import Result
 from entityshape.models.shape import Shape
@@ -10,49 +11,54 @@
 
 class EntityShape(BaseModel):
     """This class models the entityshape API
     It has a default timeout of 10 seconds
 
     The API currently only support items"""
 
-    qid = ""  # item
-    eid = ""  # entityshape
-    lang = ""  # language
+    entity_id: str = ""  # item or lexeme
+    eid: str = ""  # entityshape
+    lang: str = "en"  # language defaults to English
     result: Result = Result()
     eid_regex = re.compile(r"E\d+")
-    qid_regex = re.compile(r"Q\d+")
-    compare_shape_result: dict = {}
+    entity_id_regex = re.compile(r"[QL]\d+")
+    compare_shape_result: Optional[Dict[str, Any]] = None
 
     def __check_inputs__(self):
         if not self.lang:
             raise LangError("We only support 2 and 3 letter language codes")
         if not self.eid:
             raise EidError("We need an entityshape EID")
         if not re.match(self.eid_regex, self.eid):
             raise EidError("EID has to be E followed by only numbers like this: E100")
-        if not self.qid:
+        if not self.entity_id:
             raise QidError("We need an item QID")
-        if not re.match(self.qid_regex, self.qid):
+        if not re.match(self.entity_id_regex, self.entity_id):
             raise QidError("QID has to be Q followed by only numbers like this: Q100")
 
     def validate_and_get_result(self) -> Result:
         """This method checks if we got the 3 parameters we need and
         gets the results and return them"""
         self.__check_inputs__()
         self.__validate__()
         return self.__parse_result__()
 
     def __validate__(self):
         shape: Shape = Shape(self.eid, self.lang)
         comparison: CompareShape = CompareShape(
-            shape.get_schema_shape(), self.qid, self.lang
+            shape.get_schema_shape(), self.entity_id, self.lang
         )
-        self.compare_shape_result: dict = {
+        self.compare_shape_result = {}
+        self.compare_shape_result = {
             "general": comparison.get_general(),
             "properties": comparison.get_properties(),
             "statements": comparison.get_statements(),
         }
 
     def __parse_result__(self) -> Result:
-        self.result = Result(**self.compare_shape_result)
-        self.result.analyze()
-        return self.result
+        if self.compare_shape_result:
+            self.result = Result(**self.compare_shape_result)
+            self.result.lang = self.lang
+            self.result.analyze()
+            return self.result
+        else:
+            return Result()
```

### Comparing `entityshape-0.1.0/entityshape/enums.py` & `entityshape-0.1.1/entityshape/enums.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/compareshape.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/compareshape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/conditions.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/conditions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/property_value.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/property_value.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/result.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/result.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,100 +1,116 @@
 magic:    0xa70d0d0a
-moddate:  0x8f519864 (Sun Jun 25 14:39:11 2023 UTC)
-files sz: 7004
+moddate:  0x3369b964 (Thu Jul 20 17:04:51 2023 UTC)
+files sz: 8659
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
-      00640064036c056d065a066d075a070100640064046c086d095a096d0a5a
-      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00020065006a1000000000000000006511a6010000ab0100000000000000
-      005a12020047006407840064086506a6030000ab0300000000000000005a
-      1364015300
+      0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
+      055a050100640064036c066d075a070100640064046c086d095a09010064
+      0064056c0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064066c0e6d0f5a0f01
+      00640064076c106d115a110100640064086c126d135a130100020065006a
+      1400000000000000006515a6010000ab0100000000000000005a16020047
+      0064098400640a6507a6030000ab0300000000000000005a1764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Any', 'Dict', 'Set'))
+                12 LOAD_CONST               2 (('Any', 'Dict', 'List', 'Set'))
                 14 IMPORT_NAME              1 (typing)
                 16 IMPORT_FROM              2 (Any)
                 18 STORE_NAME               2 (Any)
                 20 IMPORT_FROM              3 (Dict)
                 22 STORE_NAME               3 (Dict)
-                24 IMPORT_FROM              4 (Set)
-                26 STORE_NAME               4 (Set)
-                28 POP_TOP
+                24 IMPORT_FROM              4 (List)
+                26 STORE_NAME               4 (List)
+                28 IMPORT_FROM              5 (Set)
+                30 STORE_NAME               5 (Set)
+                32 POP_TOP
    
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('BaseModel', 'ValidationError'))
-                34 IMPORT_NAME              5 (pydantic)
-                36 IMPORT_FROM              6 (BaseModel)
-                38 STORE_NAME               6 (BaseModel)
-                40 IMPORT_FROM              7 (ValidationError)
-                42 STORE_NAME               7 (ValidationError)
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('BaseModel',))
+                38 IMPORT_NAME              6 (pydantic)
+                40 IMPORT_FROM              7 (BaseModel)
+                42 STORE_NAME               7 (BaseModel)
                 44 POP_TOP
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('Necessity', 'PropertyResponse', 'StatementResponse'))
-                50 IMPORT_NAME              8 (entityshape.enums)
-                52 IMPORT_FROM              9 (Necessity)
-                54 STORE_NAME               9 (Necessity)
-                56 IMPORT_FROM             10 (PropertyResponse)
-                58 STORE_NAME              10 (PropertyResponse)
-                60 IMPORT_FROM             11 (StatementResponse)
-                62 STORE_NAME              11 (StatementResponse)
-                64 POP_TOP
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('WikibaseIntegrator',))
+                50 IMPORT_NAME              8 (wikibaseintegrator)
+                52 IMPORT_FROM              9 (WikibaseIntegrator)
+                54 STORE_NAME               9 (WikibaseIntegrator)
+                56 POP_TOP
    
-     7          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('PropertyValue',))
-                70 IMPORT_NAME             12 (entityshape.models.property_value)
-                72 IMPORT_FROM             13 (PropertyValue)
-                74 STORE_NAME              13 (PropertyValue)
+     7          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('Necessity', 'PropertyResponse', 'StatementResponse'))
+                62 IMPORT_NAME             10 (entityshape.enums)
+                64 IMPORT_FROM             11 (Necessity)
+                66 STORE_NAME              11 (Necessity)
+                68 IMPORT_FROM             12 (PropertyResponse)
+                70 STORE_NAME              12 (PropertyResponse)
+                72 IMPORT_FROM             13 (StatementResponse)
+                74 STORE_NAME              13 (StatementResponse)
                 76 POP_TOP
    
      8          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('StatementValue',))
-                82 IMPORT_NAME             14 (entityshape.models.statement_value)
-                84 IMPORT_FROM             15 (StatementValue)
-                86 STORE_NAME              15 (StatementValue)
+                80 LOAD_CONST               6 (('PropertyValue',))
+                82 IMPORT_NAME             14 (entityshape.models.property_value)
+                84 IMPORT_FROM             15 (PropertyValue)
+                86 STORE_NAME              15 (PropertyValue)
                 88 POP_TOP
    
-    10          90 PUSH_NULL
-                92 LOAD_NAME                0 (logging)
-                94 LOAD_ATTR               16 (getLogger)
-               104 LOAD_NAME               17 (__name__)
-               106 PRECALL                  1
-               110 CALL                     1
-               120 STORE_NAME              18 (logger)
+     9          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               7 (('ResultProperty',))
+                94 IMPORT_NAME             16 (entityshape.models.result_property)
+                96 IMPORT_FROM             17 (ResultProperty)
+                98 STORE_NAME              17 (ResultProperty)
+               100 POP_TOP
    
-    13         122 PUSH_NULL
-               124 LOAD_BUILD_CLASS
-               126 LOAD_CONST               7 (<code object Result, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 13>)
-               128 MAKE_FUNCTION            0
-               130 LOAD_CONST               8 ('Result')
-               132 LOAD_NAME                6 (BaseModel)
-               134 PRECALL                  3
-               138 CALL                     3
-               148 STORE_NAME              19 (Result)
-               150 LOAD_CONST               1 (None)
-               152 RETURN_VALUE
+    10         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('StatementValue',))
+               106 IMPORT_NAME             18 (entityshape.models.statement_value)
+               108 IMPORT_FROM             19 (StatementValue)
+               110 STORE_NAME              19 (StatementValue)
+               112 POP_TOP
+   
+    12         114 PUSH_NULL
+               116 LOAD_NAME                0 (logging)
+               118 LOAD_ATTR               20 (getLogger)
+               128 LOAD_NAME               21 (__name__)
+               130 PRECALL                  1
+               134 CALL                     1
+               144 STORE_NAME              22 (logger)
+   
+    15         146 PUSH_NULL
+               148 LOAD_BUILD_CLASS
+               150 LOAD_CONST               9 (<code object Result, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 15>)
+               152 MAKE_FUNCTION            0
+               154 LOAD_CONST              10 ('Result')
+               156 LOAD_NAME                7 (BaseModel)
+               158 PRECALL                  3
+               162 CALL                     3
+               172 STORE_NAME              23 (Result)
+               174 LOAD_CONST               1 (None)
+               176 RETURN_VALUE
    consts
       0
       None
-      ('Any', 'Dict', 'Set')
-      ('BaseModel', 'ValidationError')
+      ('Any', 'Dict', 'List', 'Set')
+      ('BaseModel',)
+      ('WikibaseIntegrator',)
       ('Necessity', 'PropertyResponse', 'StatementResponse')
       ('PropertyValue',)
+      ('ResultProperty',)
       ('StatementValue',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
@@ -112,319 +128,338 @@
             1465156506640c3c0000000200650da6000000ab0000000000000000005a
             16650f6508190000000000000000006506640d3c0000000200650da60000
             00ab0000000000000000005a17650f650819000000000000000000650664
             0e3c0000000200650da6000000ab0000000000000000005a18650f650819
             0000000000000000006506640f3c0000000200650da6000000ab00000000
             00000000005a19650f650819000000000000000000650664103c00000002
             00650da6000000ab0000000000000000005a1a650f650819000000000000
-            000000650664113c000000651b64128400a6000000ab0000000000000000
-            005a1c651b64138400a6000000ab0000000000000000005a1d651b641484
-            00a6000000ab0000000000000000005a1e651b64158400a6000000ab0000
-            000000000000005a1f651b64168400a6000000ab0000000000000000005a
-            20651b64176515660264188404a6000000ab0000000000000000005a2165
-            1b64198400a6000000ab0000000000000000005a22641a84005a23641b84
-            005a24641c84005a25641d84005a26641e84005a27641f84005a28642084
-            005a29642184005a2a642284005a2b642384005a2c642484005a2d642584
-            005a2e64265300
-          13           0 RESUME                   0
+            000000650664113c00000064125a1b6508650664133c000000651c641484
+            00a6000000ab0000000000000000005a1d651c64158400a6000000ab0000
+            000000000000005a1e651c64168400a6000000ab0000000000000000005a
+            1f651c64178400a6000000ab0000000000000000005a20651c64188400a6
+            000000ab0000000000000000005a21651c641965156602641a8404a60000
+            00ab0000000000000000005a22651c641b8400a6000000ab000000000000
+            0000005a23641c84005a24641d84005a25641e84005a26641f84005a2764
+            2084005a28642184005a29642284005a2a642384005a2b642484005a2c64
+            2584005a2d6426650f6508190000000000000000006602642784045a2e64
+            2884005a2f642984005a30642a5300
+          15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Result')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          14          12 BUILD_MAP                0
+          16          12 BUILD_MAP                0
                       14 STORE_NAME               3 (general)
                       16 LOAD_NAME                4 (Dict)
                       18 LOAD_NAME                5 (Any)
                       20 LOAD_NAME                5 (Any)
                       22 BUILD_TUPLE              2
                       24 BINARY_SUBSCR
                       34 LOAD_NAME                6 (__annotations__)
                       36 LOAD_CONST               1 ('general')
                       38 STORE_SUBSCR
          
-          15          42 LOAD_CONST               2 ('')
+          17          42 LOAD_CONST               2 ('')
                       44 STORE_NAME               7 (name)
                       46 LOAD_NAME                8 (str)
                       48 LOAD_NAME                6 (__annotations__)
                       50 LOAD_CONST               3 ('name')
                       52 STORE_SUBSCR
          
-          16          56 BUILD_MAP                0
+          18          56 BUILD_MAP                0
                       58 STORE_NAME               9 (properties)
                       60 LOAD_NAME                4 (Dict)
                       62 LOAD_NAME                8 (str)
                       64 LOAD_NAME               10 (PropertyValue)
                       66 BUILD_TUPLE              2
                       68 BINARY_SUBSCR
                       78 LOAD_NAME                6 (__annotations__)
                       80 LOAD_CONST               4 ('properties')
                       82 STORE_SUBSCR
          
-          17          86 BUILD_MAP                0
+          19          86 BUILD_MAP                0
                       88 STORE_NAME              11 (statements)
                       90 LOAD_NAME                4 (Dict)
                       92 LOAD_NAME                5 (Any)
                       94 LOAD_NAME               12 (StatementValue)
                       96 BUILD_TUPLE              2
                       98 BINARY_SUBSCR
                      108 LOAD_NAME                6 (__annotations__)
                      110 LOAD_CONST               5 ('statements')
                      112 STORE_SUBSCR
          
-          18         116 PUSH_NULL
+          20         116 PUSH_NULL
                      118 LOAD_NAME               13 (set)
                      120 PRECALL                  0
                      124 CALL                     0
                      134 STORE_NAME              14 (missing_properties)
                      136 LOAD_NAME               15 (Set)
                      138 LOAD_NAME                8 (str)
                      140 BINARY_SUBSCR
                      150 LOAD_NAME                6 (__annotations__)
                      152 LOAD_CONST               6 ('missing_properties')
                      154 STORE_SUBSCR
          
-          19         158 PUSH_NULL
+          21         158 PUSH_NULL
                      160 LOAD_NAME               13 (set)
                      162 PRECALL                  0
                      166 CALL                     0
                      176 STORE_NAME              16 (required_properties)
                      178 LOAD_NAME               15 (Set)
                      180 LOAD_NAME                8 (str)
                      182 BINARY_SUBSCR
                      192 LOAD_NAME                6 (__annotations__)
                      194 LOAD_CONST               7 ('required_properties')
                      196 STORE_SUBSCR
          
-          20         200 PUSH_NULL
+          22         200 PUSH_NULL
                      202 LOAD_NAME               13 (set)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 STORE_NAME              17 (incorrect_statements)
                      220 LOAD_NAME               15 (Set)
                      222 LOAD_NAME                8 (str)
                      224 BINARY_SUBSCR
                      234 LOAD_NAME                6 (__annotations__)
                      236 LOAD_CONST               8 ('incorrect_statements')
                      238 STORE_SUBSCR
          
-          21         242 PUSH_NULL
+          23         242 PUSH_NULL
                      244 LOAD_NAME               13 (set)
                      246 PRECALL                  0
                      250 CALL                     0
                      260 STORE_NAME              18 (missing_statements)
                      262 LOAD_NAME               15 (Set)
                      264 LOAD_NAME                8 (str)
                      266 BINARY_SUBSCR
                      276 LOAD_NAME                6 (__annotations__)
                      278 LOAD_CONST               9 ('missing_statements')
                      280 STORE_SUBSCR
          
-          22         284 PUSH_NULL
+          24         284 PUSH_NULL
                      286 LOAD_NAME               13 (set)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 STORE_NAME              19 (properties_with_too_many_statements)
                      304 LOAD_NAME               15 (Set)
                      306 LOAD_NAME                8 (str)
                      308 BINARY_SUBSCR
                      318 LOAD_NAME                6 (__annotations__)
                      320 LOAD_CONST              10 ('properties_with_too_many_statements')
                      322 STORE_SUBSCR
          
-          23         326 LOAD_CONST              11 (False)
+          25         326 LOAD_CONST              11 (False)
                      328 STORE_NAME              20 (analyzed)
                      330 LOAD_NAME               21 (bool)
                      332 LOAD_NAME                6 (__annotations__)
                      334 LOAD_CONST              12 ('analyzed')
                      336 STORE_SUBSCR
          
-          24         340 PUSH_NULL
+          26         340 PUSH_NULL
                      342 LOAD_NAME               13 (set)
                      344 PRECALL                  0
                      348 CALL                     0
                      358 STORE_NAME              22 (required_properties_that_are_missing)
                      360 LOAD_NAME               15 (Set)
                      362 LOAD_NAME                8 (str)
                      364 BINARY_SUBSCR
                      374 LOAD_NAME                6 (__annotations__)
                      376 LOAD_CONST              13 ('required_properties_that_are_missing')
                      378 STORE_SUBSCR
          
-          25         382 PUSH_NULL
+          27         382 PUSH_NULL
                      384 LOAD_NAME               13 (set)
                      386 PRECALL                  0
                      390 CALL                     0
                      400 STORE_NAME              23 (optional_properties_that_are_missing)
                      402 LOAD_NAME               15 (Set)
                      404 LOAD_NAME                8 (str)
                      406 BINARY_SUBSCR
                      416 LOAD_NAME                6 (__annotations__)
                      418 LOAD_CONST              14 ('optional_properties_that_are_missing')
                      420 STORE_SUBSCR
          
-          26         424 PUSH_NULL
+          28         424 PUSH_NULL
                      426 LOAD_NAME               13 (set)
                      428 PRECALL                  0
                      432 CALL                     0
                      442 STORE_NAME              24 (properties_without_enough_correct_statements)
                      444 LOAD_NAME               15 (Set)
                      446 LOAD_NAME                8 (str)
                      448 BINARY_SUBSCR
                      458 LOAD_NAME                6 (__annotations__)
                      460 LOAD_CONST              15 ('properties_without_enough_correct_statements')
                      462 STORE_SUBSCR
          
-          27         466 PUSH_NULL
+          29         466 PUSH_NULL
                      468 LOAD_NAME               13 (set)
                      470 PRECALL                  0
                      474 CALL                     0
                      484 STORE_NAME              25 (properties_that_are_not_allowed)
                      486 LOAD_NAME               15 (Set)
                      488 LOAD_NAME                8 (str)
                      490 BINARY_SUBSCR
                      500 LOAD_NAME                6 (__annotations__)
                      502 LOAD_CONST              16 ('properties_that_are_not_allowed')
                      504 STORE_SUBSCR
          
-          28         508 PUSH_NULL
+          30         508 PUSH_NULL
                      510 LOAD_NAME               13 (set)
                      512 PRECALL                  0
                      516 CALL                     0
                      526 STORE_NAME              26 (statements_with_property_that_is_not_allowed)
                      528 LOAD_NAME               15 (Set)
                      530 LOAD_NAME                8 (str)
                      532 BINARY_SUBSCR
                      542 LOAD_NAME                6 (__annotations__)
                      544 LOAD_CONST              17 ('statements_with_property_that_is_not_allowed')
                      546 STORE_SUBSCR
          
-          30         550 LOAD_NAME               27 (property)
+          31         550 LOAD_CONST              18 ('en')
+                     552 STORE_NAME              27 (lang)
+                     554 LOAD_NAME                8 (str)
+                     556 LOAD_NAME                6 (__annotations__)
+                     558 LOAD_CONST              19 ('lang')
+                     560 STORE_SUBSCR
+         
+          33         564 LOAD_NAME               28 (property)
+         
+          34         566 LOAD_CONST              20 (<code object some_required_properties_are_missing, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 33>)
+                     568 MAKE_FUNCTION            0
+         
+          33         570 PRECALL                  0
+                     574 CALL                     0
+         
+          34         584 STORE_NAME              29 (some_required_properties_are_missing)
          
-          31         552 LOAD_CONST              18 (<code object some_required_properties_are_missing, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 30>)
-                     554 MAKE_FUNCTION            0
+          37         586 LOAD_NAME               28 (property)
          
-          30         556 PRECALL                  0
-                     560 CALL                     0
+          38         588 LOAD_CONST              21 (<code object properties_with_too_many_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 37>)
+                     590 MAKE_FUNCTION            0
          
-          31         570 STORE_NAME              28 (some_required_properties_are_missing)
+          37         592 PRECALL                  0
+                     596 CALL                     0
          
-          34         572 LOAD_NAME               27 (property)
+          38         606 STORE_NAME              30 (properties_with_too_many_statements_found)
          
-          35         574 LOAD_CONST              19 (<code object properties_with_too_many_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 34>)
-                     576 MAKE_FUNCTION            0
+          41         608 LOAD_NAME               28 (property)
          
-          34         578 PRECALL                  0
-                     582 CALL                     0
+          42         610 LOAD_CONST              22 (<code object incorrect_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 41>)
+                     612 MAKE_FUNCTION            0
          
-          35         592 STORE_NAME              29 (properties_with_too_many_statements_found)
+          41         614 PRECALL                  0
+                     618 CALL                     0
          
-          38         594 LOAD_NAME               27 (property)
+          42         628 STORE_NAME              31 (incorrect_statements_found)
          
-          39         596 LOAD_CONST              20 (<code object incorrect_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 38>)
-                     598 MAKE_FUNCTION            0
+          45         630 LOAD_NAME               28 (property)
          
-          38         600 PRECALL                  0
-                     604 CALL                     0
+          46         632 LOAD_CONST              23 (<code object properties_without_enough_correct_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 45>)
+                     634 MAKE_FUNCTION            0
          
-          39         614 STORE_NAME              30 (incorrect_statements_found)
+          45         636 PRECALL                  0
+                     640 CALL                     0
          
-          42         616 LOAD_NAME               27 (property)
+          46         650 STORE_NAME              32 (properties_without_enough_correct_statements_found)
          
-          43         618 LOAD_CONST              21 (<code object properties_without_enough_correct_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 42>)
-                     620 MAKE_FUNCTION            0
+          49         652 LOAD_NAME               28 (property)
          
-          42         622 PRECALL                  0
-                     626 CALL                     0
+          50         654 LOAD_CONST              24 (<code object statements_with_properties_that_are_not_allowed_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 49>)
+                     656 MAKE_FUNCTION            0
          
-          43         636 STORE_NAME              31 (properties_without_enough_correct_statements_found)
+          49         658 PRECALL                  0
+                     662 CALL                     0
          
-          46         638 LOAD_NAME               27 (property)
+          50         672 STORE_NAME              33 (statements_with_properties_that_are_not_allowed_found)
          
-          47         640 LOAD_CONST              22 (<code object statements_with_properties_that_are_not_allowed_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 46>)
-                     642 MAKE_FUNCTION            0
+          53         674 LOAD_NAME               28 (property)
          
-          46         644 PRECALL                  0
-                     648 CALL                     0
+          54         676 LOAD_CONST              25 ('return')
+                     678 LOAD_NAME               21 (bool)
+                     680 BUILD_TUPLE              2
+                     682 LOAD_CONST              26 (<code object is_valid, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 53>)
+                     684 MAKE_FUNCTION            4 (annotations)
          
-          47         658 STORE_NAME              32 (statements_with_properties_that_are_not_allowed_found)
+          53         686 PRECALL                  0
+                     690 CALL                     0
          
-          50         660 LOAD_NAME               27 (property)
+          54         700 STORE_NAME              34 (is_valid)
          
-          51         662 LOAD_CONST              23 ('return')
-                     664 LOAD_NAME               21 (bool)
-                     666 BUILD_TUPLE              2
-                     668 LOAD_CONST              24 (<code object is_valid, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 50>)
-                     670 MAKE_FUNCTION            4 (annotations)
+          68         702 LOAD_NAME               28 (property)
          
-          50         672 PRECALL                  0
-                     676 CALL                     0
+          69         704 LOAD_CONST              27 (<code object is_empty, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 68>)
+                     706 MAKE_FUNCTION            0
          
-          51         686 STORE_NAME              33 (is_valid)
+          68         708 PRECALL                  0
+                     712 CALL                     0
          
-          65         688 LOAD_NAME               27 (property)
+          69         722 STORE_NAME              35 (is_empty)
          
-          66         690 LOAD_CONST              25 (<code object is_empty, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 65>)
-                     692 MAKE_FUNCTION            0
+          72         724 LOAD_CONST              28 (<code object analyze, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 72>)
+                     726 MAKE_FUNCTION            0
+                     728 STORE_NAME              36 (analyze)
          
-          65         694 PRECALL                  0
-                     698 CALL                     0
+          85         730 LOAD_CONST              29 (<code object __find_properties_with_too_many_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 85>)
+                     732 MAKE_FUNCTION            0
+                     734 STORE_NAME              37 (__find_properties_with_too_many_statements__)
          
-          66         708 STORE_NAME              34 (is_empty)
+          91         736 LOAD_CONST              30 (<code object __find_incorrect_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 91>)
+                     738 MAKE_FUNCTION            0
+                     740 STORE_NAME              38 (__find_incorrect_statements__)
          
-          69         710 LOAD_CONST              26 (<code object analyze, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 69>)
-                     712 MAKE_FUNCTION            0
-                     714 STORE_NAME              35 (analyze)
+         103         742 LOAD_CONST              31 (<code object __find_required_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 103>)
+                     744 MAKE_FUNCTION            0
+                     746 STORE_NAME              39 (__find_required_properties__)
          
-          82         716 LOAD_CONST              27 (<code object __find_properties_with_too_many_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 82>)
-                     718 MAKE_FUNCTION            0
-                     720 STORE_NAME              36 (__find_properties_with_too_many_statements__)
+         109         748 LOAD_CONST              32 (<code object __find_missing_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 109>)
+                     750 MAKE_FUNCTION            0
+                     752 STORE_NAME              40 (__find_missing_properties__)
          
-          88         722 LOAD_CONST              28 (<code object __find_incorrect_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 88>)
-                     724 MAKE_FUNCTION            0
-                     726 STORE_NAME              37 (__find_incorrect_statements__)
+         115         754 LOAD_CONST              33 (<code object __find_required_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 115>)
+                     756 MAKE_FUNCTION            0
+                     758 STORE_NAME              41 (__find_required_properties_that_are_missing__)
          
-         100         728 LOAD_CONST              29 (<code object __find_required_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 100>)
-                     730 MAKE_FUNCTION            0
-                     732 STORE_NAME              38 (__find_required_properties__)
+         122         760 LOAD_CONST              34 (<code object __find_optional_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 122>)
+                     762 MAKE_FUNCTION            0
+                     764 STORE_NAME              42 (__find_optional_properties_that_are_missing__)
          
-         106         734 LOAD_CONST              30 (<code object __find_missing_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 106>)
-                     736 MAKE_FUNCTION            0
-                     738 STORE_NAME              39 (__find_missing_properties__)
+         128         766 LOAD_CONST              35 (<code object __find_properties_with_not_enough_correct_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 128>)
+                     768 MAKE_FUNCTION            0
+                     770 STORE_NAME              43 (__find_properties_with_not_enough_correct_statements__)
          
-         112         740 LOAD_CONST              31 (<code object __find_required_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 112>)
-                     742 MAKE_FUNCTION            0
-                     744 STORE_NAME              40 (__find_required_properties_that_are_missing__)
+         134         772 LOAD_CONST              36 (<code object __find_properties_that_are_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 134>)
+                     774 MAKE_FUNCTION            0
+                     776 STORE_NAME              44 (__find_properties_that_are_not_allowed__)
          
-         119         746 LOAD_CONST              32 (<code object __find_optional_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 119>)
-                     748 MAKE_FUNCTION            0
-                     750 STORE_NAME              41 (__find_optional_properties_that_are_missing__)
+         140         778 LOAD_CONST              37 (<code object __find_statements_with_property_that_is_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 140>)
+                     780 MAKE_FUNCTION            0
+                     782 STORE_NAME              45 (__find_statements_with_property_that_is_not_allowed__)
          
-         125         752 LOAD_CONST              33 (<code object __find_properties_with_not_enough_correct_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 125>)
-                     754 MAKE_FUNCTION            0
-                     756 STORE_NAME              42 (__find_properties_with_not_enough_correct_statements__)
+         146         784 LOAD_CONST              38 ('string_properties')
          
-         131         758 LOAD_CONST              34 (<code object __find_properties_that_are_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 131>)
-                     760 MAKE_FUNCTION            0
-                     762 STORE_NAME              43 (__find_properties_that_are_not_allowed__)
+         147         786 LOAD_NAME               15 (Set)
+                     788 LOAD_NAME                8 (str)
+                     790 BINARY_SUBSCR
          
-         137         764 LOAD_CONST              35 (<code object __find_statements_with_property_that_is_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 137>)
-                     766 MAKE_FUNCTION            0
-                     768 STORE_NAME              44 (__find_statements_with_property_that_is_not_allowed__)
+         146         800 BUILD_TUPLE              2
+                     802 LOAD_CONST              39 (<code object get_properties_as_a_string_with_labels_and_pid, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 146>)
+                     804 MAKE_FUNCTION            4 (annotations)
+                     806 STORE_NAME              46 (get_properties_as_a_string_with_labels_and_pid)
          
-         143         770 LOAD_CONST              36 (<code object __str__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 143>)
-                     772 MAKE_FUNCTION            0
-                     774 STORE_NAME              45 (__str__)
+         159         808 LOAD_CONST              40 (<code object __str__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 159>)
+                     810 MAKE_FUNCTION            0
+                     812 STORE_NAME              47 (__str__)
          
-         146         776 LOAD_CONST              37 (<code object __repr__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 146>)
-                     778 MAKE_FUNCTION            0
-                     780 STORE_NAME              46 (__repr__)
-                     782 LOAD_CONST              38 (None)
-                     784 RETURN_VALUE
+         162         814 LOAD_CONST              41 (<code object __repr__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 162>)
+                     816 MAKE_FUNCTION            0
+                     818 STORE_NAME              48 (__repr__)
+                     820 LOAD_CONST              42 (None)
+                     822 RETURN_VALUE
          consts
             'Result'
             'general'
             ''
             'name'
             'properties'
             'statements'
@@ -436,220 +471,222 @@
             False
             'analyzed'
             'required_properties_that_are_missing'
             'optional_properties_that_are_missing'
             'properties_without_enough_correct_statements'
             'properties_that_are_not_allowed'
             'statements_with_property_that_is_not_allowed'
+            'en'
+            'lang'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                30           0 RESUME                   0
+                33           0 RESUME                   0
                
-                32           2 LOAD_GLOBAL              1 (NULL + bool)
+                35           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (required_properties_that_are_missing)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'required_properties_that_are_missing')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'some_required_properties_are_missing'
-               firstlineno 30
+               firstlineno 33
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                34           0 RESUME                   0
+                37           0 RESUME                   0
                
-                36           2 LOAD_GLOBAL              1 (NULL + bool)
+                39           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (properties_with_too_many_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'properties_with_too_many_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'properties_with_too_many_statements_found'
-               firstlineno 34
+               firstlineno 37
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                38           0 RESUME                   0
+                41           0 RESUME                   0
                
-                40           2 LOAD_GLOBAL              1 (NULL + bool)
+                43           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (incorrect_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'incorrect_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'incorrect_statements_found'
-               firstlineno 38
+               firstlineno 41
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                42           0 RESUME                   0
+                45           0 RESUME                   0
                
-                44           2 LOAD_GLOBAL              1 (NULL + bool)
+                47           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (properties_without_enough_correct_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'properties_without_enough_correct_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'properties_without_enough_correct_statements_found'
-               firstlineno 42
+               firstlineno 45
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                46           0 RESUME                   0
+                49           0 RESUME                   0
                
-                48           2 LOAD_GLOBAL              1 (NULL + bool)
+                51           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (statements_with_property_that_is_not_allowed)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'statements_with_property_that_is_not_allowed')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'statements_with_properties_that_are_not_allowed_found'
-               firstlineno 46
+               firstlineno 49
                lnotab 0x0202
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007403000000000000000000007c006a0200
                   000000000000000c006f1f7c006a0300000000000000000c006f177c006a
                   0400000000000000000c006f0f7c006a0500000000000000000c006f077c
                   006a0600000000000000000c00a6010000ab0100000000000000005300
-                50           0 RESUME                   0
+                53           0 RESUME                   0
                
-                56           2 LOAD_FAST                0 (self)
+                59           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (analyze)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-                57          42 LOAD_GLOBAL              3 (NULL + bool)
+                60          42 LOAD_GLOBAL              3 (NULL + bool)
                
-                58          54 LOAD_FAST                0 (self)
+                61          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (properties_with_too_many_statements_found)
                             66 UNARY_NOT
                             68 JUMP_IF_FALSE_OR_POP    31 (to 132)
                
-                59          70 LOAD_FAST                0 (self)
+                62          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                3 (incorrect_statements_found)
                             82 UNARY_NOT
                
-                58          84 JUMP_IF_FALSE_OR_POP    23 (to 132)
+                61          84 JUMP_IF_FALSE_OR_POP    23 (to 132)
                
-                60          86 LOAD_FAST                0 (self)
+                63          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                4 (some_required_properties_are_missing)
                             98 UNARY_NOT
                
-                58         100 JUMP_IF_FALSE_OR_POP    15 (to 132)
+                61         100 JUMP_IF_FALSE_OR_POP    15 (to 132)
                
-                61         102 LOAD_FAST                0 (self)
+                64         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                5 (properties_without_enough_correct_statements_found)
                            114 UNARY_NOT
                
-                58         116 JUMP_IF_FALSE_OR_POP     7 (to 132)
+                61         116 JUMP_IF_FALSE_OR_POP     7 (to 132)
                
-                62         118 LOAD_FAST                0 (self)
+                65         118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                6 (statements_with_properties_that_are_not_allowed_found)
                            130 UNARY_NOT
                
-                57     >>  132 PRECALL                  1
+                60     >>  132 PRECALL                  1
                            136 CALL                     1
                            146 RETURN_VALUE
                consts
                   'check if the properties are all allowed,\n        all required properties are present,\n        not too many statements,\n        and none of the statements are incorrect'
                names      ('analyze', 'bool', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'some_required_properties_are_missing', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'is_valid'
-               firstlineno 50
+               firstlineno 53
                lnotab 0x020628010c0110010eff02020efe02030efd02040efb
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007403000000000000000000007c006a
                   020000000000000000a6010000ab01000000000000000064016b02000000
                   006f177403000000000000000000007c006a030000000000000000a60100
                   00ab01000000000000000064016b0200000000a6010000ab010000000000
                   0000005300
-                65           0 RESUME                   0
+                68           0 RESUME                   0
                
-                67           2 LOAD_GLOBAL              1 (NULL + bool)
+                70           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_GLOBAL              3 (NULL + len)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (properties)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_CONST               1 (0)
                             54 COMPARE_OP               2 (==)
@@ -669,15 +706,15 @@
                   0
                names      ('bool', 'len', 'properties', 'statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'is_empty'
-               firstlineno 65
+               firstlineno 68
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
@@ -691,145 +728,145 @@
                   000000000001007c00a00600000000000000000000000000000000000000
                   00a6000000ab00000000000000000001007c00a007000000000000000000
                   0000000000000000000000a6000000ab00000000000000000001007c00a0
                   080000000000000000000000000000000000000000a6000000ab00000000
                   000000000001007c00a00900000000000000000000000000000000000000
                   00a6000000ab000000000000000000010064017c005f0000000000000000
                   006400530064005300
-                69           0 RESUME                   0
+                72           0 RESUME                   0
                
-                70           2 LOAD_FAST                0 (self)
+                73           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (analyzed)
                             14 POP_JUMP_FORWARD_IF_TRUE   189 (to 394)
                
-                71          16 LOAD_FAST                0 (self)
+                74          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (__find_missing_properties__)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 POP_TOP
                
-                72          56 LOAD_FAST                0 (self)
+                75          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (__find_required_properties__)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 POP_TOP
                
-                73          96 LOAD_FAST                0 (self)
+                76          96 LOAD_FAST                0 (self)
                             98 LOAD_METHOD              3 (__find_incorrect_statements__)
                            120 PRECALL                  0
                            124 CALL                     0
                            134 POP_TOP
                
-                74         136 LOAD_FAST                0 (self)
+                77         136 LOAD_FAST                0 (self)
                            138 LOAD_METHOD              4 (__find_properties_with_too_many_statements__)
                            160 PRECALL                  0
                            164 CALL                     0
                            174 POP_TOP
                
-                75         176 LOAD_FAST                0 (self)
+                78         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD              5 (__find_properties_with_not_enough_correct_statements__)
                            200 PRECALL                  0
                            204 CALL                     0
                            214 POP_TOP
                
-                76         216 LOAD_FAST                0 (self)
+                79         216 LOAD_FAST                0 (self)
                            218 LOAD_METHOD              6 (__find_required_properties_that_are_missing__)
                            240 PRECALL                  0
                            244 CALL                     0
                            254 POP_TOP
                
-                77         256 LOAD_FAST                0 (self)
+                80         256 LOAD_FAST                0 (self)
                            258 LOAD_METHOD              7 (__find_optional_properties_that_are_missing__)
                            280 PRECALL                  0
                            284 CALL                     0
                            294 POP_TOP
                
-                78         296 LOAD_FAST                0 (self)
+                81         296 LOAD_FAST                0 (self)
                            298 LOAD_METHOD              8 (__find_properties_that_are_not_allowed__)
                            320 PRECALL                  0
                            324 CALL                     0
                            334 POP_TOP
                
-                79         336 LOAD_FAST                0 (self)
+                82         336 LOAD_FAST                0 (self)
                            338 LOAD_METHOD              9 (__find_statements_with_property_that_is_not_allowed__)
                            360 PRECALL                  0
                            364 CALL                     0
                            374 POP_TOP
                
-                80         376 LOAD_CONST               1 (True)
+                83         376 LOAD_CONST               1 (True)
                            378 LOAD_FAST                0 (self)
                            380 STORE_ATTR               0 (analyzed)
                            390 LOAD_CONST               0 (None)
                            392 RETURN_VALUE
                
-                70     >>  394 LOAD_CONST               0 (None)
+                73     >>  394 LOAD_CONST               0 (None)
                            396 RETURN_VALUE
                consts
                   None
                   True
                names      ('analyzed', '__find_missing_properties__', '__find_required_properties__', '__find_incorrect_statements__', '__find_properties_with_too_many_statements__', '__find_properties_with_not_enough_correct_statements__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'analyze'
-               firstlineno 69
+               firstlineno 72
                lnotab 0x02010e0128012801280128012801280128012801280112f6
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-                82           0 RESUME                   0
+                85           0 RESUME                   0
                
-                83           2 LOAD_FAST                0 (self)
+                86           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-                84          20 LOAD_FAST                0 (self)
+                87          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                85          46 LOAD_FAST                2 (value)
+                88          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (TOO_MANY_STATEMENTS)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-                86          88 LOAD_FAST                0 (self)
+                89          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_with_too_many_statements)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-                83     >>  142 LOAD_CONST               0 (None)
+                86     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'TOO_MANY_STATEMENTS', 'properties_with_too_many_statements', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_with_too_many_statements__'
-               firstlineno 82
+               firstlineno 85
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -839,229 +876,229 @@
                   026a0200000000000000007402000000000000000000006a030000000000
                   0000006b0200000000721a7c006a040000000000000000a0050000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   0001008c542300740c00000000000000000000240072250100740e000000
                   00000000000000a008000000000000000000000000000000000000000064
                   017c026a0200000000000000009b009d02a6010000ab0100000000000000
                   00010059008c82770078035900770164005300
-                88           0 RESUME                   0
+                91           0 RESUME                   0
                
-                89           2 LOAD_FAST                0 (self)
+                92           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (statements)
                             14 GET_ITER
                        >>   16 FOR_ITER               133 (to 284)
                             18 STORE_FAST               1 (statement)
                
-                90          20 LOAD_FAST                0 (self)
+                93          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (statements)
                             32 LOAD_FAST                1 (statement)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                91          46 NOP
+                94          46 NOP
                
-                92          48 LOAD_GLOBAL              3 (NULL + StatementResponse)
+                95          48 LOAD_GLOBAL              3 (NULL + StatementResponse)
                             60 LOAD_FAST                2 (value)
                             62 LOAD_ATTR                2 (response)
                             72 PRECALL                  1
                             76 CALL                     1
                             86 POP_TOP
                
-                93          88 LOAD_FAST                2 (value)
+                96          88 LOAD_FAST                2 (value)
                             90 LOAD_ATTR                2 (response)
                            100 LOAD_GLOBAL              2 (StatementResponse)
                            112 LOAD_ATTR                3 (INCORRECT)
                            122 COMPARE_OP               2 (==)
                            128 POP_JUMP_FORWARD_IF_FALSE    26 (to 182)
                
-                94         130 LOAD_FAST                0 (self)
+                97         130 LOAD_FAST                0 (self)
                            132 LOAD_ATTR                4 (incorrect_statements)
                            142 LOAD_METHOD              5 (add)
                            164 LOAD_FAST                1 (statement)
                            166 PRECALL                  1
                            170 CALL                     1
                            180 POP_TOP
                        >>  182 JUMP_BACKWARD           84 (to 16)
                        >>  184 PUSH_EXC_INFO
                
-                95         186 LOAD_GLOBAL             12 (ValueError)
+                98         186 LOAD_GLOBAL             12 (ValueError)
                            198 CHECK_EXC_MATCH
                            200 POP_JUMP_FORWARD_IF_FALSE    37 (to 276)
                            202 POP_TOP
                
-                97         204 LOAD_GLOBAL             14 (logger)
+               100         204 LOAD_GLOBAL             14 (logger)
                            216 LOAD_METHOD              8 (warning)
                            238 LOAD_CONST               1 ('Ignoring statement response: ')
                            240 LOAD_FAST                2 (value)
                            242 LOAD_ATTR                2 (response)
                            252 FORMAT_VALUE             0
                            254 BUILD_STRING             2
                            256 PRECALL                  1
                            260 CALL                     1
                            270 POP_TOP
                
-                98         272 POP_EXCEPT
+               101         272 POP_EXCEPT
                            274 JUMP_BACKWARD          130 (to 16)
                
-                95     >>  276 RERAISE                  0
+                98     >>  276 RERAISE                  0
                        >>  278 COPY                     3
                            280 POP_EXCEPT
                            282 RERAISE                  1
                
-                89     >>  284 LOAD_CONST               0 (None)
+                92     >>  284 LOAD_CONST               0 (None)
                            286 RETURN_VALUE
                ExceptionTable:
                  48 to 180 -> 184 [1]
                  184 to 270 -> 278 [2] lasti
                  276 to 276 -> 278 [2] lasti
                consts
                   None
                   'Ignoring statement response: '
                names      ('statements', 'StatementResponse', 'response', 'INCORRECT', 'incorrect_statements', 'add', 'ValueError', 'logger', 'warning')
                varnames   ('self', 'statement', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_incorrect_statements__'
-               firstlineno 88
+               firstlineno 91
                lnotab 0x020112011a01020128012a0138011202440104fd08fa
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               100           0 RESUME                   0
+               103           0 RESUME                   0
                
-               101           2 LOAD_FAST                0 (self)
+               104           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               102          20 LOAD_FAST                0 (self)
+               105          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               103          46 LOAD_FAST                2 (value)
+               106          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (REQUIRED)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               104          88 LOAD_FAST                0 (self)
+               107          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (required_properties)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               101     >>  142 LOAD_CONST               0 (None)
+               104     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'necessity', 'Necessity', 'REQUIRED', 'required_properties', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_required_properties__'
-               firstlineno 100
+               firstlineno 103
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               106           0 RESUME                   0
+               109           0 RESUME                   0
                
-               107           2 LOAD_FAST                0 (self)
+               110           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               108          20 LOAD_FAST                0 (self)
+               111          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               109          46 LOAD_FAST                2 (value)
+               112          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (MISSING)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               110          88 LOAD_FAST                0 (self)
+               113          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (missing_properties)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               107     >>  142 LOAD_CONST               0 (None)
+               110     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'MISSING', 'missing_properties', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_missing_properties__'
-               firstlineno 106
+               firstlineno 109
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000007d017401000000000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d027c01a003000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000007c005f04000000000000000064005300
-               112           0 RESUME                   0
+               115           0 RESUME                   0
                
-               113           2 LOAD_GLOBAL              1 (NULL + set)
+               116           2 LOAD_GLOBAL              1 (NULL + set)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (missing_properties)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (a)
                
-               114          42 LOAD_GLOBAL              1 (NULL + set)
+               117          42 LOAD_GLOBAL              1 (NULL + set)
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (required_properties)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_FAST               2 (b)
                
-               117          82 LOAD_FAST                1 (a)
+               120          82 LOAD_FAST                1 (a)
                             84 LOAD_METHOD              3 (intersection)
                            106 LOAD_FAST                2 (b)
                            108 PRECALL                  1
                            112 CALL                     1
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (required_properties_that_are_missing)
                            134 LOAD_CONST               0 (None)
@@ -1070,44 +1107,44 @@
                   None
                names      ('set', 'missing_properties', 'required_properties', 'intersection', 'required_properties_that_are_missing')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_required_properties_that_are_missing__'
-               firstlineno 112
+               firstlineno 115
                lnotab 0x020128012803
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000007d017401000000000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d027c01a003000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000007c005f04000000000000000064015300
-               119           0 RESUME                   0
+               122           0 RESUME                   0
                
-               121           2 LOAD_GLOBAL              1 (NULL + set)
+               124           2 LOAD_GLOBAL              1 (NULL + set)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (missing_properties)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (a)
                
-               122          42 LOAD_GLOBAL              1 (NULL + set)
+               125          42 LOAD_GLOBAL              1 (NULL + set)
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (required_properties)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_FAST               2 (b)
                
-               123          82 LOAD_FAST                1 (a)
+               126          82 LOAD_FAST                1 (a)
                             84 LOAD_METHOD              3 (difference)
                            106 LOAD_FAST                2 (b)
                            108 PRECALL                  1
                            112 CALL                     1
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (optional_properties_that_are_missing)
                            134 LOAD_CONST               1 (None)
@@ -1117,317 +1154,503 @@
                   None
                names      ('set', 'missing_properties', 'required_properties', 'difference', 'optional_properties_that_are_missing')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_optional_properties_that_are_missing__'
-               firstlineno 119
+               firstlineno 122
                lnotab 0x020228012801
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               125           0 RESUME                   0
+               128           0 RESUME                   0
                
-               126           2 LOAD_FAST                0 (self)
+               129           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               127          20 LOAD_FAST                0 (self)
+               130          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               128          46 LOAD_FAST                2 (value)
+               131          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (NOT_ENOUGH_CORRECT_STATEMENTS)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               129          88 LOAD_FAST                0 (self)
+               132          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_without_enough_correct_statements)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               126     >>  142 LOAD_CONST               0 (None)
+               129     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'NOT_ENOUGH_CORRECT_STATEMENTS', 'properties_without_enough_correct_statements', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_with_not_enough_correct_statements__'
-               firstlineno 125
+               firstlineno 128
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               131           0 RESUME                   0
+               134           0 RESUME                   0
                
-               132           2 LOAD_FAST                0 (self)
+               135           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               133          20 LOAD_FAST                0 (self)
+               136          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               134          46 LOAD_FAST                2 (value)
+               137          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (ABSENT)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               135          88 LOAD_FAST                0 (self)
+               138          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_that_are_not_allowed)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               132     >>  142 LOAD_CONST               0 (None)
+               135     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'necessity', 'Necessity', 'ABSENT', 'properties_that_are_not_allowed', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_that_are_not_allowed__'
-               firstlineno 131
+               firstlineno 134
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d437d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721f7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c026a060000000000000000a6010000ab01000000000000000001
                   008c4464005300
-               137           0 RESUME                   0
+               140           0 RESUME                   0
                
-               138           2 LOAD_FAST                0 (self)
+               141           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (statements)
                             14 GET_ITER
                        >>   16 FOR_ITER                67 (to 152)
                             18 STORE_FAST               1 (statement)
                
-               139          20 LOAD_FAST                0 (self)
+               142          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (statements)
                             32 LOAD_FAST                1 (statement)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               140          46 LOAD_FAST                2 (value)
+               143          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (ABSENT)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    31 (to 150)
                
-               141          88 LOAD_FAST                0 (self)
+               144          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (statements_with_property_that_is_not_allowed)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                2 (value)
                            124 LOAD_ATTR                6 (property)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 POP_TOP
                        >>  150 JUMP_BACKWARD           68 (to 16)
                
-               138     >>  152 LOAD_CONST               0 (None)
+               141     >>  152 LOAD_CONST               0 (None)
                            154 RETURN_VALUE
                consts
                   None
                names      ('statements', 'necessity', 'Necessity', 'ABSENT', 'statements_with_property_that_is_not_allowed', 'add', 'property')
                varnames   ('self', 'statement', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_statements_with_property_that_is_not_allowed__'
-               firstlineno 137
+               firstlineno 140
                lnotab 0x020112011a012a0140fd
+            'string_properties'
+            code
+               argcount  : 3
+               nlocals   : 7
+               stacksize : 6
+               flags     : 3
+               code
+                  0x970067007d037c0244005d657d047c016a000000000000000000a00100
+                  000000000000000000000000000000000000007c04a6010000ab01000000
+                  00000000007d057405000000000000000000007c056a0300000000000000
+                  00a00100000000000000000000000000000000000000007c006a04000000
+                  0000000000ac01a6010000ab0100000000000000006a0500000000000000
+                  007c04ac02a6020000ab0200000000000000007d067c03a0060000000000
+                  0000000000000000000000000000007c06a6010000ab0100000000000000
+                  0001008c666403a007000000000000000000000000000000000000000064
+                  0484007c034400a6000000ab000000000000000000a6010000ab01000000
+                  00000000005300
+               146           0 RESUME                   0
+               
+               149           2 BUILD_LIST               0
+                             4 STORE_FAST               3 (properties)
+               
+               150           6 LOAD_FAST                2 (string_properties)
+                             8 GET_ITER
+                       >>   10 FOR_ITER               101 (to 214)
+                            12 STORE_FAST               4 (property_string)
+               
+               151          14 LOAD_FAST                1 (wbi)
+                            16 LOAD_ATTR                0 (property)
+                            26 LOAD_METHOD              1 (get)
+                            48 LOAD_FAST                4 (property_string)
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 STORE_FAST               5 (wbi_property)
+               
+               152          66 LOAD_GLOBAL              5 (NULL + ResultProperty)
+               
+               153          78 LOAD_FAST                5 (wbi_property)
+                            80 LOAD_ATTR                3 (labels)
+                            90 LOAD_METHOD              1 (get)
+                           112 LOAD_FAST                0 (self)
+                           114 LOAD_ATTR                4 (lang)
+                           124 KW_NAMES                 1
+                           126 PRECALL                  1
+                           130 CALL                     1
+                           140 LOAD_ATTR                5 (value)
+               
+               154         150 LOAD_FAST                4 (property_string)
+               
+               152         152 KW_NAMES                 2
+                           154 PRECALL                  2
+                           158 CALL                     2
+                           168 STORE_FAST               6 (property_object)
+               
+               156         170 LOAD_FAST                3 (properties)
+                           172 LOAD_METHOD              6 (append)
+                           194 LOAD_FAST                6 (property_object)
+                           196 PRECALL                  1
+                           200 CALL                     1
+                           210 POP_TOP
+                           212 JUMP_BACKWARD          102 (to 10)
+               
+               157     >>  214 LOAD_CONST               3 (', ')
+                           216 LOAD_METHOD              7 (join)
+                           238 LOAD_CONST               4 (<code object <listcomp>, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 157>)
+                           240 MAKE_FUNCTION            0
+                           242 LOAD_FAST                3 (properties)
+                           244 GET_ITER
+                           246 PRECALL                  0
+                           250 CALL                     0
+                           260 PRECALL                  1
+                           264 CALL                     1
+                           274 RETURN_VALUE
+               consts
+                  None
+                  ('language',)
+                  ('label', 'pid')
+                  ', '
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 5
+                     flags     : 19
+                     code
+                        0x970067007c005d117d017401000000000000000000007c01a6010000ab
+                        01000000000000000091028c125300
+                     157           0 RESUME                   0
+                                   2 BUILD_LIST               0
+                                   4 LOAD_FAST                0 (.0)
+                             >>    6 FOR_ITER                17 (to 42)
+                                   8 STORE_FAST               1 (property_)
+                                  10 LOAD_GLOBAL              1 (NULL + str)
+                                  22 LOAD_FAST                1 (property_)
+                                  24 PRECALL                  1
+                                  28 CALL                     1
+                                  38 LIST_APPEND              2
+                                  40 JUMP_BACKWARD           18 (to 6)
+                             >>   42 RETURN_VALUE
+                     consts
+                     names      ('str',)
+                     varnames   ('.0', 'property_')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
+                     name       '<listcomp>'
+                     firstlineno 157
+                     lnotab 0x
+               names      ('property', 'get', 'ResultProperty', 'labels', 'lang', 'value', 'append', 'join')
+               varnames   ('self', 'wbi', 'string_properties', 'properties', 'property_string', 'wbi_property', 'property_object')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
+               name       'get_properties_as_a_string_with_labels_and_pid'
+               firstlineno 146
+               lnotab 0x02030401080134010c01480102fe12042c01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
-                  00ab000000000000000000010064005300
-               143           0 RESUME                   0
+                  00ab0000000000000000005300
+               159           0 RESUME                   0
                
-               144           2 LOAD_FAST                0 (self)
+               160           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (__repr__)
                             26 PRECALL                  0
                             30 CALL                     0
-                            40 POP_TOP
-                            42 LOAD_CONST               0 (None)
-                            44 RETURN_VALUE
+                            40 RETURN_VALUE
                consts
                   None
                names      ('__repr__',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__str__'
-               firstlineno 143
+               firstlineno 159
                lnotab 0x0201
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 5
+               stacksize : 4
                flags     : 3
                code
                   0x970064017c006a0000000000000000009b009d027d017c006a00000000
-                  000000000072027c0153007c006a010000000000000000720d7c0164027c
-                  006a0200000000000000009b009d027a0d00007d017c006a030000000000
-                  000000720d7c0164037c006a0400000000000000009b009d027a0d00007d
-                  017c006a050000000000000000720d7c0164047c006a0500000000000000
-                  009b009d027a0d00007d017c006a060000000000000000720d7c0164057c
-                  006a0600000000000000009b009d027a0d00007d017c015300
-               146           0 RESUME                   0
+                  000000000072027c015300640264036c016d027d02010064047c0264053c
+                  000000740700000000000000000000a6000000ab0000000000000000007d
+                  037c006a04000000000000000072247c00a0050000000000000000000000
+                  0000000000000000007c006a0600000000000000007c03ac06a6020000ab
+                  0200000000000000007d047c0164077c049b009d027a0d00007d017c006a
+                  07000000000000000072247c00a005000000000000000000000000000000
+                  00000000007c006a0800000000000000007c03ac06a6020000ab02000000
+                  00000000007d047c0164087c049b009d027a0d00007d017c006a09000000
+                  000000000072247c00a00500000000000000000000000000000000000000
+                  007c006a0900000000000000007c03ac06a6020000ab0200000000000000
+                  007d047c0164097c049b009d027a0d00007d017c006a0a00000000000000
+                  00720d7c01640a7c006a0a00000000000000009b009d027a0d00007d017c
+                  015300
+               162           0 RESUME                   0
                
-               149           2 LOAD_CONST               1 ('Valid: ')
+               168           2 LOAD_CONST               1 ('Valid: ')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (is_valid)
                             16 FORMAT_VALUE             0
                             18 BUILD_STRING             2
                             20 STORE_FAST               1 (string)
                
-               150          22 LOAD_FAST                0 (self)
+               169          22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                0 (is_valid)
                             34 POP_JUMP_FORWARD_IF_FALSE     2 (to 40)
                
-               151          36 LOAD_FAST                1 (string)
+               170          36 LOAD_FAST                1 (string)
                             38 RETURN_VALUE
                
-               153     >>   40 LOAD_FAST                0 (self)
-                            42 LOAD_ATTR                1 (properties_with_too_many_statements_found)
-                            52 POP_JUMP_FORWARD_IF_FALSE    13 (to 80)
-               
-               154          54 LOAD_FAST                1 (string)
-                            56 LOAD_CONST               2 ('\nproperties_with_too_many_statements: ')
-                            58 LOAD_FAST                0 (self)
-                            60 LOAD_ATTR                2 (properties_with_too_many_statements)
-                            70 FORMAT_VALUE             0
-                            72 BUILD_STRING             2
-                            74 BINARY_OP               13 (+=)
-                            78 STORE_FAST               1 (string)
-               
-               155     >>   80 LOAD_FAST                0 (self)
-                            82 LOAD_ATTR                3 (properties_without_enough_correct_statements_found)
-                            92 POP_JUMP_FORWARD_IF_FALSE    13 (to 120)
-               
-               156          94 LOAD_FAST                1 (string)
-                            96 LOAD_CONST               3 ('\nproperties_without_enough_correct_statements: ')
-                            98 LOAD_FAST                0 (self)
-                           100 LOAD_ATTR                4 (properties_without_enough_correct_statements)
-                           110 FORMAT_VALUE             0
-                           112 BUILD_STRING             2
-                           114 BINARY_OP               13 (+=)
-                           118 STORE_FAST               1 (string)
-               
-               157     >>  120 LOAD_FAST                0 (self)
-                           122 LOAD_ATTR                5 (required_properties_that_are_missing)
-                           132 POP_JUMP_FORWARD_IF_FALSE    13 (to 160)
-               
-               158         134 LOAD_FAST                1 (string)
-                           136 LOAD_CONST               4 ('\nrequired_properties_that_are_missing: ')
-                           138 LOAD_FAST                0 (self)
-                           140 LOAD_ATTR                5 (required_properties_that_are_missing)
-                           150 FORMAT_VALUE             0
-                           152 BUILD_STRING             2
-                           154 BINARY_OP               13 (+=)
-                           158 STORE_FAST               1 (string)
-               
-               159     >>  160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                6 (incorrect_statements)
-                           172 POP_JUMP_FORWARD_IF_FALSE    13 (to 200)
-               
-               160         174 LOAD_FAST                1 (string)
-                           176 LOAD_CONST               5 ('\nincorrect_statements: ')
-                           178 LOAD_FAST                0 (self)
-                           180 LOAD_ATTR                6 (incorrect_statements)
-                           190 FORMAT_VALUE             0
-                           192 BUILD_STRING             2
-                           194 BINARY_OP               13 (+=)
-                           198 STORE_FAST               1 (string)
+               172     >>   40 LOAD_CONST               2 (0)
+                            42 LOAD_CONST               3 (('config',))
+                            44 IMPORT_NAME              1 (wikibaseintegrator.wbi_config)
+                            46 IMPORT_FROM              2 (config)
+                            48 STORE_FAST               2 (wbi_config)
+                            50 POP_TOP
                
-               161     >>  200 LOAD_FAST                1 (string)
-                           202 RETURN_VALUE
+               176          52 LOAD_CONST               4 ('entityshape (https://github.com/dpriskorn/entityshape)')
+               
+               174          54 LOAD_FAST                2 (wbi_config)
+               
+               175          56 LOAD_CONST               5 ('USER_AGENT')
+               
+               174          58 STORE_SUBSCR
+               
+               177          62 LOAD_GLOBAL              7 (NULL + WikibaseIntegrator)
+                            74 PRECALL                  0
+                            78 CALL                     0
+                            88 STORE_FAST               3 (wbi)
+               
+               178          90 LOAD_FAST                0 (self)
+                            92 LOAD_ATTR                4 (properties_with_too_many_statements_found)
+                           102 POP_JUMP_FORWARD_IF_FALSE    36 (to 176)
+               
+               179         104 LOAD_FAST                0 (self)
+                           106 LOAD_METHOD              5 (get_properties_as_a_string_with_labels_and_pid)
+               
+               180         128 LOAD_FAST                0 (self)
+                           130 LOAD_ATTR                6 (properties_with_too_many_statements)
+                           140 LOAD_FAST                3 (wbi)
+               
+               179         142 KW_NAMES                 6
+                           144 PRECALL                  2
+                           148 CALL                     2
+                           158 STORE_FAST               4 (properties_string)
+               
+               182         160 LOAD_FAST                1 (string)
+                           162 LOAD_CONST               7 ('\nProperties with too many statements: ')
+                           164 LOAD_FAST                4 (properties_string)
+                           166 FORMAT_VALUE             0
+                           168 BUILD_STRING             2
+                           170 BINARY_OP               13 (+=)
+                           174 STORE_FAST               1 (string)
+               
+               183     >>  176 LOAD_FAST                0 (self)
+                           178 LOAD_ATTR                7 (properties_without_enough_correct_statements_found)
+                           188 POP_JUMP_FORWARD_IF_FALSE    36 (to 262)
+               
+               184         190 LOAD_FAST                0 (self)
+                           192 LOAD_METHOD              5 (get_properties_as_a_string_with_labels_and_pid)
+               
+               185         214 LOAD_FAST                0 (self)
+                           216 LOAD_ATTR                8 (properties_without_enough_correct_statements)
+               
+               186         226 LOAD_FAST                3 (wbi)
+               
+               184         228 KW_NAMES                 6
+                           230 PRECALL                  2
+                           234 CALL                     2
+                           244 STORE_FAST               4 (properties_string)
+               
+               188         246 LOAD_FAST                1 (string)
+               
+               189         248 LOAD_CONST               8 ('\nProperties without enough correct statements: ')
+               
+               190         250 LOAD_FAST                4 (properties_string)
+               
+               189         252 FORMAT_VALUE             0
+                           254 BUILD_STRING             2
+               
+               188         256 BINARY_OP               13 (+=)
+                           260 STORE_FAST               1 (string)
+               
+               192     >>  262 LOAD_FAST                0 (self)
+                           264 LOAD_ATTR                9 (required_properties_that_are_missing)
+                           274 POP_JUMP_FORWARD_IF_FALSE    36 (to 348)
+               
+               193         276 LOAD_FAST                0 (self)
+                           278 LOAD_METHOD              5 (get_properties_as_a_string_with_labels_and_pid)
+               
+               194         300 LOAD_FAST                0 (self)
+                           302 LOAD_ATTR                9 (required_properties_that_are_missing)
+                           312 LOAD_FAST                3 (wbi)
+               
+               193         314 KW_NAMES                 6
+                           316 PRECALL                  2
+                           320 CALL                     2
+                           330 STORE_FAST               4 (properties_string)
+               
+               196         332 LOAD_FAST                1 (string)
+                           334 LOAD_CONST               9 ('\nRequired properties that are missing: ')
+                           336 LOAD_FAST                4 (properties_string)
+                           338 FORMAT_VALUE             0
+                           340 BUILD_STRING             2
+                           342 BINARY_OP               13 (+=)
+                           346 STORE_FAST               1 (string)
+               
+               197     >>  348 LOAD_FAST                0 (self)
+                           350 LOAD_ATTR               10 (incorrect_statements)
+                           360 POP_JUMP_FORWARD_IF_FALSE    13 (to 388)
+               
+               198         362 LOAD_FAST                1 (string)
+                           364 LOAD_CONST              10 ('\nIncorrect statements: ')
+                           366 LOAD_FAST                0 (self)
+                           368 LOAD_ATTR               10 (incorrect_statements)
+                           378 FORMAT_VALUE             0
+                           380 BUILD_STRING             2
+                           382 BINARY_OP               13 (+=)
+                           386 STORE_FAST               1 (string)
+               
+               199     >>  388 LOAD_FAST                1 (string)
+                           390 RETURN_VALUE
                consts
-                  'Return the result of the validation as a formatted string\n        with output exactly describing what caused the validation to fail'
+                  'Return the result of the validation as a formatted string\n        with output exactly describing what caused the validation to fail\n\n        We lookup the labels by default.\n        If no language is set we fall back to English'
                   'Valid: '
-                  '\nproperties_with_too_many_statements: '
-                  '\nproperties_without_enough_correct_statements: '
-                  '\nrequired_properties_that_are_missing: '
-                  '\nincorrect_statements: '
-               names      ('is_valid', 'properties_with_too_many_statements_found', 'properties_with_too_many_statements', 'properties_without_enough_correct_statements_found', 'properties_without_enough_correct_statements', 'required_properties_that_are_missing', 'incorrect_statements')
-               varnames   ('self', 'string')
+                  0
+                  ('config',)
+                  'entityshape (https://github.com/dpriskorn/entityshape)'
+                  'USER_AGENT'
+                  ('string_properties', 'wbi')
+                  '\nProperties with too many statements: '
+                  '\nProperties without enough correct statements: '
+                  '\nRequired properties that are missing: '
+                  '\nIncorrect statements: '
+               names      ('is_valid', 'wikibaseintegrator.wbi_config', 'config', 'WikibaseIntegrator', 'properties_with_too_many_statements_found', 'get_properties_as_a_string_with_labels_and_pid', 'properties_with_too_many_statements', 'properties_without_enough_correct_statements_found', 'properties_without_enough_correct_statements', 'required_properties_that_are_missing', 'incorrect_statements')
+               varnames   ('self', 'string', 'wbi_config', 'wbi', 'properties_string')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__repr__'
-               firstlineno 146
-               lnotab 0x020314010e0104020e011a010e011a010e011a010e011a01
+               firstlineno 162
+               lnotab
+                  0x020614010e0104020c0402fe020102ff04031c010e0118010eff120310
+                  010e0118010c0102fe12040201020102ff04ff06040e0118010eff120310
+                  010e011a01
             None
-         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'missing_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__', '__str__', '__repr__')
+         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'missing_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'lang', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__', 'get_properties_as_a_string_with_labels_and_pid', '__str__', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
          name       'Result'
-         firstlineno 13
+         firstlineno 15
          lnotab
             0x0c011e010e011e011e012a012a012a012a012a010e012a012a012a012a
-            012a02020104ff0e010203020104ff0e010203020104ff0e010203020104
-            ff0e010203020104ff0e01020302010aff0e01020e020104ff0e01020306
-            0d0606060c06060606060706060606060606060603
+            012a010e02020104ff0e010203020104ff0e010203020104ff0e01020302
+            0104ff0e010203020104ff0e01020302010aff0e01020e020104ff0e0102
+            03060d0606060c060606060607060606060606060602010eff080d0603
       'Result'
-   names      ('logging', 'typing', 'Any', 'Dict', 'Set', 'pydantic', 'BaseModel', 'ValidationError', 'entityshape.enums', 'Necessity', 'PropertyResponse', 'StatementResponse', 'entityshape.models.property_value', 'PropertyValue', 'entityshape.models.statement_value', 'StatementValue', 'getLogger', '__name__', 'logger', 'Result')
+   names      ('logging', 'typing', 'Any', 'Dict', 'List', 'Set', 'pydantic', 'BaseModel', 'wikibaseintegrator', 'WikibaseIntegrator', 'entityshape.enums', 'Necessity', 'PropertyResponse', 'StatementResponse', 'entityshape.models.property_value', 'PropertyValue', 'entityshape.models.result_property', 'ResultProperty', 'entityshape.models.statement_value', 'StatementValue', 'getLogger', '__name__', 'logger', 'Result')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108011402100214010c010c022003
+   lnotab 0x00ff0201080118020c010c0214010c010c010c022003
```

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/shape.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/shape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/shape_claim.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/shape_claim.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/__pycache__/statement_value.cpython-311.pyc` & `entityshape-0.1.1/entityshape/models/__pycache__/statement_value.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/compareshape.py` & `entityshape-0.1.1/entityshape/models/compareshape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/entityshape/models/result.py` & `entityshape-0.1.1/entityshape/models/result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
-from typing import Any, Dict, Set
+from typing import Any, Dict, List, Set
 
-from pydantic import BaseModel, ValidationError
+from pydantic import BaseModel
+from wikibaseintegrator import WikibaseIntegrator  # type: ignore
 
 from entityshape.enums import Necessity, PropertyResponse, StatementResponse
 from entityshape.models.property_value import PropertyValue
+from entityshape.models.result_property import ResultProperty
 from entityshape.models.statement_value import StatementValue
 
 logger = logging.getLogger(__name__)
 
 
 class Result(BaseModel):
     general: Dict[Any, Any] = {}
@@ -22,14 +24,15 @@
     properties_with_too_many_statements: Set[str] = set()
     analyzed: bool = False
     required_properties_that_are_missing: Set[str] = set()
     optional_properties_that_are_missing: Set[str] = set()
     properties_without_enough_correct_statements: Set[str] = set()
     properties_that_are_not_allowed: Set[str] = set()
     statements_with_property_that_is_not_allowed: Set[str] = set()
+    lang: str = "en"
 
     @property
     def some_required_properties_are_missing(self):
         return bool(self.required_properties_that_are_missing)
 
     @property
     def properties_with_too_many_statements_found(self):
@@ -136,26 +139,61 @@
 
     def __find_statements_with_property_that_is_not_allowed__(self):
         for statement in self.statements:
             value: StatementValue = self.statements[statement]
             if value.necessity == Necessity.ABSENT:
                 self.statements_with_property_that_is_not_allowed.add(value.property)
 
+    def get_properties_as_a_string_with_labels_and_pid(
+        self, wbi, string_properties: Set[str]
+    ):
+        properties: List[ResultProperty] = []
+        for property_string in string_properties:
+            wbi_property = wbi.property.get(property_string)
+            property_object = ResultProperty(
+                label=wbi_property.labels.get(language=self.lang).value,
+                pid=property_string,
+            )
+            properties.append(property_object)
+        return ", ".join([str(property_) for property_ in properties])
+
     def __str__(self):
-        self.__repr__()
+        return self.__repr__()
 
     def __repr__(self):
         """Return the result of the validation as a formatted string
-        with output exactly describing what caused the validation to fail"""
+        with output exactly describing what caused the validation to fail
+
+        We lookup the labels by default.
+        If no language is set we fall back to English"""
         string = f"Valid: {self.is_valid}"
         if self.is_valid:
             return string
         else:
+            from wikibaseintegrator.wbi_config import config as wbi_config  # type: ignore
+
+            wbi_config[
+                "USER_AGENT"
+            ] = "entityshape (https://github.com/dpriskorn/entityshape)"
+            wbi = WikibaseIntegrator()
             if self.properties_with_too_many_statements_found:
-                string += f"\nproperties_with_too_many_statements: {self.properties_with_too_many_statements}"
+                properties_string = self.get_properties_as_a_string_with_labels_and_pid(
+                    string_properties=self.properties_with_too_many_statements, wbi=wbi
+                )
+                string += f"\nProperties with too many statements: {properties_string}"
             if self.properties_without_enough_correct_statements_found:
-                string += f"\nproperties_without_enough_correct_statements: {self.properties_without_enough_correct_statements}"
+                properties_string = self.get_properties_as_a_string_with_labels_and_pid(
+                    string_properties=self.properties_without_enough_correct_statements,
+                    wbi=wbi,
+                )
+                string += (
+                    f"\nProperties without enough correct statements: "
+                    f"{properties_string}"
+                )
             if self.required_properties_that_are_missing:
-                string += f"\nrequired_properties_that_are_missing: {self.required_properties_that_are_missing}"
+                properties_string = self.get_properties_as_a_string_with_labels_and_pid(
+                    string_properties=self.required_properties_that_are_missing, wbi=wbi
+                )
+                string += f"\nRequired properties that are missing: {properties_string}"
             if self.incorrect_statements:
-                string += f"\nincorrect_statements: {self.incorrect_statements}"
+                string += f"\nIncorrect statements: {self.incorrect_statements}"
             return string
```

### Comparing `entityshape-0.1.0/entityshape/models/shape.py` & `entityshape-0.1.1/entityshape/models/shape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.1.0/pyproject.toml` & `entityshape-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Entityshape"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python library to validate Wikidata items."
 authors = ["Mark Tully aka Teester", "Dennis Priskorn <68460690+dpriskorn@users.noreply.github.com>"]
 license = "GPLv3+"
 readme = "README.md"
 repository = "https://github.com/dpriskorn/entityshape"
 keywords = ["wikidata", "entityschema", "entity validation"]
 classifiers = [
@@ -14,14 +14,15 @@
     { include = "entityshape" },
 ]
 
 [tool.poetry.dependencies]
 pydantic = "^1.10.9"
 python = ">=3.8,<=3.12"
 requests = "^2.28.1"
+wikibaseintegrator = "^0.12.4"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.4.2"
 black = "^22.8.0"
 codespell = "^2.2.1"
 coverage = "^6.5.0"
 dead = "^1.5.0"
```

### Comparing `entityshape-0.1.0/PKG-INFO` & `entityshape-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entityshape
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library to validate Wikidata items.
 Home-page: https://github.com/dpriskorn/entityshape
 License: GPLv3+
 Keywords: wikidata,entityschema,entity validation
 Author: Mark Tully aka Teester
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: wikibaseintegrator (>=0.12.4,<0.13.0)
 Project-URL: Repository, https://github.com/dpriskorn/entityshape
 Description-Content-Type: text/markdown
 
 # [Entityshape](https://www.wikidata.org/wiki/Q119899931)
 A python library to compare a wikidata item with an entityschema
 
 Based on https://github.com/Teester/entityshape by Mark Tully 
@@ -33,14 +34,17 @@
 The shape and compareshape classes currently only support:
 * cardinality (too many or not enough values)
 * whether the property is allowed or not
 * whether the value of a statement on a given property is correct/incorrect
 
 It is still a bit unclear if and how the qualifier validation works.
 
+Only Wikidata is supported currently when fetching labels for the result.
+If you need support for other Wikibase installations, [comment here](https://github.com/dpriskorn/entityshape/issues/15).
+
 # Installation
 Get it from pypi
 
 `$ pip install pyentityshape`
 
 # Usage
 
@@ -50,18 +54,18 @@
 [campsites](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-campsites-in-sweden.ipynb) 
 [shelters](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-shelters-in-sweden.ipynb)
 
 ## CLI
 Example:
 ```
 e = EntityShape(eid="E1", lang="en", qid="Q1")
-result = e.get_result()
+result = e.validate_and_get_result()
 # Get human readable result
 print(result)
-"Valid: False\nproperties_without_enough_correct_statements: {'P31'}"
+"Valid: False\nProperties_without_enough_correct_statements: instance of (P31)"
 # Access the data
 print(result.properties_without_enough_correct_statements)
 "{'P31'}"
 ```
 
 ## Validation
 The is_valid method on the Result object mimics all red warnings displayed by https://www.wikidata.org/wiki/User:Teester/EntityShape.js 
@@ -70,15 +74,15 @@
 1.  properties with too many statements found
 2.   incorrect statements found
 3.   some required properties are missing
 4.   properties without enough correct statements found
 5.   statements with properties that are not allowed found
 
 ## Known working schemas
-This library currently only supports a subset of all features in the ShEx specifikation.
+This library currently only supports a subset of all features in the ShEx specification.
 
 The following Entity Schemas are known to work:
 * [hiking path](https://www.wikidata.org/w/index.php?title=EntitySchema:E375&oldid=1833851062)
 * [shelter](https://www.wikidata.org/w/index.php?title=EntitySchema:E398&oldid=1923235264)
 
 # Background
 This library is the glue between libraries like [Wikibase
```

