# Comparing `tmp/bamboo-crawler-0.1.4.tar.gz` & `tmp/bamboo-crawler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamboo-crawler-0.1.4.tar", last modified: Mon Jan  9 14:33:15 2023, max compression
+gzip compressed data, was "bamboo-crawler-0.1.5.tar", last modified: Thu Jul 20 14:40:48 2023, max compression
```

## Comparing `bamboo-crawler-0.1.4.tar` & `bamboo-crawler-0.1.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.742895 bamboo-crawler-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.750896 bamboo-crawler-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   104952 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.754896 bamboo-crawler-0.1.4/bamboo_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.754896 bamboo-crawler-0.1.4/bamboo_crawler/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/crawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/directives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/directives/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/directives/searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/file/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/gzip/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/gzip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/inputter.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/outputter.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/interfaces/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/json/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/sqs_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/sqs_s3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/bamboo_crawler/stdio/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/stdio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/bamboo_crawler/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.754896 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-09 14:33:15.000000 bamboo-crawler-0.1.4/bamboo_crawler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/example/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/aws/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/aws/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/aws/test_aws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/tests/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/constants/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/constants/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/tests/crawling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/crawling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.758896 bamboo-crawler-0.1.4/tests/crawling/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/crawling/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/crawling/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/crawling/test_crawling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/tests/scraping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/scraping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/tests/scraping/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/scraping/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/scraping/assets/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/scraping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/scraping/test_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:33:15.762896 bamboo-crawler-0.1.4/tests/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/sql/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-01-09 14:32:20.000000 bamboo-crawler-0.1.4/tests/sql/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.587859 bamboo-crawler-0.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.587859 bamboo-crawler-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/crawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/directives/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/directives/searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler/gzip/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/gzip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/inputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/outputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/interfaces/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/sqs_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/sqs_s3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/bamboo_crawler/stdio/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/stdio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/bamboo_crawler/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.591859 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 14:40:48.000000 bamboo-crawler-0.1.5/bamboo_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/cached_property.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/example/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   228640 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/aws/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/aws/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/aws/test_aws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.595859 bamboo-crawler-0.1.5/tests/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/constants/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/constants/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/tests/crawling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/crawling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/tests/crawling/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/crawling/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/crawling/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/crawling/test_crawling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/tests/scraping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/scraping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/tests/scraping/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/scraping/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/scraping/assets/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/scraping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/scraping/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:48.599859 bamboo-crawler-0.1.5/tests/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/sql/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-20 14:40:18.000000 bamboo-crawler-0.1.5/tests/sql/test_sql.py
```

### Comparing `bamboo-crawler-0.1.4/.gitignore` & `bamboo-crawler-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/LICENSE` & `bamboo-crawler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/PKG-INFO` & `bamboo-crawler-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-crawler
-Version: 0.1.4
+Version: 0.1.5
 Summary: a hobby crawler
 Home-page: https://github.com/kitsuyui/bamboo-crawler
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -18,17 +18,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Bamboo Crawler
 
+[![Python](https://img.shields.io/pypi/pyversions/bamboo-crawler.svg)](https://badge.fury.io/py/tbamboo-crawler)
+[![PyPI version](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 [![codecov](https://codecov.io/gh/kitsuyui/bamboo-crawler/branch/main/graph/badge.svg?token=s7NTzwl5fl)](https://codecov.io/gh/kitsuyui/bamboo-crawler)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![PyPI version shields.io](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 
 A Hobby Crawler.
 It is almost under construction.
 
 # Usage
 
 ## Installation
```

### Comparing `bamboo-crawler-0.1.4/README.md` & `bamboo-crawler-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Bamboo Crawler
 
+[![Python](https://img.shields.io/pypi/pyversions/bamboo-crawler.svg)](https://badge.fury.io/py/tbamboo-crawler)
+[![PyPI version](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 [![codecov](https://codecov.io/gh/kitsuyui/bamboo-crawler/branch/main/graph/badge.svg?token=s7NTzwl5fl)](https://codecov.io/gh/kitsuyui/bamboo-crawler)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![PyPI version shields.io](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 
 A Hobby Crawler.
 It is almost under construction.
 
 # Usage
 
 ## Installation
```

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/cli.py` & `bamboo-crawler-0.1.5/bamboo_crawler/cli.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/constants/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/crawler/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/directives/default.py` & `bamboo-crawler-0.1.5/bamboo_crawler/directives/default.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/directives/searcher.py` & `bamboo-crawler-0.1.5/bamboo_crawler/directives/searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, TypeVar
+from typing import Any, Type, TypeVar
 
 from ..constants import NullDeserializer, NullSerializer
 from ..interfaces.deserializer import Deserializer
 from ..interfaces.inputter import Inputter
 from ..interfaces.outputter import Outputter
 from ..interfaces.processor import Processor
 from ..interfaces.serializer import Serializer
 from ..task import Task
 
-InputterType = TypeVar("InputterType", bound=type[Inputter])
+InputterType = TypeVar("InputterType", bound=Type[Inputter])
 
 
 @dataclass
 class DirectiveSearcher:
-    deserializers: dict[str, type[Deserializer]]
-    inputters: dict[str, type[Inputter]]
-    outputters: dict[str, type[Outputter]]
-    processors: dict[str, type[Processor]]
-    serializers: dict[str, type[Serializer]]
+    deserializers: dict[str, Type[Deserializer]]
+    inputters: dict[str, Type[Inputter]]
+    outputters: dict[str, Type[Outputter]]
+    processors: dict[str, Type[Processor]]
+    serializers: dict[str, Type[Serializer]]
 
     @classmethod
     def create(cls) -> DirectiveSearcher:
         return cls({}, {}, {}, {}, {})
 
     def add_inputter(self, inputter: InputterType) -> None:
         self.inputters[inputter.__name__] = inputter
 
-    def add_outputter(self, outputter: type[Outputter]) -> None:
+    def add_outputter(self, outputter: Type[Outputter]) -> None:
         self.outputters[outputter.__name__] = outputter
 
-    def add_deserializer(self, deserializer: type[Deserializer]) -> None:
+    def add_deserializer(self, deserializer: Type[Deserializer]) -> None:
         self.deserializers[deserializer.__name__] = deserializer
 
-    def add_processor(self, processor: type[Processor]) -> None:
+    def add_processor(self, processor: Type[Processor]) -> None:
         self.processors[processor.__name__] = processor
 
-    def add_serializer(self, serializer: type[Serializer]) -> None:
+    def add_serializer(self, serializer: Type[Serializer]) -> None:
         self.serializers[serializer.__name__] = serializer
 
     def get_inputter(self, directive: TypeDirective) -> Inputter:
         return self.inputters[directive.type](**directive.options)
 
     def get_outputter(self, directive: TypeDirective) -> Outputter:
         return self.outputters[directive.type](**directive.options)
```

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/job.py` & `bamboo-crawler-0.1.5/bamboo_crawler/job.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/parser.py` & `bamboo-crawler-0.1.5/bamboo_crawler/parser.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/python/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/python/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/scraper/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/scraper/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
+from __future__ import annotations
+
 import abc
-import functools
+import sys
+
+if sys.version_info < (3, 8):
+    from cached_property import cached_property
+else:
+    from functools import cached_property
+
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import lxml.html
 
 from ..interfaces.context import Context
@@ -71,24 +79,24 @@
         return [e.attrib[attribute] for e in elements.cssselect(selector)]
 
 
 @dataclass
 class MixedHTMLScraper(Scraper):
     targets: Dict[str, Dict[str, str]] = field(default_factory=dict)
 
-    @functools.cached_property
+    @cached_property
     def xpath_scraper(self) -> XPathScraper:
         xpaths = {
             key: target["xpath"]
             for key, target in self.targets.items()
             if "xpath" in target
         }
         return XPathScraper(xpaths=xpaths)
 
-    @functools.cached_property
+    @cached_property
     def cssselector_scraper(self) -> CSSSelectorScraper:
         css = {
             key: target["css"]
             for key, target in self.targets.items()
             if "css" in target
         }
         return CSSSelectorScraper(selectors=css)
```

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/sqs_s3/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/sqs_s3/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-import functools
+from __future__ import annotations
+
+import sys
+
+if sys.version_info < (3, 8):
+    from cached_property import cached_property
+else:
+    from functools import cached_property
+
 import hashlib
 import json
 import sys
 import time
 from dataclasses import dataclass, field
 from typing import Any, Dict, Optional, Tuple, Union
 
@@ -21,21 +29,21 @@
 class SQSS3Inputter(Inputter[bytes]):
     bucket_name: str
     queue_name: str
     s3_config: Dict[str, Any] = field(default_factory=dict)
     sqs_config: Dict[str, Any] = field(default_factory=dict)
     message: Optional[SQSMessage] = None
 
-    @functools.cached_property
+    @cached_property
     def queue(self) -> SQSQueue:
         sqs = boto3.resource("sqs", **self.sqs_config)
         queue = sqs.get_queue_by_name(QueueName=self.queue_name)
         return queue
 
-    @functools.cached_property
+    @cached_property
     def bucket(self) -> S3Bucket:
         s3 = boto3.resource("s3", **self.s3_config)
         return s3.Bucket(self.bucket_name)
 
     def read(self) -> Context[bytes]:
         message = self.__read_sqs()
         body, meta = self.__read_s3(message)
```

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/stdio/__init__.py` & `bamboo-crawler-0.1.5/bamboo_crawler/stdio/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler/task.py` & `bamboo-crawler-0.1.5/bamboo_crawler/task.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler.egg-info/PKG-INFO` & `bamboo-crawler-0.1.5/bamboo_crawler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-crawler
-Version: 0.1.4
+Version: 0.1.5
 Summary: a hobby crawler
 Home-page: https://github.com/kitsuyui/bamboo-crawler
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -18,17 +18,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Bamboo Crawler
 
+[![Python](https://img.shields.io/pypi/pyversions/bamboo-crawler.svg)](https://badge.fury.io/py/tbamboo-crawler)
+[![PyPI version](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 [![codecov](https://codecov.io/gh/kitsuyui/bamboo-crawler/branch/main/graph/badge.svg?token=s7NTzwl5fl)](https://codecov.io/gh/kitsuyui/bamboo-crawler)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![PyPI version shields.io](https://img.shields.io/pypi/v/bamboo-crawler.svg)](https://pypi.python.org/pypi/bamboo-crawler/)
 
 A Hobby Crawler.
 It is almost under construction.
 
 # Usage
 
 ## Installation
```

### Comparing `bamboo-crawler-0.1.4/bamboo_crawler.egg-info/SOURCES.txt` & `bamboo-crawler-0.1.5/bamboo_crawler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .gitignore
 .gitignore.in
 LICENSE
 MANIFEST.in
-Makefile
-Pipfile
-Pipfile.lock
 README.md
+cached_property.pyi
 mypy.ini
+poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
+.github/renovate.json5
 .github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 bamboo_crawler/__init__.py
 bamboo_crawler/__main__.py
 bamboo_crawler/_version.py
 bamboo_crawler/cli.py
 bamboo_crawler/job.py
 bamboo_crawler/parser.py
 bamboo_crawler/task.py
```

### Comparing `bamboo-crawler-0.1.4/mypy.ini` & `bamboo-crawler-0.1.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/setup.cfg` & `bamboo-crawler-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/aws/recipe.yml` & `bamboo-crawler-0.1.5/tests/aws/recipe.yml`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/aws/test_aws.py` & `bamboo-crawler-0.1.5/tests/aws/test_aws.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/crawling/test_crawling.py` & `bamboo-crawler-0.1.5/tests/crawling/test_crawling.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/scraping/recipe.yml` & `bamboo-crawler-0.1.5/tests/scraping/recipe.yml`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/scraping/test_scraper.py` & `bamboo-crawler-0.1.5/tests/scraping/test_scraper.py`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/sql/recipe.yml` & `bamboo-crawler-0.1.5/tests/sql/recipe.yml`

 * *Files identical despite different names*

### Comparing `bamboo-crawler-0.1.4/tests/sql/test_sql.py` & `bamboo-crawler-0.1.5/tests/sql/test_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import json
 import os
 import sqlite3
 import subprocess
+import threading
 from typing import Any
 
 import pytest
 
 Database = Any
 
 
+lock = threading.Lock()
 @pytest.fixture
 def database() -> None:  # type: ignore
+    lock.acquire()
     db_filepath = "/tmp/test1"
     with open(db_filepath, "w"):
         pass
     db = sqlite3.connect(db_filepath)
     c = db.cursor()
     c.execute("CREATE TABLE test_table1 (col1 text, col2 int);")
     c.execute("INSERT INTO test_table1 (col1, col2) VALUES ('test', 1);")
     c.execute("INSERT INTO test_table1 (col1, col2) VALUES ('test', 2);")
     c.execute("INSERT INTO test_table1 (col1, col2) VALUES ('test', 3);")
     db.commit()
     yield db
     db.close()
     os.unlink(db_filepath)
+    lock.release()
 
 
 def run_recipe(taskname: str):  # type: ignore
     c = subprocess.run(
         [
             "python",
             "-m",
```

