# Comparing `tmp/pyCHX-4.1.2.tar.gz` & `tmp/pyCHX-4.2.0-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCHX-4.1.2.tar", last modified: Fri Feb  4 21:36:29 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

