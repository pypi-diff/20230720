# Comparing `tmp/data_job_etl-1.1.3-py3-none-any.whl.zip` & `tmp/data_job_etl-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,27 @@
-Zip file size: 213341 bytes, number of entries: 26
+Zip file size: 180481 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/.ipynb_checkpoints/rank-checkpoint.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/__init__.py
--rw-r--r--  2.0 unx    75536 b- defN 80-Jan-01 00:00 data_job_etl/analysis.ipynb
--rw-r--r--  2.0 unx     3487 b- defN 80-Jan-01 00:00 data_job_etl/build_technos.py
+-rw-r--r--  2.0 unx     3432 b- defN 80-Jan-01 00:00 data_job_etl/build_technos.py
 -rw-r--r--  2.0 unx      371 b- defN 80-Jan-01 00:00 data_job_etl/config/definitions.py
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 data_job_etl/config/etl_logger.py
 -rw-r--r--  2.0 unx     2300 b- defN 80-Jan-01 00:00 data_job_etl/config/postgres_schema.py
 -rw-r--r--  2.0 unx      518 b- defN 80-Jan-01 00:00 data_job_etl/credentials.json
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/data/__init__.py
 -rw-r--r--  2.0 unx   799758 b- defN 80-Jan-01 00:00 data_job_etl/data/mad2023.json
--rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 data_job_etl/etl.py
--rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 data_job_etl/extract/extract.py
+-rw-r--r--  2.0 unx     1298 b- defN 80-Jan-01 00:00 data_job_etl/etl.py
+-rw-r--r--  2.0 unx      405 b- defN 80-Jan-01 00:00 data_job_etl/extract/extract.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/file.log
 -rw-r--r--  2.0 unx      380 b- defN 80-Jan-01 00:00 data_job_etl/load/create_tables.py
--rw-r--r--  2.0 unx     4661 b- defN 80-Jan-01 00:00 data_job_etl/load/load.py
--rw-r--r--  2.0 unx     5979 b- defN 80-Jan-01 00:00 data_job_etl/message.py
+-rw-r--r--  2.0 unx     4635 b- defN 80-Jan-01 00:00 data_job_etl/load/load.py
+-rw-r--r--  2.0 unx     5981 b- defN 80-Jan-01 00:00 data_job_etl/message.py
 -rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/rank.py
 -rw-r--r--  2.0 unx     8076 b- defN 80-Jan-01 00:00 data_job_etl/recommendation_system.py
 -rw-r--r--  2.0 unx     2547 b- defN 80-Jan-01 00:00 data_job_etl/summarise.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/transform/file.log
--rw-r--r--  2.0 unx     1991 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
--rw-r--r--  2.0 unx     2254 b- defN 80-Jan-01 00:00 data_job_etl/transform/process.py
--rw-r--r--  2.0 unx     1674 b- defN 80-Jan-01 00:00 data_job_etl/update_table.py
--rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 data_job_etl-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2203 b- defN 16-Jan-01 00:00 data_job_etl-1.1.3.dist-info/RECORD
-26 files, 923515 bytes uncompressed, 209759 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx     2019 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
+-rw-r--r--  2.0 unx     2241 b- defN 80-Jan-01 00:00 data_job_etl/transform/process.py
+-rw-r--r--  2.0 unx     1641 b- defN 80-Jan-01 00:00 data_job_etl/update_table.py
+-rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 data_job_etl-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2118 b- defN 16-Jan-01 00:00 data_job_etl-1.1.4.dist-info/RECORD
+25 files, 847719 bytes uncompressed, 177029 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,16 +1,13 @@
 Filename: data_job_etl/.ipynb_checkpoints/rank-checkpoint.py
 Comment: 
 
 Filename: data_job_etl/__init__.py
 Comment: 
 
-Filename: data_job_etl/analysis.ipynb
-Comment: 
-
 Filename: data_job_etl/build_technos.py
 Comment: 
 
 Filename: data_job_etl/config/definitions.py
 Comment: 
 
 Filename: data_job_etl/config/etl_logger.py
@@ -63,17 +60,17 @@
 
 Filename: data_job_etl/transform/process.py
 Comment: 
 
 Filename: data_job_etl/update_table.py
 Comment: 
 
-Filename: data_job_etl-1.1.3.dist-info/METADATA
+Filename: data_job_etl-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: data_job_etl-1.1.3.dist-info/WHEEL
+Filename: data_job_etl-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: data_job_etl-1.1.3.dist-info/RECORD
+Filename: data_job_etl-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_job_etl/build_technos.py

```diff
@@ -1,14 +1,14 @@
 import json
 
 
 class TechnoBuilder:
     
     def build_all_technos(self):
-        with open('/Users/donor/PycharmProjects/data-job-etl/data_job_etl/data/mad2023.json', 'r') as f:
+        with open('data/mad2023.json', 'r') as f:
             mad = json.load(f)
         
         mad_technos = [x['name'] for x in mad]
         other_technos = {'DataBuildTool', 'MxNet', 'Hadoop', 'Beam', 'BigQuery', 'Pig', 'DataStudio', 'Redshift', 'Shell',
                          'Gitlab', 'data vault', 'Ceph', 'Airflow', 'GCP', 'IAM', 'k8s', 'Numpy', 'MAPR', 'Node', 'Athena',
                          'Unix', 'NiFi', 'Mongo', 'NoSQL', 'Unix Shell', 'Azure', 'Go', 'Golang', 'Perl', 'EC2', 'EMR', 'SPAR',
                          'Jenkins', 'Git', 'C/C\\+\\+', 'airflow', 'CloudSQL', 'Ruby', 'Redshift Spectrum', 'Glue', 'Postgres',
```

## data_job_etl/etl.py

```diff
@@ -1,25 +1,25 @@
 import logging
-from data_job_etl.config.etl_logger import logger
+from config.etl_logger import logger
 
-from data_job_etl.extract.extract import Extractor
-from data_job_etl.transform.preprocess import Preprocessor
-from data_job_etl.transform.process import Processor
-from data_job_etl.load.load import Loader
+from extract.extract import Extractor
+from transform.preprocess import Preprocessor
+from transform.process import Processor
+from load.load import Loader
 
 
 def extract():
     extractor = Extractor()
     new_raw_query = """
         SELECT *
         FROM raw_jobs
         WHERE created_at = (
             SELECT created_at
             FROM raw_jobs
-            ORDER BY created_at DESC limit 1);
+            ORDER BY created_at DESC limit 5);
     """
     new_raw_jobs = extractor.extract_query(new_raw_query)
     return new_raw_jobs
 
 
 def transform(raw_jobs):
     preprocessor = Preprocessor(raw_jobs)
```

## data_job_etl/extract/extract.py

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy import create_engine
 import pandas as pd
 
-from data_job_etl.config.definitions import DB_STRING
+from config.definitions import DB_STRING
 
 
 class Extractor:
 
     def __init__(self):
         self.engine = create_engine(DB_STRING)
```

## data_job_etl/load/load.py

```diff
@@ -1,15 +1,15 @@
 import numpy
 from psycopg2.extensions import register_adapter, AsIs
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.orm import Session, sessionmaker
 from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 
-from data_job_etl.config.definitions import DB_STRING
-from data_job_etl.config.postgres_schema import PivottedJob, ProcessedJob, Base
+from config.definitions import DB_STRING
+from config.postgres_schema import PivottedJob, ProcessedJob, Base
 
 
 def adapt_numpy_float64(numpy_float64):
     return AsIs(numpy_float64)
 
 
 def adapt_numpy_int64(numpy_int64):
```

## data_job_etl/message.py

```diff
@@ -48,15 +48,15 @@
             ORDER BY created_at DESC limit 1;
         """
         last_scraped_date = self.extractor.extract_query(last_scraped_date_query)
         self.last_scraped_date = last_scraped_date.loc[0, 'created_at']
         query = f"""
             SELECT * FROM relevant
             WHERE created_at = '2023-05-03'
-            ORDER BY rank DESC;
+            ORDER BY rating DESC;
         """
         recent_ranked_jobs = self.extractor.extract_query(query)
         return recent_ranked_jobs
 
     def format_simple_message(self, jobs):
         text = "Hi, here are new jobs for you."
```

## data_job_etl/transform/preprocess.py

```diff
@@ -49,18 +49,17 @@
         text = text.replace(u'\xa0', u' ')  # \xa0 (non-breaking space in Latin1 ISO 8859-1)
         text = re.sub(r'\s\s\s+', ' ', text)
         text = re.sub(r'\s\s+', ' ', text)
         return text.strip()
 
     @staticmethod
     def process_remote(original):
+        if pd.isna(original):
+            return None
         if 'partiel' in original:
             return 'partiel'
         elif 'ponctuel' in original:
             return 'ponctuel'
         elif 'total' in original:
             return 'total'
         else:
             return original
-
-
-print(dir(Preprocessor))
```

## data_job_etl/transform/process.py

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import re
 
-from data_job_etl.build_technos import TechnoBuilder
+from build_technos import TechnoBuilder
 
 
 class Processor:
 
     def process_technos(self, jobs):
         """
         Add columns to a dataframe with technology names from a text.
```

## data_job_etl/update_table.py

```diff
@@ -10,15 +10,14 @@
     """
     Modify table once outside the automated workflow.
     """
 
     def __init__(self):
         self.extractor = Extractor()
         self.loader = Loader()
-        print(dir(Preprocessor))
 
     def extract_processed_jobs(self):
         return self.extractor.extract_table('processed_jobs')
 
     def update_remote(self):
         """Modification of remote field in processed_jobs table."""
         processed_jobs = self.extract_processed_jobs()
```

## Comparing `data_job_etl-1.1.3.dist-info/RECORD` & `data_job_etl-1.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 data_job_etl/.ipynb_checkpoints/rank-checkpoint.py,sha256=opyH6EnTLpLUs-166yN71uiCu4Yklp4yzGJb5_MiNUI,4480
 data_job_etl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-data_job_etl/analysis.ipynb,sha256=70AjHmGw0SkS-6cyvsw3uVY6s0ZqNvKTMb1Nh3NVMzU,75536
-data_job_etl/build_technos.py,sha256=kfIvA3c1_nzuYj6ssb68TwnrgRYI4FVXvOGLZi-_93s,3487
+data_job_etl/build_technos.py,sha256=VGinvVfuz_1xqIMn1FjWeQsDCyHSvMDsCq7LFKD1exA,3432
 data_job_etl/config/definitions.py,sha256=1ZrAqDFV2uvn4FtYlem2hQYx14v_4EJMVuCYUG3f52w,371
 data_job_etl/config/etl_logger.py,sha256=1BE7eKhdw37uAxSWDu0IJYmDJhY8lZ2iwjzJ0hNZ8_4,486
 data_job_etl/config/postgres_schema.py,sha256=IiBBuLrwSsGrZq7o4joFfmTuUAm4TGFW612sCKOHAIk,2300
 data_job_etl/credentials.json,sha256=l9Os9iRXhIFYA5dyN3hIwwLXw50HhrrSFHaApx1PaxI,518
 data_job_etl/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_job_etl/data/mad2023.json,sha256=xEOg0W-CB2XswC-gp1dX4y6_hls-HiAXgRTSOfttU_A,799758
-data_job_etl/etl.py,sha256=XLATUe1psRm9j3fWYBxL0-jwC7eOOvcIY-B04T2qCCo,1363
-data_job_etl/extract/extract.py,sha256=KZ2Vtye9N6xzLzAOxx-DeljrWobCvLHF4bSqDYtA_Cs,418
+data_job_etl/etl.py,sha256=_QBYfYGUr08ey3sheJw2CWnxh5ZXAogbs8HVj-zTumk,1298
+data_job_etl/extract/extract.py,sha256=DsBeX-beEidyhnSRNUC8hYXSX1B2XCoOhhrVOd3OvE8,405
 data_job_etl/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_job_etl/load/create_tables.py,sha256=InZHxc-rU0W-1mLmgU9Ul7b5w7CkSI4aoW84tQNx-OU,380
-data_job_etl/load/load.py,sha256=CzogYxoKwlh4TX0sYa1i-oVciMl-q2OWCyPmi0EGG98,4661
-data_job_etl/message.py,sha256=8nHJ7Lrh7IHZ0sPZ5Ge6TNP4pJIheOrJz8F9bxUq4_Y,5979
+data_job_etl/load/load.py,sha256=HVAyEfoyHsOBOvZo5PdiR5UO_0WsvKXpm7jMfebu6tM,4635
+data_job_etl/message.py,sha256=88ZSORYHH1nz3UlqLwOWI29aen6KWqssp6y05a8e6fk,5981
 data_job_etl/rank.py,sha256=opyH6EnTLpLUs-166yN71uiCu4Yklp4yzGJb5_MiNUI,4480
 data_job_etl/recommendation_system.py,sha256=QvF-hJMHk5dv-4yRhpMO0STcQnhRB3VIqTUO_Uivvw0,8076
 data_job_etl/summarise.py,sha256=-CwLg-gTooiRHwCFBlLytwRuM9T1wqwWCq4P7ZQ9_Ok,2547
 data_job_etl/transform/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-data_job_etl/transform/preprocess.py,sha256=xzGV7Lg0cWW8hDCZcQbYCiOKvN1O2zSEOKeZzSiKRyc,1991
-data_job_etl/transform/process.py,sha256=xgL0CWAVwJN4kSECexOI4odt7HWWyk90943Uzcv8B7I,2254
-data_job_etl/update_table.py,sha256=Hg1zcM3PjgMvxKSkqjb-8Anw50rta9Y43fKg41xri0o,1674
-data_job_etl-1.1.3.dist-info/METADATA,sha256=7glyf6qE7AfiUFGOjghTvHKZzWt6iaoxFaO_hWDxFqA,465
-data_job_etl-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-data_job_etl-1.1.3.dist-info/RECORD,,
+data_job_etl/transform/preprocess.py,sha256=NEzA5i2_qhXUci4hOBZSwUWWhmnAqrxtt38veTrqB3g,2019
+data_job_etl/transform/process.py,sha256=KTD8_i3Z5nFEIjCrp-zQp4iRsqFYH_omGt1XVoX_VMg,2241
+data_job_etl/update_table.py,sha256=9maWu5wjwXFseMbs5B6yfS6_CygBRW7DzJtKzo_jSIA,1641
+data_job_etl-1.1.4.dist-info/METADATA,sha256=PpMN1HkpGTIwCkepQXJrd45T4X9c4-ThXv6owpdqXng,465
+data_job_etl-1.1.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+data_job_etl-1.1.4.dist-info/RECORD,,
```

