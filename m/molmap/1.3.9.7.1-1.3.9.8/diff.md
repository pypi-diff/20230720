# Comparing `tmp/molmap-1.3.9.7.1.tar.gz` & `tmp/molmap-1.3.9.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molmap-1.3.9.7.1.tar", last modified: Fri Jul 14 06:15:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

