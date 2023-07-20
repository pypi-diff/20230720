# Comparing `tmp/screenpy_selenium-4.0.3.tar.gz` & `tmp/screenpy_selenium-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_selenium-4.0.3.tar", last modified: Sun Sep 18 23:50:31 2022, max compression
+gzip compressed data, was "screenpy_selenium-4.0.4.tar", max compression
```

## Comparing `screenpy_selenium-4.0.3.tar` & `screenpy_selenium-4.0.4.tar`

### file list

```diff
@@ -1,74 +1,59 @@
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.721503 screenpy_selenium-4.0.3/
--rw-r--r--   0 perry      (501) staff       (20)     1066 2022-02-21 21:41:06.000000 screenpy_selenium-4.0.3/LICENSE
--rw-r--r--   0 perry      (501) staff       (20)     2825 2022-09-18 23:50:31.721162 screenpy_selenium-4.0.3/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)     2018 2022-03-14 04:23:17.000000 screenpy_selenium-4.0.3/README.md
--rw-r--r--   0 perry      (501) staff       (20)       40 2022-09-18 23:38:13.000000 screenpy_selenium-4.0.3/pyproject.toml
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.712319 screenpy_selenium-4.0.3/screenpy_selenium/
--rw-r--r--   0 perry      (501) staff       (20)      984 2022-02-23 03:41:34.000000 screenpy_selenium-4.0.3/screenpy_selenium/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)      893 2022-09-18 23:45:56.000000 screenpy_selenium-4.0.3/screenpy_selenium/__version__.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.713310 screenpy_selenium-4.0.3/screenpy_selenium/abilities/
--rw-r--r--   0 perry      (501) staff       (20)      133 2022-02-23 03:33:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/abilities/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     4507 2022-02-22 14:36:06.000000 screenpy_selenium-4.0.3/screenpy_selenium/abilities/browse_the_web.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.717059 screenpy_selenium-4.0.3/screenpy_selenium/actions/
--rw-r--r--   0 perry      (501) staff       (20)     1833 2022-02-23 03:32:46.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)      781 2022-02-22 14:36:57.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/accept_alert.py
--rw-r--r--   0 perry      (501) staff       (20)     1598 2022-08-09 21:22:34.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/chain.py
--rw-r--r--   0 perry      (501) staff       (20)     1428 2022-02-23 03:32:02.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/clear.py
--rw-r--r--   0 perry      (501) staff       (20)     2192 2022-02-23 03:32:02.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/click.py
--rw-r--r--   0 perry      (501) staff       (20)      795 2022-02-22 14:39:27.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/dismiss_alert.py
--rw-r--r--   0 perry      (501) staff       (20)     2088 2022-02-23 03:32:02.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/double_click.py
--rw-r--r--   0 perry      (501) staff       (20)     3799 2022-09-06 17:44:39.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/enter.py
--rw-r--r--   0 perry      (501) staff       (20)     1792 2022-02-23 03:32:02.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/enter_2fa_token.py
--rw-r--r--   0 perry      (501) staff       (20)      690 2022-02-22 14:44:04.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/go_back.py
--rw-r--r--   0 perry      (501) staff       (20)      714 2022-02-22 14:44:13.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/go_forward.py
--rw-r--r--   0 perry      (501) staff       (20)     2645 2022-02-23 03:32:02.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/hold_down.py
--rw-r--r--   0 perry      (501) staff       (20)     3686 2022-02-22 14:45:46.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/move_mouse.py
--rw-r--r--   0 perry      (501) staff       (20)     1778 2022-02-22 14:46:45.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/open.py
--rw-r--r--   0 perry      (501) staff       (20)     1201 2022-02-22 14:47:33.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/pause.py
--rw-r--r--   0 perry      (501) staff       (20)      688 2022-02-22 14:47:47.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/refresh_page.py
--rw-r--r--   0 perry      (501) staff       (20)     2257 2022-03-06 08:34:55.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/release.py
--rw-r--r--   0 perry      (501) staff       (20)     1234 2022-02-22 14:52:21.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/respond_to_the_prompt.py
--rw-r--r--   0 perry      (501) staff       (20)     2363 2022-02-22 14:52:31.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/right_click.py
--rw-r--r--   0 perry      (501) staff       (20)     2821 2022-08-09 21:22:34.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/save_console_log.py
--rw-r--r--   0 perry      (501) staff       (20)     2524 2022-08-09 21:22:34.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/save_screenshot.py
--rw-r--r--   0 perry      (501) staff       (20)     6887 2022-02-22 14:57:20.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/select.py
--rw-r--r--   0 perry      (501) staff       (20)     1603 2022-02-22 15:00:00.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/switch_to.py
--rw-r--r--   0 perry      (501) staff       (20)      864 2022-02-22 14:57:33.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/switch_to_tab.py
--rw-r--r--   0 perry      (501) staff       (20)     4849 2022-02-22 15:00:06.000000 screenpy_selenium-4.0.3/screenpy_selenium/actions/wait.py
--rw-r--r--   0 perry      (501) staff       (20)      298 2022-02-23 03:35:07.000000 screenpy_selenium-4.0.3/screenpy_selenium/exceptions.py
--rw-r--r--   0 perry      (501) staff       (20)      635 2022-09-18 23:42:54.000000 screenpy_selenium-4.0.3/screenpy_selenium/protocols.py
--rw-r--r--   0 perry      (501) staff       (20)       39 2022-02-22 22:18:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/py.typed
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.718584 screenpy_selenium-4.0.3/screenpy_selenium/questions/
--rw-r--r--   0 perry      (501) staff       (20)     1036 2022-02-23 03:35:36.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     2106 2022-02-22 15:01:53.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/attribute.py
--rw-r--r--   0 perry      (501) staff       (20)      820 2022-02-22 15:03:51.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/browser_title.py
--rw-r--r--   0 perry      (501) staff       (20)      802 2022-02-22 15:03:55.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/browser_url.py
--rw-r--r--   0 perry      (501) staff       (20)      910 2022-02-22 15:03:58.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/cookies.py
--rw-r--r--   0 perry      (501) staff       (20)     1108 2022-08-09 21:22:34.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/element.py
--rw-r--r--   0 perry      (501) staff       (20)     1045 2022-02-22 15:04:04.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/list.py
--rw-r--r--   0 perry      (501) staff       (20)      964 2022-02-22 15:04:07.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/number.py
--rw-r--r--   0 perry      (501) staff       (20)     2260 2022-02-22 15:03:46.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/selected.py
--rw-r--r--   0 perry      (501) staff       (20)     1560 2022-02-22 15:04:28.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/text.py
--rw-r--r--   0 perry      (501) staff       (20)      817 2022-02-22 15:04:17.000000 screenpy_selenium-4.0.3/screenpy_selenium/questions/text_of_the_alert.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.719321 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/
--rw-r--r--   0 perry      (501) staff       (20)      742 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/__init__.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.720811 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/
--rw-r--r--   0 perry      (501) staff       (20)      416 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)     1506 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_clickable_element.py
--rw-r--r--   0 perry      (501) staff       (20)     1452 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_invisible_element.py
--rw-r--r--   0 perry      (501) staff       (20)     1300 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_present_element.py
--rw-r--r--   0 perry      (501) staff       (20)     1421 2022-05-01 16:48:03.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_visible_element.py
--rw-r--r--   0 perry      (501) staff       (20)      600 2022-05-13 16:42:48.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_clickable.py
--rw-r--r--   0 perry      (501) staff       (20)      612 2022-05-13 16:42:48.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_invisible.py
--rw-r--r--   0 perry      (501) staff       (20)      720 2022-05-13 16:42:48.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_present.py
--rw-r--r--   0 perry      (501) staff       (20)      590 2022-05-13 16:42:48.000000 screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_visible.py
--rw-r--r--   0 perry      (501) staff       (20)      269 2022-03-06 08:34:55.000000 screenpy_selenium-4.0.3/screenpy_selenium/speech_tools.py
--rw-r--r--   0 perry      (501) staff       (20)     4259 2022-09-18 23:46:28.000000 screenpy_selenium-4.0.3/screenpy_selenium/target.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2022-09-18 23:50:31.713055 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/
--rw-r--r--   0 perry      (501) staff       (20)     2825 2022-09-18 23:50:31.000000 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)     2537 2022-09-18 23:50:31.000000 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 perry      (501) staff       (20)        1 2022-09-18 23:50:31.000000 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 perry      (501) staff       (20)       94 2022-09-18 23:50:31.000000 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/requires.txt
--rw-r--r--   0 perry      (501) staff       (20)       18 2022-09-18 23:50:31.000000 screenpy_selenium-4.0.3/screenpy_selenium.egg-info/top_level.txt
--rw-r--r--   0 perry      (501) staff       (20)       38 2022-09-18 23:50:31.721775 screenpy_selenium-4.0.3/setup.cfg
--rw-r--r--   0 perry      (501) staff       (20)     1325 2022-09-18 23:43:07.000000 screenpy_selenium-4.0.3/setup.py
+-rw-r--r--   0        0        0     1071 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/LICENSE
+-rw-r--r--   0        0        0     2854 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/README.md
+-rw-r--r--   0        0        0     2918 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1455 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/__version__.py
+-rw-r--r--   0        0        0      133 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/abilities/__init__.py
+-rw-r--r--   0        0        0     4853 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/abilities/browse_the_web.py
+-rw-r--r--   0        0        0     3366 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/__init__.py
+-rw-r--r--   0        0        0      781 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/accept_alert.py
+-rw-r--r--   0        0        0     1598 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/chain.py
+-rw-r--r--   0        0        0     2175 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/clear.py
+-rw-r--r--   0        0        0     2877 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/click.py
+-rw-r--r--   0        0        0      795 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/dismiss_alert.py
+-rw-r--r--   0        0        0     2899 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/double_click.py
+-rw-r--r--   0        0        0     5479 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/enter.py
+-rw-r--r--   0        0        0     2296 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/enter_2fa_token.py
+-rw-r--r--   0        0        0      690 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/go_back.py
+-rw-r--r--   0        0        0      714 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/go_forward.py
+-rw-r--r--   0        0        0     2893 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/hold_down.py
+-rw-r--r--   0        0        0     5122 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/move_mouse.py
+-rw-r--r--   0        0        0     2203 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/open.py
+-rw-r--r--   0        0        0     1199 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/pause.py
+-rw-r--r--   0        0        0      688 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/refresh_page.py
+-rw-r--r--   0        0        0     2499 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/release.py
+-rw-r--r--   0        0        0     1448 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/respond_to_the_prompt.py
+-rw-r--r--   0        0        0     3151 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/right_click.py
+-rw-r--r--   0        0        0     3235 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/save_console_log.py
+-rw-r--r--   0        0        0     2938 2023-07-20 14:43:26.026200 screenpy_selenium-4.0.4/screenpy_selenium/actions/save_screenshot.py
+-rw-r--r--   0        0        0     7438 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/actions/select.py
+-rw-r--r--   0        0        0     1812 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/actions/switch_to.py
+-rw-r--r--   0        0        0      864 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/actions/switch_to_tab.py
+-rw-r--r--   0        0        0     5397 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/actions/wait.py
+-rw-r--r--   0        0        0      298 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/exceptions.py
+-rw-r--r--   0        0        0      635 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/protocols.py
+-rw-r--r--   0        0        0       39 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/py.typed
+-rw-r--r--   0        0        0     1036 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/__init__.py
+-rw-r--r--   0        0        0     2106 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/attribute.py
+-rw-r--r--   0        0        0      820 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/browser_title.py
+-rw-r--r--   0        0        0      802 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/browser_url.py
+-rw-r--r--   0        0        0      910 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/cookies.py
+-rw-r--r--   0        0        0     1108 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/element.py
+-rw-r--r--   0        0        0     1938 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/list.py
+-rw-r--r--   0        0        0     1107 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/number.py
+-rw-r--r--   0        0        0     3099 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/selected.py
+-rw-r--r--   0        0        0     2247 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/text.py
+-rw-r--r--   0        0        0      817 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/questions/text_of_the_alert.py
+-rw-r--r--   0        0        0      743 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/__init__.py
+-rw-r--r--   0        0        0      416 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     1506 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_clickable_element.py
+-rw-r--r--   0        0        0     1338 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_invisible_element.py
+-rw-r--r--   0        0        0     1300 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_present_element.py
+-rw-r--r--   0        0        0     1421 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_visible_element.py
+-rw-r--r--   0        0        0      600 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_clickable.py
+-rw-r--r--   0        0        0      612 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_invisible.py
+-rw-r--r--   0        0        0      720 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_present.py
+-rw-r--r--   0        0        0      590 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_visible.py
+-rw-r--r--   0        0        0      269 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/speech_tools.py
+-rw-r--r--   0        0        0     4675 2023-07-20 14:43:26.030200 screenpy_selenium-4.0.4/screenpy_selenium/target.py
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 screenpy_selenium-4.0.4/PKG-INFO
```

### Comparing `screenpy_selenium-4.0.3/LICENSE` & `screenpy_selenium-4.0.4/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Perry Goy
+Copyright (c) 2022-2023 Perry Goy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `screenpy_selenium-4.0.3/PKG-INFO` & `screenpy_selenium-4.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-Metadata-Version: 2.1
-Name: screenpy_selenium
-Version: 4.0.3
-Summary: ScreenPy extension to enable interacting with Selenium.
-Home-page: https://github.com/ScreenPyHQ/screenpy_selenium
-Author: Perry Goy
-Author-email: perry.goy@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: BDD
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ScreenPy Selenium
 =================
 
+[![Build Status](../../actions/workflows/tests.yml/badge.svg)](../../actions/workflows/tests.yml)
+[![Build Status](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)
+
+[![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy-selenium.svg)](https://pypi.org/project/screenpy)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 ```
 TITLE CARD:
                                "ScreenPy Selenium"
 TITLE DISAPPEARS.
                                                                       FADE IN:
 EXT. DOCUMENTATION - AFTERNOON, CLOUDY
 
@@ -75,14 +62,17 @@
 You can also read the [ScreenPy Docs](https://screenpy-docs.readthedocs.io/en/latest/) for more information about ScreenPy in general.
 
 
 Contributing
 ------------
 You want to contribute? Great! Here are the things you should do before submitting your PR:
 
-1. Install [`pre-commit`](https://pre-commit.com/)
-1. run `pre-commit install` once.
-1. run `tox` to perform tests frequently.
+1. Fork the repo and git clone your fork.
+1. `dev` install the project package:
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
+1. Run `pre-commit install` once.
+1. Run `tox` to perform tests frequently.
+1. Create pull-request from your branch.
 
 That's it! :)
-
-
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/abilities/browse_the_web.py` & `screenpy_selenium-4.0.4/screenpy_selenium/abilities/browse_the_web.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 """
 Enable the actor to browse the web.
 """
 
 import os
+from typing import Type, TypeVar
 
 from selenium.webdriver import Chrome, Firefox, Remote, Safari
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from ..exceptions import BrowsingError
 
 DEFAULT_APPIUM_HUB_URL = "http://localhost:4723/wd/hub"
 
 
+SelfBrowseTheWeb = TypeVar("SelfBrowseTheWeb", bound="BrowseTheWeb")
+
+
 class BrowseTheWeb:
     """Use Selenium to enable browsing the web with a web browser.
 
     Examples::
 
         Perry = AnActor.named("Perry").who_can(
             BrowseTheWeb.using_firefox()
         )
 
         Perry = AnActor.named("Perry").who_can(
             BrowseTheWeb.using(driver)
         )
     """
 
-    @staticmethod
-    def using_chrome() -> "BrowseTheWeb":
+    browser: WebDriver
+
+    @classmethod
+    def using_chrome(cls: Type[SelfBrowseTheWeb]) -> SelfBrowseTheWeb:
         """Create and use a default Chrome Selenium webdriver instance."""
-        return BrowseTheWeb.using(Chrome())
+        return cls.using(browser=Chrome())
 
-    @staticmethod
-    def using_firefox() -> "BrowseTheWeb":
+    @classmethod
+    def using_firefox(cls: Type[SelfBrowseTheWeb]) -> SelfBrowseTheWeb:
         """Create and use a default Firefox Selenium webdriver instance."""
-        return BrowseTheWeb.using(Firefox())
+        return cls.using(browser=Firefox())
 
-    @staticmethod
-    def using_safari() -> "BrowseTheWeb":
+    @classmethod
+    def using_safari(cls: Type[SelfBrowseTheWeb]) -> SelfBrowseTheWeb:
         """Create and use a default Safari Selenium webdriver instance."""
-        return BrowseTheWeb.using(Safari())
+        return cls.using(browser=Safari())
 
-    @staticmethod
-    def using_ios() -> "BrowseTheWeb":
+    @classmethod
+    def using_ios(cls: Type[SelfBrowseTheWeb]) -> SelfBrowseTheWeb:
         """
         Create and use a default Remote driver instance to connect to a
         running Appium server and open Safari on iOS.
 
         Note that Appium requires non-trivial setup to be able to connect
         to iPhone simulators. See the Appium documentation to get started:
         http://appium.io/docs/en/writing-running-appium/running-tests/
@@ -66,18 +72,18 @@
             "deviceName": os.getenv("IOS_DEVICE_NAME", "iPhone Simulator"),
             "automationName": "xcuitest",
             "browserName": "Safari",
         }
         if IOS_CAPABILITIES["platformVersion"] is None:
             raise BrowsingError("IOS_DEVICE_VERSION Environment variable must be set.")
 
-        return BrowseTheWeb.using(Remote(hub_url, IOS_CAPABILITIES))
+        return cls.using(browser=Remote(hub_url, IOS_CAPABILITIES))
 
-    @staticmethod
-    def using_android() -> "BrowseTheWeb":
+    @classmethod
+    def using_android(cls: Type[SelfBrowseTheWeb]) -> SelfBrowseTheWeb:
         """
         Create and use a default Remote driver instance to connect to a
         running Appium server and open Chrome on Android.
 
         Note that Appium requires non-trivial setup to be able to connect
         to Android emulators. See the Appium documentation to get started:
         http://appium.io/docs/en/writing-running-appium/running-tests/
@@ -99,25 +105,25 @@
             "browserName": "Chrome",
         }
         if ANDROID_CAPABILITIES["platformVersion"] is None:
             raise BrowsingError(
                 "ANDROID_DEVICE_VERSION environment variable must be set."
             )
 
-        return BrowseTheWeb.using(Remote(hub_url, ANDROID_CAPABILITIES))
+        return cls.using(browser=Remote(hub_url, ANDROID_CAPABILITIES))
 
-    @staticmethod
-    def using(browser: WebDriver) -> "BrowseTheWeb":
+    @classmethod
+    def using(cls: Type[SelfBrowseTheWeb], browser: WebDriver) -> SelfBrowseTheWeb:
         """Provide an already-set-up WebDriver to use to browse the web."""
-        return BrowseTheWeb(browser)
+        return cls(browser=browser)
 
-    def forget(self) -> None:
+    def forget(self: SelfBrowseTheWeb) -> None:
         """Quit the attached browser."""
         self.browser.quit()
 
-    def __repr__(self) -> str:
+    def __repr__(self: SelfBrowseTheWeb) -> str:
         return "Browse the Web"
 
     __str__ = __repr__
 
-    def __init__(self, browser: WebDriver) -> None:
+    def __init__(self: SelfBrowseTheWeb, browser: WebDriver) -> None:
         self.browser = browser
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/accept_alert.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/accept_alert.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/chain.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/chain.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/clear.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/clear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 """
 Clear text from an input.
 """
+from typing import Type, TypeVar
 
 from screenpy.actor import Actor
 from screenpy.exceptions import DeliveryError
 from screenpy.pacing import beat
 from selenium.common.exceptions import WebDriverException
 
 from ..target import Target
 
+SelfClear = TypeVar("SelfClear", bound="Clear")
+
 
 class Clear:
     """Clear the text from an input field.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
     Examples::
 
         the_actor.attempts_to(Clear.the_text_from_the(NAME_INPUT))
     """
 
-    @staticmethod
-    def the_text_from_the(target: Target) -> "Clear":
-        """Specify the Target from which to clear the text."""
-        return Clear(target)
-
-    the_text_from = the_text_from_the_first_of_the = the_text_from_the
+    @classmethod
+    def the_text_from_the(cls: Type[SelfClear], target: Target) -> SelfClear:
+        """
+        Specify the Target from which to clear the text.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Clear.the_text_from`
+            * :meth:`~screenpy_selenium.actions.Clear.the_text_from_the_first_of_the`
+        """
+        return cls(target=target)
+
+    @classmethod
+    def the_text_from(cls: Type[SelfClear], target: Target) -> SelfClear:
+        """Alias for :meth:`~screenpy_selenium.actions.Clear.the_text_from_the`"""
+        return cls.the_text_from_the(target=target)
+
+    @classmethod
+    def the_text_from_the_first_of_the(
+        cls: Type[SelfClear], target: Target
+    ) -> SelfClear:
+        """Alias for :meth:`~screenpy_selenium.actions.Clear.the_text_from_the`"""
+        return cls.the_text_from_the(target=target)
 
-    def describe(self) -> str:
+    def describe(self: SelfClear) -> str:
         """Describe the Action in present tense."""
         return f"Clear the text from the {self.target}."
 
     @beat("{} clears text from the {target}.")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfClear, the_actor: Actor) -> None:
         """Direct the Actor to clear the text from the input field."""
         element = self.target.found_by(the_actor)
 
         try:
             element.clear()
         except WebDriverException as e:
             msg = (
                 "Encountered an issue while attempting to clear "
                 f"{self.target}: {e.__class__.__name__}"
             )
             raise DeliveryError(msg) from e
 
-    def __init__(self, target: Target) -> None:
+    def __init__(self: SelfClear, target: Target) -> None:
         self.target = target
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/dismiss_alert.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/dismiss_alert.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/double_click.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/double_click.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Double-click on an element, or wherever the cursor currently is.
 """
 
-from typing import Optional
+from typing import Optional, Type, TypeVar
 
 from screenpy.actor import Actor
 from screenpy.pacing import beat
 from selenium.webdriver.common.action_chains import ActionChains
 
 from ..abilities import BrowseTheWeb
 from ..target import Target
 
+SelfDoubleClick = TypeVar("SelfDoubleClick", bound="DoubleClick")
+
 
 class DoubleClick:
     """Double-click on an element, or wherever the cursor currently is.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -23,43 +25,63 @@
         the_actor.attempts_to(DoubleClick.on_the(FILE_ICON))
 
         the_actor.attempts_to(Chain(DoubleClick()))
     """
 
     target: Optional[Target]
 
-    @staticmethod
-    def on_the(target: Target) -> "DoubleClick":
-        """Target the element to double-click on."""
-        return DoubleClick(target=target)
-
-    on = on_the_first_of_the = on_the
-
-    def _add_action_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @classmethod
+    def on_the(cls: Type[SelfDoubleClick], target: Target) -> SelfDoubleClick:
+        """
+        Target the element to double-click on.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.DoubleClick.on`
+            * :meth:`~screenpy_selenium.actions.DoubleClick.on_the_first_of_the`
+        """
+        return cls(target=target)
+
+    @classmethod
+    def on(cls: Type[SelfDoubleClick], target: Target) -> SelfDoubleClick:
+        """Alias for :meth:`~screenpy_selenium.actions.DoubleClick.on_the`"""
+        return cls.on_the(target=target)
+
+    @classmethod
+    def on_the_first_of_the(
+        cls: Type[SelfDoubleClick], target: Target
+    ) -> SelfDoubleClick:
+        """Alias for :meth:`~screenpy_selenium.actions.DoubleClick.on_the`"""
+        return cls.on_the(target=target)
+
+    def _add_action_to_chain(
+        self: SelfDoubleClick, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Private method to add this Action to the chain."""
         if self.target is not None:
             the_element = self.target.found_by(the_actor)
         else:
             the_element = None
 
         the_chain.double_click(on_element=the_element)
 
-    def describe(self) -> str:
+    def describe(self: SelfDoubleClick) -> str:
         """Describe the Action in present tense."""
         return f"Double-click{self.description}."
 
     @beat("{} double-clicks{description}.")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfDoubleClick, the_actor: Actor) -> None:
         """Direct the Actor to double-click on the element."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         the_chain = ActionChains(browser)
         self._add_action_to_chain(the_actor, the_chain)
         the_chain.perform()
 
-    @beat("  Double-click{description}!")
-    def add_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @beat("Double-click{description}!")
+    def add_to_chain(
+        self: SelfDoubleClick, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Add the DoubleClick Action to a Chain of Actions."""
         self._add_action_to_chain(the_actor, the_chain)
 
-    def __init__(self, target: Optional[Target] = None) -> None:
+    def __init__(self: SelfDoubleClick, target: Optional[Target] = None) -> None:
         self.target = target
         self.description = f" on the {target}" if target is not None else ""
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/enter_2fa_token.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/enter_2fa_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 """
 Enter a 2-factor authentication code into a text field.
 """
+from typing import Type, TypeVar
 
 from screenpy.actor import Actor
 from screenpy.pacing import beat
 from screenpy_pyotp.abilities import AuthenticateWith2FA
 from selenium.webdriver.common.action_chains import ActionChains
 
 from ..target import Target
 from .enter import Enter
 
+SelfEnter2FAToken = TypeVar("SelfEnter2FAToken", bound="Enter2FAToken")
+
 
 class Enter2FAToken:
     """Enter the current two-factor authentication token into an input field.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
         :external+screenpy_pyotp:class:`~screenpy_pyotp.abilities.AuthenticateWith2FA`
 
     Examples::
 
         the_actor.attempts_to(Enter2FAToken.into_the(2FA_INPUT_FIELD))
     """
 
-    @staticmethod
-    def into_the(target: Target) -> "Enter2FAToken":
-        """Target the element into which to enter the 2FA token."""
-        return Enter2FAToken(target)
-
-    into = into_the
+    @classmethod
+    def into_the(cls: Type[SelfEnter2FAToken], target: Target) -> SelfEnter2FAToken:
+        """
+        Target the element into which to enter the 2FA token.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Enter2FAToken.into`
+        """
+        return cls(target)
+
+    @classmethod
+    def into(cls: Type[SelfEnter2FAToken], target: Target) -> SelfEnter2FAToken:
+        """Alias for :meth:`~screenpy_selenium.actions.Enter2FAToken.into_the`."""
+        return cls.into_the(target=target)
 
     def describe(self) -> str:
         """Describe the Action in present tense."""
         return f"Enter a 2FA token into the {self.target}."
 
     @beat("{} enters their 2FA token into the {target}.")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfEnter2FAToken, the_actor: Actor) -> None:
         """Direct the Actor to enter their 2FA token into the element."""
         token = the_actor.uses_ability_to(AuthenticateWith2FA).to_get_token()
         the_actor.attempts_to(Enter.the_text(token).into_the(self.target))
 
-    @beat("  Enter their 2FA token into the {target}!")
-    def add_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @beat("Enter their 2FA token into the {target}!")
+    def add_to_chain(
+        self: SelfEnter2FAToken, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Add the Enter2FAToken Action to a Chain of Actions."""
         token = the_actor.uses_ability_to(AuthenticateWith2FA).to_get_token()
         the_chain.send_keys_to_element(self.target.found_by(the_actor), token)
 
-    def __init__(self, target: Target) -> None:
+    def __init__(self: SelfEnter2FAToken, target: Target) -> None:
         self.target = target
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/go_back.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/go_back.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/go_forward.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/go_forward.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/hold_down.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/hold_down.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Hold down a specific key or the left mouse button, optionally on an element.
 """
 
 import platform
-from typing import Optional
+from typing import Optional, Type, TypeVar
 
 from screenpy import Actor
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import beat
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 
 from ..speech_tools import KEY_NAMES
 from ..target import Target
 
+SelfHoldDown = TypeVar("SelfHoldDown", bound="HoldDown")
+
 
 class HoldDown:
     """Hold down the specified key or left mouse button.
 
     This Action can only be used with :class:`~screenpy_selenium.actions.Chain`,
     and it is expected that a :class:`~screenpy_selenium.actions.Release` Action
     occurs later in the Chain to release the held key or button.
@@ -33,50 +35,57 @@
 
         the_actor.attempts_to(
             Chain(HoldDown.left_mouse_button().on_the(DRAGGABLE_BOX))
         )
     """
 
     target: Optional[Target]
+    key: Optional[str]
+    lmb: bool
+    description: str
 
-    @staticmethod
-    def command_or_control_key() -> "HoldDown":
+    @classmethod
+    def command_or_control_key(cls: Type[SelfHoldDown]) -> SelfHoldDown:
         """
         A convenience method that figures out what operating system the Actor
         is using and directs the Actor which execution key to hold down.
         """
         if platform.system() == "Darwin":
-            return HoldDown(Keys.COMMAND)
-        return HoldDown(Keys.CONTROL)
+            return cls(Keys.COMMAND)
+        return cls(Keys.CONTROL)
 
-    @staticmethod
-    def left_mouse_button() -> "HoldDown":
+    @classmethod
+    def left_mouse_button(cls: Type[SelfHoldDown]) -> SelfHoldDown:
         """Hold down the left mouse button."""
-        return HoldDown(lmb=True)
+        return cls(lmb=True)
 
-    def on_the(self, target: Target) -> "HoldDown":
+    def on_the(self: SelfHoldDown, target: Target) -> SelfHoldDown:
         """Target an element to hold down left click on."""
         self.target = target
         return self
 
     on = on_the
 
-    def describe(self) -> str:
+    def describe(self: SelfHoldDown) -> str:
         """Describe the Action in present tense."""
         return f"Hold down {self.description}."
 
-    @beat("  Hold down {description}!")
-    def add_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @beat("Hold down {description}!")
+    def add_to_chain(
+        self: SelfHoldDown, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Add the HoldDown Action to a Chain of Actions."""
         if self.lmb:
             element = self.target.found_by(the_actor) if self.target else None
             the_chain.click_and_hold(on_element=element)
         elif self.key is not None:
             the_chain.key_down(self.key)
         else:
             raise UnableToAct("HoldDown must be told what to hold down.")
 
-    def __init__(self, key: Optional[str] = None, lmb: bool = False) -> None:
+    def __init__(
+        self: SelfHoldDown, key: Optional[str] = None, lmb: bool = False
+    ) -> None:
         self.key = key
         self.lmb = lmb
         self.target = None
         self.description = "LEFT MOUSE BUTTON" if lmb else KEY_NAMES[key]
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/open.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/open.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Open a browser on a URL.
 """
 
 import os
-from typing import Union
+from typing import Type, TypeVar, Union
 
 from screenpy import Actor
 from screenpy.pacing import beat
 
 from ..abilities import BrowseTheWeb
 
+SelfOpen = TypeVar("SelfOpen", bound="Open")
+
 
 class Open:
     """Go to a specific URL!
 
     This Action supports using the BASE_URL environment variable to
     set a base URL. If you set BASE_URL, the url passed in to this
     Action will be appended to the end of it. For example, if you
@@ -33,28 +35,36 @@
         # using environment variable BASE_URL
         the_actor.attempts_to(Open.their_browser_on("/login"))
 
         # using a page object with HomepageObject.url
         the_actor.attempts_to(Open.browser_on(HomepageObject))
     """
 
-    @staticmethod
-    def their_browser_on(location: Union[str, object]) -> "Open":
-        """Provide a URL to visit."""
-        return Open(location)
-
-    browser_on = their_browser_on
+    @classmethod
+    def their_browser_on(cls: Type[SelfOpen], location: Union[str, object]) -> SelfOpen:
+        """
+        Provide a URL to visit.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Open.browser_on`
+        """
+        return cls(location=location)
+
+    @classmethod
+    def browser_on(cls: Type[SelfOpen], location: Union[str, object]) -> SelfOpen:
+        """Alias for :meth:`~screenpy_selenium.actions.Open.their_browser_on`."""
+        return cls.their_browser_on(location=location)
 
-    def describe(self) -> str:
+    def describe(self: SelfOpen) -> str:
         """Describe the Action in present tense."""
         return f"Visit {self.url}."
 
     @beat("{} visits {url}")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfOpen, the_actor: Actor) -> None:
         """Direct the Actor to visit the specified URL."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         browser.get(self.url)
 
-    def __init__(self, location: Union[str, object]) -> None:
+    def __init__(self: SelfOpen, location: Union[str, object]) -> None:
         url = getattr(location, "url", location)
         url = f'{os.getenv("BASE_URL", "")}{url}'
         self.url = url
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/pause.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/pause.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,11 +30,11 @@
                     "the fancy menu slide-in animation needs to finish."
                 ),
                 Click.on_the(SUBMENU_OPTION),
             )
         )
     """
 
-    @beat("  Pause for {number} {unit} ({reason})!")
+    @beat("Pause for {number} {unit} ({reason})!")
     def add_to_chain(self, _: Actor, the_chain: ActionChains) -> None:
         """Add the Pause Action to a Chain of Actions."""
         the_chain.pause(self.time)
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/refresh_page.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/refresh_page.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/release.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/release.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Release the left mouse button or a held modifier key.
 """
 
 import platform
-from typing import Optional
+from typing import Optional, Type, TypeVar
 
 from screenpy import Actor
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import beat
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 
 from ..speech_tools import KEY_NAMES
 
+SelfRelease = TypeVar("SelfRelease", bound="Release")
+
 
 class Release:
     """Release the specified key or left mouse button.
 
     This Action can only be used with :class:`~screenpy_selenium.actions.Chain`,
     and it expects that a corresponding :class:`~screenpy_selenium.actions.HoldDown`
     Action was called earlier in the Chain.
@@ -29,42 +31,49 @@
         the_actor.attempts_to(Release.left_mouse_button())
 
         the_actor.attempts_to(Release(Keys.SHIFT))
 
         the_actor.attempts_to(Release.command_or_control_key())
     """
 
-    @staticmethod
-    def command_or_control_key() -> "Release":
+    key: Optional[str]
+    lmb: bool
+    description: str
+    the_kraken: str
+
+    @classmethod
+    def command_or_control_key(cls: Type[SelfRelease]) -> SelfRelease:
         """
         A convenience method that figures out what operating system the Actor
         is using and tells the Actor which execution key to release.
         """
         if platform.system() == "Darwin":
-            return Release(Keys.COMMAND)
-        return Release(Keys.CONTROL)
+            return cls(key=Keys.COMMAND)
+        return cls(key=Keys.CONTROL)
 
-    @staticmethod
-    def left_mouse_button() -> "Release":
+    @classmethod
+    def left_mouse_button(cls: Type[SelfRelease]) -> SelfRelease:
         """Release the left mouse button."""
-        return Release(lmb=True)
+        return cls(lmb=True)
 
-    def describe(self) -> str:
+    def describe(self: SelfRelease) -> str:
         """Describe the Action in present tense."""
         # darn, it doesn't work quite as well here. :P
         return f"Release {self.the_kraken}."
 
-    @beat("  Release {the_kraken}!")
-    def add_to_chain(self, _: Actor, the_chain: ActionChains) -> None:
+    @beat("Release {the_kraken}!")
+    def add_to_chain(self: SelfRelease, _: Actor, the_chain: ActionChains) -> None:
         """Add the Release Action to a Chain of Actions."""
         if self.lmb:
             the_chain.release()
         elif self.key is not None:
             the_chain.key_up(self.key)
         else:
             raise UnableToAct("Release must be told what to release.")
 
-    def __init__(self, key: Optional[str] = None, lmb: bool = False) -> None:
+    def __init__(
+        self: SelfRelease, key: Optional[str] = None, lmb: bool = False
+    ) -> None:
         self.key = key
         self.lmb = lmb
         self.description = "LEFT MOUSE BUTTON" if lmb else KEY_NAMES[key]
         self.the_kraken = self.description  # i can't help myself
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/respond_to_the_prompt.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/switch_to.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 """
-Respond to a prompt.
+Switch the driver's frame of reference.
 """
 
+from typing import Optional, Type, TypeVar
+
 from screenpy.actor import Actor
-from screenpy.pacing import aside, beat
+from screenpy.pacing import beat
 
 from ..abilities import BrowseTheWeb
+from ..target import Target
+
+SelfSwitchTo = TypeVar("SelfSwitchTo", bound="SwitchTo")
 
 
-class RespondToThePrompt:
-    """Enter text into and accept a javascript prompt.
+class SwitchTo:
+    """Switch to an element, most likely an iframe, or back to default.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
     Examples::
 
-        the_actor.attempts_to(
-            RespondToThePrompt.with_("Roger, Roger. What's your vector, Victor?")
-        )
+        the_actor.attempts_to(SwitchTo(THE_ORDERS_FRAME))
+
+        the_actor.attempts_to(SwitchTo.the(ORDERS_FRAME))
+
+        the_actor.attempts_to(SwitchTo.default())
     """
 
-    @staticmethod
-    def with_(text: str) -> "RespondToThePrompt":
-        """Provide the text to enter into the prompt."""
-        return RespondToThePrompt(text)
+    @classmethod
+    def the(cls: Type[SelfSwitchTo], target: Target) -> SelfSwitchTo:
+        """Target an element, probably an iframe, to switch to."""
+        return cls(target=target, frame_to_log=str(target))
+
+    @classmethod
+    def default(cls: Type[SelfSwitchTo]) -> SelfSwitchTo:
+        """Switch back to the default frame, the browser window."""
+        return cls(target=None, frame_to_log="default frame")
 
-    def describe(self) -> str:
+    def describe(self: SelfSwitchTo) -> str:
         """Describe the Action in present tense."""
-        return f'Respond to the prompt with "{self.text}".'
-
-    @beat('{} responds to the prompt with "{text}".')
-    def perform_as(self, the_actor: Actor) -> None:
-        """Direct the Actor to respond to the prompt using the given text."""
-        browser = the_actor.uses_ability_to(BrowseTheWeb).browser
-        alert = browser.switch_to.alert
-        aside(f"... the alert says {alert.text}")
-        alert.send_keys(self.text)
-        alert.accept()
+        return f"Switch to the {self.frame_to_log}."
 
-    def __init__(self, text: str) -> None:
-        self.text = text
+    @beat("{} switches to the {frame_to_log}.")
+    def perform_as(self: SelfSwitchTo, the_actor: Actor) -> None:
+        """Direct the Actor to switch to an element or back to default."""
+        browser = the_actor.ability_to(BrowseTheWeb).browser
+        if self.target is None:
+            browser.switch_to.default_content()
+        else:
+            browser.switch_to.frame(self.target.found_by(the_actor))
+
+    def __init__(
+        self: SelfSwitchTo, target: Optional[Target], frame_to_log: str
+    ) -> None:
+        self.target = target
+        self.frame_to_log = frame_to_log
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/right_click.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/right_click.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Right-click on an element, or wherever the cursor currently is.
 """
 
-from typing import Optional
+from typing import Optional, Type, TypeVar
 
 from screenpy import Actor
 from screenpy.pacing import beat
 from selenium.webdriver.common.action_chains import ActionChains
 
 from ..abilities import BrowseTheWeb
 from ..target import Target
 
+SelfRightClick = TypeVar("SelfRightClick", bound="RightClick")
+
 
 class RightClick:
     """Right-click on an element, or wherever the cursor currently is.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -28,43 +30,62 @@
     right-clicks is not interactable through Selenium, because it is an
     application-level menu. A website will need to have implemented a custom
     context menu made of web elements to be able to interact with it.
     """
 
     target: Optional[Target]
 
-    @staticmethod
-    def on_the(target: Target) -> "RightClick":
-        """Target an element to right-click on."""
-        return RightClick(target=target)
-
-    on = on_the_first_of_the = on_the
-
-    def _add_action_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @classmethod
+    def on_the(cls: Type[SelfRightClick], target: Target) -> SelfRightClick:
+        """Target an element to right-click on.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.RightClick.on`
+            * :meth:`~screenpy_selenium.actions.RightClick.on_the_first_of_the`
+        """
+        return cls(target=target)
+
+    @classmethod
+    def on(cls: Type[SelfRightClick], target: Target) -> SelfRightClick:
+        """Alias for :meth:`~screenpy_selenium.actions.RightClick.on_the`."""
+        return cls.on_the(target=target)
+
+    @classmethod
+    def on_the_first_of_the(
+        cls: Type[SelfRightClick], target: Target
+    ) -> SelfRightClick:
+        """Alias for :meth:`~screenpy_selenium.actions.RightClick.on_the`."""
+        return cls.on_the(target=target)
+
+    def _add_action_to_chain(
+        self: SelfRightClick, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Private method to add this Action to the chain."""
         if self.target is not None:
             the_element = self.target.found_by(the_actor)
         else:
             the_element = None
 
         the_chain.context_click(on_element=the_element)
 
-    def describe(self) -> str:
+    def describe(self: SelfRightClick) -> str:
         """Describe the Action in present tense."""
         return f"Right-click{self.description}."
 
     @beat("{} right-clicks{description}.")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfRightClick, the_actor: Actor) -> None:
         """Direct the Actor to right-click on the element."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         the_chain = ActionChains(browser)
         self._add_action_to_chain(the_actor, the_chain)
         the_chain.perform()
 
-    @beat("  Right-click{description}!")
-    def add_to_chain(self, the_actor: Actor, the_chain: ActionChains) -> None:
+    @beat("Right-click{description}!")
+    def add_to_chain(
+        self: SelfRightClick, the_actor: Actor, the_chain: ActionChains
+    ) -> None:
         """Add the RightClick Action to a Chain of Actions."""
         self._add_action_to_chain(the_actor, the_chain)
 
-    def __init__(self, target: Optional[Target] = None) -> None:
+    def __init__(self: SelfRightClick, target: Optional[Target] = None) -> None:
         self.target = target
         self.description = f" on the {target}" if target is not None else ""
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/save_console_log.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/save_console_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Save the browser console log.
 """
 
 import os
-from typing import Any, Optional
+from typing import Any, Optional, Type, TypeVar
 
 from screenpy import Actor
 from screenpy.actions import AttachTheFile
 from screenpy.pacing import beat
 
 from ..abilities import BrowseTheWeb
 
+SelfSaveConsoleLog = TypeVar("SelfSaveConsoleLog", bound="SaveConsoleLog")
+
 
 class SaveConsoleLog:
     """Save the Actor's browser's console log.
 
     Note that you may need to set additional driver properties when creating
     the Actor's browser to enable the console log (e.g. setting
     ``capabilities["goog:loggingPrefs"] = {"browser": "ALL"}``.)
@@ -29,58 +31,63 @@
 
     Examples::
 
         the_actor.attempts_to(SaveConsoleLog("console_log.txt"))
 
         the_actor.attempts_to(SaveConsoleLog.as_(filepath))
 
+        # attach file to the Narrator's reports (behavior depends on adapter).
         the_actor.attempts_to(SaveConsoleLog.as_(filepath).and_attach_it())
 
+        # using screenpy_adapter_allure plugin!
+        from allure_commons.types import AttachmentType
         the_actor.attempts_to(
             SaveConsoleLog.as_(filepath).and_attach_it_with(
                 attachment_type=AttachmentTypes.TEXT,
             ),
         )
     """
 
     attach_kwargs: Optional[dict]
+    path: str
+    filename: str
 
-    def describe(self) -> str:
+    def describe(self: SelfSaveConsoleLog) -> str:
         """Describe the Action in present tense."""
         return f"Save browser console log as {self.filename}"
 
-    @staticmethod
-    def as_(path: str) -> "SaveConsoleLog":
+    @classmethod
+    def as_(cls: Type[SelfSaveConsoleLog], path: str) -> SelfSaveConsoleLog:
         """Supply the name and/or filepath for the saved text file.
 
         If only a name is supplied, the text file will appear in the current
         working directory.
         """
-        return SaveConsoleLog(path)
+        return cls(path=path)
 
-    def and_attach_it(self, **kwargs: Any) -> "SaveConsoleLog":
+    def and_attach_it(self: SelfSaveConsoleLog, **kwargs: Any) -> SelfSaveConsoleLog:
         """Indicate the console log file should be attached to any reports.
 
         This method accepts any additional keywords needed by any adapters
         attached for :external+screenpy:ref:`Narration`.
         """
         self.attach_kwargs = kwargs
         return self
 
     and_attach_it_with = and_attach_it
 
     @beat("{} saves their browser's console log as {filename}")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfSaveConsoleLog, the_actor: Actor) -> None:
         """Direct the actor to save their browser's console log."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         js_log = "\n".join([str(entry) for entry in browser.get_log("browser")])
 
         with open(self.path, "w+", encoding="utf-8") as js_log_file:
             js_log_file.write(js_log)
 
         if self.attach_kwargs is not None:
             the_actor.attempts_to(AttachTheFile(self.path, **self.attach_kwargs))
 
-    def __init__(self, path: str) -> None:
+    def __init__(self: SelfSaveConsoleLog, path: str) -> None:
         self.path = path
         self.filename = path.split(os.path.sep)[-1]
         self.attach_kwargs = None
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/save_screenshot.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/save_screenshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Save a screenshot.
 """
 
 import os
-from typing import Any, Optional
+from typing import Any, Optional, Type, TypeVar
 
 from screenpy import Actor
 from screenpy.actions import AttachTheFile
 from screenpy.pacing import beat
 
 from ..abilities import BrowseTheWeb
 
+SelfSaveScreenshot = TypeVar("SelfSaveScreenshot", bound="SaveScreenshot")
+
 
 class SaveScreenshot:
     """Save a screenshot from the actor's browser.
 
     Use the :meth:`~screenpy_selenium.actions.SaveScreenshot.and_attach_it`
     method to indicate that this screenshot should be attached to all reports
     through the Narrator's adapters. This method also accepts any keyword
@@ -25,58 +27,63 @@
 
     Examples::
 
         the_actor.attempts_to(SaveScreenshot("screenshot.png"))
 
         the_actor.attempts_to(SaveScreenshot.as_(filepath))
 
+        # attach file to the Narrator's reports (behavior depends on adapter).
         the_actor.attempts_to(SaveScreenshot.as_(filepath).and_attach_it())
 
+        # using screenpy_adapter_allure plugin!
+        from allure_commons.types import AttachmentType
         the_actor.attempts_to(
             SaveScreenshot.as_(filepath).and_attach_it_with(
                 attachment_type=AttachmentTypes.PNG,
             ),
         )
     """
 
     attach_kwargs: Optional[dict]
+    path: str
+    filename: str
 
-    def describe(self) -> str:
+    def describe(self: SelfSaveScreenshot) -> str:
         """Describe the Action in present tense."""
         return f"Save screenshot as {self.filename}"
 
-    @staticmethod
-    def as_(path: str) -> "SaveScreenshot":
+    @classmethod
+    def as_(cls: Type[SelfSaveScreenshot], path: str) -> SelfSaveScreenshot:
         """Supply the name and/or filepath for the screenshot.
 
         If only a name is supplied, the screenshot will appear in the current
         working directory.
         """
-        return SaveScreenshot(path)
+        return cls(path=path)
 
-    def and_attach_it(self, **kwargs: Any) -> "SaveScreenshot":
+    def and_attach_it(self: SelfSaveScreenshot, **kwargs: Any) -> SelfSaveScreenshot:
         """Indicate the screenshot should be attached to any reports.
 
         This method accepts any additional keywords needed by any adapters
         attached for :external+screenpy:ref:`Narration`.
         """
         self.attach_kwargs = kwargs
         return self
 
     and_attach_it_with = and_attach_it
 
     @beat("{} saves a screenshot as {filename}")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfSaveScreenshot, the_actor: Actor) -> None:
         """Direct the actor to save a screenshot."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         screenshot = browser.get_screenshot_as_png()
 
         with open(self.path, "wb+") as screenshot_file:
             screenshot_file.write(screenshot)
 
         if self.attach_kwargs is not None:
             the_actor.attempts_to(AttachTheFile(self.path, **self.attach_kwargs))
 
-    def __init__(self, path: str) -> None:
+    def __init__(self: SelfSaveScreenshot, path: str) -> None:
         self.path = path
         self.filename = path.split(os.path.sep)[-1]
         self.attach_kwargs = None
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/select.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/select.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Select an item from a multi-selection field or dropdown.
 """
 
-from typing import Optional, Union
+from typing import Optional, TypeVar, Union
 
 from screenpy import Actor
 from screenpy.exceptions import DeliveryError, UnableToAct
 from screenpy.pacing import beat
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.support.ui import Select as SeleniumSelect
 
 from ..target import Target
 
+SelfSelectByText = TypeVar("SelfSelectByText", bound="SelectByText")
+SelfSelectByIndex = TypeVar("SelfSelectByIndex", bound="SelectByIndex")
+SelfSelectByValue = TypeVar("SelfSelectByValue", bound="SelectByValue")
+
 
 class Select:
     """Select an option from a dropdown menu.
 
     This is an entry point that will create the correct specific Select Action
     to be used, depending on how the option needs to be selected.
 
@@ -44,15 +48,15 @@
 
     @staticmethod
     def the_option_at_index(index: Union[int, str]) -> "SelectByIndex":
         """Select the option by its index. This index is 0-based."""
         return SelectByIndex(index)
 
     @staticmethod
-    def the_option_with_value(value: str) -> "SelectByValue":
+    def the_option_with_value(value: Union[int, str]) -> "SelectByValue":
         """Select the option by its value."""
         return SelectByValue(value)
 
 
 class SelectByText:
     """Select an option in a dropdown or multi-select field by its text.
 
@@ -60,30 +64,31 @@
     by calling :meth:`~screenpy_selenium.actions.Select.the_option_named`.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
     """
 
     target: Optional[Target]
+    text: str
 
-    def from_the(self, target: Target) -> "SelectByText":
+    def from_the(self: SelfSelectByText, target: Target) -> SelfSelectByText:
         """
         Target the dropdown or multi-select field to select the option from.
         """
         self.target = target
         return self
 
     from_ = from_the_first_of_the = from_the
 
-    def describe(self) -> str:
+    def describe(self: SelfSelectByText) -> str:
         """Describe the Action in present tense."""
         return f'Select the option "{self.text}" from the {self.target}.'
 
     @beat('{} selects the option "{text}" from the {target}.')
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfSelectByText, the_actor: Actor) -> None:
         """Direct the Actor to select the option by its text."""
         if self.target is None:
             raise UnableToAct(
                 "Target was not provided for SelectByText. Provide a Target using the "
                 ".from_() or .from_the() methods."
             )
 
@@ -94,15 +99,17 @@
         except WebDriverException as e:
             msg = (
                 "Encountered an issue while attempting to select the option with text "
                 f"'{self.text}' from {self.target}: {e.__class__.__name__}"
             )
             raise DeliveryError(msg) from e
 
-    def __init__(self, text: str, target: Optional[Target] = None) -> None:
+    def __init__(
+        self: SelfSelectByText, text: str, target: Optional[Target] = None
+    ) -> None:
         self.target = target
         self.text = text
 
 
 class SelectByIndex:
     """Select an option in a dropdown or multi-select field by its index.
 
@@ -110,30 +117,31 @@
     by calling :meth:`~screenpy_selenium.actions.Select.the_option_at_index`.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
     """
 
     target: Optional[Target]
+    index: int
 
-    def from_the(self, target: Target) -> "SelectByIndex":
+    def from_the(self: SelfSelectByIndex, target: Target) -> SelfSelectByIndex:
         """
         Target the dropdown or multi-select field to select the option from.
         """
         self.target = target
         return self
 
     from_ = from_the_first_of_the = from_the
 
-    def describe(self) -> str:
+    def describe(self: SelfSelectByIndex) -> str:
         """Describe the Action in present tense."""
         return f"Select the option at index {self.index} from the {self.target}."
 
     @beat("{} selects the option at index {index} from the {target}.")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfSelectByIndex, the_actor: Actor) -> None:
         """Direct the Actor to select the option using its index."""
         if self.target is None:
             raise UnableToAct(
                 "Target was not provided for SelectByIndex. Provide a Target using the "
                 ".from_() or .from_the() methods."
             )
 
@@ -144,46 +152,49 @@
         except WebDriverException as e:
             msg = (
                 "Encountered an issue while attempting to select the option at index "
                 f"{self.index} from {self.target}: {e.__class__.__name__}"
             )
             raise DeliveryError(msg) from e
 
-    def __init__(self, index: Union[int, str], target: Optional[Target] = None) -> None:
+    def __init__(
+        self: SelfSelectByIndex, index: Union[int, str], target: Optional[Target] = None
+    ) -> None:
         self.target = target
-        self.index = str(index)
+        self.index = int(index)
 
 
 class SelectByValue:
     """Select an option in a dropdown or multi-select field by its value.
 
     This Action will probably not be used directly, rather it will be returned
     by calling :meth:`~screenpy_selenium.actions.Select.the_option_with_value`.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
     """
 
     target: Optional[Target]
+    value: str
 
-    def from_the(self, target: Target) -> "SelectByValue":
+    def from_the(self: SelfSelectByValue, target: Target) -> SelfSelectByValue:
         """
         Target the dropdown or multi-select field to select the option from.
         """
         self.target = target
         return self
 
     from_ = from_the_first_of_the = from_the
 
-    def describe(self) -> str:
+    def describe(self: SelfSelectByValue) -> str:
         """Describe the Action in present tense."""
         return f'Select the option with value "{self.value}" from the {self.target}.'
 
     @beat('{} selects the option with value "{value}" from the {target}.')
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfSelectByValue, the_actor: Actor) -> None:
         """Direct the Actor to select the option by its value."""
         if self.target is None:
             raise UnableToAct(
                 "Target was not provided for SelectByValue. Provide a Target using the "
                 ".from_() or .from_the() methods."
             )
 
@@ -194,10 +205,12 @@
         except WebDriverException as e:
             msg = (
                 "Encountered an issue while attempting to select the option with value "
                 f"{self.value} from {self.target}: {e.__class__.__name__}"
             )
             raise DeliveryError(msg) from e
 
-    def __init__(self, value: Union[int, str], target: Optional[Target] = None) -> None:
+    def __init__(
+        self: SelfSelectByValue, value: Union[int, str], target: Optional[Target] = None
+    ) -> None:
         self.target = target
         self.value = str(value)
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/switch_to_tab.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/switch_to_tab.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/actions/wait.py` & `screenpy_selenium-4.0.4/screenpy_selenium/actions/wait.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Wait for the application to fulfill a given condition.
 """
 
-from typing import Any, Callable, Iterable, Optional
+from typing import Any, Callable, Iterable, Optional, Type, TypeVar
 
 from screenpy import Actor, settings
 from screenpy.exceptions import DeliveryError
 from screenpy.pacing import beat
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from ..abilities import BrowseTheWeb
 from ..target import Target
 
+SelfWait = TypeVar("SelfWait", bound="Wait")
+
 
 class Wait:
     """Wait for the application to fulfill a given condition.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -43,32 +45,41 @@
             Wait().using(
                 cookies_to_contain, "for a cookie that has {0}"
             ).with_("delicious=true")
         )
     """
 
     args: Iterable[Any]
+    timeout: float
+    log_detail: Optional[str]
+
+    @classmethod
+    def for_the(cls: Type[SelfWait], target: Target) -> SelfWait:
+        """Set the Target to wait for.
 
-    @staticmethod
-    def for_the(target: Target) -> "Wait":
-        """Set the Target to wait for."""
-        return Wait(settings.TIMEOUT, [target])
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Wait.for_`
+        """
+        return cls(seconds=settings.TIMEOUT, args=[target])
 
-    for_ = for_the
+    @classmethod
+    def for_(cls: Type[SelfWait], target: Target) -> SelfWait:
+        """Alias for :meth:`~screenpy_selenium.actions.Wait.for_the`"""
+        return cls.for_the(target=target)
 
-    def seconds_for_the(self, target: Target) -> "Wait":
+    def seconds_for_the(self: SelfWait, target: Target) -> SelfWait:
         """Set the Target to wait for, after changing the default timeout."""
         self.args = [target]
         return self
 
     second_for = second_for_the = seconds_for = seconds_for_the
 
     def using(
-        self, strategy: Callable[..., Any], log_detail: Optional[str] = None
-    ) -> "Wait":
+        self: SelfWait, strategy: Callable[..., Any], log_detail: Optional[str] = None
+    ) -> SelfWait:
         """Use the given strategy to wait for the Target.
 
         Args:
             strategy: the condition to use to wait. This can be one of
                 Selenium's Expected Conditions, or any custom Callable
                 that returns a boolean.
             log_detail: a nicer-looking message to log than the default.
@@ -77,65 +88,67 @@
         """
         self.condition = strategy
         self.log_detail = log_detail
         return self
 
     to = seconds_using = using
 
-    def with_(self, *args: Any) -> "Wait":
+    def with_(self: SelfWait, *args: Any) -> SelfWait:
         """Set the arguments to pass in to the wait condition."""
         self.args = args
         return self
 
-    def to_appear(self) -> "Wait":
+    def to_appear(self: SelfWait) -> SelfWait:
         """Use Selenium's "visibility of element located" strategy."""
         return self.using(EC.visibility_of_element_located, "for the {0} to appear...")
 
-    def to_be_clickable(self) -> "Wait":
+    def to_be_clickable(self: SelfWait) -> SelfWait:
         """Use Selenium's "to be clickable" strategy."""
         return self.using(EC.element_to_be_clickable, "for the {0} to be clickable...")
 
-    def to_disappear(self) -> "Wait":
+    def to_disappear(self: SelfWait) -> SelfWait:
         """Use Selenium's "invisibility of element located" strategy."""
         return self.using(
             EC.invisibility_of_element_located, "for the {0} to disappear..."
         )
 
-    def to_contain_text(self, text: str) -> "Wait":
+    def to_contain_text(self: SelfWait, text: str) -> SelfWait:
         """Use Selenium's "text to be present in element" strategy."""
         return self.using(
             EC.text_to_be_present_in_element, 'for "{1}" to appear in the {0}...'
         ).with_(*self.args, text)
 
     @property
-    def log_message(self) -> str:
+    def log_message(self: SelfWait) -> str:
         """Format the nice log message, or give back the default."""
         if self.log_detail is None:
             return f"using {self.condition.__name__} with {self.args}"
 
         return self.log_detail.format(*self.args)
 
-    def describe(self) -> str:
+    def describe(self: SelfWait) -> str:
         """Describe the Action in present tense."""
         return f"Wait {self.timeout} seconds {self.log_message}."
 
     @beat("{} waits up to {timeout} seconds {log_message}")
-    def perform_as(self, the_actor: Actor) -> None:
+    def perform_as(self: SelfWait, the_actor: Actor) -> None:
         """Direct the Actor to wait for the condition to be satisfied."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
 
         try:
             WebDriverWait(browser, self.timeout).until(self.condition(*self.args))
         except WebDriverException as e:
             msg = (
                 f"Encountered an exception using {self.condition.__name__} with "
                 f"[{', '.join(map(str, self.args))}]: {e.__class__.__name__}"
             )
             raise DeliveryError(msg) from e
 
     def __init__(
-        self, seconds: Optional[int] = None, args: Optional[Iterable[Any]] = None
+        self: SelfWait,
+        seconds: Optional[float] = None,
+        args: Optional[Iterable[Any]] = None,
     ) -> None:
         self.args = args if args is not None else []
         self.timeout = seconds if seconds is not None else settings.TIMEOUT
         self.condition = EC.visibility_of_element_located
         self.log_detail = None
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/protocols.py` & `screenpy_selenium-4.0.4/screenpy_selenium/protocols.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/__init__.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/attribute.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/attribute.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/browser_title.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/browser_title.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/browser_url.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/browser_url.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/cookies.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/cookies.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/element.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/element.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/number.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/number.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """
 Investigate how many of an element are present on the page.
 """
 
+from typing import Type, TypeVar
+
 from screenpy import Actor
 from screenpy.pacing import beat
 
 from ..target import Target
 
+SelfNumber = TypeVar("SelfNumber", bound="Number")
+
 
 class Number:
     """Ask how many of a certain element are on the page.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
     Examples::
 
         the_actor.should(See.the(Number.of(SEARCH_RESULTS), IsEqualTo(4)))
     """
 
-    @staticmethod
-    def of(target: Target) -> "Number":
+    @classmethod
+    def of(cls: Type[SelfNumber], target: Target) -> SelfNumber:
         """Target the element to be counted."""
-        return Number(target=target)
+        return cls(target=target)
 
-    def describe(self) -> str:
+    def describe(self: SelfNumber) -> str:
         """Describe the Question."""
         return f"The number of {self.target}."
 
     @beat("{} counts the number of {target}.")
-    def answered_by(self, the_actor: Actor) -> int:
+    def answered_by(self: SelfNumber, the_actor: Actor) -> int:
         """Direct the Actor to count the elements."""
         return len(self.target.all_found_by(the_actor))
 
-    def __init__(self, target: Target) -> None:
+    def __init__(self: SelfNumber, target: Target) -> None:
         self.target = target
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/selected.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/selected.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Investigate the text of the selected option or options from a dropdown or
 multi-select field.
 """
 
-from typing import List, Union
+from typing import List, Type, TypeVar, Union
 
 from screenpy import Actor
 from screenpy.pacing import beat
 from selenium.webdriver.support.ui import Select as SeleniumSelect
 
 from ..target import Target
 
+SelfSelected = TypeVar("SelfSelected", bound="Selected")
+
 
 class Selected:
     """Ask for the text of selected option(s) in a dropdown or multi-select field.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -23,50 +25,69 @@
         the_actor.should(
             See.the(Selected.option_from(THE_STATE_DROPDOWN), ReadsExactly("Minnesota"))
         )
 
         the_actor.should(See.the(Selected.options_from(INDUSTRIES), HasLength(5)))
     """
 
-    @staticmethod
-    def option_from_the(target: Target) -> "Selected":
+    target: Target
+    multi: bool
+
+    @classmethod
+    def option_from_the(cls: Type[SelfSelected], target: Target) -> SelfSelected:
         """
         Get the option that is currently selected in a dropdown or the first
         option selected in a multi-select field.
 
         *Note*: if this method is used for a multi-select field, only the
         first selected option will be returned.
-        """
-        return Selected(target)
 
-    option_from = option_from_the
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Selected.option_from`
+        """
+        return cls(target=target)
 
-    @staticmethod
-    def options_from_the(multiselect_target: Target) -> "Selected":
+    @classmethod
+    def option_from(cls: Type[SelfSelected], target: Target) -> SelfSelected:
+        """Alias of :meth:`~screenpy_selenium.actions.Selected.option_from_the`."""
+        return cls.option_from_the(target=target)
+
+    @classmethod
+    def options_from_the(
+        cls: Type[SelfSelected], multiselect_target: Target
+    ) -> SelfSelected:
         """
         Get all the options that are currently selected in a multi-select
         field.
 
         *Note*: this method should not be used for single-select dropdowns,
         that will cause a NotImplemented error to be raised from Selenium when
         answering this Question.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Selected.options_from`
         """
-        return Selected(multiselect_target, multi=True)
+        return cls(target=multiselect_target, multi=True)
 
-    options_from = options_from_the
+    @classmethod
+    def options_from(
+        cls: Type[SelfSelected], multiselect_target: Target
+    ) -> SelfSelected:
+        """Alias of :meth:`~screenpy_selenium.actions.Selected.options_from_the`."""
+        return cls.options_from_the(multiselect_target=multiselect_target)
 
-    def describe(self) -> str:
+    def describe(self: SelfSelected) -> str:
         """Describe the Question."""
         return f"The selected option(s) from the {self.target}."
 
     @beat("{} checks the selected option(s) from the {target}.")
-    def answered_by(self, the_actor: Actor) -> Union[str, List[str]]:
+    def answered_by(self: SelfSelected, the_actor: Actor) -> Union[str, List[str]]:
         """Direct the Actor to name the selected option(s)."""
         select = SeleniumSelect(self.target.found_by(the_actor))
 
         if self.multi:
             return [e.text for e in select.all_selected_options]
         return select.first_selected_option.text
 
-    def __init__(self, target: Target, multi: bool = False):
+    def __init__(self: SelfSelected, target: Target, multi: bool = False):
         self.target = target
         self.multi = multi
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/text.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Investigate the text of an element or many elements.
 """
 
-from typing import List, Union
+from typing import List, Type, TypeVar, Union
 
 from screenpy import Actor
 from screenpy.pacing import beat
 
 from ..target import Target
 
+SelfText = TypeVar("SelfText", bound="Text")
+
 
 class Text:
     """Ask what text appears in an element or elements.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -23,33 +25,49 @@
         )
 
         the_actor.should(
             See.the(Text.of_all(SEARCH_RESULTS), ContainsTheItem("Rear Window"))
         )
     """
 
-    @staticmethod
-    def of_the(target: Target) -> "Text":
-        """Target the element to extract the text from."""
-        return Text(target=target)
+    target: Target
+    multi: bool
 
-    of = of_the_first_of_the = of_the
+    @classmethod
+    def of_the(cls: Type[SelfText], target: Target) -> SelfText:
+        """Target the element to extract the text from.
+
+        Aliases:
+            * :meth:`~screenpy_selenium.actions.Text.of`
+            * :meth:`~screenpy_selenium.actions.Text.of_the_first_of_the`
+        """
+        return cls(target=target)
+
+    @classmethod
+    def of(cls: Type[SelfText], target: Target) -> SelfText:
+        """Alias of :meth:`~screenpy_selenium.actions.Text.of_the`."""
+        return cls.of_the(target=target)
+
+    @classmethod
+    def of_the_first_of_the(cls: Type[SelfText], target: Target) -> SelfText:
+        """Alias of :meth:`~screenpy_selenium.actions.Text.of_the`."""
+        return cls.of_the(target=target)
 
-    @staticmethod
-    def of_all(multi_target: Target) -> "Text":
+    @classmethod
+    def of_all(cls: Type[SelfText], multi_target: Target) -> SelfText:
         """Target the elements, plural, to extract the text from."""
-        return Text(target=multi_target, multi=True)
+        return cls(target=multi_target, multi=True)
 
-    def describe(self) -> str:
+    def describe(self: SelfText) -> str:
         """Describe the Question."""
         return f"The text from the {self.target}."
 
     @beat("{} reads the text from the {target}.")
-    def answered_by(self, the_actor: Actor) -> Union[str, List[str]]:
+    def answered_by(self: SelfText, the_actor: Actor) -> Union[str, List[str]]:
         """Direct the Actor to read off the text of the element(s)."""
         if self.multi:
             return [e.text for e in self.target.all_found_by(the_actor)]
         return self.target.found_by(the_actor).text
 
-    def __init__(self, target: Target, multi: bool = False) -> None:
+    def __init__(self: SelfText, target: Target, multi: bool = False) -> None:
         self.target = target
         self.multi = multi
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/questions/text_of_the_alert.py` & `screenpy_selenium-4.0.4/screenpy_selenium/questions/text_of_the_alert.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/__init__.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # Natural-language-enabling syntactic sugar
 IsEnabled = Enabled = Clickable = IsClickable
 IsDisplayed = Displayed = Visible = IsVisible
 IsNotDisplayed = NotDisplayed = Invisible = IsInvisible
 Exist = Exists = Present = IsPresent
 
+
 __all__ = [
     "Clickable",
     "Displayed",
     "Enabled",
     "Exist",
     "Exists",
     "Invisible",
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_clickable_element.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_clickable_element.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_invisible_element.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_invisible_element.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class IsInvisibleElement(BaseMatcher[Optional[WebElement]]):
     """
     Matches an element whose ``is_displayed`` method returns False.
     """
 
     def _matches(self, item: Optional[WebElement]) -> bool:
         if item is None:
-            return False
+            return True
         return item.is_displayed() is False
 
     def describe_to(self, description: Description) -> None:
         """Describe the passing case."""
         description.append_text("the element is invisible")
 
     def describe_match(
@@ -30,16 +30,13 @@
     ) -> None:
         match_description.append_text("it was invisible")
 
     def describe_mismatch(
         self, item: Optional[WebElement], mismatch_description: Description
     ) -> None:
         """Describe the failing case."""
-        if item is None:
-            mismatch_description.append_text("was not even present")
-            return
         mismatch_description.append_text("was not invisible")
 
 
 def is_invisible_element() -> IsInvisibleElement:
     """This matcher matches any element that is invisible."""
     return IsInvisibleElement()
```

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_present_element.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_present_element.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/custom_matchers/is_visible_element.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/custom_matchers/is_visible_element.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_clickable.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_clickable.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_invisible.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_invisible.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_present.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_present.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/resolutions/is_visible.py` & `screenpy_selenium-4.0.4/screenpy_selenium/resolutions/is_visible.py`

 * *Files identical despite different names*

### Comparing `screenpy_selenium-4.0.3/screenpy_selenium/target.py` & `screenpy_selenium-4.0.4/screenpy_selenium/target.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Provides an object to store a locator with a human-readable string. The
 human-readable string will be used in logging and reporting; the locator
 will be used by Actors to find elements.
 """
 
-from typing import Iterator, List, Optional, Tuple, Union
+from typing import Iterator, List, Optional, Tuple, Type, TypeVar, Union
 
 from screenpy.actor import Actor
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebElement
 
 from .abilities.browse_the_web import BrowseTheWeb
 from .exceptions import TargetingError
 
+SelfTarget = TypeVar("SelfTarget", bound="Target")
+
 
 class Target:
     """Describe an element with a human-readable string and a locator.
 
     Abilities Required:
         :class:`~screenpy_selenium.abilities.BrowseTheWeb`
 
@@ -30,36 +32,39 @@
         Target().located_by((By.ID, "username-field"))
     """
 
     _description: Optional[str] = None
     locator: Optional[Tuple[str, str]] = None
 
     @property
-    def target_name(self):
+    def target_name(self: SelfTarget) -> Optional[str]:
+        """return the description when set or the 2nd half of the locator"""
         if self._description is not None:
             return self._description
         return self.locator[1] if self.locator else None
 
     @target_name.setter
-    def target_name(self, value):
+    def target_name(self: SelfTarget, value) -> None:
         self._description = value
 
     @target_name.deleter
-    def target_name(self):
+    def target_name(self: SelfTarget) -> None:
         del self._description
 
-    @staticmethod
-    def the(desc: str) -> "Target":
+    @classmethod
+    def the(cls: Type[SelfTarget], desc: str) -> SelfTarget:
         """Name this Target.
 
         Beginning with a lower-case letter makes the logs look the nicest.
         """
-        return Target(desc)
+        return cls(desc=desc)
 
-    def located_by(self, locator: Union[Tuple[str, str], str]) -> "Target":
+    def located_by(
+        self: SelfTarget, locator: Union[Tuple[str, str], str]
+    ) -> SelfTarget:
         """Set the locator for this Target.
 
         Possible values for locator:
             * A tuple of a By classifier and a string (e.g. ``(By.ID, "welcome")``)
             * An XPATH string (e.g. ``"//div/h3"``)
             * A CSS selector string (e.g. ``"div.confetti"``)
 
@@ -76,54 +81,58 @@
         elif locator[0] in ("(", "/"):
             self.locator = (By.XPATH, locator)
         else:
             self.locator = (By.CSS_SELECTOR, locator)
 
         return self
 
-    def located(self, locator: Union[Tuple[str, str], str]) -> "Target":
+    def located(self: SelfTarget, locator: Union[Tuple[str, str], str]) -> SelfTarget:
         """Alias for :meth:~screenpy_selenium.Target.located_by"""
         return self.located_by(locator)
 
-    def get_locator(self) -> Tuple[str, str]:
+    def get_locator(self: SelfTarget) -> Tuple[str, str]:
         """Return the stored locator.
 
         Raises:
             TargetingError: if no locator was set.
         """
         if self.locator is None:
             raise TargetingError(
                 f"Locator was not supplied to the {self} target. Make sure to use "
                 "either .located() or .located_by() to supply a locator."
             )
         return self.locator
 
-    def found_by(self, the_actor: Actor) -> WebElement:
+    def found_by(self: SelfTarget, the_actor: Actor) -> WebElement:
         """Retrieve the |WebElement| as viewed by the Actor."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         try:
             return browser.find_element(*self)
         except WebDriverException as e:
             raise TargetingError(f"{e} raised while trying to find {self}.") from e
 
-    def all_found_by(self, the_actor: Actor) -> List[WebElement]:
+    def all_found_by(self: SelfTarget, the_actor: Actor) -> List[WebElement]:
         """Retrieve a list of |WebElement| objects as viewed by the Actor."""
         browser = the_actor.ability_to(BrowseTheWeb).browser
         try:
             return browser.find_elements(*self)
         except WebDriverException as e:
             raise TargetingError(f"{e} raised while trying to find {self}.") from e
 
-    def __repr__(self) -> str:
+    def __repr__(self: SelfTarget) -> str:
         return f"{self.target_name}"
 
     __str__ = __repr__
 
-    def __iter__(self) -> Iterator[str]:
+    def __iter__(self: SelfTarget) -> Iterator[str]:
         return self.get_locator().__iter__()
 
-    def __getitem__(self, index: int) -> str:
+    def __getitem__(self: SelfTarget, index: int) -> str:
         return self.get_locator()[index]
 
-    def __init__(self, desc: str = None, locator: Tuple[str, str] = None) -> None:
+    def __init__(
+        self: SelfTarget,
+        desc: Optional[str] = None,
+        locator: Optional[Tuple[str, str]] = None,
+    ) -> None:
         self.target_name = desc
         self.locator = locator
```

