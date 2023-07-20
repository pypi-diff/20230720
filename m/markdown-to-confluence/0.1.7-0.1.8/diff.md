# Comparing `tmp/markdown-to-confluence-0.1.7.tar.gz` & `tmp/markdown-to-confluence-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-confluence-0.1.7.tar", last modified: Fri Jul 14 12:11:38 2023, max compression
+gzip compressed data, was "markdown-to-confluence-0.1.8.tar", last modified: Thu Jul 20 19:54:59 2023, max compression
```

## Comparing `markdown-to-confluence-0.1.7.tar` & `markdown-to-confluence-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.711354 markdown-to-confluence-0.1.7/
--rw-rw-rw-   0        0        0     1098 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     6346 2023-07-14 12:11:38.711354 markdown-to-confluence-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5487 2023-07-14 12:04:51.000000 markdown-to-confluence-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.686558 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/
--rw-rw-rw-   0        0        0     6346 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 10:47:45.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.707083 markdown-to-confluence-0.1.7/md2conf/
--rw-rw-rw-   0        0        0      415 2023-07-14 12:05:03.000000 markdown-to-confluence-0.1.7/md2conf/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/__main__.py
--rw-rw-rw-   0        0        0    11622 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/api.py
--rw-rw-rw-   0        0        0      894 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/application.py
--rw-rw-rw-   0        0        0    11336 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/converter.py
--rw-rw-rw-   0        0        0    30752 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/entities.dtd
--rw-rw-rw-   0        0        0        0 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/py.typed
--rw-rw-rw-   0        0        0       97 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0     1169 2023-07-14 12:11:38.713351 markdown-to-confluence-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.710396 markdown-to-confluence-0.1.7/tests/
--rw-rw-rw-   0        0        0     2533 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/tests/test_api.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-20 19:54:59.215227 markdown-to-confluence-0.1.8/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2023-04-21 19:22:25.000000 markdown-to-confluence-0.1.8/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7031 2023-07-20 19:54:59.215451 markdown-to-confluence-0.1.8/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6195 2023-07-20 19:02:54.000000 markdown-to-confluence-0.1.8/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-20 19:54:59.210491 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7031 2023-07-20 19:54:59.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      476 2023-07-20 19:54:59.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-20 19:54:59.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      105 2023-07-20 19:54:59.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        8 2023-07-20 19:54:59.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-20 19:54:58.000000 markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/zip-safe
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-20 19:54:59.214151 markdown-to-confluence-0.1.8/md2conf/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      402 2023-07-20 19:04:30.000000 markdown-to-confluence-0.1.8/md2conf/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2597 2023-07-20 19:02:54.000000 markdown-to-confluence-0.1.8/md2conf/__main__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11946 2023-07-20 19:02:54.000000 markdown-to-confluence-0.1.8/md2conf/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3562 2023-07-20 19:02:54.000000 markdown-to-confluence-0.1.8/md2conf/application.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13150 2023-07-20 19:02:54.000000 markdown-to-confluence-0.1.8/md2conf/converter.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    30215 2023-07-13 14:32:38.000000 markdown-to-confluence-0.1.8/md2conf/entities.dtd
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 19:11:21.000000 markdown-to-confluence-0.1.8/md2conf/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-06-17 11:04:46.000000 markdown-to-confluence-0.1.8/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1120 2023-07-20 19:54:59.216439 markdown-to-confluence-0.1.8/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-06-17 11:09:13.000000 markdown-to-confluence-0.1.8/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-20 19:54:59.214669 markdown-to-confluence-0.1.8/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3338 2023-07-20 19:50:37.000000 markdown-to-confluence-0.1.8/tests/test_api.py
```

### Comparing `markdown-to-confluence-0.1.7/PKG-INFO` & `markdown-to-confluence-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,140 +1,154 @@
-Metadata-Version: 2.1
-Name: markdown-to-confluence
-Version: 0.1.7
-Summary: Publish Markdown files to Confluence wiki
-Home-page: https://github.com/hunyadi/md2conf
-Author: Levente Hunyadi
-Author-email: hunyadi@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Publish Markdown files to Confluence wiki
-
-Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
-
-Replicating documentation to Confluence by hand is tedious, and a lack of automated synchronization with the project repositories where the documents live leads to outdated documentation.
-
-This Python package
-* parses Markdown files,
-* converts Markdown content into the Confluence Storage Format (XHTML),
-* invokes Confluence API endpoints to upload images and content.
-
-## Features
-
-* Sections and subsections
-* Text with **bold**, *italic*, `monospace`, <ins>underline</ins> and ~~strikethrough~~
-* Link to [external locations](http://example.com/)
-* Ordered and unordered lists
-* Code blocks (e.g. Python, JSON, XML)
-* Image references (uploaded as Confluence page attachments)
-* [Table of Contents](https://docs.gitlab.com/ee/user/markdown.html#table-of-contents)
-
-## Getting started
-
-In order to get started, you will need
-* your organization domain name (e.g. `instructure.atlassian.net`),
-* your Confluence username (e.g. `levente.hunyadi@instructure.com`),
-* a Confluence API token (a string of alphanumeric characters), and
-* the space key in Confluence (e.g. `DAP`) you are publishing content to.
-
-### Obtaining an API token
-
-1. Log in to https://id.atlassian.com/manage/api-tokens.
-2. Click *Create API token*.
-3. From the dialog that appears, enter a memorable and concise *Label* for your token and click *Create*.
-4. Click *Copy to clipboard*, then paste the token to your script, or elsewhere to save.
-
-### Setting up the environment
-
-Confluence organization URL, username, API token and space key can be specified at runtime or set as Confluence environment variables (e.g. add to your `~/.profile` on Linux, or `~/.bash_profile` or `~/.zshenv` on MacOS):
-```bash
-export CONFLUENCE_DOMAIN='instructure.atlassian.net'
-export CONFLUENCE_USER_NAME='levente.hunyadi@instructure.com'
-export CONFLUENCE_API_KEY='0123456789abcdef'
-export CONFLUENCE_SPACE_KEY='DAP'
-```
-
-On Windows, these can be set via system properties.
-
-The tool requires appropriate permissions in Confluence in order to invoke endpoints.
-
-### Associating a Markdown file with a wiki page
-
-Each Markdown file is associated with a Confluence wiki page with a Markdown comment:
-
-```markdown
-<!-- confluence-page-id: 85668266616 -->
-```
-
-The above tells the tool to synchronize the Markdown file with the given Confluence page ID. This implies that the Confluence wiki page must exist such that it has an ID. The comment can be placed anywhere in the source file.
-
-### Setting the Confluence space
-
-If you work in an environment where there are multiple Confluence spaces, and some Markdown pages may go into one space, whereas other pages may go into another, you can set the target space on a per-document basis:
-
-```markdown
-<!-- confluence-space-key: DAP -->
-```
-
-This overrides the default space set via command-line arguments or environment variables.
-
-### Setting generated-by prompt text for wiki pages
-
-In order to ensure readers are not editing a generated document, the tool adds a warning message at the top of the Confluence page as an *info panel*. You can customize the text that appears. The text can contain markup as per the [Confluence Storage Format](https://confluence.atlassian.com/doc/confluence-storage-format-790796544.html), and is emitted directly into the *info panel* macro.
-
-Provide generated-by prompt text in the Markdown file with a tag:
-
-```markdown
-<!-- generated-by: Do not edit! Check out the <a href="https://example.com/project">original source</a>. -->
-```
-
-Alternatively, use the `--generated-by GENERATED_BY` option. The tag takes precedence.
-
-### Running the tool
-
-You execute the command-line tool `md2conf` to synchronize the Markdown file with Confluence:
-
-```console
-$ python3 -m md2conf example.md
-```
-
-Use the `--help` switch to get a full list of supported command-line options:
-
-```console
-$ python3 -m md2conf --help
-usage: md2conf [-h] [-d DOMAIN] [-u USERNAME] [-a APIKEY] [-s SPACE] [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
-               [--generated-by GENERATED_BY] [--no-generated-by]
-               mdfile
-
-positional arguments:
-  mdfile                Markdown file to convert and publish.
-
-options:
-  -h, --help            show this help message and exit
-  -d DOMAIN, --domain DOMAIN
-                        Confluence organization domain.
-  -u USERNAME, --username USERNAME
-                        Confluence user name.
-  -a APIKEY, --apikey APIKEY
-                        Confluence API key. Refer to documentation how to obtain one.
-  -s SPACE, --space SPACE
-                        Confluence space key for pages to be published. If omitted, will default to user space.
-  -l {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}
-                        Use this option to set the log verbosity.
-  --generated-by GENERATED_BY
-                        Add prompt to pages (default: 'This page has been generated with a tool.').
-  --no-generated-by     Do not add 'generated by a tool' prompt to pages.
-```
+Metadata-Version: 2.1
+Name: markdown-to-confluence
+Version: 0.1.8
+Summary: Publish Markdown files to Confluence wiki
+Home-page: https://github.com/hunyadi/md2conf
+Author: Levente Hunyadi
+Author-email: hunyadi@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Publish Markdown files to Confluence wiki
+
+Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
+
+Replicating documentation to Confluence by hand is tedious, and a lack of automated synchronization with the project repositories where the documents live leads to outdated documentation.
+
+This Python package
+* parses Markdown files,
+* converts Markdown content into the Confluence Storage Format (XHTML),
+* invokes Confluence API endpoints to upload images and content.
+
+## Features
+
+* Sections and subsections
+* Text with **bold**, *italic*, `monospace`, <ins>underline</ins> and ~~strikethrough~~
+* Link to [external locations](http://example.com/)
+* Ordered and unordered lists
+* Code blocks (e.g. Python, JSON, XML)
+* Image references (uploaded as Confluence page attachments)
+* [Table of Contents](https://docs.gitlab.com/ee/user/markdown.html#table-of-contents)
+
+## Getting started
+
+In order to get started, you will need
+* your organization domain name (e.g. `instructure.atlassian.net`),
+* base path for Confluence wiki (typically `/wiki/` for managed Confluence, `/` for on-premise)
+* your Confluence username (e.g. `levente.hunyadi@instructure.com`) (only if required by your deployment),
+* a Confluence API token (a string of alphanumeric characters), and
+* the space key in Confluence (e.g. `DAP`) you are publishing content to.
+
+### Obtaining an API token
+
+1. Log in to https://id.atlassian.com/manage/api-tokens.
+2. Click *Create API token*.
+3. From the dialog that appears, enter a memorable and concise *Label* for your token and click *Create*.
+4. Click *Copy to clipboard*, then paste the token to your script, or elsewhere to save.
+
+### Setting up the environment
+
+Confluence organization domain, base path, username, API token and space key can be specified at runtime or set as Confluence environment variables (e.g. add to your `~/.profile` on Linux, or `~/.bash_profile` or `~/.zshenv` on MacOS):
+```bash
+export CONFLUENCE_DOMAIN='instructure.atlassian.net'
+export CONFLUENCE_PATH='/wiki/'
+export CONFLUENCE_USER_NAME='levente.hunyadi@instructure.com'
+export CONFLUENCE_API_KEY='0123456789abcdef'
+export CONFLUENCE_SPACE_KEY='DAP'
+```
+
+On Windows, these can be set via system properties.
+
+### Permissions
+
+The tool requires appropriate permissions in Confluence in order to invoke endpoints.
+
+If a Confluence username is set, the tool uses HTTP *Basic* authentication to pass the username and the API key to Confluence REST API endpoints. If no username is provided, the tool authenticates with HTTP *Bearer*, and passes the API key as the bearer token.
+
+If you lack appropriate permissions, you will get an *Unauthorized* response from Confluence. The tool will emit a message that looks as follows:
+
+```
+2023-06-30 23:59:59,000 - ERROR - <module> [80] - 401 Client Error: Unauthorized for url: ...
+```
+
+### Associating a Markdown file with a wiki page
+
+Each Markdown file is associated with a Confluence wiki page with a Markdown comment:
+
+```markdown
+<!-- confluence-page-id: 85668266616 -->
+```
+
+The above tells the tool to synchronize the Markdown file with the given Confluence page ID. This implies that the Confluence wiki page must exist such that it has an ID. The comment can be placed anywhere in the source file.
+
+### Setting the Confluence space
+
+If you work in an environment where there are multiple Confluence spaces, and some Markdown pages may go into one space, whereas other pages may go into another, you can set the target space on a per-document basis:
+
+```markdown
+<!-- confluence-space-key: DAP -->
+```
+
+This overrides the default space set via command-line arguments or environment variables.
+
+### Setting generated-by prompt text for wiki pages
+
+In order to ensure readers are not editing a generated document, the tool adds a warning message at the top of the Confluence page as an *info panel*. You can customize the text that appears. The text can contain markup as per the [Confluence Storage Format](https://confluence.atlassian.com/doc/confluence-storage-format-790796544.html), and is emitted directly into the *info panel* macro.
+
+Provide generated-by prompt text in the Markdown file with a tag:
+
+```markdown
+<!-- generated-by: Do not edit! Check out the <a href="https://example.com/project">original source</a>. -->
+```
+
+Alternatively, use the `--generated-by GENERATED_BY` option. The tag takes precedence.
+
+### Running the tool
+
+You execute the command-line tool `md2conf` to synchronize the Markdown file with Confluence:
+
+```console
+$ python3 -m md2conf sample/example.md
+```
+
+Use the `--help` switch to get a full list of supported command-line options:
+
+```console
+$ python3 -m md2conf --help
+usage: md2conf [-h] [-d DOMAIN] [-p PATH] [-u USERNAME] [-a APIKEY] [-s SPACE]
+               [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [--generated-by GENERATED_BY] [--no-generated-by]
+               mdpath
+
+positional arguments:
+  mdpath                Path to Markdown file or directory to convert and publish.
+
+options:
+  -h, --help            show this help message and exit
+  -d DOMAIN, --domain DOMAIN
+                        Confluence organization domain.
+  -p PATH, --path PATH  Base path for Confluece wiki.
+  -u USERNAME, --username USERNAME
+                        Confluence user name.
+  -a APIKEY, --apikey APIKEY
+                        Confluence API key. Refer to documentation how to obtain one.
+  -s SPACE, --space SPACE
+                        Confluence space key for pages to be published. If omitted, will default to user
+                        space.
+  -l {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}
+                        Use this option to set the log verbosity.
+  --generated-by GENERATED_BY
+                        Add prompt to pages (default: 'This page has been generated with a tool.').
+  --no-generated-by     Do not add 'generated by a tool' prompt to pages.
+```
```

### Comparing `markdown-to-confluence-0.1.7/README.md` & `markdown-to-confluence-0.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,343 +1,388 @@
 00000000: 2320 5075 626c 6973 6820 4d61 726b 646f  # Publish Markdo
 00000010: 776e 2066 696c 6573 2074 6f20 436f 6e66  wn files to Conf
-00000020: 6c75 656e 6365 2077 696b 690d 0a0d 0a43  luence wiki....C
-00000030: 6f6e 7472 6962 7574 6f72 7320 746f 2073  ontributors to s
-00000040: 6f66 7477 6172 6520 7072 6f6a 6563 7473  oftware projects
-00000050: 2074 7970 6963 616c 6c79 2077 7269 7465   typically write
-00000060: 2064 6f63 756d 656e 7461 7469 6f6e 2069   documentation i
-00000070: 6e20 4d61 726b 646f 776e 2066 6f72 6d61  n Markdown forma
-00000080: 7420 616e 6420 686f 7374 204d 6172 6b64  t and host Markd
-00000090: 6f77 6e20 6669 6c65 7320 696e 2063 6f6c  own files in col
-000000a0: 6c61 626f 7261 7469 7665 2076 6572 7369  laborative versi
-000000b0: 6f6e 2063 6f6e 7472 6f6c 2073 7973 7465  on control syste
-000000c0: 6d73 2028 5643 5329 2073 7563 6820 6173  ms (VCS) such as
-000000d0: 2047 6974 4875 6220 6f72 2047 6974 4c61   GitHub or GitLa
-000000e0: 6220 746f 2074 7261 636b 2063 6861 6e67  b to track chang
-000000f0: 6573 2061 6e64 2066 6163 696c 6974 6174  es and facilitat
-00000100: 6520 7468 6520 7265 7669 6577 2070 726f  e the review pro
-00000110: 6365 7373 2e20 486f 7765 7665 722c 206e  cess. However, n
-00000120: 6f74 2065 7665 7279 6f6e 6520 6174 2061  ot everyone at a
-00000130: 2063 6f6d 7061 6e79 2068 6173 2061 6363   company has acc
-00000140: 6573 7320 746f 2056 4353 2c20 616e 6420  ess to VCS, and 
-00000150: 646f 6375 6d65 6e74 7320 6172 6520 6f66  documents are of
-00000160: 7465 6e20 6369 7263 756c 6174 6564 2069  ten circulated i
-00000170: 6e20 436f 6e66 6c75 656e 6365 2077 696b  n Confluence wik
-00000180: 6920 696e 7374 6561 642e 0d0a 0d0a 5265  i instead.....Re
-00000190: 706c 6963 6174 696e 6720 646f 6375 6d65  plicating docume
-000001a0: 6e74 6174 696f 6e20 746f 2043 6f6e 666c  ntation to Confl
-000001b0: 7565 6e63 6520 6279 2068 616e 6420 6973  uence by hand is
-000001c0: 2074 6564 696f 7573 2c20 616e 6420 6120   tedious, and a 
-000001d0: 6c61 636b 206f 6620 6175 746f 6d61 7465  lack of automate
-000001e0: 6420 7379 6e63 6872 6f6e 697a 6174 696f  d synchronizatio
-000001f0: 6e20 7769 7468 2074 6865 2070 726f 6a65  n with the proje
-00000200: 6374 2072 6570 6f73 6974 6f72 6965 7320  ct repositories 
-00000210: 7768 6572 6520 7468 6520 646f 6375 6d65  where the docume
-00000220: 6e74 7320 6c69 7665 206c 6561 6473 2074  nts live leads t
-00000230: 6f20 6f75 7464 6174 6564 2064 6f63 756d  o outdated docum
-00000240: 656e 7461 7469 6f6e 2e0d 0a0d 0a54 6869  entation.....Thi
-00000250: 7320 5079 7468 6f6e 2070 6163 6b61 6765  s Python package
-00000260: 0d0a 2a20 7061 7273 6573 204d 6172 6b64  ..* parses Markd
-00000270: 6f77 6e20 6669 6c65 732c 0d0a 2a20 636f  own files,..* co
-00000280: 6e76 6572 7473 204d 6172 6b64 6f77 6e20  nverts Markdown 
-00000290: 636f 6e74 656e 7420 696e 746f 2074 6865  content into the
-000002a0: 2043 6f6e 666c 7565 6e63 6520 5374 6f72   Confluence Stor
-000002b0: 6167 6520 466f 726d 6174 2028 5848 544d  age Format (XHTM
-000002c0: 4c29 2c0d 0a2a 2069 6e76 6f6b 6573 2043  L),..* invokes C
-000002d0: 6f6e 666c 7565 6e63 6520 4150 4920 656e  onfluence API en
-000002e0: 6470 6f69 6e74 7320 746f 2075 706c 6f61  dpoints to uploa
-000002f0: 6420 696d 6167 6573 2061 6e64 2063 6f6e  d images and con
-00000300: 7465 6e74 2e0d 0a0d 0a23 2320 4665 6174  tent.....## Feat
-00000310: 7572 6573 0d0a 0d0a 2a20 5365 6374 696f  ures....* Sectio
-00000320: 6e73 2061 6e64 2073 7562 7365 6374 696f  ns and subsectio
-00000330: 6e73 0d0a 2a20 5465 7874 2077 6974 6820  ns..* Text with 
-00000340: 2a2a 626f 6c64 2a2a 2c20 2a69 7461 6c69  **bold**, *itali
-00000350: 632a 2c20 606d 6f6e 6f73 7061 6365 602c  c*, `monospace`,
-00000360: 203c 696e 733e 756e 6465 726c 696e 653c   <ins>underline<
-00000370: 2f69 6e73 3e20 616e 6420 7e7e 7374 7269  /ins> and ~~stri
-00000380: 6b65 7468 726f 7567 687e 7e0d 0a2a 204c  kethrough~~..* L
-00000390: 696e 6b20 746f 205b 6578 7465 726e 616c  ink to [external
-000003a0: 206c 6f63 6174 696f 6e73 5d28 6874 7470   locations](http
-000003b0: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f29  ://example.com/)
-000003c0: 0d0a 2a20 4f72 6465 7265 6420 616e 6420  ..* Ordered and 
-000003d0: 756e 6f72 6465 7265 6420 6c69 7374 730d  unordered lists.
-000003e0: 0a2a 2043 6f64 6520 626c 6f63 6b73 2028  .* Code blocks (
-000003f0: 652e 672e 2050 7974 686f 6e2c 204a 534f  e.g. Python, JSO
-00000400: 4e2c 2058 4d4c 290d 0a2a 2049 6d61 6765  N, XML)..* Image
-00000410: 2072 6566 6572 656e 6365 7320 2875 706c   references (upl
-00000420: 6f61 6465 6420 6173 2043 6f6e 666c 7565  oaded as Conflue
-00000430: 6e63 6520 7061 6765 2061 7474 6163 686d  nce page attachm
-00000440: 656e 7473 290d 0a2a 205b 5461 626c 6520  ents)..* [Table 
-00000450: 6f66 2043 6f6e 7465 6e74 735d 2868 7474  of Contents](htt
-00000460: 7073 3a2f 2f64 6f63 732e 6769 746c 6162  ps://docs.gitlab
-00000470: 2e63 6f6d 2f65 652f 7573 6572 2f6d 6172  .com/ee/user/mar
-00000480: 6b64 6f77 6e2e 6874 6d6c 2374 6162 6c65  kdown.html#table
-00000490: 2d6f 662d 636f 6e74 656e 7473 290d 0a0d  -of-contents)...
-000004a0: 0a23 2320 4765 7474 696e 6720 7374 6172  .## Getting star
-000004b0: 7465 640d 0a0d 0a49 6e20 6f72 6465 7220  ted....In order 
-000004c0: 746f 2067 6574 2073 7461 7274 6564 2c20  to get started, 
-000004d0: 796f 7520 7769 6c6c 206e 6565 640d 0a2a  you will need..*
-000004e0: 2079 6f75 7220 6f72 6761 6e69 7a61 7469   your organizati
-000004f0: 6f6e 2064 6f6d 6169 6e20 6e61 6d65 2028  on domain name (
-00000500: 652e 672e 2060 696e 7374 7275 6374 7572  e.g. `instructur
-00000510: 652e 6174 6c61 7373 6961 6e2e 6e65 7460  e.atlassian.net`
-00000520: 292c 0d0a 2a20 796f 7572 2043 6f6e 666c  ),..* your Confl
-00000530: 7565 6e63 6520 7573 6572 6e61 6d65 2028  uence username (
-00000540: 652e 672e 2060 6c65 7665 6e74 652e 6875  e.g. `levente.hu
-00000550: 6e79 6164 6940 696e 7374 7275 6374 7572  nyadi@instructur
-00000560: 652e 636f 6d60 292c 0d0a 2a20 6120 436f  e.com`),..* a Co
-00000570: 6e66 6c75 656e 6365 2041 5049 2074 6f6b  nfluence API tok
-00000580: 656e 2028 6120 7374 7269 6e67 206f 6620  en (a string of 
-00000590: 616c 7068 616e 756d 6572 6963 2063 6861  alphanumeric cha
-000005a0: 7261 6374 6572 7329 2c20 616e 640d 0a2a  racters), and..*
-000005b0: 2074 6865 2073 7061 6365 206b 6579 2069   the space key i
-000005c0: 6e20 436f 6e66 6c75 656e 6365 2028 652e  n Confluence (e.
-000005d0: 672e 2060 4441 5060 2920 796f 7520 6172  g. `DAP`) you ar
-000005e0: 6520 7075 626c 6973 6869 6e67 2063 6f6e  e publishing con
-000005f0: 7465 6e74 2074 6f2e 0d0a 0d0a 2323 2320  tent to.....### 
-00000600: 4f62 7461 696e 696e 6720 616e 2041 5049  Obtaining an API
-00000610: 2074 6f6b 656e 0d0a 0d0a 312e 204c 6f67   token....1. Log
-00000620: 2069 6e20 746f 2068 7474 7073 3a2f 2f69   in to https://i
-00000630: 642e 6174 6c61 7373 6961 6e2e 636f 6d2f  d.atlassian.com/
-00000640: 6d61 6e61 6765 2f61 7069 2d74 6f6b 656e  manage/api-token
-00000650: 732e 0d0a 322e 2043 6c69 636b 202a 4372  s...2. Click *Cr
-00000660: 6561 7465 2041 5049 2074 6f6b 656e 2a2e  eate API token*.
-00000670: 0d0a 332e 2046 726f 6d20 7468 6520 6469  ..3. From the di
-00000680: 616c 6f67 2074 6861 7420 6170 7065 6172  alog that appear
-00000690: 732c 2065 6e74 6572 2061 206d 656d 6f72  s, enter a memor
-000006a0: 6162 6c65 2061 6e64 2063 6f6e 6369 7365  able and concise
-000006b0: 202a 4c61 6265 6c2a 2066 6f72 2079 6f75   *Label* for you
-000006c0: 7220 746f 6b65 6e20 616e 6420 636c 6963  r token and clic
-000006d0: 6b20 2a43 7265 6174 652a 2e0d 0a34 2e20  k *Create*...4. 
-000006e0: 436c 6963 6b20 2a43 6f70 7920 746f 2063  Click *Copy to c
-000006f0: 6c69 7062 6f61 7264 2a2c 2074 6865 6e20  lipboard*, then 
-00000700: 7061 7374 6520 7468 6520 746f 6b65 6e20  paste the token 
-00000710: 746f 2079 6f75 7220 7363 7269 7074 2c20  to your script, 
-00000720: 6f72 2065 6c73 6577 6865 7265 2074 6f20  or elsewhere to 
-00000730: 7361 7665 2e0d 0a0d 0a23 2323 2053 6574  save.....### Set
-00000740: 7469 6e67 2075 7020 7468 6520 656e 7669  ting up the envi
-00000750: 726f 6e6d 656e 740d 0a0d 0a43 6f6e 666c  ronment....Confl
-00000760: 7565 6e63 6520 6f72 6761 6e69 7a61 7469  uence organizati
-00000770: 6f6e 2055 524c 2c20 7573 6572 6e61 6d65  on URL, username
-00000780: 2c20 4150 4920 746f 6b65 6e20 616e 6420  , API token and 
-00000790: 7370 6163 6520 6b65 7920 6361 6e20 6265  space key can be
-000007a0: 2073 7065 6369 6669 6564 2061 7420 7275   specified at ru
-000007b0: 6e74 696d 6520 6f72 2073 6574 2061 7320  ntime or set as 
-000007c0: 436f 6e66 6c75 656e 6365 2065 6e76 6972  Confluence envir
-000007d0: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-000007e0: 2028 652e 672e 2061 6464 2074 6f20 796f   (e.g. add to yo
-000007f0: 7572 2060 7e2f 2e70 726f 6669 6c65 6020  ur `~/.profile` 
-00000800: 6f6e 204c 696e 7578 2c20 6f72 2060 7e2f  on Linux, or `~/
-00000810: 2e62 6173 685f 7072 6f66 696c 6560 206f  .bash_profile` o
-00000820: 7220 607e 2f2e 7a73 6865 6e76 6020 6f6e  r `~/.zshenv` on
-00000830: 204d 6163 4f53 293a 0d0a 6060 6062 6173   MacOS):..```bas
-00000840: 680d 0a65 7870 6f72 7420 434f 4e46 4c55  h..export CONFLU
-00000850: 454e 4345 5f44 4f4d 4149 4e3d 2769 6e73  ENCE_DOMAIN='ins
-00000860: 7472 7563 7475 7265 2e61 746c 6173 7369  tructure.atlassi
-00000870: 616e 2e6e 6574 270d 0a65 7870 6f72 7420  an.net'..export 
-00000880: 434f 4e46 4c55 454e 4345 5f55 5345 525f  CONFLUENCE_USER_
-00000890: 4e41 4d45 3d27 6c65 7665 6e74 652e 6875  NAME='levente.hu
-000008a0: 6e79 6164 6940 696e 7374 7275 6374 7572  nyadi@instructur
-000008b0: 652e 636f 6d27 0d0a 6578 706f 7274 2043  e.com'..export C
-000008c0: 4f4e 464c 5545 4e43 455f 4150 495f 4b45  ONFLUENCE_API_KE
-000008d0: 593d 2730 3132 3334 3536 3738 3961 6263  Y='0123456789abc
-000008e0: 6465 6627 0d0a 6578 706f 7274 2043 4f4e  def'..export CON
-000008f0: 464c 5545 4e43 455f 5350 4143 455f 4b45  FLUENCE_SPACE_KE
-00000900: 593d 2744 4150 270d 0a60 6060 0d0a 0d0a  Y='DAP'..```....
-00000910: 4f6e 2057 696e 646f 7773 2c20 7468 6573  On Windows, thes
-00000920: 6520 6361 6e20 6265 2073 6574 2076 6961  e can be set via
-00000930: 2073 7973 7465 6d20 7072 6f70 6572 7469   system properti
-00000940: 6573 2e0d 0a0d 0a54 6865 2074 6f6f 6c20  es.....The tool 
-00000950: 7265 7175 6972 6573 2061 7070 726f 7072  requires appropr
-00000960: 6961 7465 2070 6572 6d69 7373 696f 6e73  iate permissions
-00000970: 2069 6e20 436f 6e66 6c75 656e 6365 2069   in Confluence i
-00000980: 6e20 6f72 6465 7220 746f 2069 6e76 6f6b  n order to invok
-00000990: 6520 656e 6470 6f69 6e74 732e 0d0a 0d0a  e endpoints.....
-000009a0: 2323 2320 4173 736f 6369 6174 696e 6720  ### Associating 
-000009b0: 6120 4d61 726b 646f 776e 2066 696c 6520  a Markdown file 
-000009c0: 7769 7468 2061 2077 696b 6920 7061 6765  with a wiki page
-000009d0: 0d0a 0d0a 4561 6368 204d 6172 6b64 6f77  ....Each Markdow
-000009e0: 6e20 6669 6c65 2069 7320 6173 736f 6369  n file is associ
-000009f0: 6174 6564 2077 6974 6820 6120 436f 6e66  ated with a Conf
-00000a00: 6c75 656e 6365 2077 696b 6920 7061 6765  luence wiki page
-00000a10: 2077 6974 6820 6120 4d61 726b 646f 776e   with a Markdown
-00000a20: 2063 6f6d 6d65 6e74 3a0d 0a0d 0a60 6060   comment:....```
-00000a30: 6d61 726b 646f 776e 0d0a 3c21 2d2d 2063  markdown..<!-- c
-00000a40: 6f6e 666c 7565 6e63 652d 7061 6765 2d69  onfluence-page-i
-00000a50: 643a 2038 3536 3638 3236 3636 3136 202d  d: 85668266616 -
-00000a60: 2d3e 0d0a 6060 600d 0a0d 0a54 6865 2061  ->..```....The a
-00000a70: 626f 7665 2074 656c 6c73 2074 6865 2074  bove tells the t
-00000a80: 6f6f 6c20 746f 2073 796e 6368 726f 6e69  ool to synchroni
-00000a90: 7a65 2074 6865 204d 6172 6b64 6f77 6e20  ze the Markdown 
-00000aa0: 6669 6c65 2077 6974 6820 7468 6520 6769  file with the gi
-00000ab0: 7665 6e20 436f 6e66 6c75 656e 6365 2070  ven Confluence p
-00000ac0: 6167 6520 4944 2e20 5468 6973 2069 6d70  age ID. This imp
-00000ad0: 6c69 6573 2074 6861 7420 7468 6520 436f  lies that the Co
-00000ae0: 6e66 6c75 656e 6365 2077 696b 6920 7061  nfluence wiki pa
-00000af0: 6765 206d 7573 7420 6578 6973 7420 7375  ge must exist su
-00000b00: 6368 2074 6861 7420 6974 2068 6173 2061  ch that it has a
-00000b10: 6e20 4944 2e20 5468 6520 636f 6d6d 656e  n ID. The commen
-00000b20: 7420 6361 6e20 6265 2070 6c61 6365 6420  t can be placed 
-00000b30: 616e 7977 6865 7265 2069 6e20 7468 6520  anywhere in the 
-00000b40: 736f 7572 6365 2066 696c 652e 0d0a 0d0a  source file.....
-00000b50: 2323 2320 5365 7474 696e 6720 7468 6520  ### Setting the 
-00000b60: 436f 6e66 6c75 656e 6365 2073 7061 6365  Confluence space
-00000b70: 0d0a 0d0a 4966 2079 6f75 2077 6f72 6b20  ....If you work 
-00000b80: 696e 2061 6e20 656e 7669 726f 6e6d 656e  in an environmen
-00000b90: 7420 7768 6572 6520 7468 6572 6520 6172  t where there ar
-00000ba0: 6520 6d75 6c74 6970 6c65 2043 6f6e 666c  e multiple Confl
-00000bb0: 7565 6e63 6520 7370 6163 6573 2c20 616e  uence spaces, an
-00000bc0: 6420 736f 6d65 204d 6172 6b64 6f77 6e20  d some Markdown 
-00000bd0: 7061 6765 7320 6d61 7920 676f 2069 6e74  pages may go int
-00000be0: 6f20 6f6e 6520 7370 6163 652c 2077 6865  o one space, whe
-00000bf0: 7265 6173 206f 7468 6572 2070 6167 6573  reas other pages
-00000c00: 206d 6179 2067 6f20 696e 746f 2061 6e6f   may go into ano
-00000c10: 7468 6572 2c20 796f 7520 6361 6e20 7365  ther, you can se
-00000c20: 7420 7468 6520 7461 7267 6574 2073 7061  t the target spa
-00000c30: 6365 206f 6e20 6120 7065 722d 646f 6375  ce on a per-docu
-00000c40: 6d65 6e74 2062 6173 6973 3a0d 0a0d 0a60  ment basis:....`
-00000c50: 6060 6d61 726b 646f 776e 0d0a 3c21 2d2d  ``markdown..<!--
-00000c60: 2063 6f6e 666c 7565 6e63 652d 7370 6163   confluence-spac
-00000c70: 652d 6b65 793a 2044 4150 202d 2d3e 0d0a  e-key: DAP -->..
-00000c80: 6060 600d 0a0d 0a54 6869 7320 6f76 6572  ```....This over
-00000c90: 7269 6465 7320 7468 6520 6465 6661 756c  rides the defaul
-00000ca0: 7420 7370 6163 6520 7365 7420 7669 6120  t space set via 
-00000cb0: 636f 6d6d 616e 642d 6c69 6e65 2061 7267  command-line arg
-00000cc0: 756d 656e 7473 206f 7220 656e 7669 726f  uments or enviro
-00000cd0: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
-00000ce0: 0d0a 0d0a 2323 2320 5365 7474 696e 6720  ....### Setting 
-00000cf0: 6765 6e65 7261 7465 642d 6279 2070 726f  generated-by pro
-00000d00: 6d70 7420 7465 7874 2066 6f72 2077 696b  mpt text for wik
-00000d10: 6920 7061 6765 730d 0a0d 0a49 6e20 6f72  i pages....In or
-00000d20: 6465 7220 746f 2065 6e73 7572 6520 7265  der to ensure re
-00000d30: 6164 6572 7320 6172 6520 6e6f 7420 6564  aders are not ed
-00000d40: 6974 696e 6720 6120 6765 6e65 7261 7465  iting a generate
-00000d50: 6420 646f 6375 6d65 6e74 2c20 7468 6520  d document, the 
-00000d60: 746f 6f6c 2061 6464 7320 6120 7761 726e  tool adds a warn
-00000d70: 696e 6720 6d65 7373 6167 6520 6174 2074  ing message at t
-00000d80: 6865 2074 6f70 206f 6620 7468 6520 436f  he top of the Co
-00000d90: 6e66 6c75 656e 6365 2070 6167 6520 6173  nfluence page as
-00000da0: 2061 6e20 2a69 6e66 6f20 7061 6e65 6c2a   an *info panel*
-00000db0: 2e20 596f 7520 6361 6e20 6375 7374 6f6d  . You can custom
-00000dc0: 697a 6520 7468 6520 7465 7874 2074 6861  ize the text tha
-00000dd0: 7420 6170 7065 6172 732e 2054 6865 2074  t appears. The t
-00000de0: 6578 7420 6361 6e20 636f 6e74 6169 6e20  ext can contain 
-00000df0: 6d61 726b 7570 2061 7320 7065 7220 7468  markup as per th
-00000e00: 6520 5b43 6f6e 666c 7565 6e63 6520 5374  e [Confluence St
-00000e10: 6f72 6167 6520 466f 726d 6174 5d28 6874  orage Format](ht
-00000e20: 7470 733a 2f2f 636f 6e66 6c75 656e 6365  tps://confluence
-00000e30: 2e61 746c 6173 7369 616e 2e63 6f6d 2f64  .atlassian.com/d
-00000e40: 6f63 2f63 6f6e 666c 7565 6e63 652d 7374  oc/confluence-st
-00000e50: 6f72 6167 652d 666f 726d 6174 2d37 3930  orage-format-790
-00000e60: 3739 3635 3434 2e68 746d 6c29 2c20 616e  796544.html), an
-00000e70: 6420 6973 2065 6d69 7474 6564 2064 6972  d is emitted dir
-00000e80: 6563 746c 7920 696e 746f 2074 6865 202a  ectly into the *
-00000e90: 696e 666f 2070 616e 656c 2a20 6d61 6372  info panel* macr
-00000ea0: 6f2e 0d0a 0d0a 5072 6f76 6964 6520 6765  o.....Provide ge
-00000eb0: 6e65 7261 7465 642d 6279 2070 726f 6d70  nerated-by promp
-00000ec0: 7420 7465 7874 2069 6e20 7468 6520 4d61  t text in the Ma
-00000ed0: 726b 646f 776e 2066 696c 6520 7769 7468  rkdown file with
-00000ee0: 2061 2074 6167 3a0d 0a0d 0a60 6060 6d61   a tag:....```ma
-00000ef0: 726b 646f 776e 0d0a 3c21 2d2d 2067 656e  rkdown..<!-- gen
-00000f00: 6572 6174 6564 2d62 793a 2044 6f20 6e6f  erated-by: Do no
-00000f10: 7420 6564 6974 2120 4368 6563 6b20 6f75  t edit! Check ou
-00000f20: 7420 7468 6520 3c61 2068 7265 663d 2268  t the <a href="h
-00000f30: 7474 7073 3a2f 2f65 7861 6d70 6c65 2e63  ttps://example.c
-00000f40: 6f6d 2f70 726f 6a65 6374 223e 6f72 6967  om/project">orig
-00000f50: 696e 616c 2073 6f75 7263 653c 2f61 3e2e  inal source</a>.
-00000f60: 202d 2d3e 0d0a 6060 600d 0a0d 0a41 6c74   -->..```....Alt
-00000f70: 6572 6e61 7469 7665 6c79 2c20 7573 6520  ernatively, use 
-00000f80: 7468 6520 602d 2d67 656e 6572 6174 6564  the `--generated
-00000f90: 2d62 7920 4745 4e45 5241 5445 445f 4259  -by GENERATED_BY
-00000fa0: 6020 6f70 7469 6f6e 2e20 5468 6520 7461  ` option. The ta
-00000fb0: 6720 7461 6b65 7320 7072 6563 6564 656e  g takes preceden
-00000fc0: 6365 2e0d 0a0d 0a23 2323 2052 756e 6e69  ce.....### Runni
-00000fd0: 6e67 2074 6865 2074 6f6f 6c0d 0a0d 0a59  ng the tool....Y
-00000fe0: 6f75 2065 7865 6375 7465 2074 6865 2063  ou execute the c
-00000ff0: 6f6d 6d61 6e64 2d6c 696e 6520 746f 6f6c  ommand-line tool
-00001000: 2060 6d64 3263 6f6e 6660 2074 6f20 7379   `md2conf` to sy
-00001010: 6e63 6872 6f6e 697a 6520 7468 6520 4d61  nchronize the Ma
-00001020: 726b 646f 776e 2066 696c 6520 7769 7468  rkdown file with
-00001030: 2043 6f6e 666c 7565 6e63 653a 0d0a 0d0a   Confluence:....
-00001040: 6060 6063 6f6e 736f 6c65 0d0a 2420 7079  ```console..$ py
-00001050: 7468 6f6e 3320 2d6d 206d 6432 636f 6e66  thon3 -m md2conf
-00001060: 2065 7861 6d70 6c65 2e6d 640d 0a60 6060   example.md..```
-00001070: 0d0a 0d0a 5573 6520 7468 6520 602d 2d68  ....Use the `--h
-00001080: 656c 7060 2073 7769 7463 6820 746f 2067  elp` switch to g
-00001090: 6574 2061 2066 756c 6c20 6c69 7374 206f  et a full list o
-000010a0: 6620 7375 7070 6f72 7465 6420 636f 6d6d  f supported comm
-000010b0: 616e 642d 6c69 6e65 206f 7074 696f 6e73  and-line options
-000010c0: 3a0d 0a0d 0a60 6060 636f 6e73 6f6c 650d  :....```console.
-000010d0: 0a24 2070 7974 686f 6e33 202d 6d20 6d64  .$ python3 -m md
-000010e0: 3263 6f6e 6620 2d2d 6865 6c70 0d0a 7573  2conf --help..us
-000010f0: 6167 653a 206d 6432 636f 6e66 205b 2d68  age: md2conf [-h
-00001100: 5d20 5b2d 6420 444f 4d41 494e 5d20 5b2d  ] [-d DOMAIN] [-
-00001110: 7520 5553 4552 4e41 4d45 5d20 5b2d 6120  u USERNAME] [-a 
-00001120: 4150 494b 4559 5d20 5b2d 7320 5350 4143  APIKEY] [-s SPAC
-00001130: 455d 205b 2d6c 207b 4445 4255 472c 494e  E] [-l {DEBUG,IN
-00001140: 464f 2c57 4152 4e49 4e47 2c45 5252 4f52  FO,WARNING,ERROR
-00001150: 2c43 5249 5449 4341 4c7d 5d0d 0a20 2020  ,CRITICAL}]..   
-00001160: 2020 2020 2020 2020 2020 2020 5b2d 2d67              [--g
-00001170: 656e 6572 6174 6564 2d62 7920 4745 4e45  enerated-by GENE
-00001180: 5241 5445 445f 4259 5d20 5b2d 2d6e 6f2d  RATED_BY] [--no-
-00001190: 6765 6e65 7261 7465 642d 6279 5d0d 0a20  generated-by].. 
-000011a0: 2020 2020 2020 2020 2020 2020 2020 6d64                md
-000011b0: 6669 6c65 0d0a 0d0a 706f 7369 7469 6f6e  file....position
-000011c0: 616c 2061 7267 756d 656e 7473 3a0d 0a20  al arguments:.. 
-000011d0: 206d 6466 696c 6520 2020 2020 2020 2020   mdfile         
-000011e0: 2020 2020 2020 204d 6172 6b64 6f77 6e20         Markdown 
-000011f0: 6669 6c65 2074 6f20 636f 6e76 6572 7420  file to convert 
-00001200: 616e 6420 7075 626c 6973 682e 0d0a 0d0a  and publish.....
-00001210: 6f70 7469 6f6e 733a 0d0a 2020 2d68 2c20  options:..  -h, 
-00001220: 2d2d 6865 6c70 2020 2020 2020 2020 2020  --help          
-00001230: 2020 7368 6f77 2074 6869 7320 6865 6c70    show this help
-00001240: 206d 6573 7361 6765 2061 6e64 2065 7869   message and exi
-00001250: 740d 0a20 202d 6420 444f 4d41 494e 2c20  t..  -d DOMAIN, 
-00001260: 2d2d 646f 6d61 696e 2044 4f4d 4149 4e0d  --domain DOMAIN.
-00001270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001280: 2020 2020 2020 2020 2043 6f6e 666c 7565           Conflue
-00001290: 6e63 6520 6f72 6761 6e69 7a61 7469 6f6e  nce organization
-000012a0: 2064 6f6d 6169 6e2e 0d0a 2020 2d75 2055   domain...  -u U
-000012b0: 5345 524e 414d 452c 202d 2d75 7365 726e  SERNAME, --usern
-000012c0: 616d 6520 5553 4552 4e41 4d45 0d0a 2020  ame USERNAME..  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 436f 6e66 6c75 656e 6365        Confluence
-000012f0: 2075 7365 7220 6e61 6d65 2e0d 0a20 202d   user name...  -
-00001300: 6120 4150 494b 4559 2c20 2d2d 6170 696b  a APIKEY, --apik
-00001310: 6579 2041 5049 4b45 590d 0a20 2020 2020  ey APIKEY..     
-00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 2020 2043 6f6e 666c 7565 6e63 6520 4150     Confluence AP
-00001340: 4920 6b65 792e 2052 6566 6572 2074 6f20  I key. Refer to 
-00001350: 646f 6375 6d65 6e74 6174 696f 6e20 686f  documentation ho
-00001360: 7720 746f 206f 6274 6169 6e20 6f6e 652e  w to obtain one.
-00001370: 0d0a 2020 2d73 2053 5041 4345 2c20 2d2d  ..  -s SPACE, --
-00001380: 7370 6163 6520 5350 4143 450d 0a20 2020  space SPACE..   
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 2020 2043 6f6e 666c 7565 6e63 6520       Confluence 
-000013b0: 7370 6163 6520 6b65 7920 666f 7220 7061  space key for pa
-000013c0: 6765 7320 746f 2062 6520 7075 626c 6973  ges to be publis
-000013d0: 6865 642e 2049 6620 6f6d 6974 7465 642c  hed. If omitted,
-000013e0: 2077 696c 6c20 6465 6661 756c 7420 746f   will default to
-000013f0: 2075 7365 7220 7370 6163 652e 0d0a 2020   user space...  
-00001400: 2d6c 207b 4445 4255 472c 494e 464f 2c57  -l {DEBUG,INFO,W
-00001410: 4152 4e49 4e47 2c45 5252 4f52 2c43 5249  ARNING,ERROR,CRI
-00001420: 5449 4341 4c7d 2c20 2d2d 6c6f 676c 6576  TICAL}, --loglev
-00001430: 656c 207b 4445 4255 472c 494e 464f 2c57  el {DEBUG,INFO,W
-00001440: 4152 4e49 4e47 2c45 5252 4f52 2c43 5249  ARNING,ERROR,CRI
-00001450: 5449 4341 4c7d 0d0a 2020 2020 2020 2020  TICAL}..        
-00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001470: 5573 6520 7468 6973 206f 7074 696f 6e20  Use this option 
-00001480: 746f 2073 6574 2074 6865 206c 6f67 2076  to set the log v
-00001490: 6572 626f 7369 7479 2e0d 0a20 202d 2d67  erbosity...  --g
-000014a0: 656e 6572 6174 6564 2d62 7920 4745 4e45  enerated-by GENE
-000014b0: 5241 5445 445f 4259 0d0a 2020 2020 2020  RATED_BY..      
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2020 4164 6420 7072 6f6d 7074 2074 6f20    Add prompt to 
-000014e0: 7061 6765 7320 2864 6566 6175 6c74 3a20  pages (default: 
-000014f0: 2754 6869 7320 7061 6765 2068 6173 2062  'This page has b
-00001500: 6565 6e20 6765 6e65 7261 7465 6420 7769  een generated wi
-00001510: 7468 2061 2074 6f6f 6c2e 2729 2e0d 0a20  th a tool.')... 
-00001520: 202d 2d6e 6f2d 6765 6e65 7261 7465 642d   --no-generated-
-00001530: 6279 2020 2020 2044 6f20 6e6f 7420 6164  by     Do not ad
-00001540: 6420 2767 656e 6572 6174 6564 2062 7920  d 'generated by 
-00001550: 6120 746f 6f6c 2720 7072 6f6d 7074 2074  a tool' prompt t
-00001560: 6f20 7061 6765 732e 0d0a 6060 600d 0a    o pages...```..
+00000020: 6c75 656e 6365 2077 696b 690a 0a43 6f6e  luence wiki..Con
+00000030: 7472 6962 7574 6f72 7320 746f 2073 6f66  tributors to sof
+00000040: 7477 6172 6520 7072 6f6a 6563 7473 2074  tware projects t
+00000050: 7970 6963 616c 6c79 2077 7269 7465 2064  ypically write d
+00000060: 6f63 756d 656e 7461 7469 6f6e 2069 6e20  ocumentation in 
+00000070: 4d61 726b 646f 776e 2066 6f72 6d61 7420  Markdown format 
+00000080: 616e 6420 686f 7374 204d 6172 6b64 6f77  and host Markdow
+00000090: 6e20 6669 6c65 7320 696e 2063 6f6c 6c61  n files in colla
+000000a0: 626f 7261 7469 7665 2076 6572 7369 6f6e  borative version
+000000b0: 2063 6f6e 7472 6f6c 2073 7973 7465 6d73   control systems
+000000c0: 2028 5643 5329 2073 7563 6820 6173 2047   (VCS) such as G
+000000d0: 6974 4875 6220 6f72 2047 6974 4c61 6220  itHub or GitLab 
+000000e0: 746f 2074 7261 636b 2063 6861 6e67 6573  to track changes
+000000f0: 2061 6e64 2066 6163 696c 6974 6174 6520   and facilitate 
+00000100: 7468 6520 7265 7669 6577 2070 726f 6365  the review proce
+00000110: 7373 2e20 486f 7765 7665 722c 206e 6f74  ss. However, not
+00000120: 2065 7665 7279 6f6e 6520 6174 2061 2063   everyone at a c
+00000130: 6f6d 7061 6e79 2068 6173 2061 6363 6573  ompany has acces
+00000140: 7320 746f 2056 4353 2c20 616e 6420 646f  s to VCS, and do
+00000150: 6375 6d65 6e74 7320 6172 6520 6f66 7465  cuments are ofte
+00000160: 6e20 6369 7263 756c 6174 6564 2069 6e20  n circulated in 
+00000170: 436f 6e66 6c75 656e 6365 2077 696b 6920  Confluence wiki 
+00000180: 696e 7374 6561 642e 0a0a 5265 706c 6963  instead...Replic
+00000190: 6174 696e 6720 646f 6375 6d65 6e74 6174  ating documentat
+000001a0: 696f 6e20 746f 2043 6f6e 666c 7565 6e63  ion to Confluenc
+000001b0: 6520 6279 2068 616e 6420 6973 2074 6564  e by hand is ted
+000001c0: 696f 7573 2c20 616e 6420 6120 6c61 636b  ious, and a lack
+000001d0: 206f 6620 6175 746f 6d61 7465 6420 7379   of automated sy
+000001e0: 6e63 6872 6f6e 697a 6174 696f 6e20 7769  nchronization wi
+000001f0: 7468 2074 6865 2070 726f 6a65 6374 2072  th the project r
+00000200: 6570 6f73 6974 6f72 6965 7320 7768 6572  epositories wher
+00000210: 6520 7468 6520 646f 6375 6d65 6e74 7320  e the documents 
+00000220: 6c69 7665 206c 6561 6473 2074 6f20 6f75  live leads to ou
+00000230: 7464 6174 6564 2064 6f63 756d 656e 7461  tdated documenta
+00000240: 7469 6f6e 2e0a 0a54 6869 7320 5079 7468  tion...This Pyth
+00000250: 6f6e 2070 6163 6b61 6765 0a2a 2070 6172  on package.* par
+00000260: 7365 7320 4d61 726b 646f 776e 2066 696c  ses Markdown fil
+00000270: 6573 2c0a 2a20 636f 6e76 6572 7473 204d  es,.* converts M
+00000280: 6172 6b64 6f77 6e20 636f 6e74 656e 7420  arkdown content 
+00000290: 696e 746f 2074 6865 2043 6f6e 666c 7565  into the Conflue
+000002a0: 6e63 6520 5374 6f72 6167 6520 466f 726d  nce Storage Form
+000002b0: 6174 2028 5848 544d 4c29 2c0a 2a20 696e  at (XHTML),.* in
+000002c0: 766f 6b65 7320 436f 6e66 6c75 656e 6365  vokes Confluence
+000002d0: 2041 5049 2065 6e64 706f 696e 7473 2074   API endpoints t
+000002e0: 6f20 7570 6c6f 6164 2069 6d61 6765 7320  o upload images 
+000002f0: 616e 6420 636f 6e74 656e 742e 0a0a 2323  and content...##
+00000300: 2046 6561 7475 7265 730a 0a2a 2053 6563   Features..* Sec
+00000310: 7469 6f6e 7320 616e 6420 7375 6273 6563  tions and subsec
+00000320: 7469 6f6e 730a 2a20 5465 7874 2077 6974  tions.* Text wit
+00000330: 6820 2a2a 626f 6c64 2a2a 2c20 2a69 7461  h **bold**, *ita
+00000340: 6c69 632a 2c20 606d 6f6e 6f73 7061 6365  lic*, `monospace
+00000350: 602c 203c 696e 733e 756e 6465 726c 696e  `, <ins>underlin
+00000360: 653c 2f69 6e73 3e20 616e 6420 7e7e 7374  e</ins> and ~~st
+00000370: 7269 6b65 7468 726f 7567 687e 7e0a 2a20  rikethrough~~.* 
+00000380: 4c69 6e6b 2074 6f20 5b65 7874 6572 6e61  Link to [externa
+00000390: 6c20 6c6f 6361 7469 6f6e 735d 2868 7474  l locations](htt
+000003a0: 703a 2f2f 6578 616d 706c 652e 636f 6d2f  p://example.com/
+000003b0: 290a 2a20 4f72 6465 7265 6420 616e 6420  ).* Ordered and 
+000003c0: 756e 6f72 6465 7265 6420 6c69 7374 730a  unordered lists.
+000003d0: 2a20 436f 6465 2062 6c6f 636b 7320 2865  * Code blocks (e
+000003e0: 2e67 2e20 5079 7468 6f6e 2c20 4a53 4f4e  .g. Python, JSON
+000003f0: 2c20 584d 4c29 0a2a 2049 6d61 6765 2072  , XML).* Image r
+00000400: 6566 6572 656e 6365 7320 2875 706c 6f61  eferences (uploa
+00000410: 6465 6420 6173 2043 6f6e 666c 7565 6e63  ded as Confluenc
+00000420: 6520 7061 6765 2061 7474 6163 686d 656e  e page attachmen
+00000430: 7473 290a 2a20 5b54 6162 6c65 206f 6620  ts).* [Table of 
+00000440: 436f 6e74 656e 7473 5d28 6874 7470 733a  Contents](https:
+00000450: 2f2f 646f 6373 2e67 6974 6c61 622e 636f  //docs.gitlab.co
+00000460: 6d2f 6565 2f75 7365 722f 6d61 726b 646f  m/ee/user/markdo
+00000470: 776e 2e68 746d 6c23 7461 626c 652d 6f66  wn.html#table-of
+00000480: 2d63 6f6e 7465 6e74 7329 0a0a 2323 2047  -contents)..## G
+00000490: 6574 7469 6e67 2073 7461 7274 6564 0a0a  etting started..
+000004a0: 496e 206f 7264 6572 2074 6f20 6765 7420  In order to get 
+000004b0: 7374 6172 7465 642c 2079 6f75 2077 696c  started, you wil
+000004c0: 6c20 6e65 6564 0a2a 2079 6f75 7220 6f72  l need.* your or
+000004d0: 6761 6e69 7a61 7469 6f6e 2064 6f6d 6169  ganization domai
+000004e0: 6e20 6e61 6d65 2028 652e 672e 2060 696e  n name (e.g. `in
+000004f0: 7374 7275 6374 7572 652e 6174 6c61 7373  structure.atlass
+00000500: 6961 6e2e 6e65 7460 292c 0a2a 2062 6173  ian.net`),.* bas
+00000510: 6520 7061 7468 2066 6f72 2043 6f6e 666c  e path for Confl
+00000520: 7565 6e63 6520 7769 6b69 2028 7479 7069  uence wiki (typi
+00000530: 6361 6c6c 7920 602f 7769 6b69 2f60 2066  cally `/wiki/` f
+00000540: 6f72 206d 616e 6167 6564 2043 6f6e 666c  or managed Confl
+00000550: 7565 6e63 652c 2060 2f60 2066 6f72 206f  uence, `/` for o
+00000560: 6e2d 7072 656d 6973 6529 0a2a 2079 6f75  n-premise).* you
+00000570: 7220 436f 6e66 6c75 656e 6365 2075 7365  r Confluence use
+00000580: 726e 616d 6520 2865 2e67 2e20 606c 6576  rname (e.g. `lev
+00000590: 656e 7465 2e68 756e 7961 6469 4069 6e73  ente.hunyadi@ins
+000005a0: 7472 7563 7475 7265 2e63 6f6d 6029 2028  tructure.com`) (
+000005b0: 6f6e 6c79 2069 6620 7265 7175 6972 6564  only if required
+000005c0: 2062 7920 796f 7572 2064 6570 6c6f 796d   by your deploym
+000005d0: 656e 7429 2c0a 2a20 6120 436f 6e66 6c75  ent),.* a Conflu
+000005e0: 656e 6365 2041 5049 2074 6f6b 656e 2028  ence API token (
+000005f0: 6120 7374 7269 6e67 206f 6620 616c 7068  a string of alph
+00000600: 616e 756d 6572 6963 2063 6861 7261 6374  anumeric charact
+00000610: 6572 7329 2c20 616e 640a 2a20 7468 6520  ers), and.* the 
+00000620: 7370 6163 6520 6b65 7920 696e 2043 6f6e  space key in Con
+00000630: 666c 7565 6e63 6520 2865 2e67 2e20 6044  fluence (e.g. `D
+00000640: 4150 6029 2079 6f75 2061 7265 2070 7562  AP`) you are pub
+00000650: 6c69 7368 696e 6720 636f 6e74 656e 7420  lishing content 
+00000660: 746f 2e0a 0a23 2323 204f 6274 6169 6e69  to...### Obtaini
+00000670: 6e67 2061 6e20 4150 4920 746f 6b65 6e0a  ng an API token.
+00000680: 0a31 2e20 4c6f 6720 696e 2074 6f20 6874  .1. Log in to ht
+00000690: 7470 733a 2f2f 6964 2e61 746c 6173 7369  tps://id.atlassi
+000006a0: 616e 2e63 6f6d 2f6d 616e 6167 652f 6170  an.com/manage/ap
+000006b0: 692d 746f 6b65 6e73 2e0a 322e 2043 6c69  i-tokens..2. Cli
+000006c0: 636b 202a 4372 6561 7465 2041 5049 2074  ck *Create API t
+000006d0: 6f6b 656e 2a2e 0a33 2e20 4672 6f6d 2074  oken*..3. From t
+000006e0: 6865 2064 6961 6c6f 6720 7468 6174 2061  he dialog that a
+000006f0: 7070 6561 7273 2c20 656e 7465 7220 6120  ppears, enter a 
+00000700: 6d65 6d6f 7261 626c 6520 616e 6420 636f  memorable and co
+00000710: 6e63 6973 6520 2a4c 6162 656c 2a20 666f  ncise *Label* fo
+00000720: 7220 796f 7572 2074 6f6b 656e 2061 6e64  r your token and
+00000730: 2063 6c69 636b 202a 4372 6561 7465 2a2e   click *Create*.
+00000740: 0a34 2e20 436c 6963 6b20 2a43 6f70 7920  .4. Click *Copy 
+00000750: 746f 2063 6c69 7062 6f61 7264 2a2c 2074  to clipboard*, t
+00000760: 6865 6e20 7061 7374 6520 7468 6520 746f  hen paste the to
+00000770: 6b65 6e20 746f 2079 6f75 7220 7363 7269  ken to your scri
+00000780: 7074 2c20 6f72 2065 6c73 6577 6865 7265  pt, or elsewhere
+00000790: 2074 6f20 7361 7665 2e0a 0a23 2323 2053   to save...### S
+000007a0: 6574 7469 6e67 2075 7020 7468 6520 656e  etting up the en
+000007b0: 7669 726f 6e6d 656e 740a 0a43 6f6e 666c  vironment..Confl
+000007c0: 7565 6e63 6520 6f72 6761 6e69 7a61 7469  uence organizati
+000007d0: 6f6e 2064 6f6d 6169 6e2c 2062 6173 6520  on domain, base 
+000007e0: 7061 7468 2c20 7573 6572 6e61 6d65 2c20  path, username, 
+000007f0: 4150 4920 746f 6b65 6e20 616e 6420 7370  API token and sp
+00000800: 6163 6520 6b65 7920 6361 6e20 6265 2073  ace key can be s
+00000810: 7065 6369 6669 6564 2061 7420 7275 6e74  pecified at runt
+00000820: 696d 6520 6f72 2073 6574 2061 7320 436f  ime or set as Co
+00000830: 6e66 6c75 656e 6365 2065 6e76 6972 6f6e  nfluence environ
+00000840: 6d65 6e74 2076 6172 6961 626c 6573 2028  ment variables (
+00000850: 652e 672e 2061 6464 2074 6f20 796f 7572  e.g. add to your
+00000860: 2060 7e2f 2e70 726f 6669 6c65 6020 6f6e   `~/.profile` on
+00000870: 204c 696e 7578 2c20 6f72 2060 7e2f 2e62   Linux, or `~/.b
+00000880: 6173 685f 7072 6f66 696c 6560 206f 7220  ash_profile` or 
+00000890: 607e 2f2e 7a73 6865 6e76 6020 6f6e 204d  `~/.zshenv` on M
+000008a0: 6163 4f53 293a 0a60 6060 6261 7368 0a65  acOS):.```bash.e
+000008b0: 7870 6f72 7420 434f 4e46 4c55 454e 4345  xport CONFLUENCE
+000008c0: 5f44 4f4d 4149 4e3d 2769 6e73 7472 7563  _DOMAIN='instruc
+000008d0: 7475 7265 2e61 746c 6173 7369 616e 2e6e  ture.atlassian.n
+000008e0: 6574 270a 6578 706f 7274 2043 4f4e 464c  et'.export CONFL
+000008f0: 5545 4e43 455f 5041 5448 3d27 2f77 696b  UENCE_PATH='/wik
+00000900: 692f 270a 6578 706f 7274 2043 4f4e 464c  i/'.export CONFL
+00000910: 5545 4e43 455f 5553 4552 5f4e 414d 453d  UENCE_USER_NAME=
+00000920: 276c 6576 656e 7465 2e68 756e 7961 6469  'levente.hunyadi
+00000930: 4069 6e73 7472 7563 7475 7265 2e63 6f6d  @instructure.com
+00000940: 270a 6578 706f 7274 2043 4f4e 464c 5545  '.export CONFLUE
+00000950: 4e43 455f 4150 495f 4b45 593d 2730 3132  NCE_API_KEY='012
+00000960: 3334 3536 3738 3961 6263 6465 6627 0a65  3456789abcdef'.e
+00000970: 7870 6f72 7420 434f 4e46 4c55 454e 4345  xport CONFLUENCE
+00000980: 5f53 5041 4345 5f4b 4559 3d27 4441 5027  _SPACE_KEY='DAP'
+00000990: 0a60 6060 0a0a 4f6e 2057 696e 646f 7773  .```..On Windows
+000009a0: 2c20 7468 6573 6520 6361 6e20 6265 2073  , these can be s
+000009b0: 6574 2076 6961 2073 7973 7465 6d20 7072  et via system pr
+000009c0: 6f70 6572 7469 6573 2e0a 0a23 2323 2050  operties...### P
+000009d0: 6572 6d69 7373 696f 6e73 0a0a 5468 6520  ermissions..The 
+000009e0: 746f 6f6c 2072 6571 7569 7265 7320 6170  tool requires ap
+000009f0: 7072 6f70 7269 6174 6520 7065 726d 6973  propriate permis
+00000a00: 7369 6f6e 7320 696e 2043 6f6e 666c 7565  sions in Conflue
+00000a10: 6e63 6520 696e 206f 7264 6572 2074 6f20  nce in order to 
+00000a20: 696e 766f 6b65 2065 6e64 706f 696e 7473  invoke endpoints
+00000a30: 2e0a 0a49 6620 6120 436f 6e66 6c75 656e  ...If a Confluen
+00000a40: 6365 2075 7365 726e 616d 6520 6973 2073  ce username is s
+00000a50: 6574 2c20 7468 6520 746f 6f6c 2075 7365  et, the tool use
+00000a60: 7320 4854 5450 202a 4261 7369 632a 2061  s HTTP *Basic* a
+00000a70: 7574 6865 6e74 6963 6174 696f 6e20 746f  uthentication to
+00000a80: 2070 6173 7320 7468 6520 7573 6572 6e61   pass the userna
+00000a90: 6d65 2061 6e64 2074 6865 2041 5049 206b  me and the API k
+00000aa0: 6579 2074 6f20 436f 6e66 6c75 656e 6365  ey to Confluence
+00000ab0: 2052 4553 5420 4150 4920 656e 6470 6f69   REST API endpoi
+00000ac0: 6e74 732e 2049 6620 6e6f 2075 7365 726e  nts. If no usern
+00000ad0: 616d 6520 6973 2070 726f 7669 6465 642c  ame is provided,
+00000ae0: 2074 6865 2074 6f6f 6c20 6175 7468 656e   the tool authen
+00000af0: 7469 6361 7465 7320 7769 7468 2048 5454  ticates with HTT
+00000b00: 5020 2a42 6561 7265 722a 2c20 616e 6420  P *Bearer*, and 
+00000b10: 7061 7373 6573 2074 6865 2041 5049 206b  passes the API k
+00000b20: 6579 2061 7320 7468 6520 6265 6172 6572  ey as the bearer
+00000b30: 2074 6f6b 656e 2e0a 0a49 6620 796f 7520   token...If you 
+00000b40: 6c61 636b 2061 7070 726f 7072 6961 7465  lack appropriate
+00000b50: 2070 6572 6d69 7373 696f 6e73 2c20 796f   permissions, yo
+00000b60: 7520 7769 6c6c 2067 6574 2061 6e20 2a55  u will get an *U
+00000b70: 6e61 7574 686f 7269 7a65 642a 2072 6573  nauthorized* res
+00000b80: 706f 6e73 6520 6672 6f6d 2043 6f6e 666c  ponse from Confl
+00000b90: 7565 6e63 652e 2054 6865 2074 6f6f 6c20  uence. The tool 
+00000ba0: 7769 6c6c 2065 6d69 7420 6120 6d65 7373  will emit a mess
+00000bb0: 6167 6520 7468 6174 206c 6f6f 6b73 2061  age that looks a
+00000bc0: 7320 666f 6c6c 6f77 733a 0a0a 6060 600a  s follows:..```.
+00000bd0: 3230 3233 2d30 362d 3330 2032 333a 3539  2023-06-30 23:59
+00000be0: 3a35 392c 3030 3020 2d20 4552 524f 5220  :59,000 - ERROR 
+00000bf0: 2d20 3c6d 6f64 756c 653e 205b 3830 5d20  - <module> [80] 
+00000c00: 2d20 3430 3120 436c 6965 6e74 2045 7272  - 401 Client Err
+00000c10: 6f72 3a20 556e 6175 7468 6f72 697a 6564  or: Unauthorized
+00000c20: 2066 6f72 2075 726c 3a20 2e2e 2e0a 6060   for url: ....``
+00000c30: 600a 0a23 2323 2041 7373 6f63 6961 7469  `..### Associati
+00000c40: 6e67 2061 204d 6172 6b64 6f77 6e20 6669  ng a Markdown fi
+00000c50: 6c65 2077 6974 6820 6120 7769 6b69 2070  le with a wiki p
+00000c60: 6167 650a 0a45 6163 6820 4d61 726b 646f  age..Each Markdo
+00000c70: 776e 2066 696c 6520 6973 2061 7373 6f63  wn file is assoc
+00000c80: 6961 7465 6420 7769 7468 2061 2043 6f6e  iated with a Con
+00000c90: 666c 7565 6e63 6520 7769 6b69 2070 6167  fluence wiki pag
+00000ca0: 6520 7769 7468 2061 204d 6172 6b64 6f77  e with a Markdow
+00000cb0: 6e20 636f 6d6d 656e 743a 0a0a 6060 606d  n comment:..```m
+00000cc0: 6172 6b64 6f77 6e0a 3c21 2d2d 2063 6f6e  arkdown.<!-- con
+00000cd0: 666c 7565 6e63 652d 7061 6765 2d69 643a  fluence-page-id:
+00000ce0: 2038 3536 3638 3236 3636 3136 202d 2d3e   85668266616 -->
+00000cf0: 0a60 6060 0a0a 5468 6520 6162 6f76 6520  .```..The above 
+00000d00: 7465 6c6c 7320 7468 6520 746f 6f6c 2074  tells the tool t
+00000d10: 6f20 7379 6e63 6872 6f6e 697a 6520 7468  o synchronize th
+00000d20: 6520 4d61 726b 646f 776e 2066 696c 6520  e Markdown file 
+00000d30: 7769 7468 2074 6865 2067 6976 656e 2043  with the given C
+00000d40: 6f6e 666c 7565 6e63 6520 7061 6765 2049  onfluence page I
+00000d50: 442e 2054 6869 7320 696d 706c 6965 7320  D. This implies 
+00000d60: 7468 6174 2074 6865 2043 6f6e 666c 7565  that the Conflue
+00000d70: 6e63 6520 7769 6b69 2070 6167 6520 6d75  nce wiki page mu
+00000d80: 7374 2065 7869 7374 2073 7563 6820 7468  st exist such th
+00000d90: 6174 2069 7420 6861 7320 616e 2049 442e  at it has an ID.
+00000da0: 2054 6865 2063 6f6d 6d65 6e74 2063 616e   The comment can
+00000db0: 2062 6520 706c 6163 6564 2061 6e79 7768   be placed anywh
+00000dc0: 6572 6520 696e 2074 6865 2073 6f75 7263  ere in the sourc
+00000dd0: 6520 6669 6c65 2e0a 0a23 2323 2053 6574  e file...### Set
+00000de0: 7469 6e67 2074 6865 2043 6f6e 666c 7565  ting the Conflue
+00000df0: 6e63 6520 7370 6163 650a 0a49 6620 796f  nce space..If yo
+00000e00: 7520 776f 726b 2069 6e20 616e 2065 6e76  u work in an env
+00000e10: 6972 6f6e 6d65 6e74 2077 6865 7265 2074  ironment where t
+00000e20: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
+00000e30: 6520 436f 6e66 6c75 656e 6365 2073 7061  e Confluence spa
+00000e40: 6365 732c 2061 6e64 2073 6f6d 6520 4d61  ces, and some Ma
+00000e50: 726b 646f 776e 2070 6167 6573 206d 6179  rkdown pages may
+00000e60: 2067 6f20 696e 746f 206f 6e65 2073 7061   go into one spa
+00000e70: 6365 2c20 7768 6572 6561 7320 6f74 6865  ce, whereas othe
+00000e80: 7220 7061 6765 7320 6d61 7920 676f 2069  r pages may go i
+00000e90: 6e74 6f20 616e 6f74 6865 722c 2079 6f75  nto another, you
+00000ea0: 2063 616e 2073 6574 2074 6865 2074 6172   can set the tar
+00000eb0: 6765 7420 7370 6163 6520 6f6e 2061 2070  get space on a p
+00000ec0: 6572 2d64 6f63 756d 656e 7420 6261 7369  er-document basi
+00000ed0: 733a 0a0a 6060 606d 6172 6b64 6f77 6e0a  s:..```markdown.
+00000ee0: 3c21 2d2d 2063 6f6e 666c 7565 6e63 652d  <!-- confluence-
+00000ef0: 7370 6163 652d 6b65 793a 2044 4150 202d  space-key: DAP -
+00000f00: 2d3e 0a60 6060 0a0a 5468 6973 206f 7665  ->.```..This ove
+00000f10: 7272 6964 6573 2074 6865 2064 6566 6175  rrides the defau
+00000f20: 6c74 2073 7061 6365 2073 6574 2076 6961  lt space set via
+00000f30: 2063 6f6d 6d61 6e64 2d6c 696e 6520 6172   command-line ar
+00000f40: 6775 6d65 6e74 7320 6f72 2065 6e76 6972  guments or envir
+00000f50: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00000f60: 2e0a 0a23 2323 2053 6574 7469 6e67 2067  ...### Setting g
+00000f70: 656e 6572 6174 6564 2d62 7920 7072 6f6d  enerated-by prom
+00000f80: 7074 2074 6578 7420 666f 7220 7769 6b69  pt text for wiki
+00000f90: 2070 6167 6573 0a0a 496e 206f 7264 6572   pages..In order
+00000fa0: 2074 6f20 656e 7375 7265 2072 6561 6465   to ensure reade
+00000fb0: 7273 2061 7265 206e 6f74 2065 6469 7469  rs are not editi
+00000fc0: 6e67 2061 2067 656e 6572 6174 6564 2064  ng a generated d
+00000fd0: 6f63 756d 656e 742c 2074 6865 2074 6f6f  ocument, the too
+00000fe0: 6c20 6164 6473 2061 2077 6172 6e69 6e67  l adds a warning
+00000ff0: 206d 6573 7361 6765 2061 7420 7468 6520   message at the 
+00001000: 746f 7020 6f66 2074 6865 2043 6f6e 666c  top of the Confl
+00001010: 7565 6e63 6520 7061 6765 2061 7320 616e  uence page as an
+00001020: 202a 696e 666f 2070 616e 656c 2a2e 2059   *info panel*. Y
+00001030: 6f75 2063 616e 2063 7573 746f 6d69 7a65  ou can customize
+00001040: 2074 6865 2074 6578 7420 7468 6174 2061   the text that a
+00001050: 7070 6561 7273 2e20 5468 6520 7465 7874  ppears. The text
+00001060: 2063 616e 2063 6f6e 7461 696e 206d 6172   can contain mar
+00001070: 6b75 7020 6173 2070 6572 2074 6865 205b  kup as per the [
+00001080: 436f 6e66 6c75 656e 6365 2053 746f 7261  Confluence Stora
+00001090: 6765 2046 6f72 6d61 745d 2868 7474 7073  ge Format](https
+000010a0: 3a2f 2f63 6f6e 666c 7565 6e63 652e 6174  ://confluence.at
+000010b0: 6c61 7373 6961 6e2e 636f 6d2f 646f 632f  lassian.com/doc/
+000010c0: 636f 6e66 6c75 656e 6365 2d73 746f 7261  confluence-stora
+000010d0: 6765 2d66 6f72 6d61 742d 3739 3037 3936  ge-format-790796
+000010e0: 3534 342e 6874 6d6c 292c 2061 6e64 2069  544.html), and i
+000010f0: 7320 656d 6974 7465 6420 6469 7265 6374  s emitted direct
+00001100: 6c79 2069 6e74 6f20 7468 6520 2a69 6e66  ly into the *inf
+00001110: 6f20 7061 6e65 6c2a 206d 6163 726f 2e0a  o panel* macro..
+00001120: 0a50 726f 7669 6465 2067 656e 6572 6174  .Provide generat
+00001130: 6564 2d62 7920 7072 6f6d 7074 2074 6578  ed-by prompt tex
+00001140: 7420 696e 2074 6865 204d 6172 6b64 6f77  t in the Markdow
+00001150: 6e20 6669 6c65 2077 6974 6820 6120 7461  n file with a ta
+00001160: 673a 0a0a 6060 606d 6172 6b64 6f77 6e0a  g:..```markdown.
+00001170: 3c21 2d2d 2067 656e 6572 6174 6564 2d62  <!-- generated-b
+00001180: 793a 2044 6f20 6e6f 7420 6564 6974 2120  y: Do not edit! 
+00001190: 4368 6563 6b20 6f75 7420 7468 6520 3c61  Check out the <a
+000011a0: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+000011b0: 7861 6d70 6c65 2e63 6f6d 2f70 726f 6a65  xample.com/proje
+000011c0: 6374 223e 6f72 6967 696e 616c 2073 6f75  ct">original sou
+000011d0: 7263 653c 2f61 3e2e 202d 2d3e 0a60 6060  rce</a>. -->.```
+000011e0: 0a0a 416c 7465 726e 6174 6976 656c 792c  ..Alternatively,
+000011f0: 2075 7365 2074 6865 2060 2d2d 6765 6e65   use the `--gene
+00001200: 7261 7465 642d 6279 2047 454e 4552 4154  rated-by GENERAT
+00001210: 4544 5f42 5960 206f 7074 696f 6e2e 2054  ED_BY` option. T
+00001220: 6865 2074 6167 2074 616b 6573 2070 7265  he tag takes pre
+00001230: 6365 6465 6e63 652e 0a0a 2323 2320 5275  cedence...### Ru
+00001240: 6e6e 696e 6720 7468 6520 746f 6f6c 0a0a  nning the tool..
+00001250: 596f 7520 6578 6563 7574 6520 7468 6520  You execute the 
+00001260: 636f 6d6d 616e 642d 6c69 6e65 2074 6f6f  command-line too
+00001270: 6c20 606d 6432 636f 6e66 6020 746f 2073  l `md2conf` to s
+00001280: 796e 6368 726f 6e69 7a65 2074 6865 204d  ynchronize the M
+00001290: 6172 6b64 6f77 6e20 6669 6c65 2077 6974  arkdown file wit
+000012a0: 6820 436f 6e66 6c75 656e 6365 3a0a 0a60  h Confluence:..`
+000012b0: 6060 636f 6e73 6f6c 650a 2420 7079 7468  ``console.$ pyth
+000012c0: 6f6e 3320 2d6d 206d 6432 636f 6e66 2073  on3 -m md2conf s
+000012d0: 616d 706c 652f 6578 616d 706c 652e 6d64  ample/example.md
+000012e0: 0a60 6060 0a0a 5573 6520 7468 6520 602d  .```..Use the `-
+000012f0: 2d68 656c 7060 2073 7769 7463 6820 746f  -help` switch to
+00001300: 2067 6574 2061 2066 756c 6c20 6c69 7374   get a full list
+00001310: 206f 6620 7375 7070 6f72 7465 6420 636f   of supported co
+00001320: 6d6d 616e 642d 6c69 6e65 206f 7074 696f  mmand-line optio
+00001330: 6e73 3a0a 0a60 6060 636f 6e73 6f6c 650a  ns:..```console.
+00001340: 2420 7079 7468 6f6e 3320 2d6d 206d 6432  $ python3 -m md2
+00001350: 636f 6e66 202d 2d68 656c 700a 7573 6167  conf --help.usag
+00001360: 653a 206d 6432 636f 6e66 205b 2d68 5d20  e: md2conf [-h] 
+00001370: 5b2d 6420 444f 4d41 494e 5d20 5b2d 7020  [-d DOMAIN] [-p 
+00001380: 5041 5448 5d20 5b2d 7520 5553 4552 4e41  PATH] [-u USERNA
+00001390: 4d45 5d20 5b2d 6120 4150 494b 4559 5d20  ME] [-a APIKEY] 
+000013a0: 5b2d 7320 5350 4143 455d 0a20 2020 2020  [-s SPACE].     
+000013b0: 2020 2020 2020 2020 2020 5b2d 6c20 7b44            [-l {D
+000013c0: 4542 5547 2c49 4e46 4f2c 5741 524e 494e  EBUG,INFO,WARNIN
+000013d0: 472c 4552 524f 522c 4352 4954 4943 414c  G,ERROR,CRITICAL
+000013e0: 7d5d 205b 2d2d 6765 6e65 7261 7465 642d  }] [--generated-
+000013f0: 6279 2047 454e 4552 4154 4544 5f42 595d  by GENERATED_BY]
+00001400: 205b 2d2d 6e6f 2d67 656e 6572 6174 6564   [--no-generated
+00001410: 2d62 795d 0a20 2020 2020 2020 2020 2020  -by].           
+00001420: 2020 2020 6d64 7061 7468 0a0a 706f 7369      mdpath..posi
+00001430: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+00001440: 3a0a 2020 6d64 7061 7468 2020 2020 2020  :.  mdpath      
+00001450: 2020 2020 2020 2020 2020 5061 7468 2074            Path t
+00001460: 6f20 4d61 726b 646f 776e 2066 696c 6520  o Markdown file 
+00001470: 6f72 2064 6972 6563 746f 7279 2074 6f20  or directory to 
+00001480: 636f 6e76 6572 7420 616e 6420 7075 626c  convert and publ
+00001490: 6973 682e 0a0a 6f70 7469 6f6e 733a 0a20  ish...options:. 
+000014a0: 202d 682c 202d 2d68 656c 7020 2020 2020   -h, --help     
+000014b0: 2020 2020 2020 2073 686f 7720 7468 6973         show this
+000014c0: 2068 656c 7020 6d65 7373 6167 6520 616e   help message an
+000014d0: 6420 6578 6974 0a20 202d 6420 444f 4d41  d exit.  -d DOMA
+000014e0: 494e 2c20 2d2d 646f 6d61 696e 2044 4f4d  IN, --domain DOM
+000014f0: 4149 4e0a 2020 2020 2020 2020 2020 2020  AIN.            
+00001500: 2020 2020 2020 2020 2020 2020 436f 6e66              Conf
+00001510: 6c75 656e 6365 206f 7267 616e 697a 6174  luence organizat
+00001520: 696f 6e20 646f 6d61 696e 2e0a 2020 2d70  ion domain..  -p
+00001530: 2050 4154 482c 202d 2d70 6174 6820 5041   PATH, --path PA
+00001540: 5448 2020 4261 7365 2070 6174 6820 666f  TH  Base path fo
+00001550: 7220 436f 6e66 6c75 6563 6520 7769 6b69  r Confluece wiki
+00001560: 2e0a 2020 2d75 2055 5345 524e 414d 452c  ..  -u USERNAME,
+00001570: 202d 2d75 7365 726e 616d 6520 5553 4552   --username USER
+00001580: 4e41 4d45 0a20 2020 2020 2020 2020 2020  NAME.           
+00001590: 2020 2020 2020 2020 2020 2020 2043 6f6e               Con
+000015a0: 666c 7565 6e63 6520 7573 6572 206e 616d  fluence user nam
+000015b0: 652e 0a20 202d 6120 4150 494b 4559 2c20  e..  -a APIKEY, 
+000015c0: 2d2d 6170 696b 6579 2041 5049 4b45 590a  --apikey APIKEY.
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 2020 2020 2020 436f 6e66 6c75 656e          Confluen
+000015f0: 6365 2041 5049 206b 6579 2e20 5265 6665  ce API key. Refe
+00001600: 7220 746f 2064 6f63 756d 656e 7461 7469  r to documentati
+00001610: 6f6e 2068 6f77 2074 6f20 6f62 7461 696e  on how to obtain
+00001620: 206f 6e65 2e0a 2020 2d73 2053 5041 4345   one..  -s SPACE
+00001630: 2c20 2d2d 7370 6163 6520 5350 4143 450a  , --space SPACE.
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 436f 6e66 6c75 656e          Confluen
+00001660: 6365 2073 7061 6365 206b 6579 2066 6f72  ce space key for
+00001670: 2070 6167 6573 2074 6f20 6265 2070 7562   pages to be pub
+00001680: 6c69 7368 6564 2e20 4966 206f 6d69 7474  lished. If omitt
+00001690: 6564 2c20 7769 6c6c 2064 6566 6175 6c74  ed, will default
+000016a0: 2074 6f20 7573 6572 0a20 2020 2020 2020   to user.       
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2073 7061 6365 2e0a 2020 2d6c 207b 4445   space..  -l {DE
+000016d0: 4255 472c 494e 464f 2c57 4152 4e49 4e47  BUG,INFO,WARNING
+000016e0: 2c45 5252 4f52 2c43 5249 5449 4341 4c7d  ,ERROR,CRITICAL}
+000016f0: 2c20 2d2d 6c6f 676c 6576 656c 207b 4445  , --loglevel {DE
+00001700: 4255 472c 494e 464f 2c57 4152 4e49 4e47  BUG,INFO,WARNING
+00001710: 2c45 5252 4f52 2c43 5249 5449 4341 4c7d  ,ERROR,CRITICAL}
+00001720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001730: 2020 2020 2020 2020 2055 7365 2074 6869           Use thi
+00001740: 7320 6f70 7469 6f6e 2074 6f20 7365 7420  s option to set 
+00001750: 7468 6520 6c6f 6720 7665 7262 6f73 6974  the log verbosit
+00001760: 792e 0a20 202d 2d67 656e 6572 6174 6564  y..  --generated
+00001770: 2d62 7920 4745 4e45 5241 5445 445f 4259  -by GENERATED_BY
+00001780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001790: 2020 2020 2020 2020 2041 6464 2070 726f           Add pro
+000017a0: 6d70 7420 746f 2070 6167 6573 2028 6465  mpt to pages (de
+000017b0: 6661 756c 743a 2027 5468 6973 2070 6167  fault: 'This pag
+000017c0: 6520 6861 7320 6265 656e 2067 656e 6572  e has been gener
+000017d0: 6174 6564 2077 6974 6820 6120 746f 6f6c  ated with a tool
+000017e0: 2e27 292e 0a20 202d 2d6e 6f2d 6765 6e65  .')..  --no-gene
+000017f0: 7261 7465 642d 6279 2020 2020 2044 6f20  rated-by     Do 
+00001800: 6e6f 7420 6164 6420 2767 656e 6572 6174  not add 'generat
+00001810: 6564 2062 7920 6120 746f 6f6c 2720 7072  ed by a tool' pr
+00001820: 6f6d 7074 2074 6f20 7061 6765 732e 0a60  ompt to pages..`
+00001830: 6060 0a                                  ``.
```

### Comparing `markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/PKG-INFO` & `markdown-to-confluence-0.1.8/markdown_to_confluence.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,140 +1,154 @@
-Metadata-Version: 2.1
-Name: markdown-to-confluence
-Version: 0.1.7
-Summary: Publish Markdown files to Confluence wiki
-Home-page: https://github.com/hunyadi/md2conf
-Author: Levente Hunyadi
-Author-email: hunyadi@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Publish Markdown files to Confluence wiki
-
-Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
-
-Replicating documentation to Confluence by hand is tedious, and a lack of automated synchronization with the project repositories where the documents live leads to outdated documentation.
-
-This Python package
-* parses Markdown files,
-* converts Markdown content into the Confluence Storage Format (XHTML),
-* invokes Confluence API endpoints to upload images and content.
-
-## Features
-
-* Sections and subsections
-* Text with **bold**, *italic*, `monospace`, <ins>underline</ins> and ~~strikethrough~~
-* Link to [external locations](http://example.com/)
-* Ordered and unordered lists
-* Code blocks (e.g. Python, JSON, XML)
-* Image references (uploaded as Confluence page attachments)
-* [Table of Contents](https://docs.gitlab.com/ee/user/markdown.html#table-of-contents)
-
-## Getting started
-
-In order to get started, you will need
-* your organization domain name (e.g. `instructure.atlassian.net`),
-* your Confluence username (e.g. `levente.hunyadi@instructure.com`),
-* a Confluence API token (a string of alphanumeric characters), and
-* the space key in Confluence (e.g. `DAP`) you are publishing content to.
-
-### Obtaining an API token
-
-1. Log in to https://id.atlassian.com/manage/api-tokens.
-2. Click *Create API token*.
-3. From the dialog that appears, enter a memorable and concise *Label* for your token and click *Create*.
-4. Click *Copy to clipboard*, then paste the token to your script, or elsewhere to save.
-
-### Setting up the environment
-
-Confluence organization URL, username, API token and space key can be specified at runtime or set as Confluence environment variables (e.g. add to your `~/.profile` on Linux, or `~/.bash_profile` or `~/.zshenv` on MacOS):
-```bash
-export CONFLUENCE_DOMAIN='instructure.atlassian.net'
-export CONFLUENCE_USER_NAME='levente.hunyadi@instructure.com'
-export CONFLUENCE_API_KEY='0123456789abcdef'
-export CONFLUENCE_SPACE_KEY='DAP'
-```
-
-On Windows, these can be set via system properties.
-
-The tool requires appropriate permissions in Confluence in order to invoke endpoints.
-
-### Associating a Markdown file with a wiki page
-
-Each Markdown file is associated with a Confluence wiki page with a Markdown comment:
-
-```markdown
-<!-- confluence-page-id: 85668266616 -->
-```
-
-The above tells the tool to synchronize the Markdown file with the given Confluence page ID. This implies that the Confluence wiki page must exist such that it has an ID. The comment can be placed anywhere in the source file.
-
-### Setting the Confluence space
-
-If you work in an environment where there are multiple Confluence spaces, and some Markdown pages may go into one space, whereas other pages may go into another, you can set the target space on a per-document basis:
-
-```markdown
-<!-- confluence-space-key: DAP -->
-```
-
-This overrides the default space set via command-line arguments or environment variables.
-
-### Setting generated-by prompt text for wiki pages
-
-In order to ensure readers are not editing a generated document, the tool adds a warning message at the top of the Confluence page as an *info panel*. You can customize the text that appears. The text can contain markup as per the [Confluence Storage Format](https://confluence.atlassian.com/doc/confluence-storage-format-790796544.html), and is emitted directly into the *info panel* macro.
-
-Provide generated-by prompt text in the Markdown file with a tag:
-
-```markdown
-<!-- generated-by: Do not edit! Check out the <a href="https://example.com/project">original source</a>. -->
-```
-
-Alternatively, use the `--generated-by GENERATED_BY` option. The tag takes precedence.
-
-### Running the tool
-
-You execute the command-line tool `md2conf` to synchronize the Markdown file with Confluence:
-
-```console
-$ python3 -m md2conf example.md
-```
-
-Use the `--help` switch to get a full list of supported command-line options:
-
-```console
-$ python3 -m md2conf --help
-usage: md2conf [-h] [-d DOMAIN] [-u USERNAME] [-a APIKEY] [-s SPACE] [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
-               [--generated-by GENERATED_BY] [--no-generated-by]
-               mdfile
-
-positional arguments:
-  mdfile                Markdown file to convert and publish.
-
-options:
-  -h, --help            show this help message and exit
-  -d DOMAIN, --domain DOMAIN
-                        Confluence organization domain.
-  -u USERNAME, --username USERNAME
-                        Confluence user name.
-  -a APIKEY, --apikey APIKEY
-                        Confluence API key. Refer to documentation how to obtain one.
-  -s SPACE, --space SPACE
-                        Confluence space key for pages to be published. If omitted, will default to user space.
-  -l {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}
-                        Use this option to set the log verbosity.
-  --generated-by GENERATED_BY
-                        Add prompt to pages (default: 'This page has been generated with a tool.').
-  --no-generated-by     Do not add 'generated by a tool' prompt to pages.
-```
+Metadata-Version: 2.1
+Name: markdown-to-confluence
+Version: 0.1.8
+Summary: Publish Markdown files to Confluence wiki
+Home-page: https://github.com/hunyadi/md2conf
+Author: Levente Hunyadi
+Author-email: hunyadi@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Publish Markdown files to Confluence wiki
+
+Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
+
+Replicating documentation to Confluence by hand is tedious, and a lack of automated synchronization with the project repositories where the documents live leads to outdated documentation.
+
+This Python package
+* parses Markdown files,
+* converts Markdown content into the Confluence Storage Format (XHTML),
+* invokes Confluence API endpoints to upload images and content.
+
+## Features
+
+* Sections and subsections
+* Text with **bold**, *italic*, `monospace`, <ins>underline</ins> and ~~strikethrough~~
+* Link to [external locations](http://example.com/)
+* Ordered and unordered lists
+* Code blocks (e.g. Python, JSON, XML)
+* Image references (uploaded as Confluence page attachments)
+* [Table of Contents](https://docs.gitlab.com/ee/user/markdown.html#table-of-contents)
+
+## Getting started
+
+In order to get started, you will need
+* your organization domain name (e.g. `instructure.atlassian.net`),
+* base path for Confluence wiki (typically `/wiki/` for managed Confluence, `/` for on-premise)
+* your Confluence username (e.g. `levente.hunyadi@instructure.com`) (only if required by your deployment),
+* a Confluence API token (a string of alphanumeric characters), and
+* the space key in Confluence (e.g. `DAP`) you are publishing content to.
+
+### Obtaining an API token
+
+1. Log in to https://id.atlassian.com/manage/api-tokens.
+2. Click *Create API token*.
+3. From the dialog that appears, enter a memorable and concise *Label* for your token and click *Create*.
+4. Click *Copy to clipboard*, then paste the token to your script, or elsewhere to save.
+
+### Setting up the environment
+
+Confluence organization domain, base path, username, API token and space key can be specified at runtime or set as Confluence environment variables (e.g. add to your `~/.profile` on Linux, or `~/.bash_profile` or `~/.zshenv` on MacOS):
+```bash
+export CONFLUENCE_DOMAIN='instructure.atlassian.net'
+export CONFLUENCE_PATH='/wiki/'
+export CONFLUENCE_USER_NAME='levente.hunyadi@instructure.com'
+export CONFLUENCE_API_KEY='0123456789abcdef'
+export CONFLUENCE_SPACE_KEY='DAP'
+```
+
+On Windows, these can be set via system properties.
+
+### Permissions
+
+The tool requires appropriate permissions in Confluence in order to invoke endpoints.
+
+If a Confluence username is set, the tool uses HTTP *Basic* authentication to pass the username and the API key to Confluence REST API endpoints. If no username is provided, the tool authenticates with HTTP *Bearer*, and passes the API key as the bearer token.
+
+If you lack appropriate permissions, you will get an *Unauthorized* response from Confluence. The tool will emit a message that looks as follows:
+
+```
+2023-06-30 23:59:59,000 - ERROR - <module> [80] - 401 Client Error: Unauthorized for url: ...
+```
+
+### Associating a Markdown file with a wiki page
+
+Each Markdown file is associated with a Confluence wiki page with a Markdown comment:
+
+```markdown
+<!-- confluence-page-id: 85668266616 -->
+```
+
+The above tells the tool to synchronize the Markdown file with the given Confluence page ID. This implies that the Confluence wiki page must exist such that it has an ID. The comment can be placed anywhere in the source file.
+
+### Setting the Confluence space
+
+If you work in an environment where there are multiple Confluence spaces, and some Markdown pages may go into one space, whereas other pages may go into another, you can set the target space on a per-document basis:
+
+```markdown
+<!-- confluence-space-key: DAP -->
+```
+
+This overrides the default space set via command-line arguments or environment variables.
+
+### Setting generated-by prompt text for wiki pages
+
+In order to ensure readers are not editing a generated document, the tool adds a warning message at the top of the Confluence page as an *info panel*. You can customize the text that appears. The text can contain markup as per the [Confluence Storage Format](https://confluence.atlassian.com/doc/confluence-storage-format-790796544.html), and is emitted directly into the *info panel* macro.
+
+Provide generated-by prompt text in the Markdown file with a tag:
+
+```markdown
+<!-- generated-by: Do not edit! Check out the <a href="https://example.com/project">original source</a>. -->
+```
+
+Alternatively, use the `--generated-by GENERATED_BY` option. The tag takes precedence.
+
+### Running the tool
+
+You execute the command-line tool `md2conf` to synchronize the Markdown file with Confluence:
+
+```console
+$ python3 -m md2conf sample/example.md
+```
+
+Use the `--help` switch to get a full list of supported command-line options:
+
+```console
+$ python3 -m md2conf --help
+usage: md2conf [-h] [-d DOMAIN] [-p PATH] [-u USERNAME] [-a APIKEY] [-s SPACE]
+               [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [--generated-by GENERATED_BY] [--no-generated-by]
+               mdpath
+
+positional arguments:
+  mdpath                Path to Markdown file or directory to convert and publish.
+
+options:
+  -h, --help            show this help message and exit
+  -d DOMAIN, --domain DOMAIN
+                        Confluence organization domain.
+  -p PATH, --path PATH  Base path for Confluece wiki.
+  -u USERNAME, --username USERNAME
+                        Confluence user name.
+  -a APIKEY, --apikey APIKEY
+                        Confluence API key. Refer to documentation how to obtain one.
+  -s SPACE, --space SPACE
+                        Confluence space key for pages to be published. If omitted, will default to user
+                        space.
+  -l {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --loglevel {DEBUG,INFO,WARNING,ERROR,CRITICAL}
+                        Use this option to set the log verbosity.
+  --generated-by GENERATED_BY
+                        Add prompt to pages (default: 'This page has been generated with a tool.').
+  --no-generated-by     Do not add 'generated by a tool' prompt to pages.
+```
```

### Comparing `markdown-to-confluence-0.1.7/md2conf/__main__.py` & `markdown-to-confluence-0.1.8/md2conf/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,97 @@
-import argparse
-import logging
-import os.path
-import sys
-from typing import Optional
-
-import requests
-
-from .api import ConfluenceAPI
-from .application import synchronize_page
-from .converter import ConfluenceDocumentOptions
-
-
-class Arguments(argparse.Namespace):
-    mdfile: str
-    domain: str
-    username: str
-    apikey: str
-    space: str
-    loglevel: str
-    generated_by: Optional[str]
-
-
-parser = argparse.ArgumentParser()
-parser.prog = os.path.basename(os.path.dirname(__file__))
-parser.add_argument("mdfile", help="Markdown file to convert and publish.")
-parser.add_argument("-d", "--domain", help="Confluence organization domain.")
-parser.add_argument("-u", "--username", help="Confluence user name.")
-parser.add_argument(
-    "-a",
-    "--apikey",
-    help="Confluence API key. Refer to documentation how to obtain one.",
-)
-parser.add_argument(
-    "-s",
-    "--space",
-    help="Confluence space key for pages to be published. If omitted, will default to user space.",
-)
-parser.add_argument(
-    "-l",
-    "--loglevel",
-    choices=[
-        logging.getLevelName(level)
-        for level in (
-            logging.DEBUG,
-            logging.INFO,
-            logging.WARN,
-            logging.ERROR,
-            logging.CRITICAL,
-        )
-    ],
-    default=logging.getLevelName(logging.INFO),
-    help="Use this option to set the log verbosity.",
-)
-parser.add_argument(
-    "--generated-by",
-    default="This page has been generated with a tool.",
-    help="Add prompt to pages (default: 'This page has been generated with a tool.').",
-)
-parser.add_argument(
-    "--no-generated-by",
-    dest="generated_by",
-    action="store_const",
-    const=None,
-    help="Do not add 'generated by a tool' prompt to pages.",
-)
-
-args = Arguments()
-parser.parse_args(namespace=args)
-
-logging.basicConfig(
-    level=getattr(logging, args.loglevel.upper(), logging.INFO),
-    format="%(asctime)s - %(levelname)s - %(funcName)s [%(lineno)d] - %(message)s",
-)
-
-try:
-    with ConfluenceAPI(args.domain, args.username, args.apikey, args.space) as api:
-        synchronize_page(api, args.mdfile, ConfluenceDocumentOptions(args.generated_by))
-except requests.exceptions.HTTPError as err:
-    logging.error(err)
-
-    # print details for a response with JSON body
-    try:
-        response: requests.Response = err.response
-        logging.error(response.json())
-    except requests.exceptions.JSONDecodeError:
-        pass
-
-    sys.exit(1)
+import argparse
+import logging
+import os.path
+import sys
+from typing import Optional
+
+import requests
+
+from .api import ConfluenceAPI
+from .application import Application
+from .converter import ConfluenceDocumentOptions
+
+
+class Arguments(argparse.Namespace):
+    mdpath: str
+    domain: str
+    path: str
+    username: str
+    apikey: str
+    space: str
+    loglevel: str
+    generated_by: Optional[str]
+
+
+parser = argparse.ArgumentParser()
+parser.prog = os.path.basename(os.path.dirname(__file__))
+parser.add_argument(
+    "mdpath", help="Path to Markdown file or directory to convert and publish."
+)
+parser.add_argument("-d", "--domain", help="Confluence organization domain.")
+parser.add_argument("-p", "--path", help="Base path for Confluece wiki.")
+parser.add_argument("-u", "--username", help="Confluence user name.")
+parser.add_argument(
+    "-a",
+    "--apikey",
+    help="Confluence API key. Refer to documentation how to obtain one.",
+)
+parser.add_argument(
+    "-s",
+    "--space",
+    help="Confluence space key for pages to be published. If omitted, will default to user space.",
+)
+parser.add_argument(
+    "-l",
+    "--loglevel",
+    choices=[
+        logging.getLevelName(level)
+        for level in (
+            logging.DEBUG,
+            logging.INFO,
+            logging.WARN,
+            logging.ERROR,
+            logging.CRITICAL,
+        )
+    ],
+    default=logging.getLevelName(logging.INFO),
+    help="Use this option to set the log verbosity.",
+)
+parser.add_argument(
+    "--generated-by",
+    default="This page has been generated with a tool.",
+    help="Add prompt to pages (default: 'This page has been generated with a tool.').",
+)
+parser.add_argument(
+    "--no-generated-by",
+    dest="generated_by",
+    action="store_const",
+    const=None,
+    help="Do not add 'generated by a tool' prompt to pages.",
+)
+
+args = Arguments()
+parser.parse_args(namespace=args)
+
+logging.basicConfig(
+    level=getattr(logging, args.loglevel.upper(), logging.INFO),
+    format="%(asctime)s - %(levelname)s - %(funcName)s [%(lineno)d] - %(message)s",
+)
+
+try:
+    with ConfluenceAPI(
+        args.domain, args.path, args.username, args.apikey, args.space
+    ) as api:
+        Application(api, ConfluenceDocumentOptions(args.generated_by)).synchronize(
+            args.mdpath
+        )
+except requests.exceptions.HTTPError as err:
+    logging.error(err)
+
+    # print details for a response with JSON body
+    try:
+        response: requests.Response = err.response
+        logging.error(response.json())
+    except requests.exceptions.JSONDecodeError:
+        pass
+
+    sys.exit(1)
```

### Comparing `markdown-to-confluence-0.1.7/md2conf/api.py` & `markdown-to-confluence-0.1.8/md2conf/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,349 +1,364 @@
-import json
-import logging
-import mimetypes
-import os
-import os.path
-import sys
-import typing
-from contextlib import contextmanager
-from dataclasses import dataclass
-from types import TracebackType
-from typing import Dict, Generator, List, Optional, Type, Union
-from urllib.parse import urlencode, urlparse, urlunparse
-
-import requests
-
-from .converter import ParseError, sanitize_confluence
-
-# a JSON type with possible `null` values
-JsonType = Union[
-    None,
-    bool,
-    int,
-    float,
-    str,
-    Dict[str, "JsonType"],
-    List["JsonType"],
-]
-
-
-def build_url(base_url: str, query: Optional[Dict[str, str]] = None) -> str:
-    "Builds a URL with scheme, host, port, path and query string parameters."
-
-    scheme, netloc, path, params, query_str, fragment = urlparse(base_url)
-
-    if params:
-        raise ValueError("expected: url with no parameters")
-    if query_str:
-        raise ValueError("expected: url with no query string")
-    if fragment:
-        raise ValueError("expected: url with no fragment")
-
-    url_parts = (scheme, netloc, path, None, urlencode(query) if query else None, None)
-    return urlunparse(url_parts)
-
-
-if sys.version_info >= (3, 9):
-
-    def removeprefix(string: str, prefix: str) -> str:
-        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
-
-        return string.removeprefix(prefix)
-
-else:
-
-    def removeprefix(string: str, prefix: str) -> str:
-        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
-
-        if string.startswith(prefix):
-            return string[len(prefix) :]
-        else:
-            return string
-
-
-LOGGER = logging.getLogger(__name__)
-
-
-class ConfluenceError(RuntimeError):
-    pass
-
-
-@dataclass
-class ConfluenceAttachment:
-    id: str
-    media_type: str
-    file_size: int
-    comment: str
-
-
-@dataclass
-class ConfluencePage:
-    id: str
-    title: str
-    version: int
-    content: str
-
-
-class ConfluenceAPI:
-    domain: str
-    space_key: str
-    user_name: str
-    api_key: str
-
-    session: Optional["ConfluenceSession"] = None
-
-    def __init__(
-        self,
-        domain: Optional[str] = None,
-        user_name: Optional[str] = None,
-        api_key: Optional[str] = None,
-        space_key: Optional[str] = None,
-    ) -> None:
-        opt_domain = domain or os.getenv("CONFLUENCE_DOMAIN")
-        opt_user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
-        opt_api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
-        opt_space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
-
-        if not opt_domain:
-            raise ConfluenceError("Confluence domain not specified")
-        if not opt_user_name:
-            raise ConfluenceError("Confluence user name not specified")
-        if not opt_api_key:
-            raise ConfluenceError("Confluence API key not specified")
-        if not opt_space_key:
-            raise ConfluenceError("Confluence space key not specified")
-
-        if opt_domain.startswith(("http://", "https://")):
-            raise ConfluenceError(
-                "Confluence domain looks like a URL; only host name required"
-            )
-
-        self.domain = opt_domain
-        self.user_name = opt_user_name
-        self.api_key = opt_api_key
-        self.space_key = opt_space_key
-
-    def __enter__(self) -> "ConfluenceSession":
-        session = requests.Session()
-        session.auth = (self.user_name, self.api_key)
-        self.session = ConfluenceSession(session, self.domain, self.space_key)
-        return self.session
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> None:
-        if self.session is not None:
-            self.session.close()
-            self.session = None
-
-
-class ConfluenceSession:
-    session: requests.Session
-    domain: str
-    space_key: str
-
-    def __init__(self, session: requests.Session, domain: str, space_key: str) -> None:
-        self.session = session
-        self.domain = domain
-        self.space_key = space_key
-
-    def close(self) -> None:
-        self.session.close()
-
-    @contextmanager
-    def switch_space(self, new_space_key: str) -> Generator[None, None, None]:
-        old_space_key = self.space_key
-        self.space_key = new_space_key
-        try:
-            yield
-        finally:
-            self.space_key = old_space_key
-
-    def _build_url(self, path: str, query: Optional[Dict[str, str]] = None) -> str:
-        base_url = f"https://{self.domain}/wiki/rest/api{path}"
-        return build_url(base_url, query)
-
-    def _invoke(self, path: str, query: Dict[str, str]) -> JsonType:
-        url = self._build_url(path, query)
-        response = self.session.get(url)
-        response.raise_for_status()
-        return response.json()
-
-    def _save(self, path: str, data: dict) -> None:
-        url = self._build_url(path)
-        response = self.session.put(
-            url,
-            data=json.dumps(data),
-            headers={"Content-Type": "application/json"},
-        )
-        response.raise_for_status()
-
-    def get_attachment_by_name(
-        self, page_id: str, filename: str
-    ) -> ConfluenceAttachment:
-        path = f"/content/{page_id}/child/attachment"
-        query = {"spaceKey": self.space_key, "filename": filename}
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-
-        results = typing.cast(List[JsonType], data["results"])
-        if len(results) != 1:
-            raise ConfluenceError(f"no such attachment on page {page_id}: {filename}")
-        result = typing.cast(Dict[str, JsonType], results[0])
-
-        id = typing.cast(str, result["id"])
-        extensions = typing.cast(Dict[str, JsonType], result["extensions"])
-        media_type = typing.cast(str, extensions["mediaType"])
-        file_size = typing.cast(int, extensions["fileSize"])
-        comment = typing.cast(str, extensions["comment"])
-        return ConfluenceAttachment(id, media_type, file_size, comment)
-
-    def upload_attachment(
-        self,
-        page_id: str,
-        attachment_path: str,
-        attachment_name: str,
-        comment: Optional[str] = None,
-    ) -> None:
-        content_type = mimetypes.guess_type(attachment_path, strict=True)[0]
-
-        if not os.path.isfile(attachment_path):
-            raise ConfluenceError(f"file not found: {attachment_path}")
-
-        try:
-            attachment = self.get_attachment_by_name(page_id, attachment_name)
-
-            if attachment.file_size == os.path.getsize(attachment_path):
-                LOGGER.info("Up-to-date attachment: %s", attachment_name)
-                return
-
-            id = removeprefix(attachment.id, "att")
-            path = f"/content/{page_id}/child/attachment/{id}/data"
-
-        except ConfluenceError:
-            path = f"/content/{page_id}/child/attachment"
-
-        url = self._build_url(path)
-
-        with open(attachment_path, "rb") as attachment_file:
-            file_to_upload = {
-                "comment": comment,
-                "file": (
-                    attachment_name,  # will truncate path component
-                    attachment_file,
-                    content_type,
-                    {"Expires": "0"},
-                ),
-            }
-            LOGGER.info("Uploading attachment: %s", attachment_name)
-            response = self.session.post(
-                url,
-                files=file_to_upload,  # type: ignore
-                headers={"X-Atlassian-Token": "no-check"},
-            )
-
-        response.raise_for_status()
-        data = response.json()
-
-        if "results" in data:
-            result = data["results"][0]
-        else:
-            result = data
-
-        attachment_id = result["id"]
-        version = result["version"]["number"] + 1
-
-        # ensure path component is retained in attachment name
-        self._update_attachment(page_id, attachment_id, version, attachment_name)
-
-    def _update_attachment(
-        self, page_id: str, attachment_id: str, version: int, attachment_title: str
-    ) -> None:
-        id = removeprefix(attachment_id, "att")
-        path = f"/content/{page_id}/child/attachment/{id}"
-        data = {
-            "id": attachment_id,
-            "type": "attachment",
-            "status": "current",
-            "title": attachment_title,
-            "space": {"key": self.space_key},
-            "version": {"minorEdit": True, "number": version},
-        }
-
-        LOGGER.info("Updating attachment: %s", attachment_id)
-        self._save(path, data)
-
-    def get_page_id_by_title(self, title: str) -> str:
-        """
-        Retrieve a Confluence wiki page details by title.
-
-        :param title: The page title.
-        :returns: Confluence page info.
-        """
-
-        LOGGER.info("Looking up page with title: %s", title)
-        path = "/content"
-        query = {"title": title, "spaceKey": self.space_key}
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-
-        results = typing.cast(List[JsonType], data["results"])
-        if len(results) != 1:
-            raise ConfluenceError(f"page not found with title: {title}")
-
-        result = typing.cast(Dict[str, JsonType], results[0])
-        id = typing.cast(str, result["id"])
-        return id
-
-    def get_page(self, page_id: str) -> ConfluencePage:
-        path = f"/content/{page_id}"
-        query = {
-            "spaceKey": self.space_key,
-            "expand": "body.storage,version",
-        }
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-        version = typing.cast(Dict[str, JsonType], data["version"])
-        body = typing.cast(Dict[str, JsonType], data["body"])
-        storage = typing.cast(Dict[str, JsonType], body["storage"])
-
-        return ConfluencePage(
-            id=page_id,
-            title=typing.cast(str, data["title"]),
-            version=typing.cast(int, version["number"]),
-            content=typing.cast(str, storage["value"]),
-        )
-
-    def get_page_version(self, page_id: str) -> int:
-        path = f"/content/{page_id}"
-        query = {
-            "spaceKey": self.space_key,
-            "expand": "version",
-        }
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-        version = typing.cast(Dict[str, JsonType], data["version"])
-        return typing.cast(int, version["number"])
-
-    def update_page(self, page_id: str, new_content: str) -> None:
-        page = self.get_page(page_id)
-
-        try:
-            old_content = sanitize_confluence(page.content)
-            if old_content == new_content:
-                LOGGER.info("Up-to-date page: %s", page_id)
-                return
-        except ParseError as exc:
-            LOGGER.warning(exc)
-
-        path = f"/content/{page_id}"
-        data = {
-            "id": page_id,
-            "type": "page",
-            "title": page.title,
-            "space": {"key": self.space_key},
-            "body": {"storage": {"value": new_content, "representation": "storage"}},
-            "version": {"minorEdit": True, "number": page.version + 1},
-        }
-
-        LOGGER.info("Updating page: %s", page_id)
-        self._save(path, data)
+import json
+import logging
+import mimetypes
+import os
+import os.path
+import sys
+import typing
+from contextlib import contextmanager
+from dataclasses import dataclass
+from types import TracebackType
+from typing import Dict, Generator, List, Optional, Type, Union
+from urllib.parse import urlencode, urlparse, urlunparse
+
+import requests
+
+from .converter import ParseError, sanitize_confluence
+
+# a JSON type with possible `null` values
+JsonType = Union[
+    None,
+    bool,
+    int,
+    float,
+    str,
+    Dict[str, "JsonType"],
+    List["JsonType"],
+]
+
+
+def build_url(base_url: str, query: Optional[Dict[str, str]] = None) -> str:
+    "Builds a URL with scheme, host, port, path and query string parameters."
+
+    scheme, netloc, path, params, query_str, fragment = urlparse(base_url)
+
+    if params:
+        raise ValueError("expected: url with no parameters")
+    if query_str:
+        raise ValueError("expected: url with no query string")
+    if fragment:
+        raise ValueError("expected: url with no fragment")
+
+    url_parts = (scheme, netloc, path, None, urlencode(query) if query else None, None)
+    return urlunparse(url_parts)
+
+
+if sys.version_info >= (3, 9):
+
+    def removeprefix(string: str, prefix: str) -> str:
+        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
+
+        return string.removeprefix(prefix)
+
+else:
+
+    def removeprefix(string: str, prefix: str) -> str:
+        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
+
+        if string.startswith(prefix):
+            return string[len(prefix) :]
+        else:
+            return string
+
+
+LOGGER = logging.getLogger(__name__)
+
+
+class ConfluenceError(RuntimeError):
+    pass
+
+
+@dataclass
+class ConfluenceAttachment:
+    id: str
+    media_type: str
+    file_size: int
+    comment: str
+
+
+@dataclass
+class ConfluencePage:
+    id: str
+    title: str
+    version: int
+    content: str
+
+
+class ConfluenceAPI:
+    domain: str
+    base_path: str
+    space_key: str
+    user_name: Optional[str]
+    api_key: str
+
+    session: Optional["ConfluenceSession"] = None
+
+    def __init__(
+        self,
+        domain: Optional[str] = None,
+        base_path: Optional[str] = None,
+        user_name: Optional[str] = None,
+        api_key: Optional[str] = None,
+        space_key: Optional[str] = None,
+    ) -> None:
+        opt_domain = domain or os.getenv("CONFLUENCE_DOMAIN")
+        opt_base_path = base_path or os.getenv("CONFLUENCE_PATH")
+        opt_user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
+        opt_api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
+        opt_space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
+
+        if not opt_domain:
+            raise ConfluenceError("Confluence domain not specified")
+        if not opt_base_path:
+            opt_base_path = "/wiki/"
+        if not opt_api_key:
+            raise ConfluenceError("Confluence API key not specified")
+        if not opt_space_key:
+            raise ConfluenceError("Confluence space key not specified")
+
+        if opt_domain.startswith(("http://", "https://")) or opt_domain.endswith("/"):
+            raise ConfluenceError(
+                "Confluence domain looks like a URL; only host name required"
+            )
+        if not opt_base_path.startswith("/") or not opt_base_path.endswith("/"):
+            raise ConfluenceError("Confluence base path must start and end with a '/'")
+
+        self.domain = opt_domain
+        self.base_path = opt_base_path
+        self.user_name = opt_user_name
+        self.api_key = opt_api_key
+        self.space_key = opt_space_key
+
+    def __enter__(self) -> "ConfluenceSession":
+        session = requests.Session()
+        if self.user_name:
+            session.auth = (self.user_name, self.api_key)
+        else:
+            session.headers.update({"Authorization": f"Bearer {self.api_key}"})
+        self.session = ConfluenceSession(
+            session, self.domain, self.base_path, self.space_key
+        )
+        return self.session
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        if self.session is not None:
+            self.session.close()
+            self.session = None
+
+
+class ConfluenceSession:
+    session: requests.Session
+    domain: str
+    base_path: str
+    space_key: str
+
+    def __init__(
+        self, session: requests.Session, domain: str, base_path: str, space_key: str
+    ) -> None:
+        self.session = session
+        self.domain = domain
+        self.base_path = base_path
+        self.space_key = space_key
+
+    def close(self) -> None:
+        self.session.close()
+
+    @contextmanager
+    def switch_space(self, new_space_key: str) -> Generator[None, None, None]:
+        old_space_key = self.space_key
+        self.space_key = new_space_key
+        try:
+            yield
+        finally:
+            self.space_key = old_space_key
+
+    def _build_url(self, path: str, query: Optional[Dict[str, str]] = None) -> str:
+        base_url = f"https://{self.domain}{self.base_path}rest/api{path}"
+        return build_url(base_url, query)
+
+    def _invoke(self, path: str, query: Dict[str, str]) -> JsonType:
+        url = self._build_url(path, query)
+        response = self.session.get(url)
+        response.raise_for_status()
+        return response.json()
+
+    def _save(self, path: str, data: dict) -> None:
+        url = self._build_url(path)
+        response = self.session.put(
+            url,
+            data=json.dumps(data),
+            headers={"Content-Type": "application/json"},
+        )
+        response.raise_for_status()
+
+    def get_attachment_by_name(
+        self, page_id: str, filename: str
+    ) -> ConfluenceAttachment:
+        path = f"/content/{page_id}/child/attachment"
+        query = {"spaceKey": self.space_key, "filename": filename}
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+
+        results = typing.cast(List[JsonType], data["results"])
+        if len(results) != 1:
+            raise ConfluenceError(f"no such attachment on page {page_id}: {filename}")
+        result = typing.cast(Dict[str, JsonType], results[0])
+
+        id = typing.cast(str, result["id"])
+        extensions = typing.cast(Dict[str, JsonType], result["extensions"])
+        media_type = typing.cast(str, extensions["mediaType"])
+        file_size = typing.cast(int, extensions["fileSize"])
+        comment = typing.cast(str, extensions["comment"])
+        return ConfluenceAttachment(id, media_type, file_size, comment)
+
+    def upload_attachment(
+        self,
+        page_id: str,
+        attachment_path: str,
+        attachment_name: str,
+        comment: Optional[str] = None,
+    ) -> None:
+        content_type = mimetypes.guess_type(attachment_path, strict=True)[0]
+
+        if not os.path.isfile(attachment_path):
+            raise ConfluenceError(f"file not found: {attachment_path}")
+
+        try:
+            attachment = self.get_attachment_by_name(page_id, attachment_name)
+
+            if attachment.file_size == os.path.getsize(attachment_path):
+                LOGGER.info("Up-to-date attachment: %s", attachment_name)
+                return
+
+            id = removeprefix(attachment.id, "att")
+            path = f"/content/{page_id}/child/attachment/{id}/data"
+
+        except ConfluenceError:
+            path = f"/content/{page_id}/child/attachment"
+
+        url = self._build_url(path)
+
+        with open(attachment_path, "rb") as attachment_file:
+            file_to_upload = {
+                "comment": comment,
+                "file": (
+                    attachment_name,  # will truncate path component
+                    attachment_file,
+                    content_type,
+                    {"Expires": "0"},
+                ),
+            }
+            LOGGER.info("Uploading attachment: %s", attachment_name)
+            response = self.session.post(
+                url,
+                files=file_to_upload,  # type: ignore
+                headers={"X-Atlassian-Token": "no-check"},
+            )
+
+        response.raise_for_status()
+        data = response.json()
+
+        if "results" in data:
+            result = data["results"][0]
+        else:
+            result = data
+
+        attachment_id = result["id"]
+        version = result["version"]["number"] + 1
+
+        # ensure path component is retained in attachment name
+        self._update_attachment(page_id, attachment_id, version, attachment_name)
+
+    def _update_attachment(
+        self, page_id: str, attachment_id: str, version: int, attachment_title: str
+    ) -> None:
+        id = removeprefix(attachment_id, "att")
+        path = f"/content/{page_id}/child/attachment/{id}"
+        data = {
+            "id": attachment_id,
+            "type": "attachment",
+            "status": "current",
+            "title": attachment_title,
+            "space": {"key": self.space_key},
+            "version": {"minorEdit": True, "number": version},
+        }
+
+        LOGGER.info("Updating attachment: %s", attachment_id)
+        self._save(path, data)
+
+    def get_page_id_by_title(self, title: str) -> str:
+        """
+        Retrieve a Confluence wiki page details by title.
+
+        :param title: The page title.
+        :returns: Confluence page info.
+        """
+
+        LOGGER.info("Looking up page with title: %s", title)
+        path = "/content"
+        query = {"title": title, "spaceKey": self.space_key}
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+
+        results = typing.cast(List[JsonType], data["results"])
+        if len(results) != 1:
+            raise ConfluenceError(f"page not found with title: {title}")
+
+        result = typing.cast(Dict[str, JsonType], results[0])
+        id = typing.cast(str, result["id"])
+        return id
+
+    def get_page(self, page_id: str) -> ConfluencePage:
+        path = f"/content/{page_id}"
+        query = {
+            "spaceKey": self.space_key,
+            "expand": "body.storage,version",
+        }
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        body = typing.cast(Dict[str, JsonType], data["body"])
+        storage = typing.cast(Dict[str, JsonType], body["storage"])
+
+        return ConfluencePage(
+            id=page_id,
+            title=typing.cast(str, data["title"]),
+            version=typing.cast(int, version["number"]),
+            content=typing.cast(str, storage["value"]),
+        )
+
+    def get_page_version(self, page_id: str) -> int:
+        path = f"/content/{page_id}"
+        query = {
+            "spaceKey": self.space_key,
+            "expand": "version",
+        }
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        return typing.cast(int, version["number"])
+
+    def update_page(self, page_id: str, new_content: str) -> None:
+        page = self.get_page(page_id)
+
+        try:
+            old_content = sanitize_confluence(page.content)
+            if old_content == new_content:
+                LOGGER.info("Up-to-date page: %s", page_id)
+                return
+        except ParseError as exc:
+            LOGGER.warning(exc)
+
+        path = f"/content/{page_id}"
+        data = {
+            "id": page_id,
+            "type": "page",
+            "title": page.title,  # title needs to be unique within a space so the original title is maintained
+            "space": {"key": self.space_key},
+            "body": {"storage": {"value": new_content, "representation": "storage"}},
+            "version": {"minorEdit": True, "number": page.version + 1},
+        }
+
+        LOGGER.info("Updating page: %s", page_id)
+        self._save(path, data)
```

### Comparing `markdown-to-confluence-0.1.7/md2conf/entities.dtd` & `markdown-to-confluence-0.1.8/md2conf/entities.dtd`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,537 +1,537 @@
-<!-- Character mnemonic entities -->
-
-<!--
-<!ENTITY % HTMLlat1 PUBLIC
-   "-//W3C//ENTITIES Latin 1 for XHTML//EN"
-   "xhtml-lat1.ent">
-%HTMLlat1;
-
-<!ENTITY % HTMLsymbol PUBLIC
-   "-//W3C//ENTITIES Symbols for XHTML//EN"
-   "xhtml-symbol.ent">
-%HTMLsymbol;
-
-<!ENTITY % HTMLspecial PUBLIC
-   "-//W3C//ENTITIES Special for XHTML//EN"
-   "xhtml-special.ent">
-%HTMLspecial;
--->
-
-<!-- Begin embedded .ent file contents -->
-
-<!-- Portions (C) International Organization for Standardization 1986
-     Permission to copy in any form is granted for use with
-     conforming SGML systems and applications as defined in
-     ISO 8879, provided this notice is included in all copies.
--->
-<!-- Character entity set. Typical invocation:
-    <!ENTITY % HTMLlat1 PUBLIC
-       "-//W3C//ENTITIES Latin 1 for XHTML//EN"
-       "http://www.w3.org/TR/xhtml1/DTD/xhtml-lat1.ent">
-    %HTMLlat1;
--->
-
-<!ENTITY nbsp   "&#160;"> <!-- no-break space = non-breaking space,
-                                  U+00A0 ISOnum -->
-<!ENTITY iexcl  "&#161;"> <!-- inverted exclamation mark, U+00A1 ISOnum -->
-<!ENTITY cent   "&#162;"> <!-- cent sign, U+00A2 ISOnum -->
-<!ENTITY pound  "&#163;"> <!-- pound sign, U+00A3 ISOnum -->
-<!ENTITY curren "&#164;"> <!-- currency sign, U+00A4 ISOnum -->
-<!ENTITY yen    "&#165;"> <!-- yen sign = yuan sign, U+00A5 ISOnum -->
-<!ENTITY brvbar "&#166;"> <!-- broken bar = broken vertical bar,
-                                  U+00A6 ISOnum -->
-<!ENTITY sect   "&#167;"> <!-- section sign, U+00A7 ISOnum -->
-<!ENTITY uml    "&#168;"> <!-- diaeresis = spacing diaeresis,
-                                  U+00A8 ISOdia -->
-<!ENTITY copy   "&#169;"> <!-- copyright sign, U+00A9 ISOnum -->
-<!ENTITY ordf   "&#170;"> <!-- feminine ordinal indicator, U+00AA ISOnum -->
-<!ENTITY laquo  "&#171;"> <!-- left-pointing double angle quotation mark
-                                  = left pointing guillemet, U+00AB ISOnum -->
-<!ENTITY not    "&#172;"> <!-- not sign = angled dash,
-                                  U+00AC ISOnum -->
-<!ENTITY shy    "&#173;"> <!-- soft hyphen = discretionary hyphen,
-                                  U+00AD ISOnum -->
-<!ENTITY reg    "&#174;"> <!-- registered sign = registered trade mark sign,
-                                  U+00AE ISOnum -->
-<!ENTITY macr   "&#175;"> <!-- macron = spacing macron = overline
-                                  = APL overbar, U+00AF ISOdia -->
-<!ENTITY deg    "&#176;"> <!-- degree sign, U+00B0 ISOnum -->
-<!ENTITY plusmn "&#177;"> <!-- plus-minus sign = plus-or-minus sign,
-                                  U+00B1 ISOnum -->
-<!ENTITY sup2   "&#178;"> <!-- superscript two = superscript digit two
-                                  = squared, U+00B2 ISOnum -->
-<!ENTITY sup3   "&#179;"> <!-- superscript three = superscript digit three
-                                  = cubed, U+00B3 ISOnum -->
-<!ENTITY acute  "&#180;"> <!-- acute accent = spacing acute,
-                                  U+00B4 ISOdia -->
-<!ENTITY micro  "&#181;"> <!-- micro sign, U+00B5 ISOnum -->
-<!ENTITY para   "&#182;"> <!-- pilcrow sign = paragraph sign,
-                                  U+00B6 ISOnum -->
-<!ENTITY middot "&#183;"> <!-- middle dot = Georgian comma
-                                  = Greek middle dot, U+00B7 ISOnum -->
-<!ENTITY cedil  "&#184;"> <!-- cedilla = spacing cedilla, U+00B8 ISOdia -->
-<!ENTITY sup1   "&#185;"> <!-- superscript one = superscript digit one,
-                                  U+00B9 ISOnum -->
-<!ENTITY ordm   "&#186;"> <!-- masculine ordinal indicator,
-                                  U+00BA ISOnum -->
-<!ENTITY raquo  "&#187;"> <!-- right-pointing double angle quotation mark
-                                  = right pointing guillemet, U+00BB ISOnum -->
-<!ENTITY frac14 "&#188;"> <!-- vulgar fraction one quarter
-                                  = fraction one quarter, U+00BC ISOnum -->
-<!ENTITY frac12 "&#189;"> <!-- vulgar fraction one half
-                                  = fraction one half, U+00BD ISOnum -->
-<!ENTITY frac34 "&#190;"> <!-- vulgar fraction three quarters
-                                  = fraction three quarters, U+00BE ISOnum -->
-<!ENTITY iquest "&#191;"> <!-- inverted question mark
-                                  = turned question mark, U+00BF ISOnum -->
-<!ENTITY Agrave "&#192;"> <!-- latin capital letter A with grave
-                                  = latin capital letter A grave,
-                                  U+00C0 ISOlat1 -->
-<!ENTITY Aacute "&#193;"> <!-- latin capital letter A with acute,
-                                  U+00C1 ISOlat1 -->
-<!ENTITY Acirc  "&#194;"> <!-- latin capital letter A with circumflex,
-                                  U+00C2 ISOlat1 -->
-<!ENTITY Atilde "&#195;"> <!-- latin capital letter A with tilde,
-                                  U+00C3 ISOlat1 -->
-<!ENTITY Auml   "&#196;"> <!-- latin capital letter A with diaeresis,
-                                  U+00C4 ISOlat1 -->
-<!ENTITY Aring  "&#197;"> <!-- latin capital letter A with ring above
-                                  = latin capital letter A ring,
-                                  U+00C5 ISOlat1 -->
-<!ENTITY AElig  "&#198;"> <!-- latin capital letter AE
-                                  = latin capital ligature AE,
-                                  U+00C6 ISOlat1 -->
-<!ENTITY Ccedil "&#199;"> <!-- latin capital letter C with cedilla,
-                                  U+00C7 ISOlat1 -->
-<!ENTITY Egrave "&#200;"> <!-- latin capital letter E with grave,
-                                  U+00C8 ISOlat1 -->
-<!ENTITY Eacute "&#201;"> <!-- latin capital letter E with acute,
-                                  U+00C9 ISOlat1 -->
-<!ENTITY Ecirc  "&#202;"> <!-- latin capital letter E with circumflex,
-                                  U+00CA ISOlat1 -->
-<!ENTITY Euml   "&#203;"> <!-- latin capital letter E with diaeresis,
-                                  U+00CB ISOlat1 -->
-<!ENTITY Igrave "&#204;"> <!-- latin capital letter I with grave,
-                                  U+00CC ISOlat1 -->
-<!ENTITY Iacute "&#205;"> <!-- latin capital letter I with acute,
-                                  U+00CD ISOlat1 -->
-<!ENTITY Icirc  "&#206;"> <!-- latin capital letter I with circumflex,
-                                  U+00CE ISOlat1 -->
-<!ENTITY Iuml   "&#207;"> <!-- latin capital letter I with diaeresis,
-                                  U+00CF ISOlat1 -->
-<!ENTITY ETH    "&#208;"> <!-- latin capital letter ETH, U+00D0 ISOlat1 -->
-<!ENTITY Ntilde "&#209;"> <!-- latin capital letter N with tilde,
-                                  U+00D1 ISOlat1 -->
-<!ENTITY Ograve "&#210;"> <!-- latin capital letter O with grave,
-                                  U+00D2 ISOlat1 -->
-<!ENTITY Oacute "&#211;"> <!-- latin capital letter O with acute,
-                                  U+00D3 ISOlat1 -->
-<!ENTITY Ocirc  "&#212;"> <!-- latin capital letter O with circumflex,
-                                  U+00D4 ISOlat1 -->
-<!ENTITY Otilde "&#213;"> <!-- latin capital letter O with tilde,
-                                  U+00D5 ISOlat1 -->
-<!ENTITY Ouml   "&#214;"> <!-- latin capital letter O with diaeresis,
-                                  U+00D6 ISOlat1 -->
-<!ENTITY times  "&#215;"> <!-- multiplication sign, U+00D7 ISOnum -->
-<!ENTITY Oslash "&#216;"> <!-- latin capital letter O with stroke
-                                  = latin capital letter O slash,
-                                  U+00D8 ISOlat1 -->
-<!ENTITY Ugrave "&#217;"> <!-- latin capital letter U with grave,
-                                  U+00D9 ISOlat1 -->
-<!ENTITY Uacute "&#218;"> <!-- latin capital letter U with acute,
-                                  U+00DA ISOlat1 -->
-<!ENTITY Ucirc  "&#219;"> <!-- latin capital letter U with circumflex,
-                                  U+00DB ISOlat1 -->
-<!ENTITY Uuml   "&#220;"> <!-- latin capital letter U with diaeresis,
-                                  U+00DC ISOlat1 -->
-<!ENTITY Yacute "&#221;"> <!-- latin capital letter Y with acute,
-                                  U+00DD ISOlat1 -->
-<!ENTITY THORN  "&#222;"> <!-- latin capital letter THORN,
-                                  U+00DE ISOlat1 -->
-<!ENTITY szlig  "&#223;"> <!-- latin small letter sharp s = ess-zed,
-                                  U+00DF ISOlat1 -->
-<!ENTITY agrave "&#224;"> <!-- latin small letter a with grave
-                                  = latin small letter a grave,
-                                  U+00E0 ISOlat1 -->
-<!ENTITY aacute "&#225;"> <!-- latin small letter a with acute,
-                                  U+00E1 ISOlat1 -->
-<!ENTITY acirc  "&#226;"> <!-- latin small letter a with circumflex,
-                                  U+00E2 ISOlat1 -->
-<!ENTITY atilde "&#227;"> <!-- latin small letter a with tilde,
-                                  U+00E3 ISOlat1 -->
-<!ENTITY auml   "&#228;"> <!-- latin small letter a with diaeresis,
-                                  U+00E4 ISOlat1 -->
-<!ENTITY aring  "&#229;"> <!-- latin small letter a with ring above
-                                  = latin small letter a ring,
-                                  U+00E5 ISOlat1 -->
-<!ENTITY aelig  "&#230;"> <!-- latin small letter ae
-                                  = latin small ligature ae, U+00E6 ISOlat1 -->
-<!ENTITY ccedil "&#231;"> <!-- latin small letter c with cedilla,
-                                  U+00E7 ISOlat1 -->
-<!ENTITY egrave "&#232;"> <!-- latin small letter e with grave,
-                                  U+00E8 ISOlat1 -->
-<!ENTITY eacute "&#233;"> <!-- latin small letter e with acute,
-                                  U+00E9 ISOlat1 -->
-<!ENTITY ecirc  "&#234;"> <!-- latin small letter e with circumflex,
-                                  U+00EA ISOlat1 -->
-<!ENTITY euml   "&#235;"> <!-- latin small letter e with diaeresis,
-                                  U+00EB ISOlat1 -->
-<!ENTITY igrave "&#236;"> <!-- latin small letter i with grave,
-                                  U+00EC ISOlat1 -->
-<!ENTITY iacute "&#237;"> <!-- latin small letter i with acute,
-                                  U+00ED ISOlat1 -->
-<!ENTITY icirc  "&#238;"> <!-- latin small letter i with circumflex,
-                                  U+00EE ISOlat1 -->
-<!ENTITY iuml   "&#239;"> <!-- latin small letter i with diaeresis,
-                                  U+00EF ISOlat1 -->
-<!ENTITY eth    "&#240;"> <!-- latin small letter eth, U+00F0 ISOlat1 -->
-<!ENTITY ntilde "&#241;"> <!-- latin small letter n with tilde,
-                                  U+00F1 ISOlat1 -->
-<!ENTITY ograve "&#242;"> <!-- latin small letter o with grave,
-                                  U+00F2 ISOlat1 -->
-<!ENTITY oacute "&#243;"> <!-- latin small letter o with acute,
-                                  U+00F3 ISOlat1 -->
-<!ENTITY ocirc  "&#244;"> <!-- latin small letter o with circumflex,
-                                  U+00F4 ISOlat1 -->
-<!ENTITY otilde "&#245;"> <!-- latin small letter o with tilde,
-                                  U+00F5 ISOlat1 -->
-<!ENTITY ouml   "&#246;"> <!-- latin small letter o with diaeresis,
-                                  U+00F6 ISOlat1 -->
-<!ENTITY divide "&#247;"> <!-- division sign, U+00F7 ISOnum -->
-<!ENTITY oslash "&#248;"> <!-- latin small letter o with stroke,
-                                  = latin small letter o slash,
-                                  U+00F8 ISOlat1 -->
-<!ENTITY ugrave "&#249;"> <!-- latin small letter u with grave,
-                                  U+00F9 ISOlat1 -->
-<!ENTITY uacute "&#250;"> <!-- latin small letter u with acute,
-                                  U+00FA ISOlat1 -->
-<!ENTITY ucirc  "&#251;"> <!-- latin small letter u with circumflex,
-                                  U+00FB ISOlat1 -->
-<!ENTITY uuml   "&#252;"> <!-- latin small letter u with diaeresis,
-                                  U+00FC ISOlat1 -->
-<!ENTITY yacute "&#253;"> <!-- latin small letter y with acute,
-                                  U+00FD ISOlat1 -->
-<!ENTITY thorn  "&#254;"> <!-- latin small letter thorn,
-                                  U+00FE ISOlat1 -->
-<!ENTITY yuml   "&#255;"> <!-- latin small letter y with diaeresis,
-                                  U+00FF ISOlat1 -->
-<!-- Mathematical, Greek and Symbolic characters for XHTML -->
-
-<!-- Character entity set. Typical invocation:
-     <!ENTITY % HTMLsymbol PUBLIC
-        "-//W3C//ENTITIES Symbols for XHTML//EN"
-        "http://www.w3.org/TR/xhtml1/DTD/xhtml-symbol.ent">
-     %HTMLsymbol;
--->
-
-<!-- Portions (C) International Organization for Standardization 1986:
-     Permission to copy in any form is granted for use with
-     conforming SGML systems and applications as defined in
-     ISO 8879, provided this notice is included in all copies.
--->
-
-<!-- Relevant ISO entity set is given unless names are newly introduced.
-     New names (i.e., not in ISO 8879 list) do not clash with any
-     existing ISO 8879 entity names. ISO 10646 character numbers
-     are given for each character, in hex. values are decimal
-     conversions of the ISO 10646 values and refer to the document
-     character set. Names are Unicode names. 
--->
-
-<!-- Latin Extended-B -->
-<!ENTITY fnof     "&#402;"> <!-- latin small letter f with hook = function
-                                    = florin, U+0192 ISOtech -->
-
-<!-- Greek -->
-<!ENTITY Alpha    "&#913;"> <!-- greek capital letter alpha, U+0391 -->
-<!ENTITY Beta     "&#914;"> <!-- greek capital letter beta, U+0392 -->
-<!ENTITY Gamma    "&#915;"> <!-- greek capital letter gamma,
-                                    U+0393 ISOgrk3 -->
-<!ENTITY Delta    "&#916;"> <!-- greek capital letter delta,
-                                    U+0394 ISOgrk3 -->
-<!ENTITY Epsilon  "&#917;"> <!-- greek capital letter epsilon, U+0395 -->
-<!ENTITY Zeta     "&#918;"> <!-- greek capital letter zeta, U+0396 -->
-<!ENTITY Eta      "&#919;"> <!-- greek capital letter eta, U+0397 -->
-<!ENTITY Theta    "&#920;"> <!-- greek capital letter theta,
-                                    U+0398 ISOgrk3 -->
-<!ENTITY Iota     "&#921;"> <!-- greek capital letter iota, U+0399 -->
-<!ENTITY Kappa    "&#922;"> <!-- greek capital letter kappa, U+039A -->
-<!ENTITY Lambda   "&#923;"> <!-- greek capital letter lamda,
-                                    U+039B ISOgrk3 -->
-<!ENTITY Mu       "&#924;"> <!-- greek capital letter mu, U+039C -->
-<!ENTITY Nu       "&#925;"> <!-- greek capital letter nu, U+039D -->
-<!ENTITY Xi       "&#926;"> <!-- greek capital letter xi, U+039E ISOgrk3 -->
-<!ENTITY Omicron  "&#927;"> <!-- greek capital letter omicron, U+039F -->
-<!ENTITY Pi       "&#928;"> <!-- greek capital letter pi, U+03A0 ISOgrk3 -->
-<!ENTITY Rho      "&#929;"> <!-- greek capital letter rho, U+03A1 -->
-<!-- there is no Sigmaf, and no U+03A2 character either -->
-<!ENTITY Sigma    "&#931;"> <!-- greek capital letter sigma,
-                                    U+03A3 ISOgrk3 -->
-<!ENTITY Tau      "&#932;"> <!-- greek capital letter tau, U+03A4 -->
-<!ENTITY Upsilon  "&#933;"> <!-- greek capital letter upsilon,
-                                    U+03A5 ISOgrk3 -->
-<!ENTITY Phi      "&#934;"> <!-- greek capital letter phi,
-                                    U+03A6 ISOgrk3 -->
-<!ENTITY Chi      "&#935;"> <!-- greek capital letter chi, U+03A7 -->
-<!ENTITY Psi      "&#936;"> <!-- greek capital letter psi,
-                                    U+03A8 ISOgrk3 -->
-<!ENTITY Omega    "&#937;"> <!-- greek capital letter omega,
-                                    U+03A9 ISOgrk3 -->
-
-<!ENTITY alpha    "&#945;"> <!-- greek small letter alpha,
-                                    U+03B1 ISOgrk3 -->
-<!ENTITY beta     "&#946;"> <!-- greek small letter beta, U+03B2 ISOgrk3 -->
-<!ENTITY gamma    "&#947;"> <!-- greek small letter gamma,
-                                    U+03B3 ISOgrk3 -->
-<!ENTITY delta    "&#948;"> <!-- greek small letter delta,
-                                    U+03B4 ISOgrk3 -->
-<!ENTITY epsilon  "&#949;"> <!-- greek small letter epsilon,
-                                    U+03B5 ISOgrk3 -->
-<!ENTITY zeta     "&#950;"> <!-- greek small letter zeta, U+03B6 ISOgrk3 -->
-<!ENTITY eta      "&#951;"> <!-- greek small letter eta, U+03B7 ISOgrk3 -->
-<!ENTITY theta    "&#952;"> <!-- greek small letter theta,
-                                    U+03B8 ISOgrk3 -->
-<!ENTITY iota     "&#953;"> <!-- greek small letter iota, U+03B9 ISOgrk3 -->
-<!ENTITY kappa    "&#954;"> <!-- greek small letter kappa,
-                                    U+03BA ISOgrk3 -->
-<!ENTITY lambda   "&#955;"> <!-- greek small letter lamda,
-                                    U+03BB ISOgrk3 -->
-<!ENTITY mu       "&#956;"> <!-- greek small letter mu, U+03BC ISOgrk3 -->
-<!ENTITY nu       "&#957;"> <!-- greek small letter nu, U+03BD ISOgrk3 -->
-<!ENTITY xi       "&#958;"> <!-- greek small letter xi, U+03BE ISOgrk3 -->
-<!ENTITY omicron  "&#959;"> <!-- greek small letter omicron, U+03BF NEW -->
-<!ENTITY pi       "&#960;"> <!-- greek small letter pi, U+03C0 ISOgrk3 -->
-<!ENTITY rho      "&#961;"> <!-- greek small letter rho, U+03C1 ISOgrk3 -->
-<!ENTITY sigmaf   "&#962;"> <!-- greek small letter final sigma,
-                                    U+03C2 ISOgrk3 -->
-<!ENTITY sigma    "&#963;"> <!-- greek small letter sigma,
-                                    U+03C3 ISOgrk3 -->
-<!ENTITY tau      "&#964;"> <!-- greek small letter tau, U+03C4 ISOgrk3 -->
-<!ENTITY upsilon  "&#965;"> <!-- greek small letter upsilon,
-                                    U+03C5 ISOgrk3 -->
-<!ENTITY phi      "&#966;"> <!-- greek small letter phi, U+03C6 ISOgrk3 -->
-<!ENTITY chi      "&#967;"> <!-- greek small letter chi, U+03C7 ISOgrk3 -->
-<!ENTITY psi      "&#968;"> <!-- greek small letter psi, U+03C8 ISOgrk3 -->
-<!ENTITY omega    "&#969;"> <!-- greek small letter omega,
-                                    U+03C9 ISOgrk3 -->
-<!ENTITY thetasym "&#977;"> <!-- greek theta symbol,
-                                    U+03D1 NEW -->
-<!ENTITY upsih    "&#978;"> <!-- greek upsilon with hook symbol,
-                                    U+03D2 NEW -->
-<!ENTITY piv      "&#982;"> <!-- greek pi symbol, U+03D6 ISOgrk3 -->
-
-<!-- General Punctuation -->
-<!ENTITY bull     "&#8226;"> <!-- bullet = black small circle,
-                                     U+2022 ISOpub  -->
-<!-- bullet is NOT the same as bullet operator, U+2219 -->
-<!ENTITY hellip   "&#8230;"> <!-- horizontal ellipsis = three dot leader,
-                                     U+2026 ISOpub  -->
-<!ENTITY prime    "&#8242;"> <!-- prime = minutes = feet, U+2032 ISOtech -->
-<!ENTITY Prime    "&#8243;"> <!-- double prime = seconds = inches,
-                                     U+2033 ISOtech -->
-<!ENTITY oline    "&#8254;"> <!-- overline = spacing overscore,
-                                     U+203E NEW -->
-<!ENTITY frasl    "&#8260;"> <!-- fraction slash, U+2044 NEW -->
-
-<!-- Letterlike Symbols -->
-<!ENTITY weierp   "&#8472;"> <!-- script capital P = power set
-                                     = Weierstrass p, U+2118 ISOamso -->
-<!ENTITY image    "&#8465;"> <!-- black-letter capital I = imaginary part,
-                                     U+2111 ISOamso -->
-<!ENTITY real     "&#8476;"> <!-- black-letter capital R = real part symbol,
-                                     U+211C ISOamso -->
-<!ENTITY trade    "&#8482;"> <!-- trade mark sign, U+2122 ISOnum -->
-<!ENTITY alefsym  "&#8501;"> <!-- alef symbol = first transfinite cardinal,
-                                     U+2135 NEW -->
-<!-- alef symbol is NOT the same as hebrew letter alef,
-     U+05D0 although the same glyph could be used to depict both characters -->
-
-<!-- Arrows -->
-<!ENTITY larr     "&#8592;"> <!-- leftwards arrow, U+2190 ISOnum -->
-<!ENTITY uarr     "&#8593;"> <!-- upwards arrow, U+2191 ISOnum-->
-<!ENTITY rarr     "&#8594;"> <!-- rightwards arrow, U+2192 ISOnum -->
-<!ENTITY darr     "&#8595;"> <!-- downwards arrow, U+2193 ISOnum -->
-<!ENTITY harr     "&#8596;"> <!-- left right arrow, U+2194 ISOamsa -->
-<!ENTITY crarr    "&#8629;"> <!-- downwards arrow with corner leftwards
-                                     = carriage return, U+21B5 NEW -->
-<!ENTITY lArr     "&#8656;"> <!-- leftwards double arrow, U+21D0 ISOtech -->
-<!-- Unicode does not say that lArr is the same as the 'is implied by' arrow
-    but also does not have any other character for that function. So lArr can
-    be used for 'is implied by' as ISOtech suggests -->
-<!ENTITY uArr     "&#8657;"> <!-- upwards double arrow, U+21D1 ISOamsa -->
-<!ENTITY rArr     "&#8658;"> <!-- rightwards double arrow,
-                                     U+21D2 ISOtech -->
-<!-- Unicode does not say this is the 'implies' character but does not have 
-     another character with this function so rArr can be used for 'implies'
-     as ISOtech suggests -->
-<!ENTITY dArr     "&#8659;"> <!-- downwards double arrow, U+21D3 ISOamsa -->
-<!ENTITY hArr     "&#8660;"> <!-- left right double arrow,
-                                     U+21D4 ISOamsa -->
-
-<!-- Mathematical Operators -->
-<!ENTITY forall   "&#8704;"> <!-- for all, U+2200 ISOtech -->
-<!ENTITY part     "&#8706;"> <!-- partial differential, U+2202 ISOtech  -->
-<!ENTITY exist    "&#8707;"> <!-- there exists, U+2203 ISOtech -->
-<!ENTITY empty    "&#8709;"> <!-- empty set = null set, U+2205 ISOamso -->
-<!ENTITY nabla    "&#8711;"> <!-- nabla = backward difference,
-                                     U+2207 ISOtech -->
-<!ENTITY isin     "&#8712;"> <!-- element of, U+2208 ISOtech -->
-<!ENTITY notin    "&#8713;"> <!-- not an element of, U+2209 ISOtech -->
-<!ENTITY ni       "&#8715;"> <!-- contains as member, U+220B ISOtech -->
-<!ENTITY prod     "&#8719;"> <!-- n-ary product = product sign,
-                                     U+220F ISOamsb -->
-<!-- prod is NOT the same character as U+03A0 'greek capital letter pi' though
-     the same glyph might be used for both -->
-<!ENTITY sum      "&#8721;"> <!-- n-ary summation, U+2211 ISOamsb -->
-<!-- sum is NOT the same character as U+03A3 'greek capital letter sigma'
-     though the same glyph might be used for both -->
-<!ENTITY minus    "&#8722;"> <!-- minus sign, U+2212 ISOtech -->
-<!ENTITY lowast   "&#8727;"> <!-- asterisk operator, U+2217 ISOtech -->
-<!ENTITY radic    "&#8730;"> <!-- square root = radical sign,
-                                     U+221A ISOtech -->
-<!ENTITY prop     "&#8733;"> <!-- proportional to, U+221D ISOtech -->
-<!ENTITY infin    "&#8734;"> <!-- infinity, U+221E ISOtech -->
-<!ENTITY ang      "&#8736;"> <!-- angle, U+2220 ISOamso -->
-<!ENTITY and      "&#8743;"> <!-- logical and = wedge, U+2227 ISOtech -->
-<!ENTITY or       "&#8744;"> <!-- logical or = vee, U+2228 ISOtech -->
-<!ENTITY cap      "&#8745;"> <!-- intersection = cap, U+2229 ISOtech -->
-<!ENTITY cup      "&#8746;"> <!-- union = cup, U+222A ISOtech -->
-<!ENTITY int      "&#8747;"> <!-- integral, U+222B ISOtech -->
-<!ENTITY there4   "&#8756;"> <!-- therefore, U+2234 ISOtech -->
-<!ENTITY sim      "&#8764;"> <!-- tilde operator = varies with = similar to,
-                                     U+223C ISOtech -->
-<!-- tilde operator is NOT the same character as the tilde, U+007E,
-     although the same glyph might be used to represent both  -->
-<!ENTITY cong     "&#8773;"> <!-- approximately equal to, U+2245 ISOtech -->
-<!ENTITY asymp    "&#8776;"> <!-- almost equal to = asymptotic to,
-                                     U+2248 ISOamsr -->
-<!ENTITY ne       "&#8800;"> <!-- not equal to, U+2260 ISOtech -->
-<!ENTITY equiv    "&#8801;"> <!-- identical to, U+2261 ISOtech -->
-<!ENTITY le       "&#8804;"> <!-- less-than or equal to, U+2264 ISOtech -->
-<!ENTITY ge       "&#8805;"> <!-- greater-than or equal to,
-                                     U+2265 ISOtech -->
-<!ENTITY sub      "&#8834;"> <!-- subset of, U+2282 ISOtech -->
-<!ENTITY sup      "&#8835;"> <!-- superset of, U+2283 ISOtech -->
-<!ENTITY nsub     "&#8836;"> <!-- not a subset of, U+2284 ISOamsn -->
-<!ENTITY sube     "&#8838;"> <!-- subset of or equal to, U+2286 ISOtech -->
-<!ENTITY supe     "&#8839;"> <!-- superset of or equal to,
-                                     U+2287 ISOtech -->
-<!ENTITY oplus    "&#8853;"> <!-- circled plus = direct sum,
-                                     U+2295 ISOamsb -->
-<!ENTITY otimes   "&#8855;"> <!-- circled times = vector product,
-                                     U+2297 ISOamsb -->
-<!ENTITY perp     "&#8869;"> <!-- up tack = orthogonal to = perpendicular,
-                                     U+22A5 ISOtech -->
-<!ENTITY sdot     "&#8901;"> <!-- dot operator, U+22C5 ISOamsb -->
-<!-- dot operator is NOT the same character as U+00B7 middle dot -->
-
-<!-- Miscellaneous Technical -->
-<!ENTITY lceil    "&#8968;"> <!-- left ceiling = APL upstile,
-                                     U+2308 ISOamsc  -->
-<!ENTITY rceil    "&#8969;"> <!-- right ceiling, U+2309 ISOamsc  -->
-<!ENTITY lfloor   "&#8970;"> <!-- left floor = APL downstile,
-                                     U+230A ISOamsc  -->
-<!ENTITY rfloor   "&#8971;"> <!-- right floor, U+230B ISOamsc  -->
-<!ENTITY lang     "&#9001;"> <!-- left-pointing angle bracket = bra,
-                                     U+2329 ISOtech -->
-<!-- lang is NOT the same character as U+003C 'less than sign' 
-     or U+2039 'single left-pointing angle quotation mark' -->
-<!ENTITY rang     "&#9002;"> <!-- right-pointing angle bracket = ket,
-                                     U+232A ISOtech -->
-<!-- rang is NOT the same character as U+003E 'greater than sign' 
-     or U+203A 'single right-pointing angle quotation mark' -->
-
-<!-- Geometric Shapes -->
-<!ENTITY loz      "&#9674;"> <!-- lozenge, U+25CA ISOpub -->
-
-<!-- Miscellaneous Symbols -->
-<!ENTITY spades   "&#9824;"> <!-- black spade suit, U+2660 ISOpub -->
-<!-- black here seems to mean filled as opposed to hollow -->
-<!ENTITY clubs    "&#9827;"> <!-- black club suit = shamrock,
-                                     U+2663 ISOpub -->
-<!ENTITY hearts   "&#9829;"> <!-- black heart suit = valentine,
-                                     U+2665 ISOpub -->
-<!ENTITY diams    "&#9830;"> <!-- black diamond suit, U+2666 ISOpub -->
-
-<!-- Special characters for XHTML -->
-
-<!-- Character entity set. Typical invocation:
-     <!ENTITY % HTMLspecial PUBLIC
-        "-//W3C//ENTITIES Special for XHTML//EN"
-        "http://www.w3.org/TR/xhtml1/DTD/xhtml-special.ent">
-     %HTMLspecial;
--->
-
-<!-- Portions (C) International Organization for Standardization 1986:
-     Permission to copy in any form is granted for use with
-     conforming SGML systems and applications as defined in
-     ISO 8879, provided this notice is included in all copies.
--->
-
-<!-- Relevant ISO entity set is given unless names are newly introduced.
-     New names (i.e., not in ISO 8879 list) do not clash with any
-     existing ISO 8879 entity names. ISO 10646 character numbers
-     are given for each character, in hex. values are decimal
-     conversions of the ISO 10646 values and refer to the document
-     character set. Names are Unicode names. 
--->
-
-<!-- C0 Controls and Basic Latin -->
-<!ENTITY quot    "&#34;"> <!--  quotation mark, U+0022 ISOnum -->
-<!ENTITY amp     "&#38;#38;"> <!--  ampersand, U+0026 ISOnum -->
-<!ENTITY lt      "&#38;#60;"> <!--  less-than sign, U+003C ISOnum -->
-<!ENTITY gt      "&#62;"> <!--  greater-than sign, U+003E ISOnum -->
-<!ENTITY apos	 "&#39;"> <!--  apostrophe = APL quote, U+0027 ISOnum -->
-
-<!-- Latin Extended-A -->
-<!ENTITY OElig   "&#338;"> <!--  latin capital ligature OE,
-                                    U+0152 ISOlat2 -->
-<!ENTITY oelig   "&#339;"> <!--  latin small ligature oe, U+0153 ISOlat2 -->
-<!-- ligature is a misnomer, this is a separate character in some languages -->
-<!ENTITY Scaron  "&#352;"> <!--  latin capital letter S with caron,
-                                    U+0160 ISOlat2 -->
-<!ENTITY scaron  "&#353;"> <!--  latin small letter s with caron,
-                                    U+0161 ISOlat2 -->
-<!ENTITY Yuml    "&#376;"> <!--  latin capital letter Y with diaeresis,
-                                    U+0178 ISOlat2 -->
-
-<!-- Spacing Modifier Letters -->
-<!ENTITY circ    "&#710;"> <!--  modifier letter circumflex accent,
-                                    U+02C6 ISOpub -->
-<!ENTITY tilde   "&#732;"> <!--  small tilde, U+02DC ISOdia -->
-
-<!-- General Punctuation -->
-<!ENTITY ensp    "&#8194;"> <!-- en space, U+2002 ISOpub -->
-<!ENTITY emsp    "&#8195;"> <!-- em space, U+2003 ISOpub -->
-<!ENTITY thinsp  "&#8201;"> <!-- thin space, U+2009 ISOpub -->
-<!ENTITY zwnj    "&#8204;"> <!-- zero width non-joiner,
-                                    U+200C NEW RFC 2070 -->
-<!ENTITY zwj     "&#8205;"> <!-- zero width joiner, U+200D NEW RFC 2070 -->
-<!ENTITY lrm     "&#8206;"> <!-- left-to-right mark, U+200E NEW RFC 2070 -->
-<!ENTITY rlm     "&#8207;"> <!-- right-to-left mark, U+200F NEW RFC 2070 -->
-<!ENTITY ndash   "&#8211;"> <!-- en dash, U+2013 ISOpub -->
-<!ENTITY mdash   "&#8212;"> <!-- em dash, U+2014 ISOpub -->
-<!ENTITY lsquo   "&#8216;"> <!-- left single quotation mark,
-                                    U+2018 ISOnum -->
-<!ENTITY rsquo   "&#8217;"> <!-- right single quotation mark,
-                                    U+2019 ISOnum -->
-<!ENTITY sbquo   "&#8218;"> <!-- single low-9 quotation mark, U+201A NEW -->
-<!ENTITY ldquo   "&#8220;"> <!-- left double quotation mark,
-                                    U+201C ISOnum -->
-<!ENTITY rdquo   "&#8221;"> <!-- right double quotation mark,
-                                    U+201D ISOnum -->
-<!ENTITY bdquo   "&#8222;"> <!-- double low-9 quotation mark, U+201E NEW -->
-<!ENTITY dagger  "&#8224;"> <!-- dagger, U+2020 ISOpub -->
-<!ENTITY Dagger  "&#8225;"> <!-- double dagger, U+2021 ISOpub -->
-<!ENTITY permil  "&#8240;"> <!-- per mille sign, U+2030 ISOtech -->
-<!ENTITY lsaquo  "&#8249;"> <!-- single left-pointing angle quotation mark,
-                                    U+2039 ISO proposed -->
-<!-- lsaquo is proposed but not yet ISO standardized -->
-<!ENTITY rsaquo  "&#8250;"> <!-- single right-pointing angle quotation mark,
-                                    U+203A ISO proposed -->
-<!-- rsaquo is proposed but not yet ISO standardized -->
-
-<!-- Currency Symbols -->
-<!ENTITY euro   "&#8364;"> <!--  euro sign, U+20AC NEW -->
-
-<!-- End embedded .ent file contents -->
+<!-- Character mnemonic entities -->
+
+<!--
+<!ENTITY % HTMLlat1 PUBLIC
+   "-//W3C//ENTITIES Latin 1 for XHTML//EN"
+   "xhtml-lat1.ent">
+%HTMLlat1;
+
+<!ENTITY % HTMLsymbol PUBLIC
+   "-//W3C//ENTITIES Symbols for XHTML//EN"
+   "xhtml-symbol.ent">
+%HTMLsymbol;
+
+<!ENTITY % HTMLspecial PUBLIC
+   "-//W3C//ENTITIES Special for XHTML//EN"
+   "xhtml-special.ent">
+%HTMLspecial;
+-->
+
+<!-- Begin embedded .ent file contents -->
+
+<!-- Portions (C) International Organization for Standardization 1986
+     Permission to copy in any form is granted for use with
+     conforming SGML systems and applications as defined in
+     ISO 8879, provided this notice is included in all copies.
+-->
+<!-- Character entity set. Typical invocation:
+    <!ENTITY % HTMLlat1 PUBLIC
+       "-//W3C//ENTITIES Latin 1 for XHTML//EN"
+       "http://www.w3.org/TR/xhtml1/DTD/xhtml-lat1.ent">
+    %HTMLlat1;
+-->
+
+<!ENTITY nbsp   "&#160;"> <!-- no-break space = non-breaking space,
+                                  U+00A0 ISOnum -->
+<!ENTITY iexcl  "&#161;"> <!-- inverted exclamation mark, U+00A1 ISOnum -->
+<!ENTITY cent   "&#162;"> <!-- cent sign, U+00A2 ISOnum -->
+<!ENTITY pound  "&#163;"> <!-- pound sign, U+00A3 ISOnum -->
+<!ENTITY curren "&#164;"> <!-- currency sign, U+00A4 ISOnum -->
+<!ENTITY yen    "&#165;"> <!-- yen sign = yuan sign, U+00A5 ISOnum -->
+<!ENTITY brvbar "&#166;"> <!-- broken bar = broken vertical bar,
+                                  U+00A6 ISOnum -->
+<!ENTITY sect   "&#167;"> <!-- section sign, U+00A7 ISOnum -->
+<!ENTITY uml    "&#168;"> <!-- diaeresis = spacing diaeresis,
+                                  U+00A8 ISOdia -->
+<!ENTITY copy   "&#169;"> <!-- copyright sign, U+00A9 ISOnum -->
+<!ENTITY ordf   "&#170;"> <!-- feminine ordinal indicator, U+00AA ISOnum -->
+<!ENTITY laquo  "&#171;"> <!-- left-pointing double angle quotation mark
+                                  = left pointing guillemet, U+00AB ISOnum -->
+<!ENTITY not    "&#172;"> <!-- not sign = angled dash,
+                                  U+00AC ISOnum -->
+<!ENTITY shy    "&#173;"> <!-- soft hyphen = discretionary hyphen,
+                                  U+00AD ISOnum -->
+<!ENTITY reg    "&#174;"> <!-- registered sign = registered trade mark sign,
+                                  U+00AE ISOnum -->
+<!ENTITY macr   "&#175;"> <!-- macron = spacing macron = overline
+                                  = APL overbar, U+00AF ISOdia -->
+<!ENTITY deg    "&#176;"> <!-- degree sign, U+00B0 ISOnum -->
+<!ENTITY plusmn "&#177;"> <!-- plus-minus sign = plus-or-minus sign,
+                                  U+00B1 ISOnum -->
+<!ENTITY sup2   "&#178;"> <!-- superscript two = superscript digit two
+                                  = squared, U+00B2 ISOnum -->
+<!ENTITY sup3   "&#179;"> <!-- superscript three = superscript digit three
+                                  = cubed, U+00B3 ISOnum -->
+<!ENTITY acute  "&#180;"> <!-- acute accent = spacing acute,
+                                  U+00B4 ISOdia -->
+<!ENTITY micro  "&#181;"> <!-- micro sign, U+00B5 ISOnum -->
+<!ENTITY para   "&#182;"> <!-- pilcrow sign = paragraph sign,
+                                  U+00B6 ISOnum -->
+<!ENTITY middot "&#183;"> <!-- middle dot = Georgian comma
+                                  = Greek middle dot, U+00B7 ISOnum -->
+<!ENTITY cedil  "&#184;"> <!-- cedilla = spacing cedilla, U+00B8 ISOdia -->
+<!ENTITY sup1   "&#185;"> <!-- superscript one = superscript digit one,
+                                  U+00B9 ISOnum -->
+<!ENTITY ordm   "&#186;"> <!-- masculine ordinal indicator,
+                                  U+00BA ISOnum -->
+<!ENTITY raquo  "&#187;"> <!-- right-pointing double angle quotation mark
+                                  = right pointing guillemet, U+00BB ISOnum -->
+<!ENTITY frac14 "&#188;"> <!-- vulgar fraction one quarter
+                                  = fraction one quarter, U+00BC ISOnum -->
+<!ENTITY frac12 "&#189;"> <!-- vulgar fraction one half
+                                  = fraction one half, U+00BD ISOnum -->
+<!ENTITY frac34 "&#190;"> <!-- vulgar fraction three quarters
+                                  = fraction three quarters, U+00BE ISOnum -->
+<!ENTITY iquest "&#191;"> <!-- inverted question mark
+                                  = turned question mark, U+00BF ISOnum -->
+<!ENTITY Agrave "&#192;"> <!-- latin capital letter A with grave
+                                  = latin capital letter A grave,
+                                  U+00C0 ISOlat1 -->
+<!ENTITY Aacute "&#193;"> <!-- latin capital letter A with acute,
+                                  U+00C1 ISOlat1 -->
+<!ENTITY Acirc  "&#194;"> <!-- latin capital letter A with circumflex,
+                                  U+00C2 ISOlat1 -->
+<!ENTITY Atilde "&#195;"> <!-- latin capital letter A with tilde,
+                                  U+00C3 ISOlat1 -->
+<!ENTITY Auml   "&#196;"> <!-- latin capital letter A with diaeresis,
+                                  U+00C4 ISOlat1 -->
+<!ENTITY Aring  "&#197;"> <!-- latin capital letter A with ring above
+                                  = latin capital letter A ring,
+                                  U+00C5 ISOlat1 -->
+<!ENTITY AElig  "&#198;"> <!-- latin capital letter AE
+                                  = latin capital ligature AE,
+                                  U+00C6 ISOlat1 -->
+<!ENTITY Ccedil "&#199;"> <!-- latin capital letter C with cedilla,
+                                  U+00C7 ISOlat1 -->
+<!ENTITY Egrave "&#200;"> <!-- latin capital letter E with grave,
+                                  U+00C8 ISOlat1 -->
+<!ENTITY Eacute "&#201;"> <!-- latin capital letter E with acute,
+                                  U+00C9 ISOlat1 -->
+<!ENTITY Ecirc  "&#202;"> <!-- latin capital letter E with circumflex,
+                                  U+00CA ISOlat1 -->
+<!ENTITY Euml   "&#203;"> <!-- latin capital letter E with diaeresis,
+                                  U+00CB ISOlat1 -->
+<!ENTITY Igrave "&#204;"> <!-- latin capital letter I with grave,
+                                  U+00CC ISOlat1 -->
+<!ENTITY Iacute "&#205;"> <!-- latin capital letter I with acute,
+                                  U+00CD ISOlat1 -->
+<!ENTITY Icirc  "&#206;"> <!-- latin capital letter I with circumflex,
+                                  U+00CE ISOlat1 -->
+<!ENTITY Iuml   "&#207;"> <!-- latin capital letter I with diaeresis,
+                                  U+00CF ISOlat1 -->
+<!ENTITY ETH    "&#208;"> <!-- latin capital letter ETH, U+00D0 ISOlat1 -->
+<!ENTITY Ntilde "&#209;"> <!-- latin capital letter N with tilde,
+                                  U+00D1 ISOlat1 -->
+<!ENTITY Ograve "&#210;"> <!-- latin capital letter O with grave,
+                                  U+00D2 ISOlat1 -->
+<!ENTITY Oacute "&#211;"> <!-- latin capital letter O with acute,
+                                  U+00D3 ISOlat1 -->
+<!ENTITY Ocirc  "&#212;"> <!-- latin capital letter O with circumflex,
+                                  U+00D4 ISOlat1 -->
+<!ENTITY Otilde "&#213;"> <!-- latin capital letter O with tilde,
+                                  U+00D5 ISOlat1 -->
+<!ENTITY Ouml   "&#214;"> <!-- latin capital letter O with diaeresis,
+                                  U+00D6 ISOlat1 -->
+<!ENTITY times  "&#215;"> <!-- multiplication sign, U+00D7 ISOnum -->
+<!ENTITY Oslash "&#216;"> <!-- latin capital letter O with stroke
+                                  = latin capital letter O slash,
+                                  U+00D8 ISOlat1 -->
+<!ENTITY Ugrave "&#217;"> <!-- latin capital letter U with grave,
+                                  U+00D9 ISOlat1 -->
+<!ENTITY Uacute "&#218;"> <!-- latin capital letter U with acute,
+                                  U+00DA ISOlat1 -->
+<!ENTITY Ucirc  "&#219;"> <!-- latin capital letter U with circumflex,
+                                  U+00DB ISOlat1 -->
+<!ENTITY Uuml   "&#220;"> <!-- latin capital letter U with diaeresis,
+                                  U+00DC ISOlat1 -->
+<!ENTITY Yacute "&#221;"> <!-- latin capital letter Y with acute,
+                                  U+00DD ISOlat1 -->
+<!ENTITY THORN  "&#222;"> <!-- latin capital letter THORN,
+                                  U+00DE ISOlat1 -->
+<!ENTITY szlig  "&#223;"> <!-- latin small letter sharp s = ess-zed,
+                                  U+00DF ISOlat1 -->
+<!ENTITY agrave "&#224;"> <!-- latin small letter a with grave
+                                  = latin small letter a grave,
+                                  U+00E0 ISOlat1 -->
+<!ENTITY aacute "&#225;"> <!-- latin small letter a with acute,
+                                  U+00E1 ISOlat1 -->
+<!ENTITY acirc  "&#226;"> <!-- latin small letter a with circumflex,
+                                  U+00E2 ISOlat1 -->
+<!ENTITY atilde "&#227;"> <!-- latin small letter a with tilde,
+                                  U+00E3 ISOlat1 -->
+<!ENTITY auml   "&#228;"> <!-- latin small letter a with diaeresis,
+                                  U+00E4 ISOlat1 -->
+<!ENTITY aring  "&#229;"> <!-- latin small letter a with ring above
+                                  = latin small letter a ring,
+                                  U+00E5 ISOlat1 -->
+<!ENTITY aelig  "&#230;"> <!-- latin small letter ae
+                                  = latin small ligature ae, U+00E6 ISOlat1 -->
+<!ENTITY ccedil "&#231;"> <!-- latin small letter c with cedilla,
+                                  U+00E7 ISOlat1 -->
+<!ENTITY egrave "&#232;"> <!-- latin small letter e with grave,
+                                  U+00E8 ISOlat1 -->
+<!ENTITY eacute "&#233;"> <!-- latin small letter e with acute,
+                                  U+00E9 ISOlat1 -->
+<!ENTITY ecirc  "&#234;"> <!-- latin small letter e with circumflex,
+                                  U+00EA ISOlat1 -->
+<!ENTITY euml   "&#235;"> <!-- latin small letter e with diaeresis,
+                                  U+00EB ISOlat1 -->
+<!ENTITY igrave "&#236;"> <!-- latin small letter i with grave,
+                                  U+00EC ISOlat1 -->
+<!ENTITY iacute "&#237;"> <!-- latin small letter i with acute,
+                                  U+00ED ISOlat1 -->
+<!ENTITY icirc  "&#238;"> <!-- latin small letter i with circumflex,
+                                  U+00EE ISOlat1 -->
+<!ENTITY iuml   "&#239;"> <!-- latin small letter i with diaeresis,
+                                  U+00EF ISOlat1 -->
+<!ENTITY eth    "&#240;"> <!-- latin small letter eth, U+00F0 ISOlat1 -->
+<!ENTITY ntilde "&#241;"> <!-- latin small letter n with tilde,
+                                  U+00F1 ISOlat1 -->
+<!ENTITY ograve "&#242;"> <!-- latin small letter o with grave,
+                                  U+00F2 ISOlat1 -->
+<!ENTITY oacute "&#243;"> <!-- latin small letter o with acute,
+                                  U+00F3 ISOlat1 -->
+<!ENTITY ocirc  "&#244;"> <!-- latin small letter o with circumflex,
+                                  U+00F4 ISOlat1 -->
+<!ENTITY otilde "&#245;"> <!-- latin small letter o with tilde,
+                                  U+00F5 ISOlat1 -->
+<!ENTITY ouml   "&#246;"> <!-- latin small letter o with diaeresis,
+                                  U+00F6 ISOlat1 -->
+<!ENTITY divide "&#247;"> <!-- division sign, U+00F7 ISOnum -->
+<!ENTITY oslash "&#248;"> <!-- latin small letter o with stroke,
+                                  = latin small letter o slash,
+                                  U+00F8 ISOlat1 -->
+<!ENTITY ugrave "&#249;"> <!-- latin small letter u with grave,
+                                  U+00F9 ISOlat1 -->
+<!ENTITY uacute "&#250;"> <!-- latin small letter u with acute,
+                                  U+00FA ISOlat1 -->
+<!ENTITY ucirc  "&#251;"> <!-- latin small letter u with circumflex,
+                                  U+00FB ISOlat1 -->
+<!ENTITY uuml   "&#252;"> <!-- latin small letter u with diaeresis,
+                                  U+00FC ISOlat1 -->
+<!ENTITY yacute "&#253;"> <!-- latin small letter y with acute,
+                                  U+00FD ISOlat1 -->
+<!ENTITY thorn  "&#254;"> <!-- latin small letter thorn,
+                                  U+00FE ISOlat1 -->
+<!ENTITY yuml   "&#255;"> <!-- latin small letter y with diaeresis,
+                                  U+00FF ISOlat1 -->
+<!-- Mathematical, Greek and Symbolic characters for XHTML -->
+
+<!-- Character entity set. Typical invocation:
+     <!ENTITY % HTMLsymbol PUBLIC
+        "-//W3C//ENTITIES Symbols for XHTML//EN"
+        "http://www.w3.org/TR/xhtml1/DTD/xhtml-symbol.ent">
+     %HTMLsymbol;
+-->
+
+<!-- Portions (C) International Organization for Standardization 1986:
+     Permission to copy in any form is granted for use with
+     conforming SGML systems and applications as defined in
+     ISO 8879, provided this notice is included in all copies.
+-->
+
+<!-- Relevant ISO entity set is given unless names are newly introduced.
+     New names (i.e., not in ISO 8879 list) do not clash with any
+     existing ISO 8879 entity names. ISO 10646 character numbers
+     are given for each character, in hex. values are decimal
+     conversions of the ISO 10646 values and refer to the document
+     character set. Names are Unicode names. 
+-->
+
+<!-- Latin Extended-B -->
+<!ENTITY fnof     "&#402;"> <!-- latin small letter f with hook = function
+                                    = florin, U+0192 ISOtech -->
+
+<!-- Greek -->
+<!ENTITY Alpha    "&#913;"> <!-- greek capital letter alpha, U+0391 -->
+<!ENTITY Beta     "&#914;"> <!-- greek capital letter beta, U+0392 -->
+<!ENTITY Gamma    "&#915;"> <!-- greek capital letter gamma,
+                                    U+0393 ISOgrk3 -->
+<!ENTITY Delta    "&#916;"> <!-- greek capital letter delta,
+                                    U+0394 ISOgrk3 -->
+<!ENTITY Epsilon  "&#917;"> <!-- greek capital letter epsilon, U+0395 -->
+<!ENTITY Zeta     "&#918;"> <!-- greek capital letter zeta, U+0396 -->
+<!ENTITY Eta      "&#919;"> <!-- greek capital letter eta, U+0397 -->
+<!ENTITY Theta    "&#920;"> <!-- greek capital letter theta,
+                                    U+0398 ISOgrk3 -->
+<!ENTITY Iota     "&#921;"> <!-- greek capital letter iota, U+0399 -->
+<!ENTITY Kappa    "&#922;"> <!-- greek capital letter kappa, U+039A -->
+<!ENTITY Lambda   "&#923;"> <!-- greek capital letter lamda,
+                                    U+039B ISOgrk3 -->
+<!ENTITY Mu       "&#924;"> <!-- greek capital letter mu, U+039C -->
+<!ENTITY Nu       "&#925;"> <!-- greek capital letter nu, U+039D -->
+<!ENTITY Xi       "&#926;"> <!-- greek capital letter xi, U+039E ISOgrk3 -->
+<!ENTITY Omicron  "&#927;"> <!-- greek capital letter omicron, U+039F -->
+<!ENTITY Pi       "&#928;"> <!-- greek capital letter pi, U+03A0 ISOgrk3 -->
+<!ENTITY Rho      "&#929;"> <!-- greek capital letter rho, U+03A1 -->
+<!-- there is no Sigmaf, and no U+03A2 character either -->
+<!ENTITY Sigma    "&#931;"> <!-- greek capital letter sigma,
+                                    U+03A3 ISOgrk3 -->
+<!ENTITY Tau      "&#932;"> <!-- greek capital letter tau, U+03A4 -->
+<!ENTITY Upsilon  "&#933;"> <!-- greek capital letter upsilon,
+                                    U+03A5 ISOgrk3 -->
+<!ENTITY Phi      "&#934;"> <!-- greek capital letter phi,
+                                    U+03A6 ISOgrk3 -->
+<!ENTITY Chi      "&#935;"> <!-- greek capital letter chi, U+03A7 -->
+<!ENTITY Psi      "&#936;"> <!-- greek capital letter psi,
+                                    U+03A8 ISOgrk3 -->
+<!ENTITY Omega    "&#937;"> <!-- greek capital letter omega,
+                                    U+03A9 ISOgrk3 -->
+
+<!ENTITY alpha    "&#945;"> <!-- greek small letter alpha,
+                                    U+03B1 ISOgrk3 -->
+<!ENTITY beta     "&#946;"> <!-- greek small letter beta, U+03B2 ISOgrk3 -->
+<!ENTITY gamma    "&#947;"> <!-- greek small letter gamma,
+                                    U+03B3 ISOgrk3 -->
+<!ENTITY delta    "&#948;"> <!-- greek small letter delta,
+                                    U+03B4 ISOgrk3 -->
+<!ENTITY epsilon  "&#949;"> <!-- greek small letter epsilon,
+                                    U+03B5 ISOgrk3 -->
+<!ENTITY zeta     "&#950;"> <!-- greek small letter zeta, U+03B6 ISOgrk3 -->
+<!ENTITY eta      "&#951;"> <!-- greek small letter eta, U+03B7 ISOgrk3 -->
+<!ENTITY theta    "&#952;"> <!-- greek small letter theta,
+                                    U+03B8 ISOgrk3 -->
+<!ENTITY iota     "&#953;"> <!-- greek small letter iota, U+03B9 ISOgrk3 -->
+<!ENTITY kappa    "&#954;"> <!-- greek small letter kappa,
+                                    U+03BA ISOgrk3 -->
+<!ENTITY lambda   "&#955;"> <!-- greek small letter lamda,
+                                    U+03BB ISOgrk3 -->
+<!ENTITY mu       "&#956;"> <!-- greek small letter mu, U+03BC ISOgrk3 -->
+<!ENTITY nu       "&#957;"> <!-- greek small letter nu, U+03BD ISOgrk3 -->
+<!ENTITY xi       "&#958;"> <!-- greek small letter xi, U+03BE ISOgrk3 -->
+<!ENTITY omicron  "&#959;"> <!-- greek small letter omicron, U+03BF NEW -->
+<!ENTITY pi       "&#960;"> <!-- greek small letter pi, U+03C0 ISOgrk3 -->
+<!ENTITY rho      "&#961;"> <!-- greek small letter rho, U+03C1 ISOgrk3 -->
+<!ENTITY sigmaf   "&#962;"> <!-- greek small letter final sigma,
+                                    U+03C2 ISOgrk3 -->
+<!ENTITY sigma    "&#963;"> <!-- greek small letter sigma,
+                                    U+03C3 ISOgrk3 -->
+<!ENTITY tau      "&#964;"> <!-- greek small letter tau, U+03C4 ISOgrk3 -->
+<!ENTITY upsilon  "&#965;"> <!-- greek small letter upsilon,
+                                    U+03C5 ISOgrk3 -->
+<!ENTITY phi      "&#966;"> <!-- greek small letter phi, U+03C6 ISOgrk3 -->
+<!ENTITY chi      "&#967;"> <!-- greek small letter chi, U+03C7 ISOgrk3 -->
+<!ENTITY psi      "&#968;"> <!-- greek small letter psi, U+03C8 ISOgrk3 -->
+<!ENTITY omega    "&#969;"> <!-- greek small letter omega,
+                                    U+03C9 ISOgrk3 -->
+<!ENTITY thetasym "&#977;"> <!-- greek theta symbol,
+                                    U+03D1 NEW -->
+<!ENTITY upsih    "&#978;"> <!-- greek upsilon with hook symbol,
+                                    U+03D2 NEW -->
+<!ENTITY piv      "&#982;"> <!-- greek pi symbol, U+03D6 ISOgrk3 -->
+
+<!-- General Punctuation -->
+<!ENTITY bull     "&#8226;"> <!-- bullet = black small circle,
+                                     U+2022 ISOpub  -->
+<!-- bullet is NOT the same as bullet operator, U+2219 -->
+<!ENTITY hellip   "&#8230;"> <!-- horizontal ellipsis = three dot leader,
+                                     U+2026 ISOpub  -->
+<!ENTITY prime    "&#8242;"> <!-- prime = minutes = feet, U+2032 ISOtech -->
+<!ENTITY Prime    "&#8243;"> <!-- double prime = seconds = inches,
+                                     U+2033 ISOtech -->
+<!ENTITY oline    "&#8254;"> <!-- overline = spacing overscore,
+                                     U+203E NEW -->
+<!ENTITY frasl    "&#8260;"> <!-- fraction slash, U+2044 NEW -->
+
+<!-- Letterlike Symbols -->
+<!ENTITY weierp   "&#8472;"> <!-- script capital P = power set
+                                     = Weierstrass p, U+2118 ISOamso -->
+<!ENTITY image    "&#8465;"> <!-- black-letter capital I = imaginary part,
+                                     U+2111 ISOamso -->
+<!ENTITY real     "&#8476;"> <!-- black-letter capital R = real part symbol,
+                                     U+211C ISOamso -->
+<!ENTITY trade    "&#8482;"> <!-- trade mark sign, U+2122 ISOnum -->
+<!ENTITY alefsym  "&#8501;"> <!-- alef symbol = first transfinite cardinal,
+                                     U+2135 NEW -->
+<!-- alef symbol is NOT the same as hebrew letter alef,
+     U+05D0 although the same glyph could be used to depict both characters -->
+
+<!-- Arrows -->
+<!ENTITY larr     "&#8592;"> <!-- leftwards arrow, U+2190 ISOnum -->
+<!ENTITY uarr     "&#8593;"> <!-- upwards arrow, U+2191 ISOnum-->
+<!ENTITY rarr     "&#8594;"> <!-- rightwards arrow, U+2192 ISOnum -->
+<!ENTITY darr     "&#8595;"> <!-- downwards arrow, U+2193 ISOnum -->
+<!ENTITY harr     "&#8596;"> <!-- left right arrow, U+2194 ISOamsa -->
+<!ENTITY crarr    "&#8629;"> <!-- downwards arrow with corner leftwards
+                                     = carriage return, U+21B5 NEW -->
+<!ENTITY lArr     "&#8656;"> <!-- leftwards double arrow, U+21D0 ISOtech -->
+<!-- Unicode does not say that lArr is the same as the 'is implied by' arrow
+    but also does not have any other character for that function. So lArr can
+    be used for 'is implied by' as ISOtech suggests -->
+<!ENTITY uArr     "&#8657;"> <!-- upwards double arrow, U+21D1 ISOamsa -->
+<!ENTITY rArr     "&#8658;"> <!-- rightwards double arrow,
+                                     U+21D2 ISOtech -->
+<!-- Unicode does not say this is the 'implies' character but does not have 
+     another character with this function so rArr can be used for 'implies'
+     as ISOtech suggests -->
+<!ENTITY dArr     "&#8659;"> <!-- downwards double arrow, U+21D3 ISOamsa -->
+<!ENTITY hArr     "&#8660;"> <!-- left right double arrow,
+                                     U+21D4 ISOamsa -->
+
+<!-- Mathematical Operators -->
+<!ENTITY forall   "&#8704;"> <!-- for all, U+2200 ISOtech -->
+<!ENTITY part     "&#8706;"> <!-- partial differential, U+2202 ISOtech  -->
+<!ENTITY exist    "&#8707;"> <!-- there exists, U+2203 ISOtech -->
+<!ENTITY empty    "&#8709;"> <!-- empty set = null set, U+2205 ISOamso -->
+<!ENTITY nabla    "&#8711;"> <!-- nabla = backward difference,
+                                     U+2207 ISOtech -->
+<!ENTITY isin     "&#8712;"> <!-- element of, U+2208 ISOtech -->
+<!ENTITY notin    "&#8713;"> <!-- not an element of, U+2209 ISOtech -->
+<!ENTITY ni       "&#8715;"> <!-- contains as member, U+220B ISOtech -->
+<!ENTITY prod     "&#8719;"> <!-- n-ary product = product sign,
+                                     U+220F ISOamsb -->
+<!-- prod is NOT the same character as U+03A0 'greek capital letter pi' though
+     the same glyph might be used for both -->
+<!ENTITY sum      "&#8721;"> <!-- n-ary summation, U+2211 ISOamsb -->
+<!-- sum is NOT the same character as U+03A3 'greek capital letter sigma'
+     though the same glyph might be used for both -->
+<!ENTITY minus    "&#8722;"> <!-- minus sign, U+2212 ISOtech -->
+<!ENTITY lowast   "&#8727;"> <!-- asterisk operator, U+2217 ISOtech -->
+<!ENTITY radic    "&#8730;"> <!-- square root = radical sign,
+                                     U+221A ISOtech -->
+<!ENTITY prop     "&#8733;"> <!-- proportional to, U+221D ISOtech -->
+<!ENTITY infin    "&#8734;"> <!-- infinity, U+221E ISOtech -->
+<!ENTITY ang      "&#8736;"> <!-- angle, U+2220 ISOamso -->
+<!ENTITY and      "&#8743;"> <!-- logical and = wedge, U+2227 ISOtech -->
+<!ENTITY or       "&#8744;"> <!-- logical or = vee, U+2228 ISOtech -->
+<!ENTITY cap      "&#8745;"> <!-- intersection = cap, U+2229 ISOtech -->
+<!ENTITY cup      "&#8746;"> <!-- union = cup, U+222A ISOtech -->
+<!ENTITY int      "&#8747;"> <!-- integral, U+222B ISOtech -->
+<!ENTITY there4   "&#8756;"> <!-- therefore, U+2234 ISOtech -->
+<!ENTITY sim      "&#8764;"> <!-- tilde operator = varies with = similar to,
+                                     U+223C ISOtech -->
+<!-- tilde operator is NOT the same character as the tilde, U+007E,
+     although the same glyph might be used to represent both  -->
+<!ENTITY cong     "&#8773;"> <!-- approximately equal to, U+2245 ISOtech -->
+<!ENTITY asymp    "&#8776;"> <!-- almost equal to = asymptotic to,
+                                     U+2248 ISOamsr -->
+<!ENTITY ne       "&#8800;"> <!-- not equal to, U+2260 ISOtech -->
+<!ENTITY equiv    "&#8801;"> <!-- identical to, U+2261 ISOtech -->
+<!ENTITY le       "&#8804;"> <!-- less-than or equal to, U+2264 ISOtech -->
+<!ENTITY ge       "&#8805;"> <!-- greater-than or equal to,
+                                     U+2265 ISOtech -->
+<!ENTITY sub      "&#8834;"> <!-- subset of, U+2282 ISOtech -->
+<!ENTITY sup      "&#8835;"> <!-- superset of, U+2283 ISOtech -->
+<!ENTITY nsub     "&#8836;"> <!-- not a subset of, U+2284 ISOamsn -->
+<!ENTITY sube     "&#8838;"> <!-- subset of or equal to, U+2286 ISOtech -->
+<!ENTITY supe     "&#8839;"> <!-- superset of or equal to,
+                                     U+2287 ISOtech -->
+<!ENTITY oplus    "&#8853;"> <!-- circled plus = direct sum,
+                                     U+2295 ISOamsb -->
+<!ENTITY otimes   "&#8855;"> <!-- circled times = vector product,
+                                     U+2297 ISOamsb -->
+<!ENTITY perp     "&#8869;"> <!-- up tack = orthogonal to = perpendicular,
+                                     U+22A5 ISOtech -->
+<!ENTITY sdot     "&#8901;"> <!-- dot operator, U+22C5 ISOamsb -->
+<!-- dot operator is NOT the same character as U+00B7 middle dot -->
+
+<!-- Miscellaneous Technical -->
+<!ENTITY lceil    "&#8968;"> <!-- left ceiling = APL upstile,
+                                     U+2308 ISOamsc  -->
+<!ENTITY rceil    "&#8969;"> <!-- right ceiling, U+2309 ISOamsc  -->
+<!ENTITY lfloor   "&#8970;"> <!-- left floor = APL downstile,
+                                     U+230A ISOamsc  -->
+<!ENTITY rfloor   "&#8971;"> <!-- right floor, U+230B ISOamsc  -->
+<!ENTITY lang     "&#9001;"> <!-- left-pointing angle bracket = bra,
+                                     U+2329 ISOtech -->
+<!-- lang is NOT the same character as U+003C 'less than sign' 
+     or U+2039 'single left-pointing angle quotation mark' -->
+<!ENTITY rang     "&#9002;"> <!-- right-pointing angle bracket = ket,
+                                     U+232A ISOtech -->
+<!-- rang is NOT the same character as U+003E 'greater than sign' 
+     or U+203A 'single right-pointing angle quotation mark' -->
+
+<!-- Geometric Shapes -->
+<!ENTITY loz      "&#9674;"> <!-- lozenge, U+25CA ISOpub -->
+
+<!-- Miscellaneous Symbols -->
+<!ENTITY spades   "&#9824;"> <!-- black spade suit, U+2660 ISOpub -->
+<!-- black here seems to mean filled as opposed to hollow -->
+<!ENTITY clubs    "&#9827;"> <!-- black club suit = shamrock,
+                                     U+2663 ISOpub -->
+<!ENTITY hearts   "&#9829;"> <!-- black heart suit = valentine,
+                                     U+2665 ISOpub -->
+<!ENTITY diams    "&#9830;"> <!-- black diamond suit, U+2666 ISOpub -->
+
+<!-- Special characters for XHTML -->
+
+<!-- Character entity set. Typical invocation:
+     <!ENTITY % HTMLspecial PUBLIC
+        "-//W3C//ENTITIES Special for XHTML//EN"
+        "http://www.w3.org/TR/xhtml1/DTD/xhtml-special.ent">
+     %HTMLspecial;
+-->
+
+<!-- Portions (C) International Organization for Standardization 1986:
+     Permission to copy in any form is granted for use with
+     conforming SGML systems and applications as defined in
+     ISO 8879, provided this notice is included in all copies.
+-->
+
+<!-- Relevant ISO entity set is given unless names are newly introduced.
+     New names (i.e., not in ISO 8879 list) do not clash with any
+     existing ISO 8879 entity names. ISO 10646 character numbers
+     are given for each character, in hex. values are decimal
+     conversions of the ISO 10646 values and refer to the document
+     character set. Names are Unicode names. 
+-->
+
+<!-- C0 Controls and Basic Latin -->
+<!ENTITY quot    "&#34;"> <!--  quotation mark, U+0022 ISOnum -->
+<!ENTITY amp     "&#38;#38;"> <!--  ampersand, U+0026 ISOnum -->
+<!ENTITY lt      "&#38;#60;"> <!--  less-than sign, U+003C ISOnum -->
+<!ENTITY gt      "&#62;"> <!--  greater-than sign, U+003E ISOnum -->
+<!ENTITY apos	 "&#39;"> <!--  apostrophe = APL quote, U+0027 ISOnum -->
+
+<!-- Latin Extended-A -->
+<!ENTITY OElig   "&#338;"> <!--  latin capital ligature OE,
+                                    U+0152 ISOlat2 -->
+<!ENTITY oelig   "&#339;"> <!--  latin small ligature oe, U+0153 ISOlat2 -->
+<!-- ligature is a misnomer, this is a separate character in some languages -->
+<!ENTITY Scaron  "&#352;"> <!--  latin capital letter S with caron,
+                                    U+0160 ISOlat2 -->
+<!ENTITY scaron  "&#353;"> <!--  latin small letter s with caron,
+                                    U+0161 ISOlat2 -->
+<!ENTITY Yuml    "&#376;"> <!--  latin capital letter Y with diaeresis,
+                                    U+0178 ISOlat2 -->
+
+<!-- Spacing Modifier Letters -->
+<!ENTITY circ    "&#710;"> <!--  modifier letter circumflex accent,
+                                    U+02C6 ISOpub -->
+<!ENTITY tilde   "&#732;"> <!--  small tilde, U+02DC ISOdia -->
+
+<!-- General Punctuation -->
+<!ENTITY ensp    "&#8194;"> <!-- en space, U+2002 ISOpub -->
+<!ENTITY emsp    "&#8195;"> <!-- em space, U+2003 ISOpub -->
+<!ENTITY thinsp  "&#8201;"> <!-- thin space, U+2009 ISOpub -->
+<!ENTITY zwnj    "&#8204;"> <!-- zero width non-joiner,
+                                    U+200C NEW RFC 2070 -->
+<!ENTITY zwj     "&#8205;"> <!-- zero width joiner, U+200D NEW RFC 2070 -->
+<!ENTITY lrm     "&#8206;"> <!-- left-to-right mark, U+200E NEW RFC 2070 -->
+<!ENTITY rlm     "&#8207;"> <!-- right-to-left mark, U+200F NEW RFC 2070 -->
+<!ENTITY ndash   "&#8211;"> <!-- en dash, U+2013 ISOpub -->
+<!ENTITY mdash   "&#8212;"> <!-- em dash, U+2014 ISOpub -->
+<!ENTITY lsquo   "&#8216;"> <!-- left single quotation mark,
+                                    U+2018 ISOnum -->
+<!ENTITY rsquo   "&#8217;"> <!-- right single quotation mark,
+                                    U+2019 ISOnum -->
+<!ENTITY sbquo   "&#8218;"> <!-- single low-9 quotation mark, U+201A NEW -->
+<!ENTITY ldquo   "&#8220;"> <!-- left double quotation mark,
+                                    U+201C ISOnum -->
+<!ENTITY rdquo   "&#8221;"> <!-- right double quotation mark,
+                                    U+201D ISOnum -->
+<!ENTITY bdquo   "&#8222;"> <!-- double low-9 quotation mark, U+201E NEW -->
+<!ENTITY dagger  "&#8224;"> <!-- dagger, U+2020 ISOpub -->
+<!ENTITY Dagger  "&#8225;"> <!-- double dagger, U+2021 ISOpub -->
+<!ENTITY permil  "&#8240;"> <!-- per mille sign, U+2030 ISOtech -->
+<!ENTITY lsaquo  "&#8249;"> <!-- single left-pointing angle quotation mark,
+                                    U+2039 ISO proposed -->
+<!-- lsaquo is proposed but not yet ISO standardized -->
+<!ENTITY rsaquo  "&#8250;"> <!-- single right-pointing angle quotation mark,
+                                    U+203A ISO proposed -->
+<!-- rsaquo is proposed but not yet ISO standardized -->
+
+<!-- Currency Symbols -->
+<!ENTITY euro   "&#8364;"> <!--  euro sign, U+20AC NEW -->
+
+<!-- End embedded .ent file contents -->
```

### Comparing `markdown-to-confluence-0.1.7/setup.cfg` & `markdown-to-confluence-0.1.8/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,70 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206d 6172 6b64 6f77 6e2d 746f 2d63   = markdown-to-c
-00000020: 6f6e 666c 7565 6e63 650d 0a76 6572 7369  onfluence..versi
-00000030: 6f6e 203d 2061 7474 723a 206d 6432 636f  on = attr: md2co
-00000040: 6e66 2e5f 5f76 6572 7369 6f6e 5f5f 0d0a  nf.__version__..
-00000050: 6465 7363 7269 7074 696f 6e20 3d20 5075  description = Pu
-00000060: 626c 6973 6820 4d61 726b 646f 776e 2066  blish Markdown f
-00000070: 696c 6573 2074 6f20 436f 6e66 6c75 656e  iles to Confluen
-00000080: 6365 2077 696b 690d 0a61 7574 686f 7220  ce wiki..author 
-00000090: 3d20 4c65 7665 6e74 6520 4875 6e79 6164  = Levente Hunyad
-000000a0: 690d 0a61 7574 686f 725f 656d 6169 6c20  i..author_email 
-000000b0: 3d20 6875 6e79 6164 6940 676d 6169 6c2e  = hunyadi@gmail.
-000000c0: 636f 6d0d 0a75 726c 203d 2068 7474 7073  com..url = https
-000000d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6875  ://github.com/hu
-000000e0: 6e79 6164 692f 6d64 3263 6f6e 660d 0a6c  nyadi/md2conf..l
-000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000100: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000110: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000120: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000130: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000140: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
-00000150: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000160: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
-00000170: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
-00000180: 7563 7469 6f6e 2f53 7461 626c 650d 0a09  uction/Stable...
-00000190: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
-000001a0: 6f6e 736f 6c65 0d0a 0949 6e74 656e 6465  onsole...Intende
-000001b0: 6420 4175 6469 656e 6365 203a 3a20 456e  d Audience :: En
-000001c0: 6420 5573 6572 732f 4465 736b 746f 700d  d Users/Desktop.
-000001d0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001e0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001f0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000210: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000230: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000240: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
-00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000260: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
-00000270: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000280: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000290: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002b0: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
-000002c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002e0: 2033 2e31 310d 0a09 5479 7069 6e67 203a   3.11...Typing :
-000002f0: 3a20 5479 7065 640d 0a0d 0a5b 6f70 7469  : Typed....[opti
-00000300: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
-00000310: 2054 7275 650d 0a69 6e63 6c75 6465 5f70   True..include_p
-00000320: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-00000330: 7565 0d0a 7061 636b 6167 6573 203d 2066  ue..packages = f
-00000340: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000350: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
-00000360: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000370: 3d20 0d0a 096c 786d 6c20 3e3d 2034 2e39  = ...lxml >= 4.9
-00000380: 0d0a 096d 6172 6b64 6f77 6e20 3e3d 2033  ...markdown >= 3
-00000390: 2e34 0d0a 0970 796d 646f 776e 2d65 7874  .4...pymdown-ext
-000003a0: 656e 7369 6f6e 7320 3e3d 2039 2e31 310d  ensions >= 9.11.
-000003b0: 0a09 7265 7175 6573 7473 203e 3d20 322e  ..requests >= 2.
-000003c0: 3238 0d0a 0974 7970 6573 2d6d 6172 6b64  28...types-markd
-000003d0: 6f77 6e20 3e3d 2033 2e34 0d0a 0974 7970  own >= 3.4...typ
-000003e0: 6573 2d72 6571 7565 7374 7320 3e3d 2032  es-requests >= 2
-000003f0: 2e32 380d 0a0d 0a5b 6f70 7469 6f6e 732e  .28....[options.
-00000400: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000410: 6578 636c 7564 6520 3d20 0d0a 0974 6573  exclude = ...tes
-00000420: 7473 2a0d 0a0d 0a5b 6f70 7469 6f6e 732e  ts*....[options.
-00000430: 7061 636b 6167 655f 6461 7461 5d0d 0a6d  package_data]..m
-00000440: 6432 636f 6e66 203d 200d 0a09 656e 7469  d2conf = ...enti
-00000450: 7469 6573 2e64 7464 0d0a 0970 792e 7479  ties.dtd...py.ty
-00000460: 7065 640d 0a0d 0a5b 6567 675f 696e 666f  ped....[egg_info
-00000470: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000480: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000490: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6d61 726b 646f 776e 2d74 6f2d 636f  = markdown-to-co
+00000020: 6e66 6c75 656e 6365 0a76 6572 7369 6f6e  nfluence.version
+00000030: 203d 2061 7474 723a 206d 6432 636f 6e66   = attr: md2conf
+00000040: 2e5f 5f76 6572 7369 6f6e 5f5f 0a64 6573  .__version__.des
+00000050: 6372 6970 7469 6f6e 203d 2050 7562 6c69  cription = Publi
+00000060: 7368 204d 6172 6b64 6f77 6e20 6669 6c65  sh Markdown file
+00000070: 7320 746f 2043 6f6e 666c 7565 6e63 6520  s to Confluence 
+00000080: 7769 6b69 0a61 7574 686f 7220 3d20 4c65  wiki.author = Le
+00000090: 7665 6e74 6520 4875 6e79 6164 690a 6175  vente Hunyadi.au
+000000a0: 7468 6f72 5f65 6d61 696c 203d 2068 756e  thor_email = hun
+000000b0: 7961 6469 4067 6d61 696c 2e63 6f6d 0a75  yadi@gmail.com.u
+000000c0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+000000d0: 6875 622e 636f 6d2f 6875 6e79 6164 692f  hub.com/hunyadi/
+000000e0: 6d64 3263 6f6e 660a 6c6f 6e67 5f64 6573  md2conf.long_des
+000000f0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+00000100: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
+00000110: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000120: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+00000130: 6d61 726b 646f 776e 0a6c 6963 656e 7365  markdown.license
+00000140: 203d 204d 4954 0a63 6c61 7373 6966 6965   = MIT.classifie
+00000150: 7273 203d 200a 0944 6576 656c 6f70 6d65  rs = ..Developme
+00000160: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00000170: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00000180: 6c65 0a09 456e 7669 726f 6e6d 656e 7420  le..Environment 
+00000190: 3a3a 2043 6f6e 736f 6c65 0a09 496e 7465  :: Console..Inte
+000001a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000001b0: 2045 6e64 2055 7365 7273 2f44 6573 6b74   End Users/Deskt
+000001c0: 6f70 0a09 4c69 6365 6e73 6520 3a3a 204f  op..License :: O
+000001d0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+000001e0: 4954 204c 6963 656e 7365 0a09 4f70 6572  IT License..Oper
+000001f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000200: 4f53 2049 6e64 6570 656e 6465 6e74 0a09  OS Independent..
+00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000230: 3a20 330a 0950 726f 6772 616d 6d69 6e67  : 3..Programming
+00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000250: 686f 6e20 3a3a 2033 2e38 0a09 5072 6f67  hon :: 3.8..Prog
+00000260: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000270: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000280: 390a 0950 726f 6772 616d 6d69 6e67 204c  9..Programming L
+00000290: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002a0: 6e20 3a3a 2033 2e31 300a 0950 726f 6772  n :: 3.10..Progr
+000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000002d0: 310a 0954 7970 696e 6720 3a3a 2054 7970  1..Typing :: Typ
+000002e0: 6564 0a0a 5b6f 7074 696f 6e73 5d0a 7a69  ed..[options].zi
+000002f0: 705f 7361 6665 203d 2054 7275 650a 696e  p_safe = True.in
+00000300: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000310: 7461 203d 2054 7275 650a 7061 636b 6167  ta = True.packag
+00000320: 6573 203d 2066 696e 643a 0a70 7974 686f  es = find:.pytho
+00000330: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000340: 2e38 0a69 6e73 7461 6c6c 5f72 6571 7569  .8.install_requi
+00000350: 7265 7320 3d20 0a09 6c78 6d6c 203e 3d20  res = ..lxml >= 
+00000360: 342e 390a 096d 6172 6b64 6f77 6e20 3e3d  4.9..markdown >=
+00000370: 2033 2e34 0a09 7079 6d64 6f77 6e2d 6578   3.4..pymdown-ex
+00000380: 7465 6e73 696f 6e73 203e 3d20 392e 3131  tensions >= 9.11
+00000390: 0a09 7265 7175 6573 7473 203e 3d20 322e  ..requests >= 2.
+000003a0: 3238 0a09 7479 7065 732d 6d61 726b 646f  28..types-markdo
+000003b0: 776e 203e 3d20 332e 340a 0974 7970 6573  wn >= 3.4..types
+000003c0: 2d72 6571 7565 7374 7320 3e3d 2032 2e32  -requests >= 2.2
+000003d0: 380a 0a5b 6f70 7469 6f6e 732e 7061 636b  8..[options.pack
+000003e0: 6167 6573 2e66 696e 645d 0a65 7863 6c75  ages.find].exclu
+000003f0: 6465 203d 200a 0974 6573 7473 2a0a 0a5b  de = ..tests*..[
+00000400: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000410: 6461 7461 5d0a 6d64 3263 6f6e 6620 3d20  data].md2conf = 
+00000420: 0a09 656e 7469 7469 6573 2e64 7464 0a09  ..entities.dtd..
+00000430: 7079 2e74 7970 6564 0a0a 5b65 6767 5f69  py.typed..[egg_i
+00000440: 6e66 6f5d 0a74 6167 5f62 7569 6c64 203d  nfo].tag_build =
+00000450: 200a 7461 675f 6461 7465 203d 2030 0a0a   .tag_date = 0..
```

