# Comparing `tmp/cLoops2-0.0.3.tar.gz` & `tmp/cLoops2-0.0.5-py3.6.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cLoops2-0.0.3.tar", last modified: Tue Nov  2 18:00:22 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

