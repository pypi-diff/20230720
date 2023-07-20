# Comparing `tmp/wisdomweaver-0.3.1.tar.gz` & `tmp/wisdomweaver-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdomweaver-0.3.1.tar", last modified: Thu May 25 16:15:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

