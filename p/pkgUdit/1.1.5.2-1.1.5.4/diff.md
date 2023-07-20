# Comparing `tmp/pkgUdit-1.1.5.2-py3-none-any.whl.zip` & `tmp/pkgUdit-1.1.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5746 bytes, number of entries: 13
+Zip file size: 6124 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 16:29 pkgUdit/Names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 16:29 pkgUdit/Places.csv
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-20 18:53 pkgUdit/__init__.py
 -rw-rw-rw-  2.0 fat     2874 b- defN 23-Jul-18 16:39 pkgUdit/d.py
--rw-rw-rw-  2.0 fat     2610 b- defN 23-Jul-20 18:41 pkgUdit/pswdGen.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Jul-20 07:12 pkgUdit/test.py
+-rw-rw-rw-  2.0 fat     2610 b- defN 23-Jul-20 19:47 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat     2319 b- defN 23-Jul-20 19:47 pkgUdit/test.py
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 20:33 pkgUdit/data/names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 20:33 pkgUdit/data/places.csv
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/License.txt
--rw-rw-rw-  2.0 fat      354 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      988 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/RECORD
-13 files, 9412 bytes uncompressed, 4102 bytes compressed:  56.4%
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      354 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      988 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/RECORD
+13 files, 10710 bytes uncompressed, 4480 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pkgUdit/data/names.csv
 Comment: 
 
 Filename: pkgUdit/data/places.csv
 Comment: 
 
-Filename: pkgUdit-1.1.5.2.dist-info/License.txt
+Filename: pkgUdit-1.1.5.4.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.2.dist-info/METADATA
+Filename: pkgUdit-1.1.5.4.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-1.1.5.2.dist-info/WHEEL
+Filename: pkgUdit-1.1.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-1.1.5.2.dist-info/top_level.txt
+Filename: pkgUdit-1.1.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.2.dist-info/RECORD
+Filename: pkgUdit-1.1.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/pswdGen.py

```diff
@@ -25,16 +25,16 @@
         list: A list containing the values read from the CSV file.
     """
     file_path = os.path.join(module_dir, file_name)
     with open(file_path) as csv_file:
         csv_reader = csv.reader(csv_file)
         return [row[0] for row in csv_reader]
 
-name_list = read_csv_file('names.csv')
-place_list = read_csv_file('places.csv')
+name_list = read_csv_file('Names.csv')
+place_list = read_csv_file('Places.csv')
 
 def custom_choice(chars):
     """
     Choose a random character from the given character set.
 
     Args:
         chars (list): A list containing characters to choose from.
```

## pkgUdit/test.py

```diff
@@ -1,35 +1,76 @@
-from pkgUdit import generatePass
+"""
+Custom Password Validator Script
+
+This script generates a random password using the `generatePass` function from the `pkgUdit` package
+and then validates it based on the following criteria:
+    - Contains at least one uppercase letter.
+    - Contains at least one lowercase letter.
+    - Contains at least one numeric value.
+    - Has a length between 6 and 12 characters.
+    - Does not match any data in 'Names.csv' and 'Places.csv' files.
+
+This script depends on the 'pkgUdit' package for generating passwords and requires 'Names.csv' and 'Places.csv'
+files in the same directory to check if the password matches any data in those files.
+
+"""
+
+from pkgUdit import generate_pass
+import os
+import csv
+
+module_dir = os.path.dirname(__file__)
+
+def read_csv_file(file_name):
+    file_path = os.path.join(module_dir, file_name)
+    with open(file_path) as csv_file:
+        return [row[0] for row in csv.reader(csv_file)]
+
+name_list = read_csv_file("Names.csv")
+place_list = read_csv_file("Places.csv")
 
 def password_validator(password):
     """
-    Validating the password based on the following criteria:
+    Validate the password based on the following criteria:
     - Contains at least one uppercase letter.
     - Contains at least one lowercase letter.
     - Contains at least one numeric value.
     - Has a length between 6 and 12 characters.
 
     Args:
         password (str): The password to be validated.
 
     Returns:
         bool: True if the password is valid, False otherwise.
     """
+
     if not 6 <= len(password) <= 12:
         return False
 
     if not any(char.isupper() for char in password):
         return False
 
     if not any(char.islower() for char in password):
         return False
 
     if not any(char.isdigit() for char in password):
         return False
 
-    return True
+    return not password in (name_list + place_list)
+
+# for single usage
 
 # Example usage:
-password = generatePass()  # Replace this with the password you want to validate
-print("password>>>>> : " + password)
-is_valid = password_validator(password)
-print(is_valid)  # Output: True or False
+# password = generatePass()
+# print("Generated Password: " + password)
+# is_valid = password_validator(password)
+# print("Password Valid: ", is_valid)  # Output: True or False
+
+
+
+# for checking mulitple password
+
+# for i in range(1000):
+#     password = generate_pass()
+#     print("Generated Password: " + password)
+#     is_valid = password_validator(password)
+#     print("Password Valid: ", is_valid)  # Output: True or False
```

## Comparing `pkgUdit-1.1.5.2.dist-info/License.txt` & `pkgUdit-1.1.5.4.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `pkgUdit-1.1.5.2.dist-info/RECORD` & `pkgUdit-1.1.5.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pkgUdit/Names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/Places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
 pkgUdit/__init__.py,sha256=-ZcvFGgCph477y-ftVPaBL2cE5w8b4fET3CjmfwYlYg,40
 pkgUdit/d.py,sha256=lTH6mkTVdjo-pWVIa1DqVY2LoUrEoSafeRyyiHOPcJY,2874
-pkgUdit/pswdGen.py,sha256=-zI345pFjsQzxigaQRkr0-rR5C6xvS2IF5cAmcoL4q8,2610
-pkgUdit/test.py,sha256=cMuY1yyvn02-7msSQNLgC3GYap6wU7a9SCZTEFKCGdc,1021
+pkgUdit/pswdGen.py,sha256=m5ZDbWrd4qTBERTsMYBYHhPNQxgPA7KT9rKQAnDdQ40,2610
+pkgUdit/test.py,sha256=YS1GnPsuVZH5EuqK0ne2vWbIFMiHQwPki6Y-BbWPODY,2319
 pkgUdit/data/names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/data/places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
-pkgUdit-1.1.5.2.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
-pkgUdit-1.1.5.2.dist-info/METADATA,sha256=8cV2hiQg1WQ_MxPVgtmWQjio2M1bLYpt0PwuvPkivpY,354
-pkgUdit-1.1.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pkgUdit-1.1.5.2.dist-info/top_level.txt,sha256=6HDcohhlcW4NGgQUEahihS6gyf5t4TajlQuyJGMTe4c,8
-pkgUdit-1.1.5.2.dist-info/RECORD,,
+pkgUdit-1.1.5.4.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
+pkgUdit-1.1.5.4.dist-info/METADATA,sha256=iEqmBPs_ftdaFR5GFHjI3UFvhnqDP0bktOBVj20G7vc,354
+pkgUdit-1.1.5.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pkgUdit-1.1.5.4.dist-info/top_level.txt,sha256=6HDcohhlcW4NGgQUEahihS6gyf5t4TajlQuyJGMTe4c,8
+pkgUdit-1.1.5.4.dist-info/RECORD,,
```

