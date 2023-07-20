# Comparing `tmp/pkgUdit-1.1.5-py3-none-any.whl.zip` & `tmp/pkgUdit-1.1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 5300 bytes, number of entries: 12
+Zip file size: 5746 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 16:29 pkgUdit/Names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 16:29 pkgUdit/Places.csv
--rw-rw-rw-  2.0 fat      292 b- defN 23-Jul-18 20:33 pkgUdit/__init__.py
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-20 18:53 pkgUdit/__init__.py
 -rw-rw-rw-  2.0 fat     2874 b- defN 23-Jul-18 16:39 pkgUdit/d.py
--rw-rw-rw-  2.0 fat     2534 b- defN 23-Jul-20 06:32 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat     2610 b- defN 23-Jul-20 18:41 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jul-20 07:12 pkgUdit/test.py
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 20:33 pkgUdit/data/names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 20:33 pkgUdit/data/places.csv
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 06:41 pkgUdit-1.1.5.dist-info/License.txt
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-20 06:41 pkgUdit-1.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 06:41 pkgUdit-1.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-20 06:41 pkgUdit-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      908 b- defN 23-Jul-20 06:41 pkgUdit-1.1.5.dist-info/RECORD
-12 files, 8497 bytes uncompressed, 3782 bytes compressed:  55.5%
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      354 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      988 b- defN 23-Jul-20 19:10 pkgUdit-1.1.5.2.dist-info/RECORD
+13 files, 9412 bytes uncompressed, 4102 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -9,29 +9,32 @@
 
 Filename: pkgUdit/d.py
 Comment: 
 
 Filename: pkgUdit/pswdGen.py
 Comment: 
 
+Filename: pkgUdit/test.py
+Comment: 
+
 Filename: pkgUdit/data/names.csv
 Comment: 
 
 Filename: pkgUdit/data/places.csv
 Comment: 
 
-Filename: pkgUdit-1.1.5.dist-info/License.txt
+Filename: pkgUdit-1.1.5.2.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.dist-info/METADATA
+Filename: pkgUdit-1.1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-1.1.5.dist-info/WHEEL
+Filename: pkgUdit-1.1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-1.1.5.dist-info/top_level.txt
+Filename: pkgUdit-1.1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.dist-info/RECORD
+Filename: pkgUdit-1.1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/__init__.py

```diff
@@ -1,18 +1,3 @@
-# import sys
-# import os
-
-# Add the parent directory to the Python path
-# print(__file__)
-# parent_dir = os.path.dirname(os.path.abspath(__file__))
-# sys.path.append(parent_dir)
-
-
-
-from .pswdGen import generatePass
-
-
-
-# def generatePassword():
-#     return generatePass()
+from .pswdGen import generate_pass
```

## pkgUdit/pswdGen.py

```diff
@@ -1,18 +1,21 @@
-
 import random
 import csv
 import os
 
-# Save the required data for making the password in lists
+# Saving the required data for making the password in lists
 numerals = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
-lowerCaps = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
-upperChars = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+lower_caps = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j',
+            'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 
+            'u', 'v', 'w', 'x', 'y', 'z']
+upper_chars = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J',
+             'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 
+             'U', 'V', 'W', 'X', 'Y', 'Z']
 
-combinedChars = numerals + lowerCaps + upperChars
+combined_chars = numerals + lower_caps + upper_chars
 module_dir = os.path.dirname(__file__)
 
 def read_csv_file(file_name):
     """
     Read a CSV file and return its contents as a list.
 
     Args:
@@ -22,16 +25,16 @@
         list: A list containing the values read from the CSV file.
     """
     file_path = os.path.join(module_dir, file_name)
     with open(file_path) as csv_file:
         csv_reader = csv.reader(csv_file)
         return [row[0] for row in csv_reader]
 
-nameList = read_csv_file('names.csv')
-placeList = read_csv_file('places.csv')
+name_list = read_csv_file('names.csv')
+place_list = read_csv_file('places.csv')
 
 def custom_choice(chars):
     """
     Choose a random character from the given character set.
 
     Args:
         chars (list): A list containing characters to choose from.
@@ -44,39 +47,42 @@
 def make_random():
     """
     Generate a random password that is not present in the name or place list.
 
     Returns:
         str: A randomly generated password.
     """
-    passLength = random.randint(6, 12)
-    password = [custom_choice(combinedChars) for _ in range(passLength)]
+    pass_length = random.randint(6, 12)
+    password = [custom_choice(combined_chars) for _ in range(pass_length)]
     password.insert(0, random.choice(numerals))  # Include one numeric value
     random.shuffle(password)
     pswd = "".join(password)
-    return pswd if passwordChecker(pswd) else make_random()
+    return pswd if password_checker(pswd) else make_random()
 
-def passwordChecker(created_pass):
+def password_checker(created_pass):
     """
     Check if the generated password is not present in the name or place list.
 
     Args:
         created_pass (str): The password to be checked.
 
     Returns:
         bool: True if the password is not in the name or place list, False otherwise.
     """
-    return created_pass not in (nameList + placeList)
+    return created_pass not in (name_list + place_list)
 
-def generatePass():
+def generate_pass():
     """
     Generate a random password that is not present in the name or place list.
 
     Returns:
         str: A randomly generated password.
     """
     return make_random()
 
 # Example usage:
-# final_pass = generatePass()
-# print(len(final_pass))
-# print(final_pass)
+final_pass = generate_pass()
+print(len(final_pass))
+print(final_pass)
+
+
+
```

## Comparing `pkgUdit-1.1.5.dist-info/License.txt` & `pkgUdit-1.1.5.2.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `pkgUdit-1.1.5.dist-info/RECORD` & `pkgUdit-1.1.5.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pkgUdit/Names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/Places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
-pkgUdit/__init__.py,sha256=MV6f8V2P6ujmoguk4-JId_rjxWCd0a_KsJ8fvb98uk8,292
+pkgUdit/__init__.py,sha256=-ZcvFGgCph477y-ftVPaBL2cE5w8b4fET3CjmfwYlYg,40
 pkgUdit/d.py,sha256=lTH6mkTVdjo-pWVIa1DqVY2LoUrEoSafeRyyiHOPcJY,2874
-pkgUdit/pswdGen.py,sha256=_k135-XcQDY4sKB3YHjGTmzvGQuKwYBNUJsKlYhPqLA,2534
+pkgUdit/pswdGen.py,sha256=-zI345pFjsQzxigaQRkr0-rR5C6xvS2IF5cAmcoL4q8,2610
+pkgUdit/test.py,sha256=cMuY1yyvn02-7msSQNLgC3GYap6wU7a9SCZTEFKCGdc,1021
 pkgUdit/data/names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/data/places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
-pkgUdit-1.1.5.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
-pkgUdit-1.1.5.dist-info/METADATA,sha256=HLe7FJ9F_E0AKDe2RKSSZeEX3l3aAaPVGedwZdNAXGw,352
-pkgUdit-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pkgUdit-1.1.5.dist-info/top_level.txt,sha256=3CwC7EPEg2sf1KipgDsLRA_30qheFVMdK8cvKwak6Uw,20
-pkgUdit-1.1.5.dist-info/RECORD,,
+pkgUdit-1.1.5.2.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
+pkgUdit-1.1.5.2.dist-info/METADATA,sha256=8cV2hiQg1WQ_MxPVgtmWQjio2M1bLYpt0PwuvPkivpY,354
+pkgUdit-1.1.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pkgUdit-1.1.5.2.dist-info/top_level.txt,sha256=6HDcohhlcW4NGgQUEahihS6gyf5t4TajlQuyJGMTe4c,8
+pkgUdit-1.1.5.2.dist-info/RECORD,,
```

