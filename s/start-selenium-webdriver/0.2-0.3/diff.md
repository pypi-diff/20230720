# Comparing `tmp/start_selenium_webdriver-0.2.tar.gz` & `tmp/start_selenium_webdriver-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_selenium_webdriver-0.2.tar", last modified: Tue Feb 28 12:11:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

