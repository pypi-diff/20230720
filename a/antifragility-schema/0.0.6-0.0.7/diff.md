# Comparing `tmp/antifragility-schema-0.0.6.tar.gz` & `tmp/antifragility-schema-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antifragility-schema-0.0.6.tar", last modified: Thu Jul 20 18:42:55 2023, max compression
+gzip compressed data, was "antifragility-schema-0.0.7.tar", last modified: Thu Jul 20 20:10:16 2023, max compression
```

## Comparing `antifragility-schema-0.0.6.tar` & `antifragility-schema-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:42:55.855424 antifragility-schema-0.0.6/
--rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 18:42:55.855195 antifragility-schema-0.0.6/PKG-INFO
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:42:55.853740 antifragility-schema-0.0.6/antifragility_schema/
--rw-r--r--   0 sol        (501) staff       (20)       22 2023-07-20 18:38:25.000000 antifragility-schema-0.0.6/antifragility_schema/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)    11952 2023-07-20 18:39:13.000000 antifragility-schema-0.0.6/antifragility_schema/models.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:42:55.854932 antifragility-schema-0.0.6/antifragility_schema.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 18:42:55.000000 antifragility-schema-0.0.6/antifragility_schema.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      297 2023-07-20 18:42:55.000000 antifragility-schema-0.0.6/antifragility_schema.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:42:55.000000 antifragility-schema-0.0.6/antifragility_schema.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 18:42:55.000000 antifragility-schema-0.0.6/antifragility_schema.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:42:55.000000 antifragility-schema-0.0.6/antifragility_schema.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      414 2023-07-20 18:38:25.000000 antifragility-schema-0.0.6/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:42:55.855483 antifragility-schema-0.0.6/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.507386 antifragility-schema-0.0.7/
+-rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:10:16.507078 antifragility-schema-0.0.7/PKG-INFO
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.504586 antifragility-schema-0.0.7/antifragility_schema/
+-rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-20 20:07:41.000000 antifragility-schema-0.0.7/antifragility_schema/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)    11977 2023-07-20 20:05:17.000000 antifragility-schema-0.0.7/antifragility_schema/models.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.506802 antifragility-schema-0.0.7/antifragility_schema.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      297 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      410 2023-07-20 20:08:57.000000 antifragility-schema-0.0.7/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 20:10:16.507511 antifragility-schema-0.0.7/setup.cfg
```

### Comparing `antifragility-schema-0.0.6/antifragility_schema/models.py` & `antifragility-schema-0.0.7/antifragility_schema/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         table_description = "Payment methods - Currencies"
         unique_together = (("pt", "cur"),)
 
 
 class Fiat(Model):
     id: int = fields.IntField(pk=True)
     ptc: fields.ForeignKeyRelation[Ptc] = fields.ForeignKeyField("models.Ptc")
-    pts: fields.ManyToManyRelation[Pt] = fields.ManyToManyField("models.Pt", through="ptc")
+    # pts: fields.ManyToManyRelation[Pt] = fields.ManyToManyField("models.Pt", through="ptc") # no ptc.fiat_id field
     country: fields.ForeignKeyRelation[Country] = fields.ForeignKeyField("models.Country", related_name="fiats")
     detail: str = fields.CharField(127)
     user: fields.ForeignKeyRelation[User] = fields.ForeignKeyField("models.User", "fiats")  # only user having client
     amount: float = fields.FloatField(default=None, null=True)
     target: float = fields.FloatField(default=None, null=True)
 
     orders: fields.ReverseRelation["Order"]
```

