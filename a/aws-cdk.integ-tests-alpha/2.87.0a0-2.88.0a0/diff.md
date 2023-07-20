# Comparing `tmp/aws-cdk.integ-tests-alpha-2.87.0a0.tar.gz` & `tmp/aws_cdk.integ_tests_alpha-2.88.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src94387485/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.87.0a0.tar", last modified: Thu Jul  6 16:50:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

