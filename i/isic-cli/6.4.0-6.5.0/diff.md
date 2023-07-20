# Comparing `tmp/isic-cli-6.4.0.tar.gz` & `tmp/isic-cli-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-6.4.0.tar", last modified: Mon Jul 17 14:02:43 2023, max compression
+gzip compressed data, was "isic-cli-6.5.0.tar", last modified: Thu Jul 20 18:25:16 2023, max compression
```

## Comparing `isic-cli-6.4.0.tar` & `isic-cli-6.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.042035 isic-cli-6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.github/zip_and_upload_package.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-17 14:02:19.000000 isic-cli-6.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:02:19.000000 isic-cli-6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 14:02:43.042035 isic-cli-6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 14:02:19.000000 isic-cli-6.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-17 14:02:19.000000 isic-cli-6.4.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.038035 isic-cli-6.4.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 14:02:43.000000 isic-cli-6.4.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 14:02:19.000000 isic-cli-6.4.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-17 14:02:19.000000 isic-cli-6.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:02:43.042035 isic-cli-6.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-17 14:02:19.000000 isic-cli-6.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:02:43.042035 isic-cli-6.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-17 14:02:19.000000 isic-cli-6.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.341301 isic-cli-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.325301 isic-cli-6.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.325301 isic-cli-6.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.github/workflows/release.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.github/zip_and_upload_package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-20 18:24:51.000000 isic-cli-6.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 18:24:51.000000 isic-cli-6.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-20 18:25:16.337301 isic-cli-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-20 18:24:51.000000 isic-cli-6.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.325301 isic-cli-6.5.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.333301 isic-cli-6.5.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.333301 isic-cli-6.5.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.337301 isic-cli-6.5.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-20 18:24:51.000000 isic-cli-6.5.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.329301 isic-cli-6.5.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 18:25:16.000000 isic-cli-6.5.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 18:24:51.000000 isic-cli-6.5.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-20 18:24:51.000000 isic-cli-6.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:25:16.341301 isic-cli-6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-20 18:24:51.000000 isic-cli-6.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:25:16.337301 isic-cli-6.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-20 18:24:51.000000 isic-cli-6.5.0/tox.ini
```

### Comparing `isic-cli-6.4.0/.github/workflows/ci.yml` & `isic-cli-6.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/.github/workflows/package.yml` & `isic-cli-6.5.0/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/.github/workflows/release.yml` & `isic-cli-6.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/.gitignore` & `isic-cli-6.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/LICENSE` & `isic-cli-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/PKG-INFO` & `isic-cli-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.4.0
+Version: 6.5.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.4.0/README.md` & `isic-cli-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/__init__.py` & `isic-cli-6.5.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/accession.py` & `isic-cli-6.5.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/collection.py` & `isic-cli-6.5.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/image.py` & `isic-cli-6.5.0/isic_cli/cli/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from more_itertools.more import chunked
 from rich.console import Console
 from rich.progress import Progress
 
 from isic_cli.cli.context import IsicContext
 from isic_cli.cli.types import CommaSeparatedIdentifiers, SearchString
 from isic_cli.cli.utils import _extract_metadata, get_attributions, suggest_guest_login
-from isic_cli.io.http import download_image, get_images, get_num_images
+from isic_cli.io.http import download_image, get_images, get_license, get_num_images
 
 
 def cleanup_partially_downloaded_files(directory: Path) -> None:
     for p in directory.glob("**/.isic-partial.*"):
         # missing_ok=True because it's possible that another thread moved the temporary file to
         # its final destination after listing it but before unlinking.
         p.unlink(missing_ok=True)
@@ -122,17 +122,26 @@
             writer.writeheader()
             writer.writerows(records)
 
         with (outdir / "attribution.txt").open("w", encoding="utf8") as outfile:
             # TODO: os.linesep?
             outfile.write("\n\n".join(get_attributions(records)))
 
+        licenses = set([record["copyright_license"] for record in records])
+        (outdir / "licenses").mkdir(exist_ok=True)
+        for license_type in licenses:
+            with (outdir / "licenses" / f"{license_type}.txt").open("w") as outfile:
+                outfile.write(get_license(ctx.session, license_type))
+
     click.echo()
     click.secho(f"Successfully downloaded {nice_num_images} images to {outdir}/.", fg="green")
     click.secho(
         f'Successfully wrote {nice_num_images} metadata records to {outdir/"metadata.csv"}.',
         fg="green",
     )
     click.secho(
         f'Successfully wrote attributions to {outdir/"attribution.txt"}.',
         fg="green",
     )
+    click.secho(
+        f'Successfully wrote {len(licenses)} license(s) to {outdir/"licenses"}.', fg="green"
+    )
```

### Comparing `isic-cli-6.4.0/isic_cli/cli/metadata.py` & `isic-cli-6.5.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/types.py` & `isic-cli-6.5.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/user.py` & `isic-cli-6.5.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/cli/utils.py` & `isic-cli-6.5.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/io/http.py` & `isic-cli-6.5.0/isic_cli/io/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,20 @@
         "limit": 1,
     }
     r = session.get("images/search/", params=params)
     r.raise_for_status()
     return r.json()["count"]
 
 
+def get_license(session: IsicCliSession, license_type: str) -> str:
+    r = session.get(f"zip-download/license-file/{license_type}/")
+    r.raise_for_status()
+    return r.text
+
+
 # see https://github.com/danlamanna/retryable-requests/issues/10 to understand the
 # scenario which requires additional retry logic.
 @retry(
     retry=retry_if_exception_type((ConnectionError, ChunkedEncodingError)),
     wait=wait_exponential(multiplier=1, min=3, max=10),
     stop=stop_after_attempt(5),
     before_sleep=before_sleep_log(logger, logging.DEBUG),
```

### Comparing `isic-cli-6.4.0/isic_cli/session.py` & `isic-cli-6.5.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli/utils/version.py` & `isic-cli-6.5.0/isic_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-6.5.0/isic_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.4.0
+Version: 6.5.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.4.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-6.5.0/isic_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/pyproject.toml` & `isic-cli-6.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/setup.py` & `isic-cli-6.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tests/conftest.py` & `isic-cli-6.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tests/test_cli_base.py` & `isic-cli-6.5.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tests/test_cli_collection.py` & `isic-cli-6.5.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tests/test_cli_image.py` & `isic-cli-6.5.0/tests/test_cli_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,7 +38,8 @@
 def test_image_download(cli_run, isolated_filesystem, outdir, mock_images):
     result = cli_run(["image", "download", outdir])
 
     assert result.exit_code == 0, result.exception
     assert os.path.exists(f"{outdir}/ISIC_0000000.JPG")
     assert os.path.exists(f"{outdir}/metadata.csv")
     assert os.path.exists(f"{outdir}/attribution.txt")
+    assert os.path.exists(f"{outdir}/licenses/CC-0.txt")
```

### Comparing `isic-cli-6.4.0/tests/test_cli_metadata.py` & `isic-cli-6.5.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tests/test_utils.py` & `isic-cli-6.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.4.0/tox.ini` & `isic-cli-6.5.0/tox.ini`

 * *Files identical despite different names*

