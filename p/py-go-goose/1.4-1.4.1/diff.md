# Comparing `tmp/py_go_goose-1.4.tar.gz` & `tmp/py_go_goose-1.4.1-cp38-cp38-macosx_13_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_go_goose-1.4.tar", last modified: Fri Jul 14 03:08:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

