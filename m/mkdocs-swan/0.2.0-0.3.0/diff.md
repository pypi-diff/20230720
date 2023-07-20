# Comparing `tmp/mkdocs-swan-0.2.0.tar.gz` & `tmp/mkdocs-swan-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-swan-0.2.0.tar", last modified: Fri Mar 17 12:59:05 2023, max compression
+gzip compressed data, was "mkdocs-swan-0.3.0.tar", last modified: Thu Jul 20 13:25:21 2023, max compression
```

## Comparing `mkdocs-swan-0.2.0.tar` & `mkdocs-swan-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/mkdocs_swan/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/mkdocs_swan/css/
--rw-r--r--   0 runner    (1001) docker     (123)   308718 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/css/notebook.css
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/full_width.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/full_width_with_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/mkdocs_swan/images/
--rw-r--r--   0 runner    (1001) docker     (123)    72566 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/images/logo_cern.png
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/mkdocs_theme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/notebook.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/mkdocs_swan/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/mkdocs_swan/partials/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 12:59:05.000000 mkdocs-swan-0.2.0/mkdocs_swan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 12:59:05.665232 mkdocs-swan-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-17 12:59:02.000000 mkdocs-swan-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.222460 mkdocs-swan-0.3.0/mkdocs_swan/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.226460 mkdocs-swan-0.3.0/mkdocs_swan/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24072 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21043 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)   308718 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/mkdocs_swan/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    72566 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/images/logo_cern.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/mkdocs_theme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/notebook.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/mkdocs_swan/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/mkdocs_swan/partials/copyright.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:25:21.222460 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 13:25:21.000000 mkdocs-swan-0.3.0/mkdocs_swan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:25:21.230461 mkdocs-swan-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 13:25:18.000000 mkdocs-swan-0.3.0/setup.py
```

### Comparing `mkdocs-swan-0.2.0/LICENSE` & `mkdocs-swan-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-swan-0.2.0/PKG-INFO` & `mkdocs-swan-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swan
-Version: 0.2.0
+Version: 0.3.0
 Summary: SWAN theme for MkDocs
 Home-page: https://github.com/swan-cern/mkdocs-swan
 Author: Diogo Castro
 Author-email: diogo.castro@cern.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/css/notebook.css` & `mkdocs-swan-0.3.0/mkdocs_swan/css/notebook.css`

 * *Files identical despite different names*

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/css/style.css` & `mkdocs-swan-0.3.0/mkdocs_swan/css/style.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,164 +1,141 @@
-.md-header,
-.md-hero {
-    background-color: #03263C;
+:root {
+    --md-primary-fg-color: #03263C;
+    --md-accent-fg-color: #0053A1;
 }
 
-.md-header[data-md-state=shadow] {
+.md-header--shadow {
     box-shadow: none;
 }
 
-.md-header-nav__title {
+.md-typeset h1,
+.md-typeset h2,
+.md-typeset h3 {
+    color: var(--md-accent-fg-color);
+}
+
+.md-typeset h1 {
+    font-weight: 400;
+}
+
+.md-typeset h2,
+.md-typeset h3 {
+    font-weight: 100;
+}
+
+
+.md-header__title {
+    margin: 0;
+    margin-left: 0 !important;
     padding: 0 0.2rem;
 }
 
+.md-header__topic:first-child {
+    font-weight: unset;
+}
+
 .md-source {
     display: none;
 }
 
 .md-content img {
     display: block;
     margin-left: auto;
     margin-right: auto;
     border: 1px solid #FAFAFA;
 }
 
-.md-header-nav__button.md-logo img,
-.md-header-nav__button.md-logo svg,
+.md-header__button.md-logo img,
+.md-header__button.md-logo svg,
 .md-nav__title .md-nav__button.md-logo img,
 .md-nav__title .md-nav__button.md-logo svg {
     width: unset;
 }
 
 @media only screen and (max-width: 76.1875em) {
     html .md-nav--primary .md-nav__title[for=__drawer] {
         background-color: #03263C;
     }
     .md-nav__source {
         display: none;
     }
 }
 
-.md-typeset h1,
-.md-typeset h2,
-.md-typeset h3 {
-    color: #0053A1;
-}
-
-.md-typeset h1 {
-    font-weight: 400;
-}
-
-.md-typeset h2,
-.md-typeset h3 {
-    font-weight: 100;
-}
-
 .md-nav__title {
     color: #777777;
 }
 
 .md-typeset a,
 .md-typeset a:active,
 .md-typeset a:focus,
 .md-nav__item .md-nav__link--active {
-    color: #0053A1;
+    color: var(--md-accent-fg-color);
     text-decoration: none;
 }
 
 .md-typeset a:hover {
-    color: #0053A1;
     text-decoration: underline;
 }
 
-.md-nav__link:hover {
-    color: #0053A1;
-}
-
 .headerlink {
     color: #777777 !important;
 }
 
 .headerlink:hover {
-    color: #0053A1 !important;
+    color: var(--md-accent-fg-color) !important;
     text-decoration: none !important;
 }
 
-
-/* .md-nav--primary {
-    color: #0053A1
-}
-
-.md-nav--primary ul ul .md-nav__item,
-.md-nav--primary ul ul .md-nav__item a {
-    color: #262626 !important
-}*/
-
 .md-nav__link--active {
-    color: #0053A1;
-    /* text-decoration: underline; */
+    color: var(--md-accent-fg-color);
 }
 
-
-/* .md-nav--primary ul ul .md-nav__item:before {
-    content: '\f105';
-    display: inline-block;
-    font: normal normal normal 14px/1 FontAwesome;
-    font-size: inherit;
-    text-rendering: auto;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-    margin-left: -11px;
-    margin-right: 6px;
-    color: #0053A1;
-} */
-
-
 /* footer style from swan */
 
 .md-footer {
     background: transparent;
 }
 
-.md-footer-meta {
+.md-footer-meta.md-typeset {
     background-color: #FAFAFA;
     border-top: solid 1px #DADADA;
     font-size: 13px;
     color: #777777;
 }
 
-.md-footer-meta img {
+.md-footer-meta.md-typeset img {
     margin: 14px 0;
     height: 55px;
 }
 
-.md-footer-meta .logo {
+.md-footer-meta.md-typeset .logo {
     float: left;
     display: inline-block;
     width: 25%;
     text-align: right;
 }
 
-.md-footer-meta .text {
+.md-footer-meta.md-typeset .text {
     float: left;
     display: inline-block;
     width: 75%;
     padding-top: 12px;
 }
 
-.md-footer-meta p {
+.md-footer-meta.md-typeset p {
     margin: 0;
 }
 
-.md-footer-meta ul {
+.md-footer-meta.md-typeset ul {
     padding: 0;
     margin: 0;
+    margin-left: 0; /* to overwrite upstream */
 }
 
-.md-footer-meta ul li {
+.md-footer-meta.md-typeset ul li {
     display: inline-block;
     margin-left: 0;
 }
 
 .md-footer-meta ul li+li:before {
     content: "| ";
     margin-left: 2px;
@@ -175,24 +152,24 @@
 html .md-footer-meta.md-typeset a:visited {
     color: inherit;
 }
 
 
 /* footer navbar */
 
-.md-footer-nav {
-    color: #0053A1;
+.md-footer__link {
+    color: var(--md-accent-fg-color);
 }
 
-span.md-footer-nav__direction {
+span.md-footer__direction {
     color: #777777;
 }
 
 @media only screen and (min-width: 76.1875em) {
-    /* remove sidebad title */
+    /* remove sidebar title */
     .md-sidebar--primary label.md-nav__title {
         display: none;
     }
 }
 
 .button__text {
     font-size: 0.6em;
@@ -267,15 +244,15 @@
     -moz-transition: all 0.2s ease-in-out;
     -o-transition: all 0.2s ease-in-out;
     transition: all 0.2s ease-in-out;
 }
 
 .gallery article .background {
     opacity: 0;
-    background-color: #0053A1;
+    background-color: var(--md-accent-fg-color);
     position: absolute;
     top: 0;
     left: 0;
     right: 0;
     bottom: 0;
     z-index: -1;
     -webkit-transition: opacity 0.2s ease-in-out;
@@ -290,13 +267,41 @@
 }
 
 .gallery article:hover .background {
     opacity: 1;
 }
 
 .gallery article:hover img {
-    border-color: #0053A1;
+    border-color: var(--md-accent-fg-color);
 }
 
 img.open_in_swan {
     margin: 0;
+}
+
+.md-header, .md-hero {
+    background-color: var(--md-primary-fg-color);
+}
+.md-hero {
+    overflow: hidden;
+    color: var(--md-primary-bg-color);
+    font-size: 1rem;
+    background-color: var(--md-primary-fg-color);
+    transition: background 250ms;
+}
+
+.md-hero__inner.hidden {
+    transform: translateY(0.625rem);
+    opacity: 0;
+    transition: transform 0ms 400ms,opacity 100ms 0ms;
+    pointer-events: none;
+}
+
+.md-hero--expand .md-hero__inner {
+    margin-bottom: 1.2rem;
+}
+.md-hero__inner {
+    margin-top: 1rem;
+    padding: 0.8rem 0.8rem 0.4rem;
+    transition: transform 400ms cubic-bezier(0.1, 0.7, 0.1, 1),opacity 250ms;
+    transition-delay: 100ms;
 }
```

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/images/favicon.ico` & `mkdocs-swan-0.3.0/mkdocs_swan/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/images/logo.png` & `mkdocs-swan-0.3.0/mkdocs_swan/images/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/images/logo_cern.png` & `mkdocs-swan-0.3.0/mkdocs_swan/images/logo_cern.png`

 * *Files identical despite different names*

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/main.html` & `mkdocs-swan-0.3.0/mkdocs_swan/main.html`

 * *Files 7% similar despite different names*

```diff
@@ -28,10 +28,11 @@
         }); 
     }
 </script>
 {% endblock %}
 
 {% block styles %}
 {{ super() }}
+<link rel="stylesheet" type="text/css" href="{{ 'css/fonts.css' | url }}" />
 <link rel="stylesheet" type="text/css" href="{{ 'css/style.css' | url }}" />
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
  {% extends "base.html" %} {% block extrahead %} {{ super() }}
  {% endblock %} {% block styles %} {{ super() }}
+
  {% endblock %}
```

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan/notebook.html` & `mkdocs-swan-0.3.0/mkdocs_swan/notebook.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "full_width.html" %}
+{% extends "main.html" %}
 
 <!-- Add Jupyter basic javascript at the head of the file -->
 {% block extrahead %}
 {{ super() }}
 <script type="text/javascript">
     function openInSwan(){
         if ( window.location !== window.parent.location ) { // Check if inside an iframe in jupyterlab
@@ -12,14 +12,31 @@
             // Skip redirecting the iframe page to start a new session inside the iframe
             return false; 
         } else {
             // When not inside an iframe, continue redirecting to the href URL to start a new SWAN session
             return true;
         }
     }
+
+    // Add a fading event to the title + download bar 
+    // when scrolling to top
+    hidden = false;
+    window.addEventListener("scroll", (event) => {
+        hero = document.getElementsByClassName("md-hero__inner")[0];
+        var y = window.scrollY;
+        if (y >= 20) {
+            if (!hidden){
+                hidden = true;
+                hero.classList.add("hidden");
+            }
+        } else if (hidden) {
+            hidden = false;
+            hero.classList.remove("hidden");
+        }
+    });
 </script>
 
 {{ super() }}
 <script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "full_width.html" %}  {% block extrahead %} {{ super() }}
+{% extends "main.html" %}  {% block extrahead %} {{ super() }}
  {{ super() }}
  {% endblock %} {% block styles %} {{ super() }}
  {% endblock %} {% if page and page.meta and page.meta.notebook_name %} {% set
 _ = page.meta.__setitem__("title", page.meta.notebook_name) %} {% block hero %}
 {{ page.meta.notebook_name }} {% if page.meta.notebook_url %} {%_include
 ".icons/material/pencil.svg"_%}_Open_in_SWAN {%_include_".icons/material/
 download.svg"_%}_Download {% endif %}
```

### Comparing `mkdocs-swan-0.2.0/mkdocs_swan.egg-info/PKG-INFO` & `mkdocs-swan-0.3.0/mkdocs_swan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swan
-Version: 0.2.0
+Version: 0.3.0
 Summary: SWAN theme for MkDocs
 Home-page: https://github.com/swan-cern/mkdocs-swan
 Author: Diogo Castro
 Author-email: diogo.castro@cern.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `mkdocs-swan-0.2.0/setup.py` & `mkdocs-swan-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load README contents
 with open("README.md", encoding = "utf-8") as data:
     long_description = data.read()
 
 setup(
     name="mkdocs-swan",
-    version='0.2.0',
+    version='0.3.0',
     url='https://github.com/swan-cern/mkdocs-swan',
     license='BSD',
     description='SWAN theme for MkDocs',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author='Diogo Castro',
     author_email='diogo.castro@cern.ch',
@@ -21,15 +21,15 @@
         "Programming Language :: Python",
         "Topic :: Documentation",
         "Topic :: Software Development :: Documentation",
         "Topic :: Text Processing :: Markup :: HTML"
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=['mkdocs-material==5.*'],
+    install_requires=['mkdocs-material==9.*'],
     entry_points={
         'mkdocs.themes': [
             'swan = mkdocs_swan',
         ]
     },
     zip_safe=False
 )
```

