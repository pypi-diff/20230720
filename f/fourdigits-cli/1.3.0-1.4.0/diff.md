# Comparing `tmp/fourdigits-cli-1.3.0.tar.gz` & `tmp/fourdigits-cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourdigits-cli-1.3.0.tar", last modified: Tue Jul 18 12:43:18 2023, max compression
+gzip compressed data, was "fourdigits-cli-1.4.0.tar", last modified: Thu Jul 20 13:46:55 2023, max compression
```

## Comparing `fourdigits-cli-1.3.0.tar` & `fourdigits-cli-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.270327 fourdigits-cli-1.3.0/fourdigits_cli/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.272328 fourdigits-cli-1.3.0/fourdigits_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5511 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.273327 fourdigits-cli-1.3.0/fourdigits_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.272328 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/tests/test_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.923601 fourdigits-cli-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-20 13:46:55.923601 fourdigits-cli-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.919601 fourdigits-cli-1.4.0/fourdigits_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.921601 fourdigits-cli-1.4.0/fourdigits_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5604 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/commands/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/commands/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.922601 fourdigits-cli-1.4.0/fourdigits_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/utils/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/fourdigits_cli/utils/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.921601 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 13:46:55.000000 fourdigits-cli-1.4.0/fourdigits_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-20 13:46:55.923601 fourdigits-cli-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:46:55.922601 fourdigits-cli-1.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-20 13:45:52.000000 fourdigits-cli-1.4.0/tests/test_settings.py
```

### Comparing `fourdigits-cli-1.3.0/PKG-INFO` & `fourdigits-cli-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.3.0
+Version: 1.4.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.3.0/README.md` & `fourdigits-cli-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/cli.py` & `fourdigits-cli-1.4.0/fourdigits_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/commands/docker.py` & `fourdigits-cli-1.4.0/fourdigits_cli/commands/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "--version",
     help="Version to build. If no version is supplied, it will try to get the current git tag",  # noqa: E501
 )
 @click.option("--push", is_flag=True, show_default=True, default=False)
 @click.option("--target")
 @click.option("--file", default="Dockerfile", show_default=True)
 @click.option("--context", default=".", show_default=True)
+@click.option("--build-arg", multiple=True)
 @click.pass_obj
 def build(docker: Docker, environment, **options):
     if environment not in DEFAULT_CONFIG.environments:
         raise click.UsageError("Environment doesn't exists in the pyproject.toml")
 
     version = validate_and_get_version(environment, version=options.get("version"))
 
@@ -73,14 +74,15 @@
         docker.build(
             build_image_name,
             file=options.get("file"),
             context=options.get("context"),
             target=options.get("target"),
             build_tag=str(version),
             cache_from=latest_image,
+            build_args=options.get("build_arg"),
         )
         for tag in [environment, str(version)]:
             docker.image_tag(
                 build_image_name,
                 docker.get_image_name(
                     repo=DEFAULT_CONFIG.docker_repo,
                     tag=tag,
```

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/commands/gitlab.py` & `fourdigits-cli-1.4.0/fourdigits_cli/commands/gitlab.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/settings.py` & `fourdigits-cli-1.4.0/fourdigits_cli/settings.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/utils/docker.py` & `fourdigits-cli-1.4.0/fourdigits_cli/utils/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         self,
         tag,
         file="Dockerfile",
         context=".",
         target=None,
         build_tag="",
         cache_from=None,
+        build_args=None,
     ):
         logger.info(f"Docker build image {tag}")
         logger.info(f" - file={file}")
         logger.info(f" - context={context}")
         logger.info(f" - target={target}")
         pip_extra_index_url = os.getenv(
             "PIP_EXTRA_INDEX_URL", "https://overmind.fourdigits.nl/products/simple/"
@@ -92,14 +93,15 @@
                         "--pull",
                         f"--target={target}" if target else None,
                         f"--tag={tag}",
                         f"--file={file}",
                         f"--cache-from={cache_from}" if cache_from else None,
                         f"--build-arg=TAG={build_tag}",
                         f"--build-arg=PIP_EXTRA_INDEX_URL={pip_extra_index_url}",
+                        *[f"--build-arg={arg}" for arg in build_args or []],
                         context,
                     ],
                 )
             )
         )
 
     def image_tag(self, tag, new_tag):
```

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli/utils/git.py` & `fourdigits-cli-1.4.0/fourdigits_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli.egg-info/PKG-INFO` & `fourdigits-cli-1.4.0/fourdigits_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.3.0
+Version: 1.4.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.3.0/fourdigits_cli.egg-info/SOURCES.txt` & `fourdigits-cli-1.4.0/fourdigits_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/setup.py` & `fourdigits-cli-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.3.0/tests/test_settings.py` & `fourdigits-cli-1.4.0/tests/test_settings.py`

 * *Files identical despite different names*

