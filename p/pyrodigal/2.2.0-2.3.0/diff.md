# Comparing `tmp/pyrodigal-2.2.0.tar.gz` & `tmp/pyrodigal-2.3.0-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrodigal-2.2.0.tar", last modified: Mon Jun 19 20:04:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

