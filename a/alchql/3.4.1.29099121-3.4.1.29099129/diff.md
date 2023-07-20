# Comparing `tmp/alchql-3.4.1.29099121.tar.gz` & `tmp/alchql-3.4.1.29099129-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.4.1.29099121.tar", last modified: Thu Jul 20 16:42:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

