# Comparing `tmp/anya_dash-0.0.2.tar.gz` & `tmp/anya_dash-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anya_dash-0.0.2.tar", last modified: Thu Jul 20 19:05:14 2023, max compression
+gzip compressed data, was "anya_dash-0.0.3.tar", last modified: Thu Jul 20 20:17:45 2023, max compression
```

## Comparing `anya_dash-0.0.2.tar` & `anya_dash-0.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 19:05:14.369189 anya_dash-0.0.2/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2023-07-17 16:00:17.000000 anya_dash-0.0.2/LICENSE
--rw-r--r--   0 estellaye   (501) staff       (20)      323 2023-07-17 16:00:17.000000 anya_dash-0.0.2/MANIFEST.in
--rw-r--r--   0 estellaye   (501) staff       (20)      247 2023-07-20 19:05:14.369042 anya_dash-0.0.2/PKG-INFO
--rw-r--r--   0 estellaye   (501) staff       (20)      305 2023-07-20 04:03:54.000000 anya_dash-0.0.2/README.md
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 19:05:14.367557 anya_dash-0.0.2/anya_dash/
--rw-r--r--   0 estellaye   (501) staff       (20)     1830 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaAffix.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3470 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaButton.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3076 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaCard.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3227 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaCheckbox.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3438 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaCheckboxGroup.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2745 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaCol.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3779 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaCollapse.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1697 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaContent.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1502 2023-07-17 21:53:12.000000 anya_dash-0.0.2/anya_dash/AnyaDash.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5657 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaDateRangePicker.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3057 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaDivider.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1084 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaExecuteJs.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1494 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaFooter.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2131 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaHeader.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1698 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaIcon.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6261 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaInput.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5607 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaInputNumber.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1637 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaLayout.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4377 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaMenu.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2826 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaModal.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2689 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaParagraph.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3894 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaRadioGroup.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2312 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaRow.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7425 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaSelect.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3061 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaSider.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4577 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaSlider.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2093 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaSpace.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3553 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaSwitch.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4462 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaTable.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3826 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaTabs.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1744 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaTag.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2665 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaText.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2525 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaTheme.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2427 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/AnyaTitle.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2043 2023-07-20 13:41:20.000000 anya_dash-0.0.2/anya_dash/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1792 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/_imports_.py
--rw-r--r--   0 estellaye   (501) staff       (20)  1380366 2023-07-20 19:00:43.000000 anya_dash-0.0.2/anya_dash/anya_dash.min.js
--rw-r--r--   0 estellaye   (501) staff       (20)  5746703 2023-07-20 19:00:43.000000 anya_dash-0.0.2/anya_dash/anya_dash.min.js.map
--rw-r--r--   0 estellaye   (501) staff       (20)   162108 2023-07-20 19:00:21.000000 anya_dash-0.0.2/anya_dash/metadata.json
--rw-r--r--   0 estellaye   (501) staff       (20)     2474 2023-07-20 19:00:20.000000 anya_dash-0.0.2/anya_dash/package-info.json
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 19:05:14.368083 anya_dash-0.0.2/anya_dash.egg-info/
--rw-r--r--   0 estellaye   (501) staff       (20)      247 2023-07-20 19:05:14.000000 anya_dash-0.0.2/anya_dash.egg-info/PKG-INFO
--rw-r--r--   0 estellaye   (501) staff       (20)     1326 2023-07-20 19:05:14.000000 anya_dash-0.0.2/anya_dash.egg-info/SOURCES.txt
--rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-07-20 19:05:14.000000 anya_dash-0.0.2/anya_dash.egg-info/dependency_links.txt
--rw-r--r--   0 estellaye   (501) staff       (20)       10 2023-07-20 19:05:14.000000 anya_dash-0.0.2/anya_dash.egg-info/top_level.txt
--rw-r--r--   0 estellaye   (501) staff       (20)     2474 2023-07-20 19:05:09.000000 anya_dash-0.0.2/package.json
--rw-r--r--   0 estellaye   (501) staff       (20)       38 2023-07-20 19:05:14.369231 anya_dash-0.0.2/setup.cfg
--rw-r--r--   0 estellaye   (501) staff       (20)      510 2023-07-17 16:00:17.000000 anya_dash-0.0.2/setup.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 19:05:14.368860 anya_dash-0.0.2/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)     8802 2023-07-19 16:22:59.000000 anya_dash-0.0.2/tests/test_cards_tabs_collapse.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3835 2023-07-19 15:55:34.000000 anya_dash-0.0.2/tests/test_common.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9440 2023-07-18 10:34:15.000000 anya_dash-0.0.2/tests/test_data_entry.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4674 2023-07-17 11:13:48.000000 anya_dash-0.0.2/tests/test_layout_collapsible_sider.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3303 2023-07-20 14:43:24.000000 anya_dash-0.0.2/tests/test_table.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5905 2023-07-17 12:09:18.000000 anya_dash-0.0.2/tests/test_typography.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 20:17:45.176409 anya_dash-0.0.3/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2023-07-17 16:00:17.000000 anya_dash-0.0.3/LICENSE
+-rw-r--r--   0 estellaye   (501) staff       (20)      323 2023-07-17 16:00:17.000000 anya_dash-0.0.3/MANIFEST.in
+-rw-r--r--   0 estellaye   (501) staff       (20)      247 2023-07-20 20:17:45.176249 anya_dash-0.0.3/PKG-INFO
+-rw-r--r--   0 estellaye   (501) staff       (20)      305 2023-07-20 04:03:54.000000 anya_dash-0.0.3/README.md
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 20:17:45.174780 anya_dash-0.0.3/anya_dash/
+-rw-r--r--   0 estellaye   (501) staff       (20)     1830 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaAffix.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3470 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaButton.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3076 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaCard.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3227 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaCheckbox.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3438 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaCheckboxGroup.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2745 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaCol.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3779 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaCollapse.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1697 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaContent.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1502 2023-07-17 21:53:12.000000 anya_dash-0.0.3/anya_dash/AnyaDash.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5657 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaDateRangePicker.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3057 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaDivider.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1084 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaExecuteJs.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1494 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaFooter.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2131 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaHeader.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1698 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaIcon.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6261 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaInput.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5607 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaInputNumber.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1637 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaLayout.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4377 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaMenu.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2826 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaModal.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2689 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaParagraph.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3894 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaRadioGroup.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2312 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaRow.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7425 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaSelect.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3061 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaSider.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4577 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaSlider.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2093 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaSpace.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3553 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaSwitch.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4461 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaTable.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3826 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaTabs.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1744 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaTag.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2665 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaText.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2525 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaTheme.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2427 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/AnyaTitle.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2043 2023-07-20 13:41:20.000000 anya_dash-0.0.3/anya_dash/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1792 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/_imports_.py
+-rw-r--r--   0 estellaye   (501) staff       (20)  1380460 2023-07-20 20:16:04.000000 anya_dash-0.0.3/anya_dash/anya_dash.min.js
+-rw-r--r--   0 estellaye   (501) staff       (20)  5747032 2023-07-20 20:16:04.000000 anya_dash-0.0.3/anya_dash/anya_dash.min.js.map
+-rw-r--r--   0 estellaye   (501) staff       (20)   162107 2023-07-20 20:16:12.000000 anya_dash-0.0.3/anya_dash/metadata.json
+-rw-r--r--   0 estellaye   (501) staff       (20)     2474 2023-07-20 20:16:11.000000 anya_dash-0.0.3/anya_dash/package-info.json
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 20:17:45.175285 anya_dash-0.0.3/anya_dash.egg-info/
+-rw-r--r--   0 estellaye   (501) staff       (20)      247 2023-07-20 20:17:45.000000 anya_dash-0.0.3/anya_dash.egg-info/PKG-INFO
+-rw-r--r--   0 estellaye   (501) staff       (20)     1326 2023-07-20 20:17:45.000000 anya_dash-0.0.3/anya_dash.egg-info/SOURCES.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-07-20 20:17:45.000000 anya_dash-0.0.3/anya_dash.egg-info/dependency_links.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)       10 2023-07-20 20:17:45.000000 anya_dash-0.0.3/anya_dash.egg-info/top_level.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)     2474 2023-07-20 20:17:18.000000 anya_dash-0.0.3/package.json
+-rw-r--r--   0 estellaye   (501) staff       (20)       38 2023-07-20 20:17:45.176454 anya_dash-0.0.3/setup.cfg
+-rw-r--r--   0 estellaye   (501) staff       (20)      510 2023-07-17 16:00:17.000000 anya_dash-0.0.3/setup.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-07-20 20:17:45.176053 anya_dash-0.0.3/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)     8802 2023-07-19 16:22:59.000000 anya_dash-0.0.3/tests/test_cards_tabs_collapse.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3835 2023-07-19 15:55:34.000000 anya_dash-0.0.3/tests/test_common.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9440 2023-07-18 10:34:15.000000 anya_dash-0.0.3/tests/test_data_entry.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4674 2023-07-17 11:13:48.000000 anya_dash-0.0.3/tests/test_layout_collapsible_sider.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3346 2023-07-20 19:07:49.000000 anya_dash-0.0.3/tests/test_table.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5905 2023-07-17 12:09:18.000000 anya_dash-0.0.3/tests/test_typography.py
```

### Comparing `anya_dash-0.0.2/anya_dash/AnyaAffix.py` & `anya_dash-0.0.3/anya_dash/AnyaAffix.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaButton.py` & `anya_dash-0.0.3/anya_dash/AnyaButton.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaCard.py` & `anya_dash-0.0.3/anya_dash/AnyaCard.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaCheckbox.py` & `anya_dash-0.0.3/anya_dash/AnyaCheckbox.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaCheckboxGroup.py` & `anya_dash-0.0.3/anya_dash/AnyaCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaCol.py` & `anya_dash-0.0.3/anya_dash/AnyaCol.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaCollapse.py` & `anya_dash-0.0.3/anya_dash/AnyaCollapse.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaContent.py` & `anya_dash-0.0.3/anya_dash/AnyaContent.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaDash.py` & `anya_dash-0.0.3/anya_dash/AnyaDash.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaDateRangePicker.py` & `anya_dash-0.0.3/anya_dash/AnyaDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaDivider.py` & `anya_dash-0.0.3/anya_dash/AnyaDivider.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaExecuteJs.py` & `anya_dash-0.0.3/anya_dash/AnyaExecuteJs.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaFooter.py` & `anya_dash-0.0.3/anya_dash/AnyaFooter.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaHeader.py` & `anya_dash-0.0.3/anya_dash/AnyaHeader.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaIcon.py` & `anya_dash-0.0.3/anya_dash/AnyaIcon.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaInput.py` & `anya_dash-0.0.3/anya_dash/AnyaInput.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaInputNumber.py` & `anya_dash-0.0.3/anya_dash/AnyaInputNumber.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaLayout.py` & `anya_dash-0.0.3/anya_dash/AnyaLayout.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaMenu.py` & `anya_dash-0.0.3/anya_dash/AnyaMenu.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaModal.py` & `anya_dash-0.0.3/anya_dash/AnyaModal.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaParagraph.py` & `anya_dash-0.0.3/anya_dash/AnyaParagraph.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaRadioGroup.py` & `anya_dash-0.0.3/anya_dash/AnyaRadioGroup.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaRow.py` & `anya_dash-0.0.3/anya_dash/AnyaRow.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaSelect.py` & `anya_dash-0.0.3/anya_dash/AnyaSelect.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaSider.py` & `anya_dash-0.0.3/anya_dash/AnyaSider.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaSlider.py` & `anya_dash-0.0.3/anya_dash/AnyaSlider.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaSpace.py` & `anya_dash-0.0.3/anya_dash/AnyaSpace.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaSwitch.py` & `anya_dash-0.0.3/anya_dash/AnyaSwitch.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaTable.py` & `anya_dash-0.0.3/anya_dash/AnyaTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 - maxHeight (number; optional):
     Set max height.
 
 - maxWidth (number; optional):
     Set max width.
 
-- pagination (dict; default {    defaultPageSize: 20,    hideOnSinglePage: True,    showSizeChanger: False,}):
+- pagination (dict; default {    defaultPageSize: 20,    hideOnSinglePage: True,    showSizeChanger: False}):
     Config of pagination. You can ref table pagination config or full
     pagination document, hide it by setting it to False.
 
     `pagination` is a dict with keys:
 
     - current (number; optional)
```

### Comparing `anya_dash-0.0.2/anya_dash/AnyaTabs.py` & `anya_dash-0.0.3/anya_dash/AnyaTabs.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaTag.py` & `anya_dash-0.0.3/anya_dash/AnyaTag.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaText.py` & `anya_dash-0.0.3/anya_dash/AnyaText.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaTheme.py` & `anya_dash-0.0.3/anya_dash/AnyaTheme.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/AnyaTitle.py` & `anya_dash-0.0.3/anya_dash/AnyaTitle.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/__init__.py` & `anya_dash-0.0.3/anya_dash/__init__.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/_imports_.py` & `anya_dash-0.0.3/anya_dash/_imports_.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/anya_dash/anya_dash.min.js` & `anya_dash-0.0.3/anya_dash/anya_dash.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -34955,15 +34955,15 @@
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
                 n = isLocalScript(t),
                 r = __jsonpScriptSrc__(e);
             if (!n) return r;
             var o = r.split("/"),
                 a = o.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_1m1689879637"), o.splice(-1, 1, a.join(".")), o.join("/")
+            return a.splice(1, 0, "v0_0_2m1689884159"), o.splice(-1, 1, a.join(".")), o.join("/")
         }
     }
     __webpack_require__.nc = void 0;
     var __webpack_exports__ = {};
     (() => {
         "use strict";
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
@@ -64672,17 +64672,21 @@
                 a = e.columns,
                 i = e.data,
                 s = e.bordered,
                 l = e.maxHeight,
                 c = e.maxWidth,
                 u = e.size,
                 d = e.cellUpdateOptimize;
-            e.setProps, o && o.position && (o = Ty(Ty({}, o), {}, {
+            e.setProps, o && (o.position && (o = Ty(Ty({}, o), {}, {
                 position: [o.position]
-            }));
+            })), o.showTotal && (o = Ty(Ty({}, o), {}, {
+                showTotal: function(e) {
+                    return "Total ".concat(e, " items")
+                }
+            })));
             for (var f = function(e) {
                     (a[e].rowSpan || a[e].colSpanRow) && (a[e].onCell = function(t, n) {
                         var r = {};
                         return a[e].rowSpan && n in a[e].rowSpan && (r.rowSpan = a[e].rowSpan[n]), a[e].colSpanRow && n in a[e].colSpanRow && (r.colSpan = a[e].colSpanRow[n]), r
                     }), a[e].className || (a[e].className = a[e].dataIndex), a[e].renderOptions && a[e].renderOptions.renderType
                 }, p = 0; p < a.length; p++) f(p);
             for (var m in d && (a = a.map((function(e) {
```

### Comparing `anya_dash-0.0.2/anya_dash/anya_dash.min.js.map` & `anya_dash-0.0.3/anya_dash/anya_dash.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9283011217732126%*

 * *Differences: {"'mappings'": "';uHACIA,EAAU,EAEVC,EAAiB,IAEjBC,EAAkB,IAElBC,EAAkB,IAElBC,EAAkB,IAElBC,EAAkB,EAElBC,EAAiB,EAGjBC,EAAe,CAAC,CAClBC,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,IACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,IACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,KACR,CACDD,MAAO,EACPC,QAAS,MAKX,SAASC,EAAMC,GACb,IAAIC,EAAID,EAAKC,EACTC,EAAIF,EAAKE,EACTC,EAAIH,EAAKG,EACTC,GAAM,QAASH,EAAGC,EAAGC,GACzB,MAAO,CACLE, […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "anya_dash.min.js",
     "names": [
         "hueStep",
         "saturationStep",
         "saturationStep2",
         "brightnessStep1",
         "brightnessStep2",
         "lightColorCount",
@@ -11818,15 +11818,15 @@
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\tloaded: false,\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Flag the module as loaded\n\tmodule.loaded = true;\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_1m1689879637\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_2m1689884159\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "__webpack_require__.nc = undefined;",
         "\n      import API from \"!../../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n      import domAPI from \"!../../../node_modules/style-loader/dist/runtime/styleDomAPI.js\";\n      import insertFn from \"!../../../node_modules/style-loader/dist/runtime/insertBySelector.js\";\n      import setAttributes from \"!../../../node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js\";\n      import insertStyleElement from \"!../../../node_modules/style-loader/dist/runtime/insertStyleElement.js\";\n      import styleTagTransformFn from \"!../../../node_modules/style-loader/dist/runtime/styleTagTransform.js\";\n      import content, * as namedExport from \"!!../../../node_modules/css-loader/dist/cjs.js!./styles.css\";\n      \n      \n\nvar options = {};\n\noptions.styleTagTransform = styleTagTransformFn;\noptions.setAttributes = setAttributes;\n\n      options.insert = insertFn.bind(null, \"head\");\n    \noptions.domAPI = domAPI;\noptions.insertStyleElement = insertStyleElement;\n\nvar update = API(content, options);\n\n\n\nexport * from \"!!../../../node_modules/css-loader/dist/cjs.js!./styles.css\";\n       export default content && content.locals ? content.locals : undefined;\n",
         "import React from 'react';\nimport PropTypes from 'prop-types';\nimport {ConfigProvider} from 'antd';\n\n/**\n * An Ant Design ConfigProvider\n * See https://ant.design/docs/react/customize-theme\n */\nconst AnyaTheme = (props) => {\n    let {\n        children,\n        colorPrimary,\n        colorSuccess,\n        colorWarning,\n        colorInfo,\n        colorTextBase,\n        colorBgLayout,\n        colorBgContainer,\n        fontSize,\n        fontFamily,\n        wireframe,\n    } = props;\n\n    return (\n        <ConfigProvider\n            theme={{\n                token: {\n                    colorPrimary: {colorPrimary}.colorPrimary,\n                    colorSuccess: {colorSuccess}.colorSuccess,\n                    colorWarning: {colorWarning}.colorWarning,\n                    colorBgLayout: {colorBgLayout}.colorBgLayout,\n                    colorBgContainer: {colorBgContainer}.colorBgContainer,\n                    colorInfo: {colorInfo}.colorInfo,\n                    colorTextBase: {colorTextBase}.colorTextBase,\n                    fontSize: {fontSize}.fontSize,\n                    wireframe: {wireframe}.wireframe,\n                    fontFamily: {fontFamily}.fontFamily\n                },\n            }}\n        >\n            {children}\n        </ConfigProvider>\n    );\n};\n\nAnyaTheme.propTypes = {\n    /**\n     * Child components inside the space\n     */\n    children: PropTypes.node,\n\n    /**\n     * Primary color\n     */\n    colorPrimary: PropTypes.string,\n    \n\n    /**\n     * Success color\n     */\n    colorSuccess: PropTypes.string,\n\n    /**\n     * Warning color\n     */\n    colorWarning: PropTypes.string,\n\n    /**\n     * Info color\n     */\n    colorInfo: PropTypes.string,\n\n    /**\n     * Text color\n     */\n    colorTextBase: PropTypes.string,\n\n    /**\n     * Layout background color\n     */\n    colorBgLayout: PropTypes.string,\n\n    /**\n     * Container background color\n     */\n    colorBgContainer: PropTypes.string,\n\n    /**\n     * Font size\n     */\n    fontSize: PropTypes.number,\n\n    /**\n     * Font family\n     */\n    fontFamily: PropTypes.string,\n\n    /**\n     * Wireframe\n     */\n    wireframe: PropTypes.bool,\n};\n\n// Default paramters\nAnyaTheme.defaultProps = {\n    colorPrimary: '#6366f1',\n    colorSuccess: '#13c2b7',\n    colorWarning: '#faad14',\n    colorInfo: '#6366f1',\n    colorTextBase: '#424245',\n    colorBgLayout: '#f0f2f5',\n    colorBgContainer: '#ffffff',\n    fontSize: 12,\n    wireframe: false,\n    fontFamily:\n        \"-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, 'Noto Sans', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji'\",\n};\n\nexport default AnyaTheme;\n",
         "import canUseDom from \"rc-util/es/Dom/canUseDom\";\nimport { isStyleSupport } from \"rc-util/es/Dom/styleChecker\";\nexport const canUseDocElement = () => canUseDom() && window.document.documentElement;\nexport { isStyleSupport };\nlet flexGapSupported;\nexport const detectFlexGapSupported = () => {\n  if (!canUseDocElement()) {\n    return false;\n  }\n  if (flexGapSupported !== undefined) {\n    return flexGapSupported;\n  }\n  // create flex container with row-gap set\n  const flex = document.createElement('div');\n  flex.style.display = 'flex';\n  flex.style.flexDirection = 'column';\n  flex.style.rowGap = '1px';\n  // create two, elements inside it\n  flex.appendChild(document.createElement('div'));\n  flex.appendChild(document.createElement('div'));\n  // some browser may not repaint when remove nodes, so we need create a new layer to detect.\n  const container = document.createElement('div');\n  container.style.position = 'absolute';\n  container.style.zIndex = '-9999';\n  container.appendChild(flex);\n  // append to the DOM (needed to obtain scrollHeight)\n  document.body.appendChild(container);\n  flexGapSupported = flex.scrollHeight === 1; // flex container should be 1px high from the row-gap\n  document.body.removeChild(container);\n  return flexGapSupported;\n};",
         "import * as React from 'react';\nimport { detectFlexGapSupported } from '../styleChecker';\nexport default (() => {\n  const [flexible, setFlexible] = React.useState(false);\n  React.useEffect(() => {\n    setFlexible(detectFlexGapSupported());\n  }, []);\n  return flexible;\n});",
         "import React from 'react';\nexport const SpaceContext = /*#__PURE__*/React.createContext({\n  latestIndex: 0,\n  horizontalSize: 0,\n  verticalSize: 0,\n  supportFlexGap: false\n});\nexport const SpaceContextProvider = SpaceContext.Provider;",
         "import * as React from 'react';\nimport { SpaceContext } from './context';\nexport default function Item(_ref) {\n  let {\n    className,\n    direction,\n    index,\n    marginDirection,\n    children,\n    split,\n    wrap,\n    style: customStyle\n  } = _ref;\n  const {\n    horizontalSize,\n    verticalSize,\n    latestIndex,\n    supportFlexGap\n  } = React.useContext(SpaceContext);\n  let style = {};\n  if (!supportFlexGap) {\n    if (direction === 'vertical') {\n      if (index < latestIndex) {\n        style = {\n          marginBottom: horizontalSize / (split ? 2 : 1)\n        };\n      }\n    } else {\n      style = Object.assign(Object.assign({}, index < latestIndex && {\n        [marginDirection]: horizontalSize / (split ? 2 : 1)\n      }), wrap && {\n        paddingBottom: verticalSize\n      });\n    }\n  }\n  if (children === null || children === undefined) {\n    return null;\n  }\n  return /*#__PURE__*/React.createElement(React.Fragment, null, /*#__PURE__*/React.createElement(\"div\", {\n    className: className,\n    style: Object.assign(Object.assign({}, style), customStyle)\n  }, children), index < latestIndex && split && /*#__PURE__*/React.createElement(\"span\", {\n    className: `${className}-split`,\n    style: style\n  }, split));\n}",
@@ -12300,15 +12300,15 @@
         "import * as React from 'react';\nexport default function useLazyKVMap(data, childrenColumnName, getRowKey) {\n  const mapCacheRef = React.useRef({});\n  function getRecordByKey(key) {\n    if (!mapCacheRef.current || mapCacheRef.current.data !== data || mapCacheRef.current.childrenColumnName !== childrenColumnName || mapCacheRef.current.getRowKey !== getRowKey) {\n      const kvMap = new Map();\n      /* eslint-disable no-inner-declarations */\n      function dig(records) {\n        records.forEach((record, index) => {\n          const rowKey = getRowKey(record, index);\n          kvMap.set(rowKey, record);\n          if (record && typeof record === 'object' && childrenColumnName in record) {\n            dig(record[childrenColumnName] || []);\n          }\n        });\n      }\n      /* eslint-enable */\n      dig(data);\n      mapCacheRef.current = {\n        data,\n        childrenColumnName,\n        kvMap,\n        getRowKey\n      };\n    }\n    return mapCacheRef.current.kvMap.get(key);\n  }\n  return [getRecordByKey];\n}",
         "import raf from \"rc-util/es/raf\";\nimport { easeInOutCubic } from './easings';\nimport getScroll, { isWindow } from './getScroll';\nexport default function scrollTo(y) {\n  let options = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};\n  const {\n    getContainer = () => window,\n    callback,\n    duration = 450\n  } = options;\n  const container = getContainer();\n  const scrollTop = getScroll(container, true);\n  const startTime = Date.now();\n  const frameFunc = () => {\n    const timestamp = Date.now();\n    const time = timestamp - startTime;\n    const nextScrollTop = easeInOutCubic(time > duration ? duration : time, scrollTop, y, duration);\n    if (isWindow(container)) {\n      container.scrollTo(window.pageXOffset, nextScrollTop);\n    } else if (container instanceof Document || container.constructor.name === 'HTMLDocument') {\n      container.documentElement.scrollTop = nextScrollTop;\n    } else {\n      container.scrollTop = nextScrollTop;\n    }\n    if (time < duration) {\n      raf(frameFunc);\n    } else if (typeof callback === 'function') {\n      callback();\n    }\n  };\n  raf(frameFunc);\n}",
         "// eslint-disable-next-line import/prefer-default-export\nexport function easeInOutCubic(t, b, c, d) {\n  const cc = c - b;\n  t /= d / 2;\n  if (t < 1) {\n    return cc / 2 * t * t * t + b;\n  }\n  // eslint-disable-next-line no-return-assign\n  return cc / 2 * ((t -= 2) * t * t + 2) + b;\n}",
         "import { EXPAND_COLUMN, Summary } from 'rc-table';\nimport * as React from 'react';\nimport Column from './Column';\nimport ColumnGroup from './ColumnGroup';\nimport InternalTable from './InternalTable';\nimport { SELECTION_ALL, SELECTION_COLUMN, SELECTION_INVERT, SELECTION_NONE } from './hooks/useSelection';\nconst Table = (props, ref) => {\n  const renderTimesRef = React.useRef(0);\n  renderTimesRef.current += 1;\n  return /*#__PURE__*/React.createElement(InternalTable, Object.assign({}, props, {\n    ref: ref,\n    _renderTimes: renderTimesRef.current\n  }));\n};\nconst ForwardTable = /*#__PURE__*/React.forwardRef(Table);\nForwardTable.SELECTION_COLUMN = SELECTION_COLUMN;\nForwardTable.EXPAND_COLUMN = EXPAND_COLUMN;\nForwardTable.SELECTION_ALL = SELECTION_ALL;\nForwardTable.SELECTION_INVERT = SELECTION_INVERT;\nForwardTable.SELECTION_NONE = SELECTION_NONE;\nForwardTable.Column = Column;\nForwardTable.ColumnGroup = ColumnGroup;\nForwardTable.Summary = Summary;\nexport default ForwardTable;",
         "/* istanbul ignore next */\n/** This is a syntactic sugar for `columns` prop. So HOC will not work on this. */\n// eslint-disable-next-line no-unused-vars\nfunction Column(_) {\n  return null;\n}\nexport default Column;",
         "/* istanbul ignore next */\n/** This is a syntactic sugar for `columns` prop. So HOC will not work on this. */\n// eslint-disable-next-line no-unused-vars\nfunction ColumnGroup(_) {\n  return null;\n}\nexport default ColumnGroup;",
         "import Table from './Table';\nexport default Table;",
-        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport useCss from '../../hooks/useCss';\nimport { isNumber, isEqual, isString } from 'lodash';\nimport {Space, Table} from 'antd';\n\n/**\n * An Ant Design Table component\n * See https://ant.design/components/table\n */\nconst AnyaTable = (props) => {\n    let {\n        id,\n        className,\n        style,\n        pagination,\n        columns,\n        data,\n        bordered,\n        maxHeight,\n        maxWidth,\n        size,\n        cellUpdateOptimize,\n        setProps,\n    } = props;\n\n    if (pagination && pagination.position) {\n        pagination = {\n            ...pagination,\n            position: [pagination.position],\n        };\n    }\n\n    for (let i = 0; i < columns.length; i++) {\n        // handle rowspan\n        if (columns[i]['rowSpan'] || columns[i]['colSpanRow']) {\n            columns[i]['onCell'] = (_, index) => {\n                const spanAttr = {};\n                if (columns[i]['rowSpan']) {\n                    if (index in columns[i]['rowSpan']) {\n                        spanAttr.rowSpan = columns[i]['rowSpan'][index];\n                    } \n                }\n                if (columns[i]['colSpanRow']) {\n                    if (index in columns[i]['colSpanRow']) {\n                        spanAttr.colSpan = columns[i]['colSpanRow'][index];\n                    }\n                }\n                return spanAttr;\n            }\n        }\n\n        // handle column classname\n        if (!columns[i]['className']) {\n            columns[i]['className'] = columns[i]['dataIndex']\n        }\n\n        if (\n            columns[i]['renderOptions'] &&\n            columns[i]['renderOptions']['renderType']\n        ) {\n        }\n    }\n\n    if (cellUpdateOptimize) {\n        columns = columns.map((item) => {\n            return {\n                ...item,\n                shouldCellUpdate: (record, prevRecord) => {\n                    if (isEqual(record, prevRecord)) {\n                        return false;\n                    }\n                    return true;\n                },\n            };\n        });\n    }\n\n    // set key for data\n    for (let i in data) {\n        if (!data[i].hasOwnProperty('key')) {\n            data[i]['key'] = i.toString()\n        }\n    }\n\n    return (\n        <Table\n            id={id}\n            className={\n                isString(className)\n                    ? className\n                    : className\n                    ? useCss(className)\n                    : undefined\n            }\n            style={style}\n            bordered={bordered}\n            dataSource={data}\n            columns={columns}\n            data={data}\n            size={size}\n            scroll={{x: maxWidth, y: maxHeight, scrollToFirstRowOnChange: true}}\n            pagination={pagination}\n        ></Table>\n    );\n};\n\nAnyaTable.propTypes = {\n    /**\n     * The ID used to identify this component\n     */\n    id: PropTypes.string,\n\n    /**\n     * CSS classes to be added to the component\n     */\n    className: PropTypes.oneOfType([PropTypes.string, PropTypes.object]),\n\n    /**\n     * Inline CSS style\n     */\n    style: PropTypes.object,\n\n    /**\n     * Columns\n     */\n    columns: PropTypes.arrayOf(\n        PropTypes.exact({\n            title: PropTypes.oneOfType([PropTypes.func, PropTypes.node])\n                .isRequired,\n            dataIndex: PropTypes.string.isRequired,\n\n            // group\n            group: PropTypes.oneOfType([\n                PropTypes.string,\n                PropTypes.arrayOf(PropTypes.string),\n            ]),\n\n            // render options\n            renderOptions: PropTypes.exact({\n                renderType: PropTypes.oneOf(['row-merge']),\n            }),\n\n            // key\n            key: PropTypes.string,\n\n            //colspan\n            colSpan: PropTypes.number,\n\n            //rowspan\n            rowSpan: PropTypes.object,\n\n            //colSpanRow\n            colSpanRow: PropTypes.object,\n\n            //css classname\n            className: PropTypes.object,\n\n            // fixed options\n            fixed: PropTypes.oneOf(['left', 'right']),\n\n            // text alignment\n            align: PropTypes.oneOf(['left', 'center', 'right']),\n\n            // width\n            width: PropTypes.oneOfType([PropTypes.number, PropTypes.string]),\n\n            // hidden\n            hidden: PropTypes.bool,\n\n            // filter reset\n            filterResetToDefaultFilteredValue: PropTypes.bool,\n\n            // ellipsis\n            ellipsis: PropTypes.any,\n\n            // not used\n            sorter: PropTypes.any,\n\n            // not used\n            render: PropTypes.any,\n\n            /// not used\n            onCell: PropTypes.any,\n        })\n    ),\n\n    /**\n     * Column data\n     */\n    data: PropTypes.arrayOf(\n        PropTypes.objectOf(\n            PropTypes.oneOfType([\n                PropTypes.arrayOf(PropTypes.any),\n                PropTypes.node,\n                PropTypes.string,\n                PropTypes.number,\n\n                // Row span\n                PropTypes.exact({\n                    content: PropTypes.oneOfType([\n                        PropTypes.number,\n                        PropTypes.string,\n                    ]),\n                    rowSpan: PropTypes.number,\n                    key: PropTypes.string\n                }),\n            ])\n        )\n    ),\n\n    /**\n     * Bordered\n     */\n    bordered: PropTypes.bool,\n\n    /**\n     * Set max height\n     */\n    maxHeight: PropTypes.number,\n\n    /**\n     * Set max width\n     */\n    maxWidth: PropTypes.number,\n\n    /**\n     * Size\n     */\n    size: PropTypes.oneOf(['small', 'default', 'large']),\n\n    /**\n     * Config of pagination. You can ref table pagination config or full pagination document, hide it by setting it to false\n     */\n    pagination: PropTypes.oneOfType([\n        PropTypes.exact({\n            position: PropTypes.oneOf([\n                'topLeft',\n                'topCenter',\n                'topRight',\n                'bottomLeft',\n                'bottomCenter',\n                'bottomRight',\n            ]),\n            pageSize: PropTypes.number,\n            current: PropTypes.number,\n            showSizeChanger: PropTypes.bool,\n            pageSizeOptions: PropTypes.arrayOf(PropTypes.number),\n            showTotal: PropTypes.bool,\n            showQuickJumper: PropTypes.bool,\n            showTotalPrefix: PropTypes.string,\n            showTotalSuffix: PropTypes.string,\n            hideOnSinglePage: PropTypes.bool,\n            simple: PropTypes.bool,\n            disabled: PropTypes.bool,\n            size: PropTypes.oneOf(['default', 'small']),\n            total: PropTypes.number,\n        }),\n        PropTypes.bool,\n        PropTypes.object,\n    ]),\n\n    /**\n     * Whether to allow cell content rendering\n     */\n    cellUpdateOptimize: PropTypes.bool,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func,\n};\n\nAnyaTable.defaultProps = {\n    size: 'small',\n    cellUpdateOptimize: true,\n    pagination: {\n        defaultPageSize: 20,\n        hideOnSinglePage: true,\n        showSizeChanger: false,\n    },\n};\n\nexport default AnyaTable;\n",
+        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport useCss from '../../hooks/useCss';\nimport { isNumber, isEqual, isString } from 'lodash';\nimport {Space, Table} from 'antd';\n\n/**\n * An Ant Design Table component\n * See https://ant.design/components/table\n */\nconst AnyaTable = (props) => {\n    let {\n        id,\n        className,\n        style,\n        pagination,\n        columns,\n        data,\n        bordered,\n        maxHeight,\n        maxWidth,\n        size,\n        cellUpdateOptimize,\n        setProps,\n    } = props;\n\n\n\n    if (pagination) {\n        if (pagination.position) {\n            pagination = {\n                ...pagination,\n                position: [pagination.position],\n            };\n        }\n        if (pagination.showTotal) {\n            pagination = {\n                ...pagination,\n                showTotal: total => `Total ${total} items`\n            }\n        }\n    }\n\n    for (let i = 0; i < columns.length; i++) {\n        // handle rowspan\n        if (columns[i]['rowSpan'] || columns[i]['colSpanRow']) {\n            columns[i]['onCell'] = (_, index) => {\n                const spanAttr = {};\n                if (columns[i]['rowSpan']) {\n                    if (index in columns[i]['rowSpan']) {\n                        spanAttr.rowSpan = columns[i]['rowSpan'][index];\n                    } \n                }\n                if (columns[i]['colSpanRow']) {\n                    if (index in columns[i]['colSpanRow']) {\n                        spanAttr.colSpan = columns[i]['colSpanRow'][index];\n                    }\n                }\n                return spanAttr;\n            }\n        }\n\n        // handle column classname\n        if (!columns[i]['className']) {\n            columns[i]['className'] = columns[i]['dataIndex']\n        }\n\n        if (\n            columns[i]['renderOptions'] &&\n            columns[i]['renderOptions']['renderType']\n        ) {\n        }\n    }\n\n    if (cellUpdateOptimize) {\n        columns = columns.map((item) => {\n            return {\n                ...item,\n                shouldCellUpdate: (record, prevRecord) => {\n                    if (isEqual(record, prevRecord)) {\n                        return false;\n                    }\n                    return true;\n                },\n            };\n        });\n    }\n\n    // set key for data\n    for (let i in data) {\n        if (!data[i].hasOwnProperty('key')) {\n            data[i]['key'] = i.toString()\n        }\n    }\n\n    return (\n        <Table\n            id={id}\n            className={\n                isString(className)\n                    ? className\n                    : className\n                    ? useCss(className)\n                    : undefined\n            }\n            style={style}\n            bordered={bordered}\n            dataSource={data}\n            columns={columns}\n            data={data}\n            size={size}\n            scroll={{x: maxWidth, y: maxHeight, scrollToFirstRowOnChange: true}}\n            pagination={pagination}\n        ></Table>\n    );\n};\n\nAnyaTable.propTypes = {\n    /**\n     * The ID used to identify this component\n     */\n    id: PropTypes.string,\n\n    /**\n     * CSS classes to be added to the component\n     */\n    className: PropTypes.oneOfType([PropTypes.string, PropTypes.object]),\n\n    /**\n     * Inline CSS style\n     */\n    style: PropTypes.object,\n\n    /**\n     * Columns\n     */\n    columns: PropTypes.arrayOf(\n        PropTypes.exact({\n            title: PropTypes.oneOfType([PropTypes.func, PropTypes.node])\n                .isRequired,\n            dataIndex: PropTypes.string.isRequired,\n\n            // group\n            group: PropTypes.oneOfType([\n                PropTypes.string,\n                PropTypes.arrayOf(PropTypes.string),\n            ]),\n\n            // render options\n            renderOptions: PropTypes.exact({\n                renderType: PropTypes.oneOf(['row-merge']),\n            }),\n\n            // key\n            key: PropTypes.string,\n\n            //colspan\n            colSpan: PropTypes.number,\n\n            //rowspan\n            rowSpan: PropTypes.object,\n\n            //colSpanRow\n            colSpanRow: PropTypes.object,\n\n            //css classname\n            className: PropTypes.object,\n\n            // fixed options\n            fixed: PropTypes.oneOf(['left', 'right']),\n\n            // text alignment\n            align: PropTypes.oneOf(['left', 'center', 'right']),\n\n            // width\n            width: PropTypes.oneOfType([PropTypes.number, PropTypes.string]),\n\n            // hidden\n            hidden: PropTypes.bool,\n\n            // filter reset\n            filterResetToDefaultFilteredValue: PropTypes.bool,\n\n            // ellipsis\n            ellipsis: PropTypes.any,\n\n            // not used\n            sorter: PropTypes.any,\n\n            // not used\n            render: PropTypes.any,\n\n            /// not used\n            onCell: PropTypes.any,\n        })\n    ),\n\n    /**\n     * Column data\n     */\n    data: PropTypes.arrayOf(\n        PropTypes.objectOf(\n            PropTypes.oneOfType([\n                PropTypes.arrayOf(PropTypes.any),\n                PropTypes.node,\n                PropTypes.string,\n                PropTypes.number,\n\n                // Row span\n                PropTypes.exact({\n                    content: PropTypes.oneOfType([\n                        PropTypes.number,\n                        PropTypes.string,\n                    ]),\n                    rowSpan: PropTypes.number,\n                    key: PropTypes.string\n                }),\n            ])\n        )\n    ),\n\n    /**\n     * Bordered\n     */\n    bordered: PropTypes.bool,\n\n    /**\n     * Set max height\n     */\n    maxHeight: PropTypes.number,\n\n    /**\n     * Set max width\n     */\n    maxWidth: PropTypes.number,\n\n    /**\n     * Size\n     */\n    size: PropTypes.oneOf(['small', 'default', 'large']),\n\n    /**\n     * Config of pagination. You can ref table pagination config or full pagination document, hide it by setting it to false\n     */\n    pagination: PropTypes.oneOfType([\n        PropTypes.exact({\n            position: PropTypes.oneOf([\n                'topLeft',\n                'topCenter',\n                'topRight',\n                'bottomLeft',\n                'bottomCenter',\n                'bottomRight',\n            ]),\n            pageSize: PropTypes.number,\n            current: PropTypes.number,\n            showSizeChanger: PropTypes.bool,\n            pageSizeOptions: PropTypes.arrayOf(PropTypes.number),\n            showTotal: PropTypes.bool,\n            showQuickJumper: PropTypes.bool,\n            showTotalPrefix: PropTypes.string,\n            showTotalSuffix: PropTypes.string,\n            hideOnSinglePage: PropTypes.bool,\n            simple: PropTypes.bool,\n            disabled: PropTypes.bool,\n            size: PropTypes.oneOf(['default', 'small']),\n            total: PropTypes.number,\n        }),\n        PropTypes.bool,\n        PropTypes.object,\n    ]),\n\n    /**\n     * Whether to allow cell content rendering\n     */\n    cellUpdateOptimize: PropTypes.bool,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func,\n};\n\nAnyaTable.defaultProps = {\n    size: 'small',\n    cellUpdateOptimize: true,\n    pagination: {\n        defaultPageSize: 20,\n        hideOnSinglePage: true,\n        showSizeChanger: false\n    },\n};\n\nexport default AnyaTable;\n",
         "// This icon file is generated automatically.\nvar CheckCircleFilled = { \"icon\": { \"tag\": \"svg\", \"attrs\": { \"viewBox\": \"64 64 896 896\", \"focusable\": \"false\" }, \"children\": [{ \"tag\": \"path\", \"attrs\": { \"d\": \"M512 64C264.6 64 64 264.6 64 512s200.6 448 448 448 448-200.6 448-448S759.4 64 512 64zm193.5 301.7l-210.6 292a31.8 31.8 0 01-51.7 0L318.5 484.9c-3.8-5.3 0-12.7 6.5-12.7h46.9c10.2 0 19.9 4.9 25.9 13.3l71.2 98.8 157.2-218c6-8.3 15.6-13.3 25.9-13.3H699c6.5 0 10.3 7.4 6.5 12.7z\" } }] }, \"name\": \"check-circle\", \"theme\": \"filled\" };\nexport default CheckCircleFilled;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\n// GENERATE BY ./scripts/generate.ts\n// DON NOT EDIT IT MANUALLY\n\nimport * as React from 'react';\nimport CheckCircleFilledSvg from \"@ant-design/icons-svg/es/asn/CheckCircleFilled\";\nimport AntdIcon from \"../components/AntdIcon\";\nvar CheckCircleFilled = function CheckCircleFilled(props, ref) {\n  return /*#__PURE__*/React.createElement(AntdIcon, _extends({}, props, {\n    ref: ref,\n    icon: CheckCircleFilledSvg\n  }));\n};\nif (process.env.NODE_ENV !== 'production') {\n  CheckCircleFilled.displayName = 'CheckCircleFilled';\n}\nexport default /*#__PURE__*/React.forwardRef(CheckCircleFilled);",
         "// This icon file is generated automatically.\nvar ExclamationCircleFilled = { \"icon\": { \"tag\": \"svg\", \"attrs\": { \"viewBox\": \"64 64 896 896\", \"focusable\": \"false\" }, \"children\": [{ \"tag\": \"path\", \"attrs\": { \"d\": \"M512 64C264.6 64 64 264.6 64 512s200.6 448 448 448 448-200.6 448-448S759.4 64 512 64zm-32 232c0-4.4 3.6-8 8-8h48c4.4 0 8 3.6 8 8v272c0 4.4-3.6 8-8 8h-48c-4.4 0-8-3.6-8-8V296zm32 440a48.01 48.01 0 010-96 48.01 48.01 0 010 96z\" } }] }, \"name\": \"exclamation-circle\", \"theme\": \"filled\" };\nexport default ExclamationCircleFilled;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\n// GENERATE BY ./scripts/generate.ts\n// DON NOT EDIT IT MANUALLY\n\nimport * as React from 'react';\nimport ExclamationCircleFilledSvg from \"@ant-design/icons-svg/es/asn/ExclamationCircleFilled\";\nimport AntdIcon from \"../components/AntdIcon\";\nvar ExclamationCircleFilled = function ExclamationCircleFilled(props, ref) {\n  return /*#__PURE__*/React.createElement(AntdIcon, _extends({}, props, {\n    ref: ref,\n    icon: ExclamationCircleFilledSvg\n  }));\n};\nif (process.env.NODE_ENV !== 'production') {\n  ExclamationCircleFilled.displayName = 'ExclamationCircleFilled';\n}\nexport default /*#__PURE__*/React.forwardRef(ExclamationCircleFilled);",
         "// This icon file is generated automatically.\nvar InfoCircleFilled = { \"icon\": { \"tag\": \"svg\", \"attrs\": { \"viewBox\": \"64 64 896 896\", \"focusable\": \"false\" }, \"children\": [{ \"tag\": \"path\", \"attrs\": { \"d\": \"M512 64C264.6 64 64 264.6 64 512s200.6 448 448 448 448-200.6 448-448S759.4 64 512 64zm32 664c0 4.4-3.6 8-8 8h-48c-4.4 0-8-3.6-8-8V456c0-4.4 3.6-8 8-8h48c4.4 0 8 3.6 8 8v272zm-32-344a48.01 48.01 0 010-96 48.01 48.01 0 010 96z\" } }] }, \"name\": \"info-circle\", \"theme\": \"filled\" };\nexport default InfoCircleFilled;\n",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\n// GENERATE BY ./scripts/generate.ts\n// DON NOT EDIT IT MANUALLY\n\nimport * as React from 'react';\nimport InfoCircleFilledSvg from \"@ant-design/icons-svg/es/asn/InfoCircleFilled\";\nimport AntdIcon from \"../components/AntdIcon\";\nvar InfoCircleFilled = function InfoCircleFilled(props, ref) {\n  return /*#__PURE__*/React.createElement(AntdIcon, _extends({}, props, {\n    ref: ref,\n    icon: InfoCircleFilledSvg\n  }));\n};\nif (process.env.NODE_ENV !== 'production') {\n  InfoCircleFilled.displayName = 'InfoCircleFilled';\n}\nexport default /*#__PURE__*/React.forwardRef(InfoCircleFilled);",
         "import useState from \"rc-util/es/hooks/useState\";\nimport * as React from 'react';\nimport Button from '../button';\nimport { convertLegacyProps } from '../button/button';\nfunction isThenable(thing) {\n  return !!(thing && thing.then);\n}\nconst ActionButton = props => {\n  const {\n    type,\n    children,\n    prefixCls,\n    buttonProps,\n    close,\n    autoFocus,\n    emitEvent,\n    quitOnNullishReturnValue,\n    actionFn\n  } = props;\n  const clickedRef = React.useRef(false);\n  const buttonRef = React.useRef(null);\n  const [loading, setLoading] = useState(false);\n  const onInternalClose = function () {\n    close === null || close === void 0 ? void 0 : close.apply(void 0, arguments);\n  };\n  React.useEffect(() => {\n    let timeoutId = null;\n    if (autoFocus) {\n      timeoutId = setTimeout(() => {\n        var _a;\n        (_a = buttonRef.current) === null || _a === void 0 ? void 0 : _a.focus();\n      });\n    }\n    return () => {\n      if (timeoutId) {\n        clearTimeout(timeoutId);\n      }\n    };\n  }, []);\n  const handlePromiseOnOk = returnValueOfOnOk => {\n    if (!isThenable(returnValueOfOnOk)) {\n      return;\n    }\n    setLoading(true);\n    returnValueOfOnOk.then(function () {\n      setLoading(false, true);\n      onInternalClose.apply(void 0, arguments);\n      clickedRef.current = false;\n    }, e => {\n      // See: https://github.com/ant-design/ant-design/issues/6183\n      setLoading(false, true);\n      clickedRef.current = false;\n      return Promise.reject(e);\n    });\n  };\n  const onClick = e => {\n    if (clickedRef.current) {\n      return;\n    }\n    clickedRef.current = true;\n    if (!actionFn) {\n      onInternalClose();\n      return;\n    }\n    let returnValueOfOnOk;\n    if (emitEvent) {\n      returnValueOfOnOk = actionFn(e);\n      if (quitOnNullishReturnValue && !isThenable(returnValueOfOnOk)) {\n        clickedRef.current = false;\n        onInternalClose(e);\n        return;\n      }\n    } else if (actionFn.length) {\n      returnValueOfOnOk = actionFn(close);\n      // https://github.com/ant-design/ant-design/issues/23358\n      clickedRef.current = false;\n    } else {\n      returnValueOfOnOk = actionFn();\n      if (!returnValueOfOnOk) {\n        onInternalClose();\n        return;\n      }\n    }\n    handlePromiseOnOk(returnValueOfOnOk);\n  };\n  return /*#__PURE__*/React.createElement(Button, Object.assign({}, convertLegacyProps(type), {\n    onClick: onClick,\n    loading: loading,\n    prefixCls: prefixCls\n  }, buttonProps, {\n    ref: buttonRef\n  }), children);\n};\nexport default ActionButton;",
```

### Comparing `anya_dash-0.0.2/anya_dash/metadata.json` & `anya_dash-0.0.3/anya_dash/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999975339330808%*

 * *Differences: {"'src/lib/components/AnyaDataDisplay/AnyaTable.react.js'": "{'props': {'pagination': "*

 * *                                                            "{'defaultValue': {'value': '{\\n    "*

 * *                                                            'defaultPageSize: 20,\\n    '*

 * *                                                            'hideOnSinglePage: true,\\n    '*

 * *                                                            "showSizeChanger: false\\n}'}}}}"}*

```diff
@@ -1263,15 +1263,15 @@
                 "type": {
                     "name": "number"
                 }
             },
             "pagination": {
                 "defaultValue": {
                     "computed": false,
-                    "value": "{\n    defaultPageSize: 20,\n    hideOnSinglePage: true,\n    showSizeChanger: false,\n}"
+                    "value": "{\n    defaultPageSize: 20,\n    hideOnSinglePage: true,\n    showSizeChanger: false\n}"
                 },
                 "description": "Config of pagination. You can ref table pagination config or full pagination document, hide it by setting it to false",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
```

### Comparing `anya_dash-0.0.2/anya_dash/package-info.json` & `anya_dash-0.0.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.3'"}*

```diff
@@ -62,9 +62,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "generateAnalyzFile": "webpack --profile --json > dist/stats.json",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python3 _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.3"
 }
```

### Comparing `anya_dash-0.0.2/anya_dash.egg-info/SOURCES.txt` & `anya_dash-0.0.3/anya_dash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/package.json` & `anya_dash-0.0.3/anya_dash/package-info.json`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/tests/test_cards_tabs_collapse.py` & `anya_dash-0.0.3/tests/test_cards_tabs_collapse.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/tests/test_common.py` & `anya_dash-0.0.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/tests/test_data_entry.py` & `anya_dash-0.0.3/tests/test_data_entry.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/tests/test_layout_collapsible_sider.py` & `anya_dash-0.0.3/tests/test_layout_collapsible_sider.py`

 * *Files identical despite different names*

### Comparing `anya_dash-0.0.2/tests/test_table.py` & `anya_dash-0.0.3/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,20 @@
                 AnyaTable(
                     columns=cols,
                     data=data,
                     pagination={
                         'pageSize': 5,
                         'hideOnSinglePag': True,
                         'showSizeChanger': False,
+                        'showTotal': True
                         # 'position': 'topRight'
                     },
                     size='small',
                     bordered=True,
-                    id='table-1'
+                    id='table-1',
                 ),
                 html.Hr(),
                 AnyaTitle('colSpan & rowSpan', level=4),
                 AnyaTable(
                     columns=cols2,
                     data=data2,
                     pagination=False,
```

### Comparing `anya_dash-0.0.2/tests/test_typography.py` & `anya_dash-0.0.3/tests/test_typography.py`

 * *Files identical despite different names*
