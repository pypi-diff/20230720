# Comparing `tmp/fastlane_bot-0.0.0.tar.gz` & `tmp/fastlane_bot-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-0.0.0.tar", last modified: Wed Jul 19 12:26:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

