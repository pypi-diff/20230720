# Comparing `tmp/efemarai-0.4.0.tar.gz` & `tmp/efemarai-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efemarai-0.4.0.tar", last modified: Fri Jun  9 14:06:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

