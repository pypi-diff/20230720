# Comparing `tmp/pyft-0.1.0.tar.gz` & `tmp/pyft-0.1.1-cp310-cp310-macosx_10_7_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

