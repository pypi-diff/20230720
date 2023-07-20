# Comparing `tmp/alchql-3.4.0.29095311.tar.gz` & `tmp/alchql-3.4.0.29095318-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.4.0.29095311.tar", last modified: Thu Jul 20 15:38:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

