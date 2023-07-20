# Comparing `tmp/reviser-0.3.0.tar.gz` & `tmp/reviser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviser-0.3.0.tar", max compression
+gzip compressed data, was "reviser-0.3.1.tar", max compression
```

## Comparing `reviser-0.3.0.tar` & `reviser-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0     1078 2022-10-16 14:00:00.574076 reviser-0.3.0/LICENSE
--rw-r--r--   0        0        0    41023 2022-10-16 14:01:36.566389 reviser-0.3.0/README.md
--rw-r--r--   0        0        0     2458 2022-10-16 14:00:00.574076 reviser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      837 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/__init__.py
--rw-r--r--   0        0        0     4779 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/bundling/__init__.py
--rw-r--r--   0        0        0     4610 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/bundling/_installer.py
--rw-r--r--   0        0        0     2837 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/cli.py
--rw-r--r--   0        0        0     1554 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/__init__.py
--rw-r--r--   0        0        0     4766 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/aliaser.py
--rw-r--r--   0        0        0     2391 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/bundler.py
--rw-r--r--   0        0        0      850 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/configer.py
--rw-r--r--   0        0        0     2008 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/deployer.py
--rw-r--r--   0        0        0      636 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/exiter.py
--rw-r--r--   0        0        0     1799 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/helper/__init__.py
--rw-r--r--   0        0        0      198 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/helper/help.jinja2
--rw-r--r--   0        0        0     5192 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/invoker.py
--rw-r--r--   0        0        0     1267 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/lister.py
--rw-r--r--   0        0        0     8202 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/pruner.py
--rw-r--r--   0        0        0      875 2022-10-16 14:00:00.575076 reviser-0.3.0/reviser/commands/pusher.py
--rw-r--r--   0        0        0     2470 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/region_switcher.py
--rw-r--r--   0        0        0     2542 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/reloader.py
--rw-r--r--   0        0        0     4697 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/reporter.py
--rw-r--r--   0        0        0     5377 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/selector.py
--rw-r--r--   0        0        0     1360 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/sheller.py
--rw-r--r--   0        0        0     5008 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/commands/tailer.py
--rw-r--r--   0        0        0     1249 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/__init__.py
--rw-r--r--   0        0        0     4398 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/abstracts.py
--rw-r--r--   0        0        0     2247 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/aws.py
--rw-r--r--   0        0        0     3698 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/__init__.py
--rw-r--r--   0        0        0     9766 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/bundling.py
--rw-r--r--   0        0        0     9682 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/depending.py
--rw-r--r--   0        0        0     3988 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/enviromentals.py
--rw-r--r--   0        0        0     2261 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/imaging.py
--rw-r--r--   0        0        0     3052 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/layering.py
--rw-r--r--   0        0        0     9875 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/configurations/targeting.py
--rw-r--r--   0        0        0     3380 2022-10-16 14:00:00.576077 reviser-0.3.0/reviser/definitions/contexts.py
--rw-r--r--   0        0        0     1126 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/definitions/enumerations.py
--rw-r--r--   0        0        0     9689 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/definitions/infomatics.py
--rw-r--r--   0        0        0      569 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/definitions/selections.py
--rw-r--r--   0        0        0     2902 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/deploying/__init__.py
--rw-r--r--   0        0        0     6356 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/deploying/publisher.py
--rw-r--r--   0        0        0     6558 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/deploying/updater.py
--rw-r--r--   0        0        0     2382 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/deploying/uploader.py
--rw-r--r--   0        0        0      508 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/__init__.py
--rw-r--r--   0        0        0     4152 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/completions.py
--rw-r--r--   0        0        0     1533 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/runner.py
--rw-r--r--   0        0        0     9570 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/shells/__init__.py
--rw-r--r--   0        0        0      293 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/shells/execution_result.jinja2
--rw-r--r--   0        0        0      514 2022-10-16 14:00:00.577077 reviser-0.3.0/reviser/interactivity/shells/prompt.jinja2
--rw-r--r--   0        0        0      277 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/interactivity/shells/splash.jinja2
--rw-r--r--   0        0        0     4468 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/parsing.py
--rw-r--r--   0        0        0      553 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/servicer/__init__.py
--rw-r--r--   0        0        0     3403 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/servicer/functioning/__init__.py
--rw-r--r--   0        0        0      334 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/servicer/functioning/echo_versions.jinja2
--rw-r--r--   0        0        0     4098 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/servicer/layering.py
--rw-r--r--   0        0        0     2360 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/templating/__init__.py
--rw-r--r--   0        0        0      260 2022-10-16 14:00:00.578077 reviser-0.3.0/reviser/templating/error.jinja2
--rw-r--r--   0        0        0     1809 2022-10-16 14:00:00.581077 reviser-0.3.0/reviser/utils.py
--rw-r--r--   0        0        0    43665 1970-01-01 00:00:00.000000 reviser-0.3.0/setup.py
--rw-r--r--   0        0        0    42405 1970-01-01 00:00:00.000000 reviser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-20 16:48:02.382369 reviser-0.3.1/LICENSE
+-rw-r--r--   0        0        0    40957 2023-07-20 16:48:33.101843 reviser-0.3.1/README.md
+-rw-r--r--   0        0        0     2646 2023-07-20 16:48:02.382369 reviser-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/__init__.py
+-rw-r--r--   0        0        0     4779 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/bundling/__init__.py
+-rw-r--r--   0        0        0     4627 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/bundling/_installer.py
+-rw-r--r--   0        0        0     2854 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/cli.py
+-rw-r--r--   0        0        0     1554 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/__init__.py
+-rw-r--r--   0        0        0     4766 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/aliaser.py
+-rw-r--r--   0        0        0     2391 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/bundler.py
+-rw-r--r--   0        0        0      850 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/configer.py
+-rw-r--r--   0        0        0     2008 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/deployer.py
+-rw-r--r--   0        0        0      636 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/exiter.py
+-rw-r--r--   0        0        0     1799 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/helper/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/helper/help.jinja2
+-rw-r--r--   0        0        0     5192 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/invoker.py
+-rw-r--r--   0        0        0     1267 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/lister.py
+-rw-r--r--   0        0        0     8355 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/pruner.py
+-rw-r--r--   0        0        0      875 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/pusher.py
+-rw-r--r--   0        0        0     2470 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/region_switcher.py
+-rw-r--r--   0        0        0     2542 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/reloader.py
+-rw-r--r--   0        0        0     4697 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/reporter.py
+-rw-r--r--   0        0        0     5377 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/selector.py
+-rw-r--r--   0        0        0     1360 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/sheller.py
+-rw-r--r--   0        0        0     5008 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/tailer.py
+-rw-r--r--   0        0        0     1249 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/__init__.py
+-rw-r--r--   0        0        0     4398 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/abstracts.py
+-rw-r--r--   0        0        0     2247 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/aws.py
+-rw-r--r--   0        0        0     3698 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/__init__.py
+-rw-r--r--   0        0        0     9766 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/bundling.py
+-rw-r--r--   0        0        0     9624 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/depending.py
+-rw-r--r--   0        0        0     3988 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/enviromentals.py
+-rw-r--r--   0        0        0     2261 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/imaging.py
+-rw-r--r--   0        0        0     3052 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/layering.py
+-rw-r--r--   0        0        0     9875 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/targeting.py
+-rw-r--r--   0        0        0     3414 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/contexts.py
+-rw-r--r--   0        0        0     1126 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/enumerations.py
+-rw-r--r--   0        0        0     9689 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/infomatics.py
+-rw-r--r--   0        0        0      569 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/selections.py
+-rw-r--r--   0        0        0     2953 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/__init__.py
+-rw-r--r--   0        0        0     6390 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/publisher.py
+-rw-r--r--   0        0        0     6558 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/updater.py
+-rw-r--r--   0        0        0     2382 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/uploader.py
+-rw-r--r--   0        0        0      508 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/__init__.py
+-rw-r--r--   0        0        0     4152 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/completions.py
+-rw-r--r--   0        0        0     1591 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/runner.py
+-rw-r--r--   0        0        0     9638 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/__init__.py
+-rw-r--r--   0        0        0      293 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/execution_result.jinja2
+-rw-r--r--   0        0        0      514 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/prompt.jinja2
+-rw-r--r--   0        0        0      277 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/splash.jinja2
+-rw-r--r--   0        0        0     4468 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/parsing.py
+-rw-r--r--   0        0        0      553 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/servicer/__init__.py
+-rw-r--r--   0        0        0     3403 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/functioning/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/functioning/echo_versions.jinja2
+-rw-r--r--   0        0        0     4098 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/layering.py
+-rw-r--r--   0        0        0     2394 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/templating/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/templating/error.jinja2
+-rw-r--r--   0        0        0     1826 2023-07-20 16:48:02.389369 reviser-0.3.1/reviser/utils.py
+-rw-r--r--   0        0        0    42379 1970-01-01 00:00:00.000000 reviser-0.3.1/PKG-INFO
```

### Comparing `reviser-0.3.0/LICENSE` & `reviser-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/README.md` & `reviser-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                        to the specified function version if the --create flag
                        is included to allow for creating a new alias.
   version              Version of the function that the alias should be
                        assigned to. This will either be an integer value or
                        $LATEST. To see what versions are available for a given
                        function use the list command.
 
-optional arguments:
+options:
   --function FUNCTION  The alias command only acts on one function. This can
                        be achieved either by selecting the function target via
                        the select command, or specifying the function name to
                        apply this change to with this flag.
   --yes                By default this command will require input confirmation
                        before carrying out the change. Specify this flag to
                        skip input confirmation and proceed without a breaking
@@ -166,15 +166,15 @@
 
 Install dependencies and copies includes into a zipped file ready for
 deployment.
 
 ```
 usage: bundle [--reinstall] [--output OUTPUT]
 
-optional arguments:
+options:
   --reinstall           Add this flag to reinstall dependencies on a repeated
                         bundle operation. By default, dependencies will remain
                         cached for the lifetime of the shell to speed up the
                         bundling process. This will force dependencies to be
                         installed even if they had been installed previously.
   --output OUTPUT, -o OUTPUT
                         Output the bundled artifacts into the specified output
@@ -201,15 +201,15 @@
 
 Upload the bundled contents to the upload S3 bucket and then publish a new
 version.
 
 ```
 usage: deploy [--description DESCRIPTION] [--dry-run]
 
-optional arguments:
+options:
   --description DESCRIPTION
                         Specify a message to assign to the version published
                         by the deploy command.
   --dry-run             If set, the deploy operation will be exercised without
                         actually carrying out the actions. This can be useful
                         to validate the deploy process without side effects.
 
@@ -253,15 +253,15 @@
 ## prune
 
 Remove old function and/or layer versions for the selected targets.
 
 ```
 usage: prune [--start START] [--end END] [--dry-run] [-y]
 
-optional arguments:
+options:
   --start START  Keep versions lower (earlier/before) this one. A negative
                  value can be specified for relative indexing in the same
                  fashion as Python lists.
   --end END      Do not prune versions higher than this value. A negative
                  value can be specified for relative indexing in the same
                  fashion as Python lists.
   --dry-run      Echo pruning operation without actually executing it.
@@ -273,15 +273,15 @@
 
 Combined single command for bundling and deploying the selected targets.
 
 ```
 usage: push [--reinstall] [--output OUTPUT] [--description DESCRIPTION]
             [--dry-run]
 
-optional arguments:
+options:
   --reinstall           Add this flag to reinstall dependencies on a repeated
                         bundle operation. By default, dependencies will remain
                         cached for the lifetime of the shell to speed up the
                         bundling process. This will force dependencies to be
                         installed even if they had been installed previously.
   --output OUTPUT, -o OUTPUT
                         Output the bundled artifacts into the specified output
@@ -332,15 +332,15 @@
                         layer target names available from the configuration.
                         This can include shell-style wildcards and will also
                         match against partial strings. If the --exact flag is
                         specified, this value must exactly match one of the
                         targets instead of the default fuzzy matching
                         behavior.
 
-optional arguments:
+options:
   --functions, --function, --func, -f
                         When specified, functions will be selected. This will
                         default to true if neither of --functions or --layers
                         is specified. Will default to false if --layers is
                         specified.
   --layers, --layer, -l
                         When specified, layers will be selected. This will
```

### Comparing `reviser-0.3.0/pyproject.toml` & `reviser-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reviser"
-version = "0.3.0"
+version = "0.3.1"
 description = "AWS Lambda function/layer version deployment manager."
 authors = [
   "Scott Ernst <swernst@gmail.com>",
   "Kevin Schiroo",
   "Rigo Silva"
 ]
 license = "MIT"
@@ -16,33 +16,37 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Utilities",
   "Typing :: Typed"
 ]
 exclude = ["reviser/tests"]
 
 [tool.poetry.scripts]
 reviser = 'reviser.cli:main'
 reviser-shell = 'reviser:main_shell'
 
 [tool.poetry.dependencies]
-python = ">=3.8.0, <3.10.0"
+python = ">=3.8.0, <3.12.0"
 boto3 = { version = ">=1.16.11", optional = true }
 colorama = { version = ">=0.4.4", optional = true }
 Jinja2 = { version = ">=2.11.2", optional = true }
 prompt-toolkit = { version = ">=3.0.8", optional = true }
 PyYAML = { version = ">=5.3.0", optional = true }
 pipper = { version = ">=0.10.0", optional = true }
 toml = { version = ">=0.10.0", optional = true }
 wheel = { version = ">=0.37.1", optional = true }
+# AWS is not currently compatible with 2+
+urllib3 = "<2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 coverage = "*"
 pytest-cov = "*"
 lobotomy = ">=0.3.0"
@@ -66,14 +70,15 @@
 hadolint = "hadolint Dockerfile"
 radon = "radon cc . && radon mi ."
 test = "pytest . --cov-report=term-missing --cov=."
 format = "task black"
 lint = "task black_lint && task flake8 && task mypy && task pydocstyle && task radon && task yamllint"
 check = "task format && task lint && task test"
 docs = "python docs_builder.py"
+build_images = "python image_builder.py"
 images = "python image_builder.py --publish"
 
 [tool.poetry.extras]
 shell = [
   "prompt-toolkit",
   "Jinja2",
   "colorama",
```

### Comparing `reviser-0.3.0/reviser/__init__.py` & `reviser-0.3.1/reviser/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/bundling/__init__.py` & `reviser-0.3.1/reviser/bundling/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/bundling/_installer.py` & `reviser-0.3.1/reviser/bundling/_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     os.system(" ".join(cmd))
 
 
 def _install_pipper_package(
     name: str,
     site_packages: pathlib.Path,
     env: dict,
-    arguments: typing.List[str] = None,
+    arguments: typing.Optional[typing.List[str]] = None,
 ):
     """Install the specified pipper package."""
     cmd = [
         "pipper",
         "install",
         name,
         "--upgrade",
```

### Comparing `reviser-0.3.0/reviser/cli.py` & `reviser-0.3.1/reviser/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return source[:index] + source[next_index:]
     except StopIteration:
         pass
 
     return source.copy()
 
 
-def main(arguments: typing.List[str] = None) -> bool:
+def main(arguments: typing.Optional[typing.List[str]] = None) -> bool:
     """Start the shell container based on the command line arguments."""
     print(f"\n[DIRECTORY]: {os.path.realpath(os.curdir)}")
     args = parsing.create_parser(False).parse_args(args=arguments)
 
     credentials_directory = (
         pathlib.Path(os.path.expandvars(args.aws_directory)).expanduser().resolve()
     )
```

### Comparing `reviser-0.3.0/reviser/commands/__init__.py` & `reviser-0.3.1/reviser/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/aliaser.py` & `reviser-0.3.1/reviser/commands/aliaser.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/bundler.py` & `reviser-0.3.1/reviser/commands/bundler.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/configer.py` & `reviser-0.3.1/reviser/commands/configer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/deployer.py` & `reviser-0.3.1/reviser/commands/deployer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/exiter.py` & `reviser-0.3.1/reviser/commands/exiter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/helper/__init__.py` & `reviser-0.3.1/reviser/commands/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/invoker.py` & `reviser-0.3.1/reviser/commands/invoker.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/lister.py` & `reviser-0.3.1/reviser/commands/lister.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/pruner.py` & `reviser-0.3.1/reviser/commands/pruner.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 def _resolve_version(
     versions: typing.Union[
         typing.List[definitions.LambdaLayer],
         typing.List[definitions.LambdaFunction],
     ],
-    value: int = None,
+    value: typing.Optional[int] = None,
 ) -> typing.Optional[int]:
     """
     Normalize specified versions by making them absolute, positive version integers.
 
     Leaves None and positive integer values alone, but will convert relative negative
     integers into their positive integer equivalents based on the available versions
     included in the version argument.
@@ -89,16 +89,16 @@
         end_value is None or int(function.version or 0) <= end_value
     )
 
 
 def _get_function_removal_versions(
     lambda_client: BaseClient,
     function_name: str,
-    start: int = None,
-    end: int = None,
+    start: typing.Optional[int] = None,
+    end: typing.Optional[int] = None,
 ):
     """Get ARNs for the function that should be pruned."""
     versions = servicer.get_function_versions(lambda_client, function_name)
     start_value = _resolve_version(versions, start)
     end_value = _resolve_version(versions, end)
     return [
         v.arn
@@ -109,16 +109,16 @@
         and not v.aliases
     ]
 
 
 def _prune_function(
     lambda_client: BaseClient,
     function_name: str,
-    start: int = None,
-    end: int = None,
+    start: typing.Optional[int] = None,
+    end: typing.Optional[int] = None,
     dry_run: typing.Optional[bool] = False,
     confirm: typing.Optional[bool] = True,
 ):
     """
     Execute a pruning operation on the given lambda functions.
 
     :param lambda_client:
@@ -168,16 +168,16 @@
 
     return removal_arns
 
 
 def _get_layer_removal_versions(
     lambda_client: BaseClient,
     layer_name: str,
-    start: int = None,
-    end: int = None,
+    start: typing.Optional[int] = None,
+    end: typing.Optional[int] = None,
 ):
     """Get ARNs for the layer that should be pruned."""
     versions = servicer.get_layer_versions(lambda_client, layer_name)
     start_value = _resolve_version(versions, start)
     end_value = _resolve_version(versions, end)
     removals = [
         version
@@ -187,16 +187,16 @@
     ]
     return [r.arn for r in removals if r.arn]
 
 
 def _prune_layer(
     lambda_client: BaseClient,
     layer_name: str,
-    start: int = None,
-    end: int = None,
+    start: typing.Optional[int] = None,
+    end: typing.Optional[int] = None,
     dry_run: typing.Optional[bool] = False,
     confirm: typing.Optional[bool] = True,
 ):
     """
     Execute a pruning operation on the given lambda layers.
 
     :param lambda_client:
```

### Comparing `reviser-0.3.0/reviser/commands/pusher.py` & `reviser-0.3.1/reviser/commands/pusher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/region_switcher.py` & `reviser-0.3.1/reviser/commands/region_switcher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/reloader.py` & `reviser-0.3.1/reviser/commands/reloader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/reporter.py` & `reviser-0.3.1/reviser/commands/reporter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/selector.py` & `reviser-0.3.1/reviser/commands/selector.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/sheller.py` & `reviser-0.3.1/reviser/commands/sheller.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/commands/tailer.py` & `reviser-0.3.1/reviser/commands/tailer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/__init__.py` & `reviser-0.3.1/reviser/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/abstracts.py` & `reviser-0.3.1/reviser/definitions/abstracts.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/aws.py` & `reviser-0.3.1/reviser/definitions/aws.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/__init__.py` & `reviser-0.3.1/reviser/definitions/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/bundling.py` & `reviser-0.3.1/reviser/definitions/configurations/bundling.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/depending.py` & `reviser-0.3.1/reviser/definitions/configurations/depending.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     connection: "aws.AwsConnection",
     dependency_data: typing.List[typing.Dict[str, typing.Any]],
     is_shared: bool = False,
 ):
     """Parse configuration dependency data into a tuple of Dependency objects."""
     output = []
 
-    dependency: Dependency
     dependency_types = enumerations.DependencyType
     mappings = typing.cast(
         typing.Dict[str, typing.Any],
         {
             dependency_types.PIP.value: PipDependency,
             dependency_types.PIPPER.value: PipperDependency,
             dependency_types.POETRY.value: PoetryDependency,
@@ -72,15 +71,14 @@
         return pathlib.Path(tempfile.gettempdir()).joinpath(self.uuid)
 
     @property
     def sources(self) -> typing.Tuple["Dependency", ...]:
         """Parse configuration dependency data into a tuple of Dependency objects."""
         output = []
 
-        dependency: Dependency
         dependency_types = enumerations.DependencyType
         mappings = typing.cast(
             typing.Dict[str, typing.Any],
             {
                 dependency_types.PIP.value: PipDependency,
                 dependency_types.PIPPER.value: PipperDependency,
                 dependency_types.POETRY.value: PoetryDependency,
```

### Comparing `reviser-0.3.0/reviser/definitions/configurations/enviromentals.py` & `reviser-0.3.1/reviser/definitions/configurations/enviromentals.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/imaging.py` & `reviser-0.3.1/reviser/definitions/configurations/imaging.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/layering.py` & `reviser-0.3.1/reviser/definitions/configurations/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/configurations/targeting.py` & `reviser-0.3.1/reviser/definitions/configurations/targeting.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/contexts.py` & `reviser-0.3.1/reviser/definitions/contexts.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             ]
         )
 
     @classmethod
     def load_from_file(
         cls,
         arguments: argparse.Namespace,
-        path: typing.Union[str, pathlib.Path] = None,
-        connection: "aws.AwsConnection" = None,
+        path: typing.Optional[typing.Union[str, pathlib.Path]] = None,
+        connection: typing.Optional["aws.AwsConnection"] = None,
     ) -> "Context":
         """
         Load a context from a configuration path target.
 
         Loads files using the `lambda.yaml` file by default as this is the preferred
         extension: https://yaml.org/faq.html
         """
```

### Comparing `reviser-0.3.0/reviser/definitions/enumerations.py` & `reviser-0.3.1/reviser/definitions/enumerations.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/infomatics.py` & `reviser-0.3.1/reviser/definitions/infomatics.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/definitions/selections.py` & `reviser-0.3.1/reviser/definitions/selections.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/deploying/__init__.py` & `reviser-0.3.1/reviser/deploying/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from reviser import definitions
 from ..deploying import publisher
 from ..deploying import uploader
 
 
 def deploy_target(
     target: "definitions.Target",
-    description: str = None,
-    published_layers: typing.List["definitions.PublishedLayer"] = None,
+    description: typing.Optional[str] = None,
+    published_layers: typing.Optional[typing.List["definitions.PublishedLayer"]] = None,
     dry_run: bool = False,
 ) -> typing.List["definitions.PublishedLayer"]:
     """
     Deploy the bundled ZIP file to S3 for access by Lambda functions.
 
     The file is uploaded to the specified storage bucket with a timestamped key and
     then published to the lambda function.
@@ -56,15 +56,15 @@
     )
     return []
 
 
 def deploy(
     context: "definitions.Context",
     selection: "definitions.Selection",
-    description: str = None,
+    description: typing.Optional[str] = None,
     dry_run: bool = False,
 ) -> typing.List["definitions.Target"]:
     """
     Execute the deploy operation on the context's configuration.
 
     This execution is filtered to targets by the specified selection argument value.
     """
```

### Comparing `reviser-0.3.0/reviser/deploying/publisher.py` & `reviser-0.3.1/reviser/deploying/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     )
 
 
 def publish_function(
     target: "definitions.Target",
     s3_keys: typing.Optional[typing.List[str]] = None,
     published_layers: typing.Optional[typing.List["definitions.PublishedLayer"]] = None,
-    description: str = None,
+    description: typing.Optional[str] = None,
     dry_run: bool = False,
 ):
     """
     Publish an updated version of the lambda function.
 
     :param target:
         The lambda function to publish.
@@ -158,15 +158,15 @@
 
     print("[DEPLOYED]: Lambda function code has been deployed\n")
 
 
 def publish_layer(
     target: "definitions.Target",
     s3_keys: typing.List[str],
-    description: str = None,
+    description: typing.Optional[str] = None,
     dry_run: bool = False,
 ) -> typing.List["definitions.PublishedLayer"]:
     """Publish an updated version of the layer after bundle has been uploaded to S3."""
     published_layers = []
     client = target.client("lambda")
 
     for name, key in zip(target.names, s3_keys):
```

### Comparing `reviser-0.3.0/reviser/deploying/updater.py` & `reviser-0.3.1/reviser/deploying/updater.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/deploying/uploader.py` & `reviser-0.3.1/reviser/deploying/uploader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/interactivity/completions.py` & `reviser-0.3.1/reviser/interactivity/completions.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/interactivity/runner.py` & `reviser-0.3.1/reviser/interactivity/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import boto3
 
 from reviser import definitions
 from reviser import interactivity
 from reviser import parsing
 
 
-def create_shell(arguments: typing.List[str] = None) -> "interactivity.Shell":
+def create_shell(
+    arguments: typing.Optional[typing.List[str]] = None,
+) -> "interactivity.Shell":
     """
     Create a shell for interactive or queued command execution.
 
     The type of shell is based on the specified command line arguments, which default
     to sys.argv if no arguments are specified.
     """
     args = parsing.create_parser(True).parse_args(arguments)
@@ -28,16 +30,16 @@
         path=directory,
         connection=definitions.AwsConnection(session),
     )
     return interactivity.Shell(context)
 
 
 def run_shell(
-    arguments: typing.List[str] = None,
-    command_queue: typing.List[str] = None,
+    arguments: typing.Optional[typing.List[str]] = None,
+    command_queue: typing.Optional[typing.List[str]] = None,
 ) -> "interactivity.Shell":
     """
     Start the shell process.
 
     The shell is started after first loading configuration from the target
     directory determined by the command line arguments.
     """
```

### Comparing `reviser-0.3.0/reviser/interactivity/shells/__init__.py` & `reviser-0.3.1/reviser/interactivity/shells/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     def timestamp(self) -> str:
         """Get a string representation of the created at datetime."""
         return self.executed_at.strftime("%Y-%m-%dT%H:%M:%S.000Z")
 
     def finalize(
         self,
         status: str,
-        message: str = None,
-        info: dict = None,
-        data: dict = None,
+        message: typing.Optional[str] = None,
+        info: typing.Optional[dict] = None,
+        data: typing.Optional[dict] = None,
         echo: bool = False,
     ) -> "Execution":
         """Copy this execution and populate it with the result."""
         return dataclasses.replace(
             self,
             result=ExecutionResult(
                 status=(status or "???").upper(),
@@ -89,15 +89,15 @@
     Interactive lambda deployer interactivity class responsible for managing
     the state and interactivity for the interface.
     """
 
     def __init__(
         self,
         context: "definitions.Context",
-        selection: "definitions.Selection" = None,
+        selection: typing.Optional["definitions.Selection"] = None,
     ):
         """Create a new shell for queued and/or interactive execution."""
         self.command_history: typing.List[str] = []
         self.execution_history: typing.List["Execution"] = []
         self._prompt_session: typing.Optional[prompt_toolkit.PromptSession] = None
         self.context = context
         self.selection = selection or definitions.Selection()
```

### Comparing `reviser-0.3.0/reviser/interactivity/shells/prompt.jinja2` & `reviser-0.3.1/reviser/interactivity/shells/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/parsing.py` & `reviser-0.3.1/reviser/parsing.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/servicer/__init__.py` & `reviser-0.3.1/reviser/servicer/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/servicer/functioning/__init__.py` & `reviser-0.3.1/reviser/servicer/functioning/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/servicer/layering.py` & `reviser-0.3.1/reviser/servicer/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.0/reviser/templating/__init__.py` & `reviser-0.3.1/reviser/templating/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def _single_line_filter(value: str) -> str:
     """Reduce a string to a single line with no insignificant padding."""
     regex = re.compile(r"\s{2,}")
     return regex.sub(" ", (value or "").replace("\n", " ")).strip()
 
 
-def _colorize_filter(value: str, color: str = None) -> str:
+def _colorize_filter(value: str, color: typing.Optional[str] = None) -> str:
     """Apply ansi console coloring to the string."""
     if color_value := _COLOR_MAP.get((color or "").lower()):
         return f'{color_value}{value or ""}{colorama.Style.RESET_ALL}'
     return value
 
 
 _environment = Environment()
@@ -60,15 +60,15 @@
 
 
 def printer(location: str, **kwargs):
     """Render the template and prints it to stdout."""
     print(render(location, **kwargs))
 
 
-def print_error(message: str, error: Exception = None):
+def print_error(message: str, error: typing.Optional[Exception] = None):
     """
     Render an exception template to stdout.
 
     If error is specified, that will be rendered as a stacktrace as well.
     """
     stack_trace: typing.Optional[str]
     if error:
```

### Comparing `reviser-0.3.0/reviser/utils.py` & `reviser-0.3.1/reviser/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return f"{value} {unit}"
 
 
 def get_matching_bucket(
     buckets: typing.Union[None, str, dict],
     aws_account_id: str,
     aws_region: str,
-    default_bucket: str = None,
+    default_bucket: typing.Optional[str] = None,
 ):
     """Fetch a bucket name from the buckets argument."""
     if not buckets:
         return default_bucket
 
     if isinstance(buckets, str):
         return buckets
```

### Comparing `reviser-0.3.0/setup.py` & `reviser-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,1320 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: reviser
+Version: 0.3.1
+Summary: AWS Lambda function/layer version deployment manager.
+Home-page: https://gitlab.com/rocket-boosters/reviser
+License: MIT
+Keywords: aws,lambda
+Author: Scott Ernst
+Author-email: swernst@gmail.com
+Requires-Python: >=3.8.0,<3.12.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Provides-Extra: shell
+Requires-Dist: Jinja2 (>=2.11.2) ; extra == "shell"
+Requires-Dist: PyYAML (>=5.3.0) ; extra == "shell"
+Requires-Dist: boto3 (>=1.16.11) ; extra == "shell"
+Requires-Dist: colorama (>=0.4.4) ; extra == "shell"
+Requires-Dist: pipper (>=0.10.0) ; extra == "shell"
+Requires-Dist: prompt-toolkit (>=3.0.8) ; extra == "shell"
+Requires-Dist: toml (>=0.10.0) ; extra == "shell"
+Requires-Dist: urllib3 (<2.0)
+Requires-Dist: wheel (>=0.37.1) ; extra == "shell"
+Project-URL: Documentation, https://gitlab.com/rocket-boosters/reviser
+Project-URL: Repository, https://gitlab.com/rocket-boosters/reviser
+Description-Content-Type: text/markdown
 
-packages = \
-['reviser',
- 'reviser.bundling',
- 'reviser.commands',
- 'reviser.commands.helper',
- 'reviser.definitions',
- 'reviser.definitions.configurations',
- 'reviser.deploying',
- 'reviser.interactivity',
- 'reviser.interactivity.shells',
- 'reviser.servicer',
- 'reviser.servicer.functioning',
- 'reviser.templating']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'shell': ['boto3>=1.16.11',
-           'colorama>=0.4.4',
-           'Jinja2>=2.11.2',
-           'prompt-toolkit>=3.0.8',
-           'PyYAML>=5.3.0',
-           'pipper>=0.10.0',
-           'toml>=0.10.0',
-           'wheel>=0.37.1']}
-
-entry_points = \
-{'console_scripts': ['reviser = reviser.cli:main',
-                     'reviser-shell = reviser:main_shell']}
-
-setup_kwargs = {
-    'name': 'reviser',
-    'version': '0.3.0',
-    'description': 'AWS Lambda function/layer version deployment manager.',
-    'long_description': '# Reviser\n\n[![PyPI version](https://badge.fury.io/py/reviser.svg)](https://pypi.org/project/reviser/)\n[![build status](https://gitlab.com/rocket-boosters/reviser/badges/main/pipeline.svg)](https://gitlab.com/rocket-boosters/reviser/commits/main)\n[![coverage report](https://gitlab.com/rocket-boosters/reviser/badges/main/coverage.svg)](https://gitlab.com/rocket-boosters/reviser/commits/main)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Code style: flake8](https://img.shields.io/badge/code%20style-flake8-white)](https://gitlab.com/pycqa/flake8)\n[![Code style: mypy](https://img.shields.io/badge/code%20style-mypy-white)](http://mypy-lang.org/)\n[![PyPI - License](https://img.shields.io/pypi/l/reviser)](https://pypi.org/project/reviser/)\n\nReviser is a tool for AWS Lambda function and layer version deployment and\nalias management specifically for Python runtimes where the actual\ninfrastructure is managed separately, mostly likely by CloudFormation or\nTerraform. There are a number of ways to manage AWS Lambda functions and layers\nalready, but their generality and all-encompassing approaches don\'t integrate\nwell with certain workflows and can be overly complex for many needs.\n\nReviser is scoped to facilitate the deployment and updating of AWS Lambda\nPython functions and layers for all version-specific configurations,\ne.g. code bundles, environment variables, memory size, and timeout lengths.\nThe expectation is that functions are created by other means and then\nconfiguration for versions is managed with the reviser through an interactive\nor scripted shell of commands.\n\n- [Basic Usage](#basic-usage)\n- [Shell Commands](#shell-commands)\n   - [alias](#alias)\n   - [bundle](#bundle)\n   - [configs](#configs)\n   - [deploy](#deploy)\n   - [exit](#exit)\n   - [help (?)](#help-)\n   - [list](#list)\n   - [prune](#prune)\n   - [push](#push)\n   - [region](#region)\n   - [reload](#reload)\n   - [select](#select)\n   - [shell](#shell)\n   - [status](#status)\n   - [tail](#tail)\n- [Configuration Files](#configuration-files)\n   - [bucket(s)](#buckets)\n   - [AWS region](#aws-region)\n   - [targets](#targets)\n      - [targets[N].kind](#targetsnkind)\n      - [targets[N].name(s)](#targetsnnames)\n      - [targets[N].region](#targetsnregion)\n      - [targets[N].dependencies](#targetsndependencies)\n      - [targets[N].dependencies.skip](#targetsndependenciesskip)\n      - [targets[N].dependencies(kind="pipper")](#targetsndependencieskindpipper)\n      - [targets[N].dependencies(kind="poetry")](#targetsndependencieskindpoetry)\n      - [targets[N].bundle](#targetsnbundle)\n         - [targets[N].bundle.include(s)](#targetsnbundleincludes)\n         - [targets[N].bundle.exclude(s)](#targetsnbundleexcludes)\n         - [targets[N].bundle.exclude_package(s)](#targetsnbundleexclude_packages)\n         - [targets[N].bundle.omit_package(s)](#targetsnbundleomit_packages)\n         - [targets[N].bundle.handler](#targetsnbundlehandler)\n   - [function targets](#function-targets)\n      - [(function) targets[N].image](#function-targetsnimage)\n         - [(function) targets[N].image.uri](#function-targetsnimageuri)\n         - [(function) targets[N].image.entrypoint](#function-targetsnimageentrypoint)\n         - [(function) targets[N].image.cmd](#function-targetsnimagecmd)\n         - [(function) targets[N].image.workingdir](#function-targetsnimageworkingdir)\n      - [(function) targets[N].layer(s)](#function-targetsnlayers)\n      - [(function) targets[N].memory](#function-targetsnmemory)\n      - [(function) targets[N].timeout](#function-targetsntimeout)\n      - [(function) targets[N].variable(s)](#function-targetsnvariables)\n      - [(function) targets[N].ignore(s)](#function-targetsnignores)\n   - [run](#run)\n   - [Shared Dependencies](#shared-dependencies)\n- [Local Execution](#local-execution)\n\n# Basic Usage\n\nA project defines one or more lambda function configuration targets in a \n`lambda.yaml` file in the root project directory. The most basic configuration\nlooks like this:\n\n```yaml\nbucket: name-of-s3-bucket-for-code-uploads\ntargets:\n- kind: function\n  name: foo-function\n```\n\nThis configuration defines a single `foo-function` lambda function target that\nwill be managed by reviser. The expectation is that this function exists and\nwas created by another means, e.g. CloudFormation or Terraform. A bucket must\nbe specified to indicate where the zipped code bundles will be uploaded prior\nto them being applied to the target(s). The bucket must already exist as well.\n\nBy default the package will include no external, e.g. pip, package\ndependencies. It will search for the first folder in the directory where the\n`lambda.yaml` file is located that contains an `__init__.py` file, identifying\nthat folder as a Python source package for the function. It will also look for\na `lambda_function.py` alongside the `lambda.yaml` file to serve as the \nentrypoint. These will be included in the uploaded and deployed code bundle\nwhen a `push` or a `deploy` command is executed. These default settings can\nall be configured along with many more as will be outlined below.\n\nTo deploy this example project, install the reviser python library and\nstart the shell with the command `reviser` in your terminal of choice\nin the directory where the `lambda.yaml` file resides. Docker must be running\nand available in the terminal in which you execute this command, as reviser\nis a containerized shell environment that runs within a container that mimics\nthe actual AWS Lambda runtime environment. Then run the `push` command within\nthe launched shell to create and upload the bundled source code and publish\na new version of the `foo-function` lambda function with the uploaded results.\n\n# Shell commands\n\nThe reviser command starts an interactive shell within a Docker container \ncompatible with the AWS Python Lambda runtime. This shell contains various\ncommands for deploying and managing deployments of lambda functions and layers\ndefined in a project\'s `lambda.yaml` configuration file, the format of which\nis described later in this document. The shell commands are:\n\n## alias\n\nAssign an alias to the specified version of the selected or specified lambda\nfunction.\n\n```\nusage: alias [--function FUNCTION] [--yes] [--create] alias version\n\npositional arguments:\n  alias                Name of an existing alias to move to the specified\n                       version, or the name of an alias to create and assign\n                       to the specified function version if the --create flag\n                       is included to allow for creating a new alias.\n  version              Version of the function that the alias should be\n                       assigned to. This will either be an integer value or\n                       $LATEST. To see what versions are available for a given\n                       function use the list command.\n\noptional arguments:\n  --function FUNCTION  The alias command only acts on one function. This can\n                       be achieved either by selecting the function target via\n                       the select command, or specifying the function name to\n                       apply this change to with this flag.\n  --yes                By default this command will require input confirmation\n                       before carrying out the change. Specify this flag to\n                       skip input confirmation and proceed without a breaking\n                       prompt.\n  --create             When specified the alias will be created instead of\n                       reassigned. Use this to create and assign new aliases\n                       to a function. When this flag is not specified, the\n                       command will fail if the alias doesn\'t exist, which\n                       helps prevent accidental alias creation.\n\n```\n\nOr it will create a new alias and assign it to the specified version if the --create\nflag is included. To assign an existing `test` alias to version 42 of the selected\nfunction, the command would be:\n\n```\n> alias test 42\n```\n\nIf multiple functions are currently selected, use `--function=<NAME>`\nto identify the function to which the alias change will be applied.\n\n## bundle\n\nInstall dependencies and copies includes into a zipped file ready for\ndeployment.\n\n```\nusage: bundle [--reinstall] [--output OUTPUT]\n\noptional arguments:\n  --reinstall           Add this flag to reinstall dependencies on a repeated\n                        bundle operation. By default, dependencies will remain\n                        cached for the lifetime of the shell to speed up the\n                        bundling process. This will force dependencies to be\n                        installed even if they had been installed previously.\n  --output OUTPUT, -o OUTPUT\n                        Output the bundled artifacts into the specified output\n                        path.\n\n```\n\nThe resulting zip file is structured correctly to be deployed to the lambda\nfunction/layer target via an S3 upload and subsequent publish command.\n\n## configs\n\nDisplay the configs merged from its source file, dynamic values and defaults.\n\n```\nusage: configs\n\n```\n\nUse this to inspect and validate that the loaded configuration meets expectations when\nparsed into the reviser shell.\n\n## deploy\n\nUpload the bundled contents to the upload S3 bucket and then publish a new\nversion.\n\n```\nusage: deploy [--description DESCRIPTION] [--dry-run]\n\noptional arguments:\n  --description DESCRIPTION\n                        Specify a message to assign to the version published\n                        by the deploy command.\n  --dry-run             If set, the deploy operation will be exercised without\n                        actually carrying out the actions. This can be useful\n                        to validate the deploy process without side effects.\n\n```\n\nThis will be carried out for each of the lambda targets with that new bundle and\nany modified settings between the current configuration and that target\'s\nexisting configuration. This command will fail if a target being deployed\nhas not already been bundled.\n\n## exit\n\nExit the shell and returns to the parent terminal.\n\n```\nusage: exit\n\n```\n\n## help (?)\n\nDisplay help information on the commands available within the shell.\n\n```\nusage: help\n\n```\n\nAdditional help on each command can be found using the --help flag on the command in\nquestion.\n\n## list\n\nList versions of the specified lambda targets with info about each version.\n\n```\nusage: list\n\n```\n\n## prune\n\nRemove old function and/or layer versions for the selected targets.\n\n```\nusage: prune [--start START] [--end END] [--dry-run] [-y]\n\noptional arguments:\n  --start START  Keep versions lower (earlier/before) this one. A negative\n                 value can be specified for relative indexing in the same\n                 fashion as Python lists.\n  --end END      Do not prune versions higher than this value. A negative\n                 value can be specified for relative indexing in the same\n                 fashion as Python lists.\n  --dry-run      Echo pruning operation without actually executing it.\n  -y, --yes      Run the prune process without reviewing first.\n\n```\n\n## push\n\nCombined single command for bundling and deploying the selected targets.\n\n```\nusage: push [--reinstall] [--output OUTPUT] [--description DESCRIPTION]\n            [--dry-run]\n\noptional arguments:\n  --reinstall           Add this flag to reinstall dependencies on a repeated\n                        bundle operation. By default, dependencies will remain\n                        cached for the lifetime of the shell to speed up the\n                        bundling process. This will force dependencies to be\n                        installed even if they had been installed previously.\n  --output OUTPUT, -o OUTPUT\n                        Output the bundled artifacts into the specified output\n                        path.\n  --description DESCRIPTION\n                        Specify a message to assign to the version published\n                        by the deploy command.\n  --dry-run             If set, the deploy operation will be exercised without\n                        actually carrying out the actions. This can be useful\n                        to validate the deploy process without side effects.\n\n```\n\n## region\n\nSwitch the target region.\n\n```\nusage: region\n              [{us-east-2,us-east-1,us-west-1,us-west-2,af-south-1,ap-east-1,ap-south-1,ap-northeast-3,ap-northeast-2,ap-southeast-1,ap-southeast-2,ap-northeast-1,ca-central-1,cn-north-1,cn-northwest-1,eu-central-1,eu-west-1,eu-west-2,eu-south-1,eu-west-3,eu-north-1,me-south-1,sa-east-1,us-gov-east-1,us-gov-west-1}]\n\npositional arguments:\n  {us-east-2,us-east-1,us-west-1,us-west-2,af-south-1,ap-east-1,ap-south-1,ap-northeast-3,ap-northeast-2,ap-southeast-1,ap-southeast-2,ap-northeast-1,ca-central-1,cn-north-1,cn-northwest-1,eu-central-1,eu-west-1,eu-west-2,eu-south-1,eu-west-3,eu-north-1,me-south-1,sa-east-1,us-gov-east-1,us-gov-west-1}\n                        AWS region name for the override. Leave it blank to\n                        return to the default region for the initially loaded\n                        credentials and/or environment variables.\n\n```\n\n## reload\n\nReload the lambda.yaml configuration file from disk.\n\n```\nusage: reload\n\n```\n\n## select\n\nAllow for selecting subsets of the targets within the loaded configuration.\n\n```\nusage: select [--functions] [--layers] [--exact] [name ...]\n\npositional arguments:\n  name                  Specifies the value to match against the function and\n                        layer target names available from the configuration.\n                        This can include shell-style wildcards and will also\n                        match against partial strings. If the --exact flag is\n                        specified, this value must exactly match one of the\n                        targets instead of the default fuzzy matching\n                        behavior.\n\noptional arguments:\n  --functions, --function, --func, -f\n                        When specified, functions will be selected. This will\n                        default to true if neither of --functions or --layers\n                        is specified. Will default to false if --layers is\n                        specified.\n  --layers, --layer, -l\n                        When specified, layers will be selected. This will\n                        default to true if neither of --functions or --layers\n                        is specified. Will default to false if --functions is\n                        specified.\n  --exact               Forces the match to be exact instead of fuzzy.\n\n```\n\nThe subsets are fuzzy-matched unless the --exact flag is used.\n\n## shell\n\nMacro command to convert to interactive shell operation.\n\n```\nusage: shell\n\n```\n\nThis is a special command to use in run command groups/macros to start interactive\ncommand mode for the terminal. Useful when in scenarios where you wish to prefix an\ninteractive session with commonly executed commands. For example, if you want to select\ncertain targets with the select command as part of starting the shell, you could create\na run command group/macro in your lambda.yaml that executes the select command and then\nexecutes the shell command. This would updated the selection and then with the shell\ncommand, start the shell in interactive mode. Without specifying the shell command\nhere, the run command group/macro would just set a selection and then exit.\n\n## status\n\nShow the current status information for each of the selected lambda targets.\n\n```\nusage: status [qualifier]\n\npositional arguments:\n  qualifier  Specifies a version or alias to show status for. If not\n             specified, $LATEST will be used for functions and the latest\n             version will be dynamically determined for layers.\n\n```\n\n## tail\n\nTail the logs for the selected lambda functions.\n\n```\nusage: tail\n\n```\n    \nMore detail on any of these commands can be found from within the shell by\nexecuting them with the `--help` flag.\n\nThe reviser application also supports non-interactive batch command\nexecution via `run` macros that behave similarly to how `npm run <command>` \ncommands are defined. For more details see the `run` attribute section of the\nconfiguration file definitions below.\n\n# Configuration Files\n\nConfiguration files, named `lambda.yaml` define the lambda targets to be\nmanaged within a project. The top-level keys in the configuration file are:\n\n## bucket(s)\n\nThis key defines the bucket or buckets where zipped source bundles will be\nuploaded before they are deployed to their lambda function and/or layer\ntargets. Basic usage is to specify the bucket as a key:\n\n```yaml\nbucket: bucket-name\n```\n\nIt\'s also possible for multi-account scenarios to specify multiple buckets as\na key-value pairing where the keys are the AWS account IDs (as strings) and\nthe values are the bucket names associated with those IDs. In this case the\nbucket selection is made dynamically based on the AWS session loaded during\nshell initialization. Specifying multiple buckets looks like:\n\n```yaml\nbuckets:\n  "123456789": bucket-in-account-123456789\n  "987654321": bucket-in-account-987654321\n```\n\nMultiple region buckets can also be specified using the AWS region as the key:\n\n```yaml\nbuckets:\n  us-east-1: bucket-in-region-us-east-1\n  us-west-2: bucket-in-region-us-west-2\n```\n\nThese can be combined to define buckets for multiple accounts and multiple\nregions as:\n\n\n```yaml\nbuckets:\n  "123456789":\n    us-east-1: bucket-123456789-in-region-us-east-1\n    us-west-2: bucket-123456789-in-region-us-west-2\n  "987654321":\n    us-east-1: bucket-987654321-in-region-us-east-1\n    us-west-2: bucket-987654321-in-region-us-west-2\n```\n\n## AWS region\n\nThe AWS region in which the resources reside can be specified at the top\nlevel of the file if desired. It is recommended that the region be specified\nwithin the calling AWS profile if possible for flexibility, but there are\nsituations where it makes more sense to make it explicit within the\nconfiguration file instead. If no region is found either in the configuration\nfile or in the AWS profile the `us-east-1` region will be used as the default\nin keeping with AWS region defaulting conventions. Specify the region with\nthe top-level key:\n\n```yaml\nregion: us-east-2\n```\n\n## targets\n\nTargets is where the bulk of the configuration resides. Each item\nis either of the *function* or *layer* kind and has associated\nconfiguration and bundling settings according to the type. Common\nto both *function* and *layer* kinds are the keys:\n\n### targets[N].kind\n\nAs mentioned already, each target must specify its object type using\nthe kind key:\n\n```yaml\ntargets:\n- kind: function\n  ...\n- kind: layer\n  ...\n```\n\n### targets[N].name(s)\n\nThe name specifies the name of the target object, not the ARN. For example,\na function named foo would be represented as:\n\n```yaml\ntargets:```\n- kind: function\n  name: foo\n```\n\nA single target can point to multiple functions. This is useful in cases\nwhere a single target could be for both development and production functions\nor where a single code-base is shared across multiple functions for logical\nor integration reasons. In this case a list of names is supplied instead:\n\n```yaml\ntargets:\n- kind: function\n  names:\n  - foo-devel\n  - foo-prod\n```\n\n### targets[N].region\n\nIn the same fashion as regions can be explicitly set as a top-level\nconfiguration key, they can also be set on a per-target basis. If set,\nthe target region will take precedence over the top-level value and\nthe profile-specified value. This makes deploying code across regions\nwithin a single configuration file possible.\n\n### targets[N].dependencies\n\nDependencies is a list of external dependency sources to install as\nsite packages in the lambda function or layer. Multiple package managers\nare supported and specified by the `kind` attribute:\n\n```yaml\ntargets:\n- kind: layer\n  name: foo\n  dependencies:\n  - kind: pip\n  - kind: pipper\n  - kind: poetry\n```\n\nCurrently `pip`, `pipper` and `poetry` package managers are supported. For any of the\npackage managers, the dependencies can be specified explicitly with the\n`package(s)` key.\n\n```yaml\ntargets:\n- kind: layer\n  name: foo\n  dependencies:\n  - kind: pip\n    packages:\n    - spam\n    - hamd\n  - kind: pipper\n    package: spammer\n```\n\nIt\'s also possible to specify a file to where the package dependencies\nhave been defined.\n\n```yaml\ntargets:\n- kind: layer\n  name: foo\n  dependencies:\n  - kind: pip\n    file: requirements.layer.txt\n  - kind: pipper\n    file: pipper.layer.json\n```\n\nIf no packages or file is specified, the default file for the given package\nmanager will be used by default (e.g. `requirements.txt` for pip,\n `pipper.json` for pipper, and `pyproject.toml` for poetry).\n\nIt is also possible to specify the same kind of package manager multiple\ntimes in this list to aggregate dependencies from multiple locations.\n\n### targets[N].dependencies.skip\n\nIt is possible to specify inline dependencies to skip during the bundling installation\nprocess. This can be useful, for example, when a particular dependency is specific to\nplatforms other than the lambda environment. Or perhaps a package like boto3 that is\nalready available in the lambda function should be skipped to save bundling space while\nstill wanting to include it in the packages dependencies for beyond-lambda deployment\npurposes.\n\nAs shown below, specify the packages to skip within the dependency as part of the\ndependency definition:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  dependencies:\n  - kind: pip\n    skip:\n    - boto3\n```\n\n### targets[N].dependencies(kind="pipper")\n\nPipper repositories have additional configuration not associated with pip\npackages. To support pipper libraries, there are two additional attributes\nthat can be specified: `bucket` and `prefix`.\n\nThe `bucket` is required as it specifies the S3 bucket used as the package\nsource and should be read-accessible by the profile invoking reviser.\n\nThe `prefix` is an optional alternate package prefix within the S3 bucket.\nUse this only if you are using an alternate prefix with for your pipper\npackage.\n\n```yaml\ntargets:\n- kind: layer\n  name: foo\n  dependencies:\n  - kind: pipper\n    file: pipper.layer.json\n    bucket: bucket-name-where-pipper-package-resides\n    prefix: a/prefix/that/is/not/just/pipper\n```\n\n### targets[N].dependencies(kind="poetry")\n\nPoetry repositories have additional `extras` configuration that can be used to\nspecify optional dependency groups to install in the lambda. This can be useful\nto separate dependencies by function.\n\n```yaml\ntargets:\n- kind: layer\n  name: foo\n  dependencies:\n  - kind: poetry\n    extras:\n    - group\n```\n\n### targets[N].bundle\n\nThe target bundle object contains the attributes that define the bundle\nthat will be created and uploaded to the functions or layers in a given\ntarget as part of the deployment process. It\'s primary purpose is to define\nwhat files should be included in the bundling process, which it achieves\nwith the following attributes.\n\n#### targets[N].bundle.include(s)\n\nThe `include(s)` key is a string or list of Python glob-styled includes\nto add to the bundle. If no includes are specified, the default behavior is:\n\n- **function targets**: copy the first directory found that contains an\n  *__init__.py* file.\n- **layer targets**: do not copy anything and assume dependencies are the\n  only files to copy into the bundle.\n\nAll paths should be referenced relative to the root path where the\n`lambda.yaml` is located. For a recursive matching pattern, the glob syntax\nshould be used as `**/*.txt` or if restricted to a folder inside of the root\ndirectory then `folder/**/*.txt`. To include the entire contents of a\ndirectory, specify the path to the folder.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  bundle:\n    includes:\n    # This is shorthand for "foo_library/**/*"\n    - foo_library\n    # All Python files in the "bin/" folder recursively.\n    - bin/**/*.py\n    # All Jinja2 files in the root directory that begin "template_".\n    - template_*.jinja2\n```\n\n#### targets[N].bundle.exclude(s)\n\nThe `exclude(s)` key is an optional one that is also a string or list of\nPython glob-styled paths to remove from the matching `include(s)`. These\nare applied to the files found via the includes and do not need to be\ncomprehensive of all files in the root directory. Building on the example\nfrom above:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  bundle:\n    includes:\n    # This is shorthand for "foo_library/**/*"\n    - foo_library\n    # All Python files in the "bin/" folder recursively.\n    - bin/**/*.py\n    # All Jinja2 files in the root directory that begin "template_".\n    - template_*.jinja2\n    exclues:\n    - template_local.jinja2\n    - template_testing.jinja2\n```\n\nThis example would remove two of the template file matches from the includes\nfrom the files copied into the bundle for deployment.\n\nAll `__pycache__`, `*.pyc` and `.DS_Store` files/directories are\nexcluded from the copying process in all cases and do not need to be\nspecified explicitly.\n\n\n#### targets[N].bundle.exclude_package(s)\n\nThe `package_exclude(s)` key is an optional one that is also a string or list of\nPython glob-styled paths. However, these are for paths to exclude when adding\nsite-packages to the bundle. Building on the example from above:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  bundle:\n    includes:\n    # This is shorthand for "foo_library/**/*"\n    - foo_library\n    # All Python files in the "bin/" folder recursively.\n    - bin/**/*.py\n    # All Jinja2 files in the root directory that begin "template_".\n    - template_*.jinja2\n    exclues:\n    - template_local.jinja2\n    - template_testing.jinja2\n    package_excludes:\n    - foo/foo_windows.py\n  dependencies:\n  - kind: pip\n```\n\nThis example would not include the `site-packages/foo/foo_windows.py` from the\nbundled zip file for the lambda function. In this case, the reason for omitting\nthis file is that "Windows" code isn\'t needed in a linux runtime, so you want to\nsave some space. This is more likely useful for large packages that include\nunneeded components, and it is desirable to save the space. This should be used\nvery carefully as it can cause external libraries to fail.\n\n#### targets[N].bundle.omit_package(s)\n\nThere can be cases where dependencies install dependencies of their own that\nyou may not want copied over to the bundle. The most common case is a\ndependency that requires `boto3`, which is available by default in lambda\nfunctions already. In that case it can be useful to list site packages that\nshould not be copied into the bundle but may have been installed as a side\neffect of the dependency installation process.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  bundle:\n    omit_package: boto3\n  dependencies:\n  - kind: pip\n    # Installs a package that requires boto3, which is therefore installed\n    # into the site-packages bundle directory as a result.\n    # https://github.com/awslabs/aws-lambda-powertools-python\n    package: aws-lambda-powertools\n```\n\nIn the above example `aws-lambda-powertools` causes `boto3` to be installed\nas well. However, since lambda functions have `boto3` installed by default,\nit\'s possible to omit that package from the bundling process so that it isn\'t\ninstalled twice.\n\nNote, however, that installing `boto3` directly in a bundle can be beneficial\nbecause it gives you the ability to install the version that is compatible\nwith your given source code and dependencies. The `boto3` version on the lambda\nfunction can be aged and stale.\n\n#### targets[N].bundle.handler\n\nThis attribute only applies to function targets and gives the location of\nfile and function entrypoint for the lambda function(s) in the target. The\nformat matches the expected value for lambda functions, which is\n`<filename_without_extension>.<function_name>`.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  bundle:\n    handler: function:main\n```\n\nIn this case the bundler would expect to find `function.py` in the top-leve\ndirectory alongside `lambda.yaml` and inside it there would be a\n`main(event, context)` function that would be called when the function(s)\nare invoked.\n\nIf this value is omitted, the default value of `lambda_function.lambda_handler`\nwill be used as this matches the AWS lambda Python function documentation.\n\n## function targets\n\nIn addition to the common attributes described above that are shared between\nboth function and layer targets, there are a number of additional\nattributes that apply only to function targets. These are:\n\n### (function) targets[N].image\n\nSpecifies the configuration of the image for image based lambda functions.\nThis cannot be used with `targets[N].bundle`. With the exception of `uri`\nall subfields are optional.\n\n```yaml\nimage:\n  uri: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag\n  entrypoint: /my/entrypoint\n  cmd:\n  - params\n  - to\n  - entrypoint\n  workingdir: /the/working/dir\n```\n\n#### (function) targets[N].image.uri\n\nThe image uri for the function\'s image. This must be a ECR uri that resides\nwithin the same region as the lambda function. If the lambda function is\ndeployed to a single region this can be configured with a string:\n\n```yaml\nuri: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag\n```\n\nIf the lambda function is deployed to multiple regions it can be configured\nwith a dictionary mapping region names to images.\n\n```yaml\nuri:\n  us-west-2: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag\n  us-east-2: 123456789012.dkr.ecr.us-east-2.amazonaws.com/repo:tag\n```\n\n#### (function) targets[N].image.entrypoint\n\nA custom entrypoint to use for the image. If this is not specified the\nentrypoint of the image will be used. This can be specified as a list or\nas a single string that will be treated as a list with one element.\n\n```yaml\nentrypoint: /my/entrypoint\n```\n\nor\n\n```yaml\nentrypoint:\n- /my/entrypoint\n```\n\n#### (function) targets[N].image.cmd\n\nA custom command to use for the image. If this is not specified the default\ncommand of the image will be used. This can be specified as a list or\nas a single string that will be treated as a list with one element.\n\n```yaml\ncmd: a_command\n```\n\nor\n\n```yaml\ncmd:\n- a_command\n- with\n- multiple\n- words\n```\n\n#### (function) targets[N].image.workingdir\n\nA custom working directory to set for the image. If this is not specified\nthe default working directory of the image will be used.\n\n```yaml\nworkingdir: /my/working/dir\n```\n\n### (function) targets[N].layer(s)\n\nSpecifies one or more layers that should be attached to the targeted\nfunction(s). Layers can be specified as fully-qualified ARNs for externally\nspecified layers, e.g. a layer created in another AWS account, or by name\nfor layers specified within the account and layers defined within the targets\nof the configuration file.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  layer: arn:aws:lambda:us-west-2:999999999:layer:bar\n  ...\n```\n\nor for multiple layers:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  layers:\n  # A layer defined in another account is specified by ARN.\n  - arn:aws:lambda:us-west-2:999999999:layer:bar\n  # A layer in this account is specified by name. This layer may also be\n  # a target in this configuration file.\n  - baz\n  ...\n- kind: layer\n  name: baz\n  ...\n```\n\nBy default, deployments will use the latest available version of each layer,\nbut this can be overridden by specifying the layer ARN with its version:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  layer: arn:aws:lambda:us-west-2:999999999:layer:bar:42\n  ...\n```\n\nIn the above example the layer will remain at version 42 until explicitly\nmodified in the configuration file.\n\nLayers can also be defined as objects instead of attributes. The two-layer\nexample from above could be rewritten as:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  layers:\n  - arn: arn:aws:lambda:us-west-2:999999999:layer:bar\n  - name: baz\n  ...\n```\n\nWhen specified as an object with attributes, there are a number of additional\nattributes that can be specified as well. First, `version` can be specified\nas a separate key from the arn or name, which in many cases can make it easier\nto work with than appending it to the end of the arn or function itself for\nprogrammatic/automation:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  layers:\n  - arn: arn:aws:lambda:us-west-2:999999999:layer:bar\n    version: 42\n  - name: baz\n    version: 123\n  ...\n```\n\nNext is that the layer objects accept `only` and `except` keys that can be\nused to attach the layers to certain functions in the target and not others.\nThis can be useful in cases where development and production targets share\na lot in common, but perhaps point to different versions of a layer or perhaps\nseparate development and production layers entirely. It can also be useful\nwhen a target of functions share a common codebase but don\'t all need the\nsame dependencies. For performance optimization, restricting the layer\ninclusions only to those that need the additional dependencies can be\nbeneficial.\n\nThe `only` and `except` attributes can be specified as a single string\nor a list of strings that match against *unix pattern matching*. For example,\nexpanding on the example from above:\n\n```yaml\ntargets:\n- kind: function\n  names:\n  - foo-devel\n  - foo-devel-worker\n  - foo-prod\n  - foo-prod-worker\n  layers:\n  - name: baz-devel\n    only: foo-devel*\n  - name: baz-devel-worker\n    only: foo-devel-worker\n  - name: baz-prod\n    only: foo-prod*\n  - name: baz-prod-worker\n    only: foo-prod-worker\n  ...\n```\n\nthis example shows 4 layers that are conditionally applied using the only\nkeyword. The example could be rewritten with the `except` key instead:\n\n```yaml\ntargets:\n- kind: function\n  names:\n  - foo-devel\n  - foo-devel-worker\n  - foo-prod\n  - foo-prod-worker\n  layers:\n  - name: baz-devel\n    except: foo-prod*\n  - name: baz-devel-worker\n    except:\n    - foo-prod*\n    - foo-devel\n  - name: baz-prod\n    except: foo-devel*\n  - name: baz-prod-worker\n    except:\n    - foo-devel*\n    - foo-prod\n  ...\n```\n\nAnd either way works. The two (`only` and `except`) can also be combined\nwhen that makes more sense. For example, the `baz-devel-worker` from above\ncould also be written as:\n\n```yaml\n  - name: baz-devel-worker\n    only: foo-devel*\n    except: foo-devel\n```\n\nNote that if `only` is specified it is processed first and then `except` is\nremoved from the matches found by `only`.\n\n### (function) targets[N].memory\n\nThis specifies the function memory in megabytes either as an integer or\na string with an `MB` suffix.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  memory: 256MB\n```\n\n### (function) targets[N].timeout\n\nThis specifies the function timeout in seconds either as an integer or\na string with an `s` suffix.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  timeout: 42s\n```\n\n### (function) targets[N].variable(s)\n\nVariables contains a list of environment variables to assign to the function.\nThey can be specified simply with as a string `<KEY>=<value>` syntax:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  variable: MODE=read-only\n```\n\nHere a single environment variable is specified that maps `"MODE"` to the\nvalue *"ready-only"*. A more programmatic-friendly way is to specify the\nname and value as attributes of a variable:\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  variables:\n  - name: MODE\n    value: read-only\n```\n\nSome environment variables may be managed through other means, e.g.\nterraform that created the function in the first place or another command\ninterface used to update the function. For those cases, the `preserve`\nattribute should be set to true and no value specified.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  variables:\n  - name: MODE\n    preserve: true\n```\n\nIn this case the `MODE` environment variable value will be preserved between\nfunction deployments to contain the value that was already set.\n\nFinally, variables support the same `only` and `exclude` attributes that\nare found for target layers so that environment variables can be specified\ndifferently for subsets of targets.\n\nThe `only` and `except` attributes can be specified as a single string\nor a list of strings that match against *unix pattern matching*. For example,\nexpanding on the example from above:\n\n```yaml\ntargets:\n- kind: function\n  names:\n  - foo-prod\n  - foo-devel\n  variables:\n  - name: MODE\n    value: write\n    only: \'*prod\'\n  - name: MODE\n    value: read-only\n    except: \'*prod\'\n```\n\n### (function) targets[N].ignore(s)\n\nIgnores allows you to specify one or more configuration keys within a function\ntarget that should be ignored during deployments. For cases where any of the\nconfiguration values:\n\n- `memory`\n- `timeout`\n- `variables`\n\nare managed by external systems, they can be specified by the ignores to\nprevent changes being applied by reviser.\n\n```yaml\ntargets:\n- kind: function\n  name: foo\n  ignores:\n  - memory\n  - timeout\n```\n\n## run\n\nThe run attribute contains an optional object of batch non-interactive commands\nto run when the shell is called with that run key. This is useful for\norchestrating actions for CI/CD purposes as the commands will be processed\nwithin a shell environment without user prompts and then the shell will exit\nwhen complete without waiting for additional input.\n\n```yaml\nrun:\n  deploy-prod:\n  - select function *prod\n  - push --description="($CI_COMMIT_SHORT_SHA): $CI_COMMIT_TITLE"\n  - alias test -1\ntargets:\n- kind: function\n  names:\n  - foo-prod\n  - foo-devel\n```\n\nIn the example above, the `deploy-prod` run command macro/group would start\nthe shell and then non-interactively execute the three commands in order\nto first select the *foo-prod* function, then to build and deploy that function\nwith a description created from CI environment variables and finally move the\n*test* alias to the newly deployed version using a negative version index of\n*-1*. After those three commands are executed reviser will exit the\nshell automatically, successfully ending that process.\n\nThere is also a special `shell` command that can be used in run command\nmacros/groups that will start the shell in interactive mode. This is useful\nfor using run command macros/groups for pre-configuration during startup of\nthe interactive shell. Building on the previous example,\n\n```yaml\nrun:\n  deploy-prod:\n  - select function *prod\n  - push --description="($CI_COMMIT_SHORT_SHA): $CI_COMMIT_TITLE"\n  - alias test -1\n  devel:\n  - select * *devel\n  - bundle\n  - shell\ntargets:\n- kind: function\n  names:\n  - foo-prod\n  - foo-devel\n- kind: layer\n  names:\n  - bar-devel\n  - bar-prod\n```\n\nhere we\'ve added a `devel` run command macro/group that will select the devel\nfunction and layer and bundle those but not deploy them. After that\'s complete\nthe shell command will kick off the interactive session and ask for user\ninput. The benefit of this particular run command macro/group is to select\nthe development targets and pre-build them to cache the dependencies for the\nshell user while they continue to develop and deploy the source code to the\nfunction.\n\n## Shared Dependencies\n\nIt is possible to share dependencies across targets. This is useful if the dependencies\nare the same but other configurations differ. The configuration will look something\nlike this:\n\n```yaml\n\ndependencies:\n  # Each shared dependency must be named, but the name can be any valid yaml key that\n  # you want.\n  shared_by_my_foo_and_bar:\n  - kind: pip\n    file: requirements.functions.txt\n  shared_by_others:\n  - kind: pip\n    file: requirements.layer.txt\n    \ntargets:\n- kind: function\n  names:\n  - foo-prod\n  - foo-devel\n  timeout: 30s\n  memory: 256\n  dependencies: shared_by_my_foo_and_bar\n\n- kind: function\n  names:\n  - bar-prod\n  - bar-devel\n  timeout: 500s\n  memory: 2048\n  dependencies: shared_by_my_foo_and_bar\n\n- kind: function\n  names:\n  - baz-prod\n  - baz-devel\n  timeout: 10s\n  memory: 128\n  dependencies: shared_by_others\n\n- kind: layer\n  names:\n  - spam-prod\n  - spam-devel\n  dependencies: shared_by_others\n```\n\nShared dependencies will be installed once reused by each target configured to use\nit. Each name shared dependency has the same structure and available options of a\nregular target dependencies definition.\n\n\n\n# Local Execution\n\nWhen running reviser in your current environment instead of launching the shell within\na new container, you will want to use the command `reviser-shell`. This is the local\nversion of the CLI that is meant to be used within a suitable container environment\nthat mimics the lambda runtime environment. It is merely a change in entrypoint, and\nhas all the shell functionality described for the `reviser` command above.\n\nAlso, to run the `reviser-shell` successfully, you must install the extra shell\ndependencies with the installation:\n\n```shell\n$ pip install reviser[shell]\n```\n\nWithout the shell extras install, the `reviser-shell` will fail. This is how you would\nuse reviser in a containerized CI environment as well.',
-    'author': 'Scott Ernst',
-    'author_email': 'swernst@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/rocket-boosters/reviser',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.0,<3.10.0',
-}
+# Reviser
 
+[![PyPI version](https://badge.fury.io/py/reviser.svg)](https://pypi.org/project/reviser/)
+[![build status](https://gitlab.com/rocket-boosters/reviser/badges/main/pipeline.svg)](https://gitlab.com/rocket-boosters/reviser/commits/main)
+[![coverage report](https://gitlab.com/rocket-boosters/reviser/badges/main/coverage.svg)](https://gitlab.com/rocket-boosters/reviser/commits/main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Code style: flake8](https://img.shields.io/badge/code%20style-flake8-white)](https://gitlab.com/pycqa/flake8)
+[![Code style: mypy](https://img.shields.io/badge/code%20style-mypy-white)](http://mypy-lang.org/)
+[![PyPI - License](https://img.shields.io/pypi/l/reviser)](https://pypi.org/project/reviser/)
 
-setup(**setup_kwargs)
+Reviser is a tool for AWS Lambda function and layer version deployment and
+alias management specifically for Python runtimes where the actual
+infrastructure is managed separately, mostly likely by CloudFormation or
+Terraform. There are a number of ways to manage AWS Lambda functions and layers
+already, but their generality and all-encompassing approaches don't integrate
+well with certain workflows and can be overly complex for many needs.
+
+Reviser is scoped to facilitate the deployment and updating of AWS Lambda
+Python functions and layers for all version-specific configurations,
+e.g. code bundles, environment variables, memory size, and timeout lengths.
+The expectation is that functions are created by other means and then
+configuration for versions is managed with the reviser through an interactive
+or scripted shell of commands.
+
+- [Basic Usage](#basic-usage)
+- [Shell Commands](#shell-commands)
+   - [alias](#alias)
+   - [bundle](#bundle)
+   - [configs](#configs)
+   - [deploy](#deploy)
+   - [exit](#exit)
+   - [help (?)](#help-)
+   - [list](#list)
+   - [prune](#prune)
+   - [push](#push)
+   - [region](#region)
+   - [reload](#reload)
+   - [select](#select)
+   - [shell](#shell)
+   - [status](#status)
+   - [tail](#tail)
+- [Configuration Files](#configuration-files)
+   - [bucket(s)](#buckets)
+   - [AWS region](#aws-region)
+   - [targets](#targets)
+      - [targets[N].kind](#targetsnkind)
+      - [targets[N].name(s)](#targetsnnames)
+      - [targets[N].region](#targetsnregion)
+      - [targets[N].dependencies](#targetsndependencies)
+      - [targets[N].dependencies.skip](#targetsndependenciesskip)
+      - [targets[N].dependencies(kind="pipper")](#targetsndependencieskindpipper)
+      - [targets[N].dependencies(kind="poetry")](#targetsndependencieskindpoetry)
+      - [targets[N].bundle](#targetsnbundle)
+         - [targets[N].bundle.include(s)](#targetsnbundleincludes)
+         - [targets[N].bundle.exclude(s)](#targetsnbundleexcludes)
+         - [targets[N].bundle.exclude_package(s)](#targetsnbundleexclude_packages)
+         - [targets[N].bundle.omit_package(s)](#targetsnbundleomit_packages)
+         - [targets[N].bundle.handler](#targetsnbundlehandler)
+   - [function targets](#function-targets)
+      - [(function) targets[N].image](#function-targetsnimage)
+         - [(function) targets[N].image.uri](#function-targetsnimageuri)
+         - [(function) targets[N].image.entrypoint](#function-targetsnimageentrypoint)
+         - [(function) targets[N].image.cmd](#function-targetsnimagecmd)
+         - [(function) targets[N].image.workingdir](#function-targetsnimageworkingdir)
+      - [(function) targets[N].layer(s)](#function-targetsnlayers)
+      - [(function) targets[N].memory](#function-targetsnmemory)
+      - [(function) targets[N].timeout](#function-targetsntimeout)
+      - [(function) targets[N].variable(s)](#function-targetsnvariables)
+      - [(function) targets[N].ignore(s)](#function-targetsnignores)
+   - [run](#run)
+   - [Shared Dependencies](#shared-dependencies)
+- [Local Execution](#local-execution)
+
+# Basic Usage
+
+A project defines one or more lambda function configuration targets in a 
+`lambda.yaml` file in the root project directory. The most basic configuration
+looks like this:
+
+```yaml
+bucket: name-of-s3-bucket-for-code-uploads
+targets:
+- kind: function
+  name: foo-function
+```
+
+This configuration defines a single `foo-function` lambda function target that
+will be managed by reviser. The expectation is that this function exists and
+was created by another means, e.g. CloudFormation or Terraform. A bucket must
+be specified to indicate where the zipped code bundles will be uploaded prior
+to them being applied to the target(s). The bucket must already exist as well.
+
+By default the package will include no external, e.g. pip, package
+dependencies. It will search for the first folder in the directory where the
+`lambda.yaml` file is located that contains an `__init__.py` file, identifying
+that folder as a Python source package for the function. It will also look for
+a `lambda_function.py` alongside the `lambda.yaml` file to serve as the 
+entrypoint. These will be included in the uploaded and deployed code bundle
+when a `push` or a `deploy` command is executed. These default settings can
+all be configured along with many more as will be outlined below.
+
+To deploy this example project, install the reviser python library and
+start the shell with the command `reviser` in your terminal of choice
+in the directory where the `lambda.yaml` file resides. Docker must be running
+and available in the terminal in which you execute this command, as reviser
+is a containerized shell environment that runs within a container that mimics
+the actual AWS Lambda runtime environment. Then run the `push` command within
+the launched shell to create and upload the bundled source code and publish
+a new version of the `foo-function` lambda function with the uploaded results.
+
+# Shell commands
+
+The reviser command starts an interactive shell within a Docker container 
+compatible with the AWS Python Lambda runtime. This shell contains various
+commands for deploying and managing deployments of lambda functions and layers
+defined in a project's `lambda.yaml` configuration file, the format of which
+is described later in this document. The shell commands are:
+
+## alias
+
+Assign an alias to the specified version of the selected or specified lambda
+function.
+
+```
+usage: alias [--function FUNCTION] [--yes] [--create] alias version
+
+positional arguments:
+  alias                Name of an existing alias to move to the specified
+                       version, or the name of an alias to create and assign
+                       to the specified function version if the --create flag
+                       is included to allow for creating a new alias.
+  version              Version of the function that the alias should be
+                       assigned to. This will either be an integer value or
+                       $LATEST. To see what versions are available for a given
+                       function use the list command.
+
+options:
+  --function FUNCTION  The alias command only acts on one function. This can
+                       be achieved either by selecting the function target via
+                       the select command, or specifying the function name to
+                       apply this change to with this flag.
+  --yes                By default this command will require input confirmation
+                       before carrying out the change. Specify this flag to
+                       skip input confirmation and proceed without a breaking
+                       prompt.
+  --create             When specified the alias will be created instead of
+                       reassigned. Use this to create and assign new aliases
+                       to a function. When this flag is not specified, the
+                       command will fail if the alias doesn't exist, which
+                       helps prevent accidental alias creation.
+
+```
+
+Or it will create a new alias and assign it to the specified version if the --create
+flag is included. To assign an existing `test` alias to version 42 of the selected
+function, the command would be:
+
+```
+> alias test 42
+```
+
+If multiple functions are currently selected, use `--function=<NAME>`
+to identify the function to which the alias change will be applied.
+
+## bundle
+
+Install dependencies and copies includes into a zipped file ready for
+deployment.
+
+```
+usage: bundle [--reinstall] [--output OUTPUT]
+
+options:
+  --reinstall           Add this flag to reinstall dependencies on a repeated
+                        bundle operation. By default, dependencies will remain
+                        cached for the lifetime of the shell to speed up the
+                        bundling process. This will force dependencies to be
+                        installed even if they had been installed previously.
+  --output OUTPUT, -o OUTPUT
+                        Output the bundled artifacts into the specified output
+                        path.
+
+```
+
+The resulting zip file is structured correctly to be deployed to the lambda
+function/layer target via an S3 upload and subsequent publish command.
+
+## configs
+
+Display the configs merged from its source file, dynamic values and defaults.
+
+```
+usage: configs
+
+```
+
+Use this to inspect and validate that the loaded configuration meets expectations when
+parsed into the reviser shell.
+
+## deploy
+
+Upload the bundled contents to the upload S3 bucket and then publish a new
+version.
+
+```
+usage: deploy [--description DESCRIPTION] [--dry-run]
+
+options:
+  --description DESCRIPTION
+                        Specify a message to assign to the version published
+                        by the deploy command.
+  --dry-run             If set, the deploy operation will be exercised without
+                        actually carrying out the actions. This can be useful
+                        to validate the deploy process without side effects.
+
+```
+
+This will be carried out for each of the lambda targets with that new bundle and
+any modified settings between the current configuration and that target's
+existing configuration. This command will fail if a target being deployed
+has not already been bundled.
+
+## exit
+
+Exit the shell and returns to the parent terminal.
+
+```
+usage: exit
+
+```
+
+## help (?)
+
+Display help information on the commands available within the shell.
+
+```
+usage: help
+
+```
+
+Additional help on each command can be found using the --help flag on the command in
+question.
+
+## list
+
+List versions of the specified lambda targets with info about each version.
+
+```
+usage: list
+
+```
+
+## prune
+
+Remove old function and/or layer versions for the selected targets.
+
+```
+usage: prune [--start START] [--end END] [--dry-run] [-y]
+
+options:
+  --start START  Keep versions lower (earlier/before) this one. A negative
+                 value can be specified for relative indexing in the same
+                 fashion as Python lists.
+  --end END      Do not prune versions higher than this value. A negative
+                 value can be specified for relative indexing in the same
+                 fashion as Python lists.
+  --dry-run      Echo pruning operation without actually executing it.
+  -y, --yes      Run the prune process without reviewing first.
+
+```
+
+## push
+
+Combined single command for bundling and deploying the selected targets.
+
+```
+usage: push [--reinstall] [--output OUTPUT] [--description DESCRIPTION]
+            [--dry-run]
+
+options:
+  --reinstall           Add this flag to reinstall dependencies on a repeated
+                        bundle operation. By default, dependencies will remain
+                        cached for the lifetime of the shell to speed up the
+                        bundling process. This will force dependencies to be
+                        installed even if they had been installed previously.
+  --output OUTPUT, -o OUTPUT
+                        Output the bundled artifacts into the specified output
+                        path.
+  --description DESCRIPTION
+                        Specify a message to assign to the version published
+                        by the deploy command.
+  --dry-run             If set, the deploy operation will be exercised without
+                        actually carrying out the actions. This can be useful
+                        to validate the deploy process without side effects.
+
+```
+
+## region
+
+Switch the target region.
+
+```
+usage: region
+              [{us-east-2,us-east-1,us-west-1,us-west-2,af-south-1,ap-east-1,ap-south-1,ap-northeast-3,ap-northeast-2,ap-southeast-1,ap-southeast-2,ap-northeast-1,ca-central-1,cn-north-1,cn-northwest-1,eu-central-1,eu-west-1,eu-west-2,eu-south-1,eu-west-3,eu-north-1,me-south-1,sa-east-1,us-gov-east-1,us-gov-west-1}]
+
+positional arguments:
+  {us-east-2,us-east-1,us-west-1,us-west-2,af-south-1,ap-east-1,ap-south-1,ap-northeast-3,ap-northeast-2,ap-southeast-1,ap-southeast-2,ap-northeast-1,ca-central-1,cn-north-1,cn-northwest-1,eu-central-1,eu-west-1,eu-west-2,eu-south-1,eu-west-3,eu-north-1,me-south-1,sa-east-1,us-gov-east-1,us-gov-west-1}
+                        AWS region name for the override. Leave it blank to
+                        return to the default region for the initially loaded
+                        credentials and/or environment variables.
+
+```
+
+## reload
+
+Reload the lambda.yaml configuration file from disk.
+
+```
+usage: reload
+
+```
+
+## select
+
+Allow for selecting subsets of the targets within the loaded configuration.
+
+```
+usage: select [--functions] [--layers] [--exact] [name ...]
+
+positional arguments:
+  name                  Specifies the value to match against the function and
+                        layer target names available from the configuration.
+                        This can include shell-style wildcards and will also
+                        match against partial strings. If the --exact flag is
+                        specified, this value must exactly match one of the
+                        targets instead of the default fuzzy matching
+                        behavior.
+
+options:
+  --functions, --function, --func, -f
+                        When specified, functions will be selected. This will
+                        default to true if neither of --functions or --layers
+                        is specified. Will default to false if --layers is
+                        specified.
+  --layers, --layer, -l
+                        When specified, layers will be selected. This will
+                        default to true if neither of --functions or --layers
+                        is specified. Will default to false if --functions is
+                        specified.
+  --exact               Forces the match to be exact instead of fuzzy.
+
+```
+
+The subsets are fuzzy-matched unless the --exact flag is used.
+
+## shell
+
+Macro command to convert to interactive shell operation.
+
+```
+usage: shell
+
+```
+
+This is a special command to use in run command groups/macros to start interactive
+command mode for the terminal. Useful when in scenarios where you wish to prefix an
+interactive session with commonly executed commands. For example, if you want to select
+certain targets with the select command as part of starting the shell, you could create
+a run command group/macro in your lambda.yaml that executes the select command and then
+executes the shell command. This would updated the selection and then with the shell
+command, start the shell in interactive mode. Without specifying the shell command
+here, the run command group/macro would just set a selection and then exit.
+
+## status
+
+Show the current status information for each of the selected lambda targets.
+
+```
+usage: status [qualifier]
+
+positional arguments:
+  qualifier  Specifies a version or alias to show status for. If not
+             specified, $LATEST will be used for functions and the latest
+             version will be dynamically determined for layers.
+
+```
+
+## tail
+
+Tail the logs for the selected lambda functions.
+
+```
+usage: tail
+
+```
+    
+More detail on any of these commands can be found from within the shell by
+executing them with the `--help` flag.
+
+The reviser application also supports non-interactive batch command
+execution via `run` macros that behave similarly to how `npm run <command>` 
+commands are defined. For more details see the `run` attribute section of the
+configuration file definitions below.
+
+# Configuration Files
+
+Configuration files, named `lambda.yaml` define the lambda targets to be
+managed within a project. The top-level keys in the configuration file are:
+
+## bucket(s)
+
+This key defines the bucket or buckets where zipped source bundles will be
+uploaded before they are deployed to their lambda function and/or layer
+targets. Basic usage is to specify the bucket as a key:
+
+```yaml
+bucket: bucket-name
+```
+
+It's also possible for multi-account scenarios to specify multiple buckets as
+a key-value pairing where the keys are the AWS account IDs (as strings) and
+the values are the bucket names associated with those IDs. In this case the
+bucket selection is made dynamically based on the AWS session loaded during
+shell initialization. Specifying multiple buckets looks like:
+
+```yaml
+buckets:
+  "123456789": bucket-in-account-123456789
+  "987654321": bucket-in-account-987654321
+```
+
+Multiple region buckets can also be specified using the AWS region as the key:
+
+```yaml
+buckets:
+  us-east-1: bucket-in-region-us-east-1
+  us-west-2: bucket-in-region-us-west-2
+```
+
+These can be combined to define buckets for multiple accounts and multiple
+regions as:
+
+
+```yaml
+buckets:
+  "123456789":
+    us-east-1: bucket-123456789-in-region-us-east-1
+    us-west-2: bucket-123456789-in-region-us-west-2
+  "987654321":
+    us-east-1: bucket-987654321-in-region-us-east-1
+    us-west-2: bucket-987654321-in-region-us-west-2
+```
+
+## AWS region
+
+The AWS region in which the resources reside can be specified at the top
+level of the file if desired. It is recommended that the region be specified
+within the calling AWS profile if possible for flexibility, but there are
+situations where it makes more sense to make it explicit within the
+configuration file instead. If no region is found either in the configuration
+file or in the AWS profile the `us-east-1` region will be used as the default
+in keeping with AWS region defaulting conventions. Specify the region with
+the top-level key:
+
+```yaml
+region: us-east-2
+```
+
+## targets
+
+Targets is where the bulk of the configuration resides. Each item
+is either of the *function* or *layer* kind and has associated
+configuration and bundling settings according to the type. Common
+to both *function* and *layer* kinds are the keys:
+
+### targets[N].kind
+
+As mentioned already, each target must specify its object type using
+the kind key:
+
+```yaml
+targets:
+- kind: function
+  ...
+- kind: layer
+  ...
+```
+
+### targets[N].name(s)
+
+The name specifies the name of the target object, not the ARN. For example,
+a function named foo would be represented as:
+
+```yaml
+targets:```
+- kind: function
+  name: foo
+```
+
+A single target can point to multiple functions. This is useful in cases
+where a single target could be for both development and production functions
+or where a single code-base is shared across multiple functions for logical
+or integration reasons. In this case a list of names is supplied instead:
+
+```yaml
+targets:
+- kind: function
+  names:
+  - foo-devel
+  - foo-prod
+```
+
+### targets[N].region
+
+In the same fashion as regions can be explicitly set as a top-level
+configuration key, they can also be set on a per-target basis. If set,
+the target region will take precedence over the top-level value and
+the profile-specified value. This makes deploying code across regions
+within a single configuration file possible.
+
+### targets[N].dependencies
+
+Dependencies is a list of external dependency sources to install as
+site packages in the lambda function or layer. Multiple package managers
+are supported and specified by the `kind` attribute:
+
+```yaml
+targets:
+- kind: layer
+  name: foo
+  dependencies:
+  - kind: pip
+  - kind: pipper
+  - kind: poetry
+```
+
+Currently `pip`, `pipper` and `poetry` package managers are supported. For any of the
+package managers, the dependencies can be specified explicitly with the
+`package(s)` key.
+
+```yaml
+targets:
+- kind: layer
+  name: foo
+  dependencies:
+  - kind: pip
+    packages:
+    - spam
+    - hamd
+  - kind: pipper
+    package: spammer
+```
+
+It's also possible to specify a file to where the package dependencies
+have been defined.
+
+```yaml
+targets:
+- kind: layer
+  name: foo
+  dependencies:
+  - kind: pip
+    file: requirements.layer.txt
+  - kind: pipper
+    file: pipper.layer.json
+```
+
+If no packages or file is specified, the default file for the given package
+manager will be used by default (e.g. `requirements.txt` for pip,
+ `pipper.json` for pipper, and `pyproject.toml` for poetry).
+
+It is also possible to specify the same kind of package manager multiple
+times in this list to aggregate dependencies from multiple locations.
+
+### targets[N].dependencies.skip
+
+It is possible to specify inline dependencies to skip during the bundling installation
+process. This can be useful, for example, when a particular dependency is specific to
+platforms other than the lambda environment. Or perhaps a package like boto3 that is
+already available in the lambda function should be skipped to save bundling space while
+still wanting to include it in the packages dependencies for beyond-lambda deployment
+purposes.
+
+As shown below, specify the packages to skip within the dependency as part of the
+dependency definition:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  dependencies:
+  - kind: pip
+    skip:
+    - boto3
+```
+
+### targets[N].dependencies(kind="pipper")
+
+Pipper repositories have additional configuration not associated with pip
+packages. To support pipper libraries, there are two additional attributes
+that can be specified: `bucket` and `prefix`.
+
+The `bucket` is required as it specifies the S3 bucket used as the package
+source and should be read-accessible by the profile invoking reviser.
+
+The `prefix` is an optional alternate package prefix within the S3 bucket.
+Use this only if you are using an alternate prefix with for your pipper
+package.
+
+```yaml
+targets:
+- kind: layer
+  name: foo
+  dependencies:
+  - kind: pipper
+    file: pipper.layer.json
+    bucket: bucket-name-where-pipper-package-resides
+    prefix: a/prefix/that/is/not/just/pipper
+```
+
+### targets[N].dependencies(kind="poetry")
+
+Poetry repositories have additional `extras` configuration that can be used to
+specify optional dependency groups to install in the lambda. This can be useful
+to separate dependencies by function.
+
+```yaml
+targets:
+- kind: layer
+  name: foo
+  dependencies:
+  - kind: poetry
+    extras:
+    - group
+```
+
+### targets[N].bundle
+
+The target bundle object contains the attributes that define the bundle
+that will be created and uploaded to the functions or layers in a given
+target as part of the deployment process. It's primary purpose is to define
+what files should be included in the bundling process, which it achieves
+with the following attributes.
+
+#### targets[N].bundle.include(s)
+
+The `include(s)` key is a string or list of Python glob-styled includes
+to add to the bundle. If no includes are specified, the default behavior is:
+
+- **function targets**: copy the first directory found that contains an
+  *__init__.py* file.
+- **layer targets**: do not copy anything and assume dependencies are the
+  only files to copy into the bundle.
+
+All paths should be referenced relative to the root path where the
+`lambda.yaml` is located. For a recursive matching pattern, the glob syntax
+should be used as `**/*.txt` or if restricted to a folder inside of the root
+directory then `folder/**/*.txt`. To include the entire contents of a
+directory, specify the path to the folder.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  bundle:
+    includes:
+    # This is shorthand for "foo_library/**/*"
+    - foo_library
+    # All Python files in the "bin/" folder recursively.
+    - bin/**/*.py
+    # All Jinja2 files in the root directory that begin "template_".
+    - template_*.jinja2
+```
+
+#### targets[N].bundle.exclude(s)
+
+The `exclude(s)` key is an optional one that is also a string or list of
+Python glob-styled paths to remove from the matching `include(s)`. These
+are applied to the files found via the includes and do not need to be
+comprehensive of all files in the root directory. Building on the example
+from above:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  bundle:
+    includes:
+    # This is shorthand for "foo_library/**/*"
+    - foo_library
+    # All Python files in the "bin/" folder recursively.
+    - bin/**/*.py
+    # All Jinja2 files in the root directory that begin "template_".
+    - template_*.jinja2
+    exclues:
+    - template_local.jinja2
+    - template_testing.jinja2
+```
+
+This example would remove two of the template file matches from the includes
+from the files copied into the bundle for deployment.
+
+All `__pycache__`, `*.pyc` and `.DS_Store` files/directories are
+excluded from the copying process in all cases and do not need to be
+specified explicitly.
+
+
+#### targets[N].bundle.exclude_package(s)
+
+The `package_exclude(s)` key is an optional one that is also a string or list of
+Python glob-styled paths. However, these are for paths to exclude when adding
+site-packages to the bundle. Building on the example from above:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  bundle:
+    includes:
+    # This is shorthand for "foo_library/**/*"
+    - foo_library
+    # All Python files in the "bin/" folder recursively.
+    - bin/**/*.py
+    # All Jinja2 files in the root directory that begin "template_".
+    - template_*.jinja2
+    exclues:
+    - template_local.jinja2
+    - template_testing.jinja2
+    package_excludes:
+    - foo/foo_windows.py
+  dependencies:
+  - kind: pip
+```
+
+This example would not include the `site-packages/foo/foo_windows.py` from the
+bundled zip file for the lambda function. In this case, the reason for omitting
+this file is that "Windows" code isn't needed in a linux runtime, so you want to
+save some space. This is more likely useful for large packages that include
+unneeded components, and it is desirable to save the space. This should be used
+very carefully as it can cause external libraries to fail.
+
+#### targets[N].bundle.omit_package(s)
+
+There can be cases where dependencies install dependencies of their own that
+you may not want copied over to the bundle. The most common case is a
+dependency that requires `boto3`, which is available by default in lambda
+functions already. In that case it can be useful to list site packages that
+should not be copied into the bundle but may have been installed as a side
+effect of the dependency installation process.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  bundle:
+    omit_package: boto3
+  dependencies:
+  - kind: pip
+    # Installs a package that requires boto3, which is therefore installed
+    # into the site-packages bundle directory as a result.
+    # https://github.com/awslabs/aws-lambda-powertools-python
+    package: aws-lambda-powertools
+```
+
+In the above example `aws-lambda-powertools` causes `boto3` to be installed
+as well. However, since lambda functions have `boto3` installed by default,
+it's possible to omit that package from the bundling process so that it isn't
+installed twice.
+
+Note, however, that installing `boto3` directly in a bundle can be beneficial
+because it gives you the ability to install the version that is compatible
+with your given source code and dependencies. The `boto3` version on the lambda
+function can be aged and stale.
+
+#### targets[N].bundle.handler
+
+This attribute only applies to function targets and gives the location of
+file and function entrypoint for the lambda function(s) in the target. The
+format matches the expected value for lambda functions, which is
+`<filename_without_extension>.<function_name>`.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  bundle:
+    handler: function:main
+```
+
+In this case the bundler would expect to find `function.py` in the top-leve
+directory alongside `lambda.yaml` and inside it there would be a
+`main(event, context)` function that would be called when the function(s)
+are invoked.
+
+If this value is omitted, the default value of `lambda_function.lambda_handler`
+will be used as this matches the AWS lambda Python function documentation.
+
+## function targets
+
+In addition to the common attributes described above that are shared between
+both function and layer targets, there are a number of additional
+attributes that apply only to function targets. These are:
+
+### (function) targets[N].image
+
+Specifies the configuration of the image for image based lambda functions.
+This cannot be used with `targets[N].bundle`. With the exception of `uri`
+all subfields are optional.
+
+```yaml
+image:
+  uri: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag
+  entrypoint: /my/entrypoint
+  cmd:
+  - params
+  - to
+  - entrypoint
+  workingdir: /the/working/dir
+```
+
+#### (function) targets[N].image.uri
+
+The image uri for the function's image. This must be a ECR uri that resides
+within the same region as the lambda function. If the lambda function is
+deployed to a single region this can be configured with a string:
+
+```yaml
+uri: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag
+```
+
+If the lambda function is deployed to multiple regions it can be configured
+with a dictionary mapping region names to images.
+
+```yaml
+uri:
+  us-west-2: 123456789012.dkr.ecr.us-west-2.amazonaws.com/repo:tag
+  us-east-2: 123456789012.dkr.ecr.us-east-2.amazonaws.com/repo:tag
+```
+
+#### (function) targets[N].image.entrypoint
+
+A custom entrypoint to use for the image. If this is not specified the
+entrypoint of the image will be used. This can be specified as a list or
+as a single string that will be treated as a list with one element.
+
+```yaml
+entrypoint: /my/entrypoint
+```
+
+or
+
+```yaml
+entrypoint:
+- /my/entrypoint
+```
+
+#### (function) targets[N].image.cmd
+
+A custom command to use for the image. If this is not specified the default
+command of the image will be used. This can be specified as a list or
+as a single string that will be treated as a list with one element.
+
+```yaml
+cmd: a_command
+```
+
+or
+
+```yaml
+cmd:
+- a_command
+- with
+- multiple
+- words
+```
+
+#### (function) targets[N].image.workingdir
+
+A custom working directory to set for the image. If this is not specified
+the default working directory of the image will be used.
+
+```yaml
+workingdir: /my/working/dir
+```
+
+### (function) targets[N].layer(s)
+
+Specifies one or more layers that should be attached to the targeted
+function(s). Layers can be specified as fully-qualified ARNs for externally
+specified layers, e.g. a layer created in another AWS account, or by name
+for layers specified within the account and layers defined within the targets
+of the configuration file.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  layer: arn:aws:lambda:us-west-2:999999999:layer:bar
+  ...
+```
+
+or for multiple layers:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  layers:
+  # A layer defined in another account is specified by ARN.
+  - arn:aws:lambda:us-west-2:999999999:layer:bar
+  # A layer in this account is specified by name. This layer may also be
+  # a target in this configuration file.
+  - baz
+  ...
+- kind: layer
+  name: baz
+  ...
+```
+
+By default, deployments will use the latest available version of each layer,
+but this can be overridden by specifying the layer ARN with its version:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  layer: arn:aws:lambda:us-west-2:999999999:layer:bar:42
+  ...
+```
+
+In the above example the layer will remain at version 42 until explicitly
+modified in the configuration file.
+
+Layers can also be defined as objects instead of attributes. The two-layer
+example from above could be rewritten as:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  layers:
+  - arn: arn:aws:lambda:us-west-2:999999999:layer:bar
+  - name: baz
+  ...
+```
+
+When specified as an object with attributes, there are a number of additional
+attributes that can be specified as well. First, `version` can be specified
+as a separate key from the arn or name, which in many cases can make it easier
+to work with than appending it to the end of the arn or function itself for
+programmatic/automation:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  layers:
+  - arn: arn:aws:lambda:us-west-2:999999999:layer:bar
+    version: 42
+  - name: baz
+    version: 123
+  ...
+```
+
+Next is that the layer objects accept `only` and `except` keys that can be
+used to attach the layers to certain functions in the target and not others.
+This can be useful in cases where development and production targets share
+a lot in common, but perhaps point to different versions of a layer or perhaps
+separate development and production layers entirely. It can also be useful
+when a target of functions share a common codebase but don't all need the
+same dependencies. For performance optimization, restricting the layer
+inclusions only to those that need the additional dependencies can be
+beneficial.
+
+The `only` and `except` attributes can be specified as a single string
+or a list of strings that match against *unix pattern matching*. For example,
+expanding on the example from above:
+
+```yaml
+targets:
+- kind: function
+  names:
+  - foo-devel
+  - foo-devel-worker
+  - foo-prod
+  - foo-prod-worker
+  layers:
+  - name: baz-devel
+    only: foo-devel*
+  - name: baz-devel-worker
+    only: foo-devel-worker
+  - name: baz-prod
+    only: foo-prod*
+  - name: baz-prod-worker
+    only: foo-prod-worker
+  ...
+```
+
+this example shows 4 layers that are conditionally applied using the only
+keyword. The example could be rewritten with the `except` key instead:
+
+```yaml
+targets:
+- kind: function
+  names:
+  - foo-devel
+  - foo-devel-worker
+  - foo-prod
+  - foo-prod-worker
+  layers:
+  - name: baz-devel
+    except: foo-prod*
+  - name: baz-devel-worker
+    except:
+    - foo-prod*
+    - foo-devel
+  - name: baz-prod
+    except: foo-devel*
+  - name: baz-prod-worker
+    except:
+    - foo-devel*
+    - foo-prod
+  ...
+```
+
+And either way works. The two (`only` and `except`) can also be combined
+when that makes more sense. For example, the `baz-devel-worker` from above
+could also be written as:
+
+```yaml
+  - name: baz-devel-worker
+    only: foo-devel*
+    except: foo-devel
+```
+
+Note that if `only` is specified it is processed first and then `except` is
+removed from the matches found by `only`.
+
+### (function) targets[N].memory
+
+This specifies the function memory in megabytes either as an integer or
+a string with an `MB` suffix.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  memory: 256MB
+```
+
+### (function) targets[N].timeout
+
+This specifies the function timeout in seconds either as an integer or
+a string with an `s` suffix.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  timeout: 42s
+```
+
+### (function) targets[N].variable(s)
+
+Variables contains a list of environment variables to assign to the function.
+They can be specified simply with as a string `<KEY>=<value>` syntax:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  variable: MODE=read-only
+```
+
+Here a single environment variable is specified that maps `"MODE"` to the
+value *"ready-only"*. A more programmatic-friendly way is to specify the
+name and value as attributes of a variable:
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  variables:
+  - name: MODE
+    value: read-only
+```
+
+Some environment variables may be managed through other means, e.g.
+terraform that created the function in the first place or another command
+interface used to update the function. For those cases, the `preserve`
+attribute should be set to true and no value specified.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  variables:
+  - name: MODE
+    preserve: true
+```
+
+In this case the `MODE` environment variable value will be preserved between
+function deployments to contain the value that was already set.
+
+Finally, variables support the same `only` and `exclude` attributes that
+are found for target layers so that environment variables can be specified
+differently for subsets of targets.
+
+The `only` and `except` attributes can be specified as a single string
+or a list of strings that match against *unix pattern matching*. For example,
+expanding on the example from above:
+
+```yaml
+targets:
+- kind: function
+  names:
+  - foo-prod
+  - foo-devel
+  variables:
+  - name: MODE
+    value: write
+    only: '*prod'
+  - name: MODE
+    value: read-only
+    except: '*prod'
+```
+
+### (function) targets[N].ignore(s)
+
+Ignores allows you to specify one or more configuration keys within a function
+target that should be ignored during deployments. For cases where any of the
+configuration values:
+
+- `memory`
+- `timeout`
+- `variables`
+
+are managed by external systems, they can be specified by the ignores to
+prevent changes being applied by reviser.
+
+```yaml
+targets:
+- kind: function
+  name: foo
+  ignores:
+  - memory
+  - timeout
+```
+
+## run
+
+The run attribute contains an optional object of batch non-interactive commands
+to run when the shell is called with that run key. This is useful for
+orchestrating actions for CI/CD purposes as the commands will be processed
+within a shell environment without user prompts and then the shell will exit
+when complete without waiting for additional input.
+
+```yaml
+run:
+  deploy-prod:
+  - select function *prod
+  - push --description="($CI_COMMIT_SHORT_SHA): $CI_COMMIT_TITLE"
+  - alias test -1
+targets:
+- kind: function
+  names:
+  - foo-prod
+  - foo-devel
+```
+
+In the example above, the `deploy-prod` run command macro/group would start
+the shell and then non-interactively execute the three commands in order
+to first select the *foo-prod* function, then to build and deploy that function
+with a description created from CI environment variables and finally move the
+*test* alias to the newly deployed version using a negative version index of
+*-1*. After those three commands are executed reviser will exit the
+shell automatically, successfully ending that process.
+
+There is also a special `shell` command that can be used in run command
+macros/groups that will start the shell in interactive mode. This is useful
+for using run command macros/groups for pre-configuration during startup of
+the interactive shell. Building on the previous example,
+
+```yaml
+run:
+  deploy-prod:
+  - select function *prod
+  - push --description="($CI_COMMIT_SHORT_SHA): $CI_COMMIT_TITLE"
+  - alias test -1
+  devel:
+  - select * *devel
+  - bundle
+  - shell
+targets:
+- kind: function
+  names:
+  - foo-prod
+  - foo-devel
+- kind: layer
+  names:
+  - bar-devel
+  - bar-prod
+```
+
+here we've added a `devel` run command macro/group that will select the devel
+function and layer and bundle those but not deploy them. After that's complete
+the shell command will kick off the interactive session and ask for user
+input. The benefit of this particular run command macro/group is to select
+the development targets and pre-build them to cache the dependencies for the
+shell user while they continue to develop and deploy the source code to the
+function.
+
+## Shared Dependencies
+
+It is possible to share dependencies across targets. This is useful if the dependencies
+are the same but other configurations differ. The configuration will look something
+like this:
+
+```yaml
+
+dependencies:
+  # Each shared dependency must be named, but the name can be any valid yaml key that
+  # you want.
+  shared_by_my_foo_and_bar:
+  - kind: pip
+    file: requirements.functions.txt
+  shared_by_others:
+  - kind: pip
+    file: requirements.layer.txt
+    
+targets:
+- kind: function
+  names:
+  - foo-prod
+  - foo-devel
+  timeout: 30s
+  memory: 256
+  dependencies: shared_by_my_foo_and_bar
+
+- kind: function
+  names:
+  - bar-prod
+  - bar-devel
+  timeout: 500s
+  memory: 2048
+  dependencies: shared_by_my_foo_and_bar
+
+- kind: function
+  names:
+  - baz-prod
+  - baz-devel
+  timeout: 10s
+  memory: 128
+  dependencies: shared_by_others
+
+- kind: layer
+  names:
+  - spam-prod
+  - spam-devel
+  dependencies: shared_by_others
+```
+
+Shared dependencies will be installed once reused by each target configured to use
+it. Each name shared dependency has the same structure and available options of a
+regular target dependencies definition.
+
+
+
+# Local Execution
+
+When running reviser in your current environment instead of launching the shell within
+a new container, you will want to use the command `reviser-shell`. This is the local
+version of the CLI that is meant to be used within a suitable container environment
+that mimics the lambda runtime environment. It is merely a change in entrypoint, and
+has all the shell functionality described for the `reviser` command above.
+
+Also, to run the `reviser-shell` successfully, you must install the extra shell
+dependencies with the installation:
+
+```shell
+$ pip install reviser[shell]
+```
+
+Without the shell extras install, the `reviser-shell` will fail. This is how you would
+use reviser in a containerized CI environment as well.
```

