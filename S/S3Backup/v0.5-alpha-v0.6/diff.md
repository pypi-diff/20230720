# Comparing `tmp/S3Backup-v0.5-alpha.zip` & `tmp/S3Backup-v0.6.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 16588 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat       67 b- defN 15-Jun-29 21:09 S3Backup-v0.5-alpha/AUTHORS
--rw-rw-rw-  2.0 fat     1105 b- defN 15-Jun-20 11:12 S3Backup-v0.5-alpha/LICENSE
--rw-rw-rw-  2.0 fat       95 b- defN 15-Jun-30 18:31 S3Backup-v0.5-alpha/MANIFEST.in
--rw-rw-rw-  2.0 fat     5571 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/PKG-INFO
--rw-rw-rw-  2.0 fat     4138 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/README.rst
--rw-rw-rw-  2.0 fat       13 b- defN 15-Jun-30 18:31 S3Backup-v0.5-alpha/requirements.txt
--rw-rw-rw-  2.0 fat       64 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/setup.cfg
--rw-rw-rw-  2.0 fat     1510 b- defN 15-Jun-30 18:31 S3Backup-v0.5-alpha/setup.py
--rw-rw-rw-  2.0 fat       25 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/version.py
--rw-rw-rw-  2.0 fat     2551 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup/config_loader.py
--rw-rw-rw-  2.0 fat     1984 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup/hash_file.py
--rw-rw-rw-  2.0 fat     6673 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup/plan.py
--rw-rw-rw-  2.0 fat     4188 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat     5571 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       11 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/requires.txt
--rw-rw-rw-  2.0 fat      351 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 15-Jun-30 19:53 S3Backup-v0.5-alpha/S3Backup.egg-info/top_level.txt
-19 files, 33929 bytes uncompressed, 13658 bytes compressed:  59.7%
+Zip file size: 16758 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat       67 b- defN 15-Jun-30 09:00 S3Backup-v0.6/AUTHORS
+-rw-rw-rw-  2.0 fat     1105 b- defN 15-Jun-19 16:08 S3Backup-v0.6/LICENSE
+-rw-rw-rw-  2.0 fat       95 b- defN 15-Jun-30 15:11 S3Backup-v0.6/MANIFEST.in
+-rw-rw-rw-  2.0 fat     5908 b- defN 15-Jul-07 10:28 S3Backup-v0.6/PKG-INFO
+-rw-rw-rw-  2.0 fat     4449 b- defN 15-Jul-02 16:44 S3Backup-v0.6/README.rst
+-rw-rw-rw-  2.0 fat       13 b- defN 15-Jun-30 16:28 S3Backup-v0.6/requirements.txt
+-rw-rw-rw-  2.0 fat       64 b- defN 15-Jul-07 10:28 S3Backup-v0.6/setup.cfg
+-rw-rw-rw-  2.0 fat     1510 b- defN 15-Jun-30 15:10 S3Backup-v0.6/setup.py
+-rw-rw-rw-  2.0 fat       19 b- defN 15-Jul-07 10:28 S3Backup-v0.6/version.py
+-rw-rw-rw-  2.0 fat     2551 b- defN 15-Jul-02 16:28 S3Backup-v0.6/S3Backup/config_loader.py
+-rw-rw-rw-  2.0 fat     1984 b- defN 15-Jul-02 16:28 S3Backup-v0.6/S3Backup/hash_file.py
+-rw-rw-rw-  2.0 fat     6673 b- defN 15-Jul-02 16:28 S3Backup-v0.6/S3Backup/plan.py
+-rw-rw-rw-  2.0 fat     4188 b- defN 15-Jul-02 16:28 S3Backup-v0.6/S3Backup/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 15-Jul-07 10:28 S3Backup-v0.6/S3Backup.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 15-Jun-30 14:32 S3Backup-v0.6/S3Backup.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat     5908 b- defN 15-Jul-07 10:28 S3Backup-v0.6/S3Backup.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       11 b- defN 15-Jul-07 10:28 S3Backup-v0.6/S3Backup.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat      351 b- defN 15-Jul-07 10:28 S3Backup-v0.6/S3Backup.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 15-Jul-07 10:28 S3Backup-v0.6/S3Backup.egg-info/top_level.txt
+19 files, 34908 bytes uncompressed, 14056 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,58 +1,58 @@
-Filename: S3Backup-v0.5-alpha/AUTHORS
+Filename: S3Backup-v0.6/AUTHORS
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/LICENSE
+Filename: S3Backup-v0.6/LICENSE
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/MANIFEST.in
+Filename: S3Backup-v0.6/MANIFEST.in
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/PKG-INFO
+Filename: S3Backup-v0.6/PKG-INFO
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/README.rst
+Filename: S3Backup-v0.6/README.rst
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/requirements.txt
+Filename: S3Backup-v0.6/requirements.txt
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/setup.cfg
+Filename: S3Backup-v0.6/setup.cfg
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/setup.py
+Filename: S3Backup-v0.6/setup.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/version.py
+Filename: S3Backup-v0.6/version.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup/config_loader.py
+Filename: S3Backup-v0.6/S3Backup/config_loader.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup/hash_file.py
+Filename: S3Backup-v0.6/S3Backup/hash_file.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup/plan.py
+Filename: S3Backup-v0.6/S3Backup/plan.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup/__init__.py
+Filename: S3Backup-v0.6/S3Backup/__init__.py
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/dependency_links.txt
+Filename: S3Backup-v0.6/S3Backup.egg-info/dependency_links.txt
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/not-zip-safe
+Filename: S3Backup-v0.6/S3Backup.egg-info/not-zip-safe
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/PKG-INFO
+Filename: S3Backup-v0.6/S3Backup.egg-info/PKG-INFO
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/requires.txt
+Filename: S3Backup-v0.6/S3Backup.egg-info/requires.txt
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/SOURCES.txt
+Filename: S3Backup-v0.6/S3Backup.egg-info/SOURCES.txt
 Comment: 
 
-Filename: S3Backup-v0.5-alpha/S3Backup.egg-info/top_level.txt
+Filename: S3Backup-v0.6/S3Backup.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `S3Backup-v0.5-alpha/LICENSE` & `S3Backup-v0.6/LICENSE`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/PKG-INFO` & `S3Backup-v0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: S3Backup
-Version: v0.5-alpha
+Version: v0.6
 Summary: Perform scripted backups to Amazon S3
 Home-page: https://github.com/mgoodfellow/s3-backup
 Author: Mike Goodfellow
 Author-email: mdgoodfellow@gmail.com
 License: MIT
 Description: S3Backup
         ========
@@ -19,15 +19,15 @@
         
         Features
         --------
         
         It supports the following features:
         
         -  Plan based backups
-        -  Custom command run pre-backup
+        -  Custom command run pre-backup (can be used to perform complex pre-backup preparation tasks)
         -  Storing to S3
         -  Calculating MD5 hashes of the backup set to avoid uploading duplicate backup sets
         -  Emailing the result of the backup plans
         -  Python standard logging framework
         
         Installation
         ------------
@@ -40,15 +40,15 @@
         
         Dependencies
         ------------
         
         S3Backup depends on:
         
         - boto (AWS SDK)
-        - glob2 (Better file globbing)
+        - `glob2 <http://github.com/miracle2k/python-glob2/>`_ (Better file globbing)
         
         Both can be installed via pip, however, if S3Backup is installed via pip then these dependencies will already be met.
         
         Configuration
         -------------
         
         The backup utility is configured through the use of a JSON configuration
@@ -63,34 +63,37 @@
               "AWS_REGION": "this is a region",
               "EMAIL_FROM": "source@address.com",
               "EMAIL_TO": "recipient@address.com",
               "HASH_CHECK_FILE": "plan_hashes.txt",
               "Plans": [
                 {
                   "Name": "MySQL Backup",
-                  "Command": "mysqldump -u bob -p password > mysql_backup.sql",
-                  "Src": "c:/mysql_backup.sql",
+                  "Command": "/home/bob/backups/backup-prep-script.sh",
+                  "Src": "/home/bob/backups/database/mysql_backup.sql",
                   "OutputPrefix": "main_db"
                 },
                 {
-                  "Name": "Website Backup",
-                  "Src": ["c:/website/*.html", "C:/website/src/**/*"],
-                  "OutputPrefix": "website"
+                  "Name": "Websites Backup",
+                  "Src": ["/var/www/html/website/**/*", "/var/www/html/website2/**/*"],
+                  "OutputPrefix": "websites_backup"
                 }
               ]
             }
         
         If emails are not required, then omit the ``EMAIL_FROM`` and
         ``EMAIL_TO`` fields of the configuration file.
         
         *Note*: When on Windows, it is better to pass the paths using forward
         slashes (/) as then escaping isn’t required (as with backslashes). The
         script will normalize the paths in these cases. However, when providing
         the command, if paths are required they will need to be double escaped.
         
+        There are more examples (including Windows examples) and further discussion
+        on `this blog post <https://mikegoodfellow.co.uk/s3-backup-utility/>`_
+        
         Usage
         -----
         
         You will need to set up an AWS account if you do not have one, and then
         obtain AWS keys for an IAM account which has the following privileges:
         
         -  S3 full access (for writing to the storage bucket)
@@ -142,12 +145,13 @@
         referred to for further information.
         
         Future Improvements
         -------------------
         
         These are some of the planned future improvements:
         
-        -  Run multiple pre-backup commands (by providing an array)
         -  Allow custom format strings for the output files (instead of the default date/time format)
         -  Modification of the glob2 library to allow hidden files to be included
+        -  Allow exclude globs to be added when providing source directory
+        
 Keywords: backup,aws,s3
 Platform: UNKNOWN
```

## Comparing `S3Backup-v0.5-alpha/README.rst` & `S3Backup-v0.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Features
 --------
 
 It supports the following features:
 
 -  Plan based backups
--  Custom command run pre-backup
+-  Custom command run pre-backup (can be used to perform complex pre-backup preparation tasks)
 -  Storing to S3
 -  Calculating MD5 hashes of the backup set to avoid uploading duplicate backup sets
 -  Emailing the result of the backup plans
 -  Python standard logging framework
 
 Installation
 ------------
@@ -32,15 +32,15 @@
 
 Dependencies
 ------------
 
 S3Backup depends on:
 
 - boto (AWS SDK)
-- glob2 (Better file globbing)
+- `glob2 <http://github.com/miracle2k/python-glob2/>`_ (Better file globbing)
 
 Both can be installed via pip, however, if S3Backup is installed via pip then these dependencies will already be met.
 
 Configuration
 -------------
 
 The backup utility is configured through the use of a JSON configuration
@@ -55,34 +55,37 @@
       "AWS_REGION": "this is a region",
       "EMAIL_FROM": "source@address.com",
       "EMAIL_TO": "recipient@address.com",
       "HASH_CHECK_FILE": "plan_hashes.txt",
       "Plans": [
         {
           "Name": "MySQL Backup",
-          "Command": "mysqldump -u bob -p password > mysql_backup.sql",
-          "Src": "c:/mysql_backup.sql",
+          "Command": "/home/bob/backups/backup-prep-script.sh",
+          "Src": "/home/bob/backups/database/mysql_backup.sql",
           "OutputPrefix": "main_db"
         },
         {
-          "Name": "Website Backup",
-          "Src": ["c:/website/*.html", "C:/website/src/**/*"],
-          "OutputPrefix": "website"
+          "Name": "Websites Backup",
+          "Src": ["/var/www/html/website/**/*", "/var/www/html/website2/**/*"],
+          "OutputPrefix": "websites_backup"
         }
       ]
     }
 
 If emails are not required, then omit the ``EMAIL_FROM`` and
 ``EMAIL_TO`` fields of the configuration file.
 
 *Note*: When on Windows, it is better to pass the paths using forward
 slashes (/) as then escaping isn’t required (as with backslashes). The
 script will normalize the paths in these cases. However, when providing
 the command, if paths are required they will need to be double escaped.
 
+There are more examples (including Windows examples) and further discussion
+on `this blog post <https://mikegoodfellow.co.uk/s3-backup-utility/>`_
+
 Usage
 -----
 
 You will need to set up an AWS account if you do not have one, and then
 obtain AWS keys for an IAM account which has the following privileges:
 
 -  S3 full access (for writing to the storage bucket)
@@ -134,10 +137,10 @@
 referred to for further information.
 
 Future Improvements
 -------------------
 
 These are some of the planned future improvements:
 
--  Run multiple pre-backup commands (by providing an array)
 -  Allow custom format strings for the output files (instead of the default date/time format)
--  Modification of the glob2 library to allow hidden files to be included
+-  Modification of the glob2 library to allow hidden files to be included
+-  Allow exclude globs to be added when providing source directory
```

## Comparing `S3Backup-v0.5-alpha/setup.py` & `S3Backup-v0.6/setup.py`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/S3Backup/config_loader.py` & `S3Backup-v0.6/S3Backup/config_loader.py`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/S3Backup/hash_file.py` & `S3Backup-v0.6/S3Backup/hash_file.py`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/S3Backup/plan.py` & `S3Backup-v0.6/S3Backup/plan.py`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/S3Backup/__init__.py` & `S3Backup-v0.6/S3Backup/__init__.py`

 * *Files identical despite different names*

## Comparing `S3Backup-v0.5-alpha/S3Backup.egg-info/PKG-INFO` & `S3Backup-v0.6/S3Backup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: S3Backup
-Version: v0.5-alpha
+Version: v0.6
 Summary: Perform scripted backups to Amazon S3
 Home-page: https://github.com/mgoodfellow/s3-backup
 Author: Mike Goodfellow
 Author-email: mdgoodfellow@gmail.com
 License: MIT
 Description: S3Backup
         ========
@@ -19,15 +19,15 @@
         
         Features
         --------
         
         It supports the following features:
         
         -  Plan based backups
-        -  Custom command run pre-backup
+        -  Custom command run pre-backup (can be used to perform complex pre-backup preparation tasks)
         -  Storing to S3
         -  Calculating MD5 hashes of the backup set to avoid uploading duplicate backup sets
         -  Emailing the result of the backup plans
         -  Python standard logging framework
         
         Installation
         ------------
@@ -40,15 +40,15 @@
         
         Dependencies
         ------------
         
         S3Backup depends on:
         
         - boto (AWS SDK)
-        - glob2 (Better file globbing)
+        - `glob2 <http://github.com/miracle2k/python-glob2/>`_ (Better file globbing)
         
         Both can be installed via pip, however, if S3Backup is installed via pip then these dependencies will already be met.
         
         Configuration
         -------------
         
         The backup utility is configured through the use of a JSON configuration
@@ -63,34 +63,37 @@
               "AWS_REGION": "this is a region",
               "EMAIL_FROM": "source@address.com",
               "EMAIL_TO": "recipient@address.com",
               "HASH_CHECK_FILE": "plan_hashes.txt",
               "Plans": [
                 {
                   "Name": "MySQL Backup",
-                  "Command": "mysqldump -u bob -p password > mysql_backup.sql",
-                  "Src": "c:/mysql_backup.sql",
+                  "Command": "/home/bob/backups/backup-prep-script.sh",
+                  "Src": "/home/bob/backups/database/mysql_backup.sql",
                   "OutputPrefix": "main_db"
                 },
                 {
-                  "Name": "Website Backup",
-                  "Src": ["c:/website/*.html", "C:/website/src/**/*"],
-                  "OutputPrefix": "website"
+                  "Name": "Websites Backup",
+                  "Src": ["/var/www/html/website/**/*", "/var/www/html/website2/**/*"],
+                  "OutputPrefix": "websites_backup"
                 }
               ]
             }
         
         If emails are not required, then omit the ``EMAIL_FROM`` and
         ``EMAIL_TO`` fields of the configuration file.
         
         *Note*: When on Windows, it is better to pass the paths using forward
         slashes (/) as then escaping isn’t required (as with backslashes). The
         script will normalize the paths in these cases. However, when providing
         the command, if paths are required they will need to be double escaped.
         
+        There are more examples (including Windows examples) and further discussion
+        on `this blog post <https://mikegoodfellow.co.uk/s3-backup-utility/>`_
+        
         Usage
         -----
         
         You will need to set up an AWS account if you do not have one, and then
         obtain AWS keys for an IAM account which has the following privileges:
         
         -  S3 full access (for writing to the storage bucket)
@@ -142,12 +145,13 @@
         referred to for further information.
         
         Future Improvements
         -------------------
         
         These are some of the planned future improvements:
         
-        -  Run multiple pre-backup commands (by providing an array)
         -  Allow custom format strings for the output files (instead of the default date/time format)
         -  Modification of the glob2 library to allow hidden files to be included
+        -  Allow exclude globs to be added when providing source directory
+        
 Keywords: backup,aws,s3
 Platform: UNKNOWN
```

