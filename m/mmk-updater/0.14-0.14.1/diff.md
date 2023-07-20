# Comparing `tmp/mmk_updater-0.14.tar.gz` & `tmp/mmk_updater-0.14.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmk_updater-0.14.tar", last modified: Tue May  9 06:35:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

