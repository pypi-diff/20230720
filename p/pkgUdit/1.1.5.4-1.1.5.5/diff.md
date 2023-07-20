# Comparing `tmp/pkgUdit-1.1.5.4-py3-none-any.whl.zip` & `tmp/pkgUdit-1.1.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6124 bytes, number of entries: 13
+Zip file size: 6132 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 16:29 pkgUdit/Names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 16:29 pkgUdit/Places.csv
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-20 18:53 pkgUdit/__init__.py
 -rw-rw-rw-  2.0 fat     2874 b- defN 23-Jul-18 16:39 pkgUdit/d.py
--rw-rw-rw-  2.0 fat     2610 b- defN 23-Jul-20 19:47 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat     2616 b- defN 23-Jul-20 19:58 pkgUdit/pswdGen.py
 -rw-rw-rw-  2.0 fat     2319 b- defN 23-Jul-20 19:47 pkgUdit/test.py
 -rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 20:33 pkgUdit/data/names.csv
 -rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 20:33 pkgUdit/data/places.csv
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/License.txt
--rw-rw-rw-  2.0 fat      354 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      988 b- defN 23-Jul-20 19:48 pkgUdit-1.1.5.4.dist-info/RECORD
-13 files, 10710 bytes uncompressed, 4480 bytes compressed:  58.2%
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-20 19:58 pkgUdit-1.1.5.5.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      354 b- defN 23-Jul-20 19:58 pkgUdit-1.1.5.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 19:58 pkgUdit-1.1.5.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 19:58 pkgUdit-1.1.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      988 b- defN 23-Jul-20 19:58 pkgUdit-1.1.5.5.dist-info/RECORD
+13 files, 10716 bytes uncompressed, 4488 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pkgUdit/data/names.csv
 Comment: 
 
 Filename: pkgUdit/data/places.csv
 Comment: 
 
-Filename: pkgUdit-1.1.5.4.dist-info/License.txt
+Filename: pkgUdit-1.1.5.5.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.4.dist-info/METADATA
+Filename: pkgUdit-1.1.5.5.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-1.1.5.4.dist-info/WHEEL
+Filename: pkgUdit-1.1.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-1.1.5.4.dist-info/top_level.txt
+Filename: pkgUdit-1.1.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-1.1.5.4.dist-info/RECORD
+Filename: pkgUdit-1.1.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/pswdGen.py

```diff
@@ -76,13 +76,13 @@
 
     Returns:
         str: A randomly generated password.
     """
     return make_random()
 
 # Example usage:
-final_pass = generate_pass()
-print(len(final_pass))
-print(final_pass)
+# final_pass = generate_pass()
+# print(len(final_pass))
+# print(final_pass)
```

## Comparing `pkgUdit-1.1.5.4.dist-info/License.txt` & `pkgUdit-1.1.5.5.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `pkgUdit-1.1.5.4.dist-info/RECORD` & `pkgUdit-1.1.5.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pkgUdit/Names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/Places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
 pkgUdit/__init__.py,sha256=-ZcvFGgCph477y-ftVPaBL2cE5w8b4fET3CjmfwYlYg,40
 pkgUdit/d.py,sha256=lTH6mkTVdjo-pWVIa1DqVY2LoUrEoSafeRyyiHOPcJY,2874
-pkgUdit/pswdGen.py,sha256=m5ZDbWrd4qTBERTsMYBYHhPNQxgPA7KT9rKQAnDdQ40,2610
+pkgUdit/pswdGen.py,sha256=giz2CAqXcugP3nNHc97-McyP3iUI7c4ERbn5LqX_VTQ,2616
 pkgUdit/test.py,sha256=YS1GnPsuVZH5EuqK0ne2vWbIFMiHQwPki6Y-BbWPODY,2319
 pkgUdit/data/names.csv,sha256=FHYqIO_gxJt7RxARqeVRimBIlmfJWWhQAuVeJDMUnyo,83
 pkgUdit/data/places.csv,sha256=jGrg5105R4wsvny7jXV3iDHOio9DcYGkMV6aaNW27Qk,90
-pkgUdit-1.1.5.4.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
-pkgUdit-1.1.5.4.dist-info/METADATA,sha256=iEqmBPs_ftdaFR5GFHjI3UFvhnqDP0bktOBVj20G7vc,354
-pkgUdit-1.1.5.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pkgUdit-1.1.5.4.dist-info/top_level.txt,sha256=6HDcohhlcW4NGgQUEahihS6gyf5t4TajlQuyJGMTe4c,8
-pkgUdit-1.1.5.4.dist-info/RECORD,,
+pkgUdit-1.1.5.5.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
+pkgUdit-1.1.5.5.dist-info/METADATA,sha256=KhTW7W0VVNAoNyyjnqrl3G0lpggJX9BkhY9H2lAdXf0,354
+pkgUdit-1.1.5.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pkgUdit-1.1.5.5.dist-info/top_level.txt,sha256=6HDcohhlcW4NGgQUEahihS6gyf5t4TajlQuyJGMTe4c,8
+pkgUdit-1.1.5.5.dist-info/RECORD,,
```

