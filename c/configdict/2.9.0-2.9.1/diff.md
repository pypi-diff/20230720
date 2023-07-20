# Comparing `tmp/configdict-2.9.0-py3-none-any.whl.zip` & `tmp/configdict-2.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 32712 bytes, number of entries: 9
+Zip file size: 32735 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    68241 b- defN 23-Jul-19 12:27 configdict/configdict.py
+-rw-rw-r--  2.0 unx    68311 b- defN 23-Jul-20 18:35 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-19 12:30 configdict-2.9.0.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-19 12:30 configdict-2.9.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-19 12:30 configdict-2.9.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-19 12:30 configdict-2.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-19 12:30 configdict-2.9.0.dist-info/RECORD
-9 files, 96753 bytes uncompressed, 31426 bytes compressed:  67.5%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-20 19:01 configdict-2.9.1.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-20 19:01 configdict-2.9.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 19:01 configdict-2.9.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-20 19:01 configdict-2.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-20 19:01 configdict-2.9.1.dist-info/RECORD
+9 files, 96823 bytes uncompressed, 31449 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.9.0.dist-info/LICENSE.md
+Filename: configdict-2.9.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.9.0.dist-info/METADATA
+Filename: configdict-2.9.1.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.9.0.dist-info/WHEEL
+Filename: configdict-2.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.9.0.dist-info/top_level.txt
+Filename: configdict-2.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.9.0.dist-info/RECORD
+Filename: configdict-2.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -572,14 +572,15 @@
         if self.default:
             if autoload:
                 self.load()
             if not strict:
                 self._normalizedKeys = {normalizeKey(k): k for k in self.default.keys()}
 
         self.readonly = readonly
+        self._strict = strict
 
     def __hash__(self) -> int:
         keyshash = hash(tuple(self.keys()))
         try:
             valueshash = hash(tuple(self.values()))
         except:
             logger.debug(f"Some values are unhashable, using unsafe hash ({self.values()}")
@@ -1323,14 +1324,15 @@
         self.fmt = fmt
         super().__init__(default=default,
                          validator=validator,
                          docs=docs,
                          callback=self._mycallback,
                          precallback=precallback,
                          autoload=False,
+                         strict=strict,
                          advancedPrefix=advancedPrefix)
         self.sortKeys = sortKeys
 
         if default is not None:
             self._updateWithDefault()
             if load:
                 self.load()
```

## Comparing `configdict-2.9.0.dist-info/LICENSE.md` & `configdict-2.9.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.9.0.dist-info/METADATA` & `configdict-2.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.9.0
+Version: 2.9.1
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

## Comparing `configdict-2.9.0.dist-info/RECORD` & `configdict-2.9.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 configdict/__init__.py,sha256=CI6gyI6isoSmOxiaMKQ1zJMLWzFYn6bOTnUcJtMAMRQ,25
-configdict/configdict.py,sha256=OTkAeM8ai_5-D2ZCA7BO-mLTjmzK2M-oK4AvfnNua8Y,68241
+configdict/configdict.py,sha256=4eT1H_E8hzQTCaZ3CB-YtesYswlV2wKuadxC2etcE0Y,68311
 configdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 configdict/__pycache__/configdict.cpython-38.pyc,sha256=pmenTOMg3mEukCVKrOf7lNx1TTPjNga5bTXY_VRnSFU,22699
-configdict-2.9.0.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
-configdict-2.9.0.dist-info/METADATA,sha256=cbapm3VUBwX87DO6Io3kZGYH17J7FF1h1DPWr610Ztw,3883
-configdict-2.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-configdict-2.9.0.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
-configdict-2.9.0.dist-info/RECORD,,
+configdict-2.9.1.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
+configdict-2.9.1.dist-info/METADATA,sha256=ffpU4_mFwC3A6Vuqz5x1L3D0MAY0vT2EW90q_3R1GCE,3883
+configdict-2.9.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+configdict-2.9.1.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
+configdict-2.9.1.dist-info/RECORD,,
```

