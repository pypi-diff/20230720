# Comparing `tmp/dblite-1.3.2.tar.gz` & `tmp/dblite-1.3.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblite-1.3.2.tar", last modified: Thu May 18 17:28:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

