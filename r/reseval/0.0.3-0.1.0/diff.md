# Comparing `tmp/reseval-0.0.3.tar.gz` & `tmp/reseval-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reseval-0.0.3.tar", last modified: Fri Jun 24 22:53:10 2022, max compression
+gzip compressed data, was "reseval-0.1.0.tar", last modified: Thu Jul 20 13:28:10 2023, max compression
```

## Comparing `reseval-0.0.3.tar` & `reseval-0.1.0.tar`

### file list

```diff
@@ -1,179 +1,182 @@
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.559229 reseval-0.0.3/
--rw-rw-rw-   0        0        0     1099 2022-02-25 18:58:25.000000 reseval-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    11883 2022-06-24 22:53:10.558229 reseval-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11491 2022-06-21 16:32:41.000000 reseval-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.341229 reseval-0.0.3/reseval/
--rw-rw-rw-   0        0        0      557 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/__init__.py
--rw-rw-rw-   0        0        0     1259 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/__main__.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.370231 reseval-0.0.3/reseval/app/
--rw-rw-rw-   0        0        0       22 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/app/__init__.py
--rw-rw-rw-   0        0        0     1719 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/app/heroku.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.380229 reseval-0.0.3/reseval/assets/
--rw-rw-rw-   0        0        0       16 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/assets/Procfile
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.388229 reseval-0.0.3/reseval/assets/client/
--rw-rw-rw-   0        0        0  1185786 2022-06-21 17:43:37.000000 reseval-0.0.3/reseval/assets/client/package-lock.json
--rw-rw-rw-   0        0        0      867 2022-06-21 17:43:37.000000 reseval-0.0.3/reseval/assets/client/package.json
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.393230 reseval-0.0.3/reseval/assets/client/public/
--rw-rw-rw-   0        0        0     1951 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/public/favicon.ico
--rw-rw-rw-   0        0        0     1769 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/public/index.html
--rw-rw-rw-   0        0        0      330 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/public/manifest.json
--rw-rw-rw-   0        0        0       70 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/public/robots.txt
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.398229 reseval-0.0.3/reseval/assets/client/src/
--rw-rw-rw-   0        0        0      235 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/App.js
--rw-rw-rw-   0        0        0     2809 2022-06-24 20:42:08.000000 reseval-0.0.3/reseval/assets/client/src/Survey.js
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.412229 reseval-0.0.3/reseval/assets/client/src/components/
--rw-rw-rw-   0        0        0      844 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/components/Audio.js
--rw-rw-rw-   0        0        0      401 2022-06-24 16:34:12.000000 reseval-0.0.3/reseval/assets/client/src/components/Button.js
--rw-rw-rw-   0        0        0      480 2022-06-21 18:18:45.000000 reseval-0.0.3/reseval/assets/client/src/components/Image.js
--rw-rw-rw-   0        0        0      463 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/components/Markdown.js
--rw-rw-rw-   0        0        0     2675 2022-06-24 16:34:21.000000 reseval-0.0.3/reseval/assets/client/src/components/Media.js
--rw-rw-rw-   0        0        0     1578 2022-06-24 16:34:30.000000 reseval-0.0.3/reseval/assets/client/src/components/MediaRadioButtonGroup.js
--rw-rw-rw-   0        0        0     4887 2022-03-08 19:07:59.000000 reseval-0.0.3/reseval/assets/client/src/components/MediaSliderGroup.js
--rw-rw-rw-   0        0        0     1294 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/components/RadioButtonGroup.js
--rw-rw-rw-   0        0        0      995 2022-06-24 16:34:40.000000 reseval-0.0.3/reseval/assets/client/src/components/Text.js
--rw-rw-rw-   0        0        0      800 2022-04-06 17:52:20.000000 reseval-0.0.3/reseval/assets/client/src/components/Video.js
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.415228 reseval-0.0.3/reseval/assets/client/src/css/
--rw-rw-rw-   0        0        0     2753 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/css/components.css
--rw-rw-rw-   0        0        0      370 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/css/index.css
--rw-rw-rw-   0        0        0      616 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/index.js
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.417232 reseval-0.0.3/reseval/assets/client/src/json/
--rw-rw-rw-   0        0        0        0 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/json/.gitkeep
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.423230 reseval-0.0.3/reseval/assets/client/src/pages/
--rw-rw-rw-   0        0        0      833 2022-03-02 20:16:42.000000 reseval-0.0.3/reseval/assets/client/src/pages/EndPage.js
--rw-rw-rw-   0        0        0     2704 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/pages/FeedbackPage.js
--rw-rw-rw-   0        0        0     9935 2022-06-24 20:44:35.000000 reseval-0.0.3/reseval/assets/client/src/pages/QualificationPage.js
--rw-rw-rw-   0        0        0     3618 2022-06-24 20:45:17.000000 reseval-0.0.3/reseval/assets/client/src/pages/TaskPage.js
--rw-rw-rw-   0        0        0      489 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/pages/WelcomePage.js
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.428228 reseval-0.0.3/reseval/assets/client/src/questions/
--rw-rw-rw-   0        0        0      244 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/src/questions/FreeResponse.js
--rw-rw-rw-   0        0        0     1434 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/questions/ListeningTest.js
--rw-rw-rw-   0        0        0     1245 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/questions/MultipleChoice.js
--rw-rw-rw-   0        0        0     1057 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/client/src/questions/Question.js
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.435229 reseval-0.0.3/reseval/assets/client/src/test/
--rw-rw-rw-   0        0        0     2266 2022-06-24 16:35:18.000000 reseval-0.0.3/reseval/assets/client/src/test/AB.js
--rw-rw-rw-   0        0        0     2931 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/test/ABX.js
--rw-rw-rw-   0        0        0     2069 2022-06-24 21:27:09.000000 reseval-0.0.3/reseval/assets/client/src/test/MOS.js
--rw-rw-rw-   0        0        0     2912 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/assets/client/src/test/MUSHRA.js
--rw-rw-rw-   0        0        0      106 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/client/static.json
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.471227 reseval-0.0.3/reseval/assets/listening_test/
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones4_0.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones4_1.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones4_2.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones4_3.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones5_0.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones5_1.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones5_2.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones5_3.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones6_0.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones6_1.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones6_2.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones6_3.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones7_0.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones7_1.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones7_2.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones7_3.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones8_0.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones8_1.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones8_2.wav
--rw-rw-rw-   0        0        0   352828 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/assets/listening_test/tones8_3.wav
--rw-rw-rw-   0        0        0   151718 2022-06-21 17:14:52.000000 reseval-0.0.3/reseval/assets/package-lock.json
--rw-rw-rw-   0        0        0      883 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/assets/package.json
--rw-rw-rw-   0        0        0      374 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/assets/policy.json
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.311229 reseval-0.0.3/reseval/assets/server/
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.473229 reseval-0.0.3/reseval/assets/server/db/
--rw-rw-rw-   0        0        0      924 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/assets/server/db/index.ts
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.479228 reseval-0.0.3/reseval/assets/server/db/queries/
--rw-rw-rw-   0        0        0      148 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/db/queries/conditions.ts
--rw-rw-rw-   0        0        0      106 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/db/queries/files.ts
--rw-rw-rw-   0        0        0     1051 2022-03-08 19:07:59.000000 reseval-0.0.3/reseval/assets/server/db/queries/participants.ts
--rw-rw-rw-   0        0        0      335 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/db/queries/responses.ts
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.480231 reseval-0.0.3/reseval/assets/server/routes/
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.488230 reseval-0.0.3/reseval/assets/server/routes/api/
--rw-rw-rw-   0        0        0      504 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/api/conditions.ts
--rw-rw-rw-   0        0        0      207 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/assets/server/routes/api/evaluators.ts
--rw-rw-rw-   0        0        0      495 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/api/files.ts
--rw-rw-rw-   0        0        0      545 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/api/index.ts
--rw-rw-rw-   0        0        0     1013 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/api/participants.ts
--rw-rw-rw-   0        0        0      666 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/api/responses.ts
--rw-rw-rw-   0        0        0      165 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/server/routes/index.ts
--rw-rw-rw-   0        0        0      776 2022-06-24 15:43:07.000000 reseval-0.0.3/reseval/assets/server.ts
--rw-rw-rw-   0        0        0     1082 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/survey.xml
--rw-rw-rw-   0        0        0    10998 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/assets/tsconfig.json
--rw-rw-rw-   0        0        0     2982 2022-06-24 20:49:46.000000 reseval-0.0.3/reseval/constants.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.494230 reseval-0.0.3/reseval/convert/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/convert/__init__.py
--rw-rw-rw-   0        0        0      723 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/convert/__main__.py
--rw-rw-rw-   0        0        0     3834 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/convert/audio.py
--rw-rw-rw-   0        0        0     2874 2022-04-06 17:52:20.000000 reseval-0.0.3/reseval/convert/image.py
--rw-rw-rw-   0        0        0     2169 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/core.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.498228 reseval-0.0.3/reseval/create/
--rw-rw-rw-   0        0        0       26 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/create/__init__.py
--rw-rw-rw-   0        0        0      968 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/create/__main__.py
--rw-rw-rw-   0        0        0     4172 2022-06-24 21:25:14.000000 reseval-0.0.3/reseval/create/core.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.503227 reseval-0.0.3/reseval/credentials/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/credentials/__init__.py
--rw-rw-rw-   0        0        0     1070 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/credentials/__main__.py
--rw-rw-rw-   0        0        0     2612 2022-03-01 16:52:44.000000 reseval-0.0.3/reseval/credentials/core.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.506227 reseval-0.0.3/reseval/crowdsource/
--rw-rw-rw-   0        0        0       42 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/crowdsource/__init__.py
--rw-rw-rw-   0        0        0     5995 2022-03-08 19:07:59.000000 reseval-0.0.3/reseval/crowdsource/core.py
--rw-rw-rw-   0        0        0    13088 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/crowdsource/mturk.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.513229 reseval-0.0.3/reseval/database/
--rw-rw-rw-   0        0        0       68 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/database/__init__.py
--rw-rw-rw-   0        0        0    10460 2022-06-24 16:33:57.000000 reseval-0.0.3/reseval/database/core.py
--rw-rw-rw-   0        0        0      912 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/database/download.py
--rw-rw-rw-   0        0        0     1151 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/database/heroku.py
--rw-rw-rw-   0        0        0     1837 2022-06-24 21:24:17.000000 reseval-0.0.3/reseval/database/localhost.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.517228 reseval-0.0.3/reseval/destroy/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/destroy/__init__.py
--rw-rw-rw-   0        0        0      823 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/destroy/__main__.py
--rw-rw-rw-   0        0        0     1660 2022-06-24 21:19:00.000000 reseval-0.0.3/reseval/destroy/core.py
--rw-rw-rw-   0        0        0      277 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/error.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.522230 reseval-0.0.3/reseval/extend/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/extend/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/extend/__main__.py
--rw-rw-rw-   0        0        0     1978 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/extend/core.py
--rw-rw-rw-   0        0        0      751 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/filter.py
--rw-rw-rw-   0        0        0     2805 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/load.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.527227 reseval-0.0.3/reseval/monitor/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/monitor/__init__.py
--rw-rw-rw-   0        0        0      825 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/monitor/__main__.py
--rw-rw-rw-   0        0        0     5278 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/monitor/core.py
--rw-rw-rw-   0        0        0     1252 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/npm.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.531229 reseval-0.0.3/reseval/pay/
--rw-rw-rw-   0        0        0       21 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/pay/__init__.py
--rw-rw-rw-   0        0        0      560 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/pay/__main__.py
--rw-rw-rw-   0        0        0      389 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/pay/core.py
--rw-rw-rw-   0        0        0     2966 2022-06-24 22:25:48.000000 reseval-0.0.3/reseval/plot.py
--rw-rw-rw-   0        0        0      252 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/random.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.535229 reseval-0.0.3/reseval/results/
--rw-rw-rw-   0        0        0       21 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/results/__init__.py
--rw-rw-rw-   0        0        0      781 2022-03-08 19:07:59.000000 reseval-0.0.3/reseval/results/__main__.py
--rw-rw-rw-   0        0        0     2564 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/results/core.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.541228 reseval-0.0.3/reseval/server/
--rw-rw-rw-   0        0        0       64 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/server/__init__.py
--rw-rw-rw-   0        0        0     1955 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/server/core.py
--rw-rw-rw-   0        0        0     3840 2022-03-04 21:00:59.000000 reseval-0.0.3/reseval/server/heroku.py
--rw-rw-rw-   0        0        0     2083 2022-06-21 16:31:22.000000 reseval-0.0.3/reseval/server/local.py
--rw-rw-rw-   0        0        0     1683 2022-03-01 16:51:58.000000 reseval-0.0.3/reseval/stats.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.546228 reseval-0.0.3/reseval/storage/
--rw-rw-rw-   0        0        0       62 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/storage/__init__.py
--rw-rw-rw-   0        0        0     4422 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/storage/aws.py
--rw-rw-rw-   0        0        0     1496 2022-05-10 15:04:45.000000 reseval-0.0.3/reseval/storage/client.py
--rw-rw-rw-   0        0        0     1447 2022-03-02 21:58:30.000000 reseval-0.0.3/reseval/storage/core.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.556228 reseval-0.0.3/reseval/test/
--rw-rw-rw-   0        0        0      137 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/test/__init__.py
--rw-rw-rw-   0        0        0     1598 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/test/ab.py
--rw-rw-rw-   0        0        0      697 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/test/abx.py
--rw-rw-rw-   0        0        0     4042 2022-06-21 16:32:41.000000 reseval-0.0.3/reseval/test/base.py
--rw-rw-rw-   0        0        0      566 2022-02-25 18:58:25.000000 reseval-0.0.3/reseval/test/core.py
--rw-rw-rw-   0        0        0     4211 2022-06-24 22:39:14.000000 reseval-0.0.3/reseval/test/mos.py
--rw-rw-rw-   0        0        0     3132 2022-06-24 22:39:23.000000 reseval-0.0.3/reseval/test/mushra.py
-drwxrwxrwx   0        0        0        0 2022-06-24 22:53:10.366230 reseval-0.0.3/reseval.egg-info/
--rw-rw-rw-   0        0        0    11883 2022-06-24 22:53:09.000000 reseval-0.0.3/reseval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4838 2022-06-24 22:53:10.000000 reseval-0.0.3/reseval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-24 22:53:09.000000 reseval-0.0.3/reseval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      185 2022-06-24 22:53:10.000000 reseval-0.0.3/reseval.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-24 22:53:10.000000 reseval-0.0.3/reseval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-24 22:53:10.559229 reseval-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1605 2022-06-21 16:32:41.000000 reseval-0.0.3/setup.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2023-04-02 16:25:40.000000 reseval-0.1.0/LICENSE
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12286 2023-07-20 13:28:10.869796 reseval-0.1.0/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    11894 2023-07-20 13:26:17.000000 reseval-0.1.0/README.md
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      534 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1218 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/app/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       21 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/app/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1306 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/app/heroku.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/assets/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       15 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/Procfile
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  1156816 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/package-lock.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      826 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/package.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/public/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1951 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/favicon.ico
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1725 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/index.html
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      315 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/manifest.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       67 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/robots.txt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      221 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/App.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2722 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/Survey.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/components/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Audio.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      386 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/components/Button.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      460 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Image.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      446 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/components/Markdown.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2578 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Media.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1509 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/MediaRadioButtonGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4720 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/MediaSliderGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1236 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/RadioButtonGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      975 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Text.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      881 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Video.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2500 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/WordSelection.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/css/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3102 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/css/components.css
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      350 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/css/index.css
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      594 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/index.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/json/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/json/.gitkeep
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/pages/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      807 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/pages/EndPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2714 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/FeedbackPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10151 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/QualificationPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3720 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/TaskPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      539 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/WelcomePage.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/questions/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      235 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/FreeResponse.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1393 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/ListeningTest.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1208 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/MultipleChoice.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1021 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/Question.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2186 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/AB.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2834 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/ABX.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1994 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/MOS.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2818 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/MUSHRA.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1967 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/WordSelect.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      100 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/static.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/listening_test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   147781 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/package-lock.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      848 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/package.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.837796 reseval-0.1.0/reseval/assets/server/
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/db/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/db/index.ts
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/db/queries/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      142 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/conditions.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      101 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/files.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1077 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/db/queries/participants.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      324 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/responses.ts
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/routes/
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/routes/api/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      484 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/conditions.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      475 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/files.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      439 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/routes/api/index.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1361 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/routes/api/participants.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      641 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/responses.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      157 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/index.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      744 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1054 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/survey.xml
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10895 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/tsconfig.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2900 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/constants.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/convert/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      697 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3706 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/audio.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2777 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/image.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2187 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/create/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       25 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/create/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      936 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/create/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5138 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/create/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/credentials/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1039 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2526 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/crowdsource/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5776 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12696 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/mturk.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/database/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       83 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3616 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10207 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      884 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/database/download.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/heroku.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1940 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/localhost.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/destroy/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/destroy/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      799 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/destroy/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1602 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/destroy/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      270 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/error.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/extend/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      986 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1922 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      731 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/filter.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2708 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/load.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/monitor/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/monitor/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      797 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/monitor/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5241 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/monitor/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1219 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/npm.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/pay/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      541 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      374 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2870 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/plot.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      244 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/random.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/results/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      754 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2481 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/server/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       79 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8144 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1901 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3737 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/heroku.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2003 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/local.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1620 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/stats.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/storage/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       59 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/storage/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5015 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/storage/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1425 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/storage/client.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1401 2023-06-02 19:25:32.000000 reseval-0.1.0/reseval/storage/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      166 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1552 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/ab.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      675 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/abx.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4016 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/base.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      615 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4103 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/mos.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3018 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/mushra.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2013 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/wordselect.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval.egg-info/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12286 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4936 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      185 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/requires.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        8 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/top_level.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-07-20 13:28:10.869796 reseval-0.1.0/setup.cfg
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1571 2023-07-20 13:27:25.000000 reseval-0.1.0/setup.py
```

### Comparing `reseval-0.0.3/LICENSE` & `reseval-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Interactive Audio Lab
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Interactive Audio Lab
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `reseval-0.0.3/PKG-INFO` & `reseval-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,428 +1,448 @@
-Metadata-Version: 2.1
-Name: reseval
-Version: 0.0.3
-Summary: Reproducible Subjective Evaluation
-Home-page: https://github.com/reseval/reseval
-Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
-Author-email: maxrmorrison@gmail.com
-Keywords: audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Reproducible Subjective Evaluation (ReSEval)
-[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
-[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
-
-ReSEval is a framework for quickly building subjective evaluations that are
-deployed on crowdworker platforms like
-[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
-A/B, ABX, MOS, and MUSHRA tests on audio, image, text, and video data.
-
-<h3 align="center">
-    While our code is free to use, performing crowdsourced subjective
-    evaluation is not free.<br/>We are not responsible for costs incurred
-    while using our code.
-</h3>
-
-
-### Citation
-
-If you use ReSEval in an academic publication, please cite
-[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
-
-
-### IEEE
-
-M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
-
-
-### BibTex
-
-```
-@inproceedings{morrison2022reproducible,
-    title={Reproducible Subjective Evaluation},
-    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
-    booktitle={ICLR Workshop on ML Evaluation Standards},
-    month={April},
-    year={2022}
-}
-```
-
-
-## Table of contents
-- [Installation](#installation)
-    * [Deploying locally](#deploying-locally)
-- [Configuration](#configuration)
-- [Adding files](#adding-files)
-    * [AB](#ab)
-    * [ABX](#abx)
-    * [MOS](#mos)
-    * [MUSHRA](#mushra)
-- [Credentials](#credentials)
-    * [Heroku](#heroku)
-    * [Amazon Web Services](#amazon-web-services)
-    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
-- [Usage](#usage)
-    * [Command-line interface](#command-line-interface)
-        * [Create](#create)
-        * [Monitor](#monitor)
-        * [Results](#results)
-        * [Pay](#pay)
-        * [Destroy](#destroy)
-        * [Extend](#extend)
-    * [Application programming interface](#application-programming-interface)
-- [Advanced usage](#advanced-usage)
-    * [CLI](#cli)
-    * [API](#api)
-- [Additional monitoring](#additional-monitoring)
-
-
-## Installation
-
-First, install the Python module. ReSEval requires Python 3.9 or higher.
-
-`pip install reseval`
-
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
-
-```
-# Linux or OS X
-sudo npm install -g n
-sudo n 17.4.0
-
-# Windows
-# Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
-```
-
-**Note** - You must restart your terminal after changing versions of node for the change to take effect
-
-### Deploying locally
-
-To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
-and obtain a username and password. The default username is `root`.
-
-Run the following to store the username and password in
-`reseval.CACHE / '.env'`.
-
-```
-python -m reseval.credentials \
-    --mysql_local_user <mysql_user> \
-    --mysql_local_password <mysql_local_password>
-```
-
-The `.env` file is used to set local environment variables and is not pushed to
-GitHub or uploaded to any remote storage.
-
-
-## Configuration
-
-All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
-
-
-## Adding files
-
-The files to be evaluated must be organized in a directory structure according
-to the type of test being run. The directory structures for each test are as
-follows. Examples of valid directories of evaluation files can be found in
-`examples/`.
-
-
-### AB
-
-```
-ab
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### ABX
-
-```
-abx
-└── reference
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### MOS
-
-```
-mos
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-### MUSHRA
-
-```
-mushra
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-## Credentials
-
-API keys are required to use the third-party services that ReSEval depends on.
-These are not required for local development. Do not share these API keys.
-
-
-### Heroku
-
-Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
-
-<p align="center">
-    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
-    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
-</p>
-
-You will also need to enable billing. You can do so [here](https://heroku.com/verify).
-
-
-### Amazon Web Services
-
-Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
-
-<p align="center">
-    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
-    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
-</p>
-
-
-### Amazon Mechanical Turk
-
-Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
-
-
-## Usage
-
-Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
-
-If you are not deploying locally, add your API keys.
-
-```
-python -m reseval.credentials \
-    --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
-    --heroku_api_key <heroku_api_key>
-```
-
- API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
-
-
-### Command-line interface
-
- Arguments for the following command-line interfaces are as follows, unless otherwise specified.
-
-- `<config>` - The configuration file
-- `<directory>` - The directory of evaluation files
-- `<name>` - The name of the evaluation given in the configuration file
-
-
-#### Create
-
-Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
-
-**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
-
-```
-# Local development
-python -m reseval.create <config> <directory> --local
-
-# Remote development
-python -m reseval.create <config> <directory>
-
-# Production
-python -m reseval.create <config> <directory> --production
-```
-
-
-#### Monitor
-
-```
-# Monitor all subjective evaluations
-python -m reseval.monitor
-
-# Monitor one subjective evaluation
-# The name of the evaluation can be found in its configuration file
-python -m reseval.monitor --name <name>
-```
-
-**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
-
-```
-# Update the monitor once every ten seconds
-python -m reseval.monitor --interval 10
-```
-
-
-#### Results
-
-```
-# Get the results of a subjective evaluation.
-# Results are stored in <directory>/<name>.
-# <directory> defaults to the current directory.
-python -m reseval.results <name> --directory <directory>
-```
-
-
-#### Pay
-
-```
-# Pay participants
-python -m reseval.pay <name>
-```
-
-
-#### Destroy
-
-```
-# Destroy the compute resources of a subjective evaluation (e.g., any cloud
-# storage, databases, or servers)
-python -m reseval.destroy <name>
-
-# Destroy a subjective evaluation even if it is still active.
-# Participants who have taken the test so far will be paid.
-python -m reseval.destroy <name> --force
-```
-
-
-#### Extend
-
-```
-# Add <participants> additional participants to a finished evaluation
-python -m reseval.extend <name> <participants>
-```
-
-
-### Application programming interface
-
-Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
-
-
-## Advanced usage
-
-Once you feel comfortable with using ReSEval step-by-step from the
-command-line and after you have added your credentials with
-`reseval.credentials`, you can use the CLI or API to run your evaluation with
-only a single command.
-
-
-### CLI
-
-```
-# Local development
-python -m reseval <config> <directory> --local
-
-# Remote development
-python -m reseval <config> <directory>
-
-# Production
-python -m reseval <config> <directory> --production
-```
-
-
-### API
-
-```
-import reseval
-
-# Local development
-reseval.run(config, directory, local=True)
-
-# Remote development
-reseval.run(config, directory)
-
-# Production
-reseval.run(config, directory, production=True)
-```
-
-
-## Additional monitoring
-
-### Heroku
-
-To monitor, edit, or delete Heroku databases and servers, use the
-[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
-any costs on the
-[billing dashboard](https://dashboard.heroku.com/account/billing).
-
-
-### AWS S3
-
-To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
-[AWS S3 console](https://aws.amazon.com/s3/).
-
-
-### MTurk
-
-HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
-You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
-on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
-at the end of the billing period.
+# Reproducible Subjective Evaluation (ReSEval)
+[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
+
+ReSEval is a framework for quickly building subjective evaluation and
+annotation tasks that are deployed on crowdworker platforms like
+[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
+A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
+
+<h3 align="center">
+    While our code is free to use, performing crowdsourced subjective
+    evaluation is not free.<br/>We are not responsible for costs incurred
+    while using our code.
+</h3>
+
+
+### Citation
+
+If you use ReSEval in an academic publication, please cite
+[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
+
+
+### IEEE
+
+M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
+
+
+### BibTex
+
+```
+@inproceedings{morrison2022reproducible,
+    title={Reproducible Subjective Evaluation},
+    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
+    booktitle={ICLR Workshop on ML Evaluation Standards},
+    month={April},
+    year={2022}
+}
+```
+
+
+## Table of contents
+- [Installation](#installation)
+    * [Deploying locally](#deploying-locally)
+- [Configuration](#configuration)
+- [Adding files](#adding-files)
+    * [AB](#ab)
+    * [ABX](#abx)
+    * [MOS](#mos)
+    * [MUSHRA](#mushra)
+    * [WordSelect](#wordselect)
+- [Credentials](#credentials)
+    * [Heroku](#heroku)
+    * [Amazon Web Services](#amazon-web-services)
+    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
+- [Usage](#usage)
+    * [Command-line interface](#command-line-interface)
+        * [Create](#create)
+        * [Monitor](#monitor)
+        * [Results](#results)
+        * [Pay](#pay)
+        * [Destroy](#destroy)
+        * [Extend](#extend)
+    * [Application programming interface](#application-programming-interface)
+- [Advanced usage](#advanced-usage)
+    * [CLI](#cli)
+    * [API](#api)
+- [Additional monitoring](#additional-monitoring)
+
+
+## Installation
+
+First, install the Python module. ReSEval requires Python 3.9 or higher.
+
+`pip install reseval`
+
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+
+```
+# Linux or OS X
+sudo npm install -g n
+sudo n 17.4.0
+
+# Windows
+# Must be run with administrator privileges
+nvm install 17.4.0
+nvm use 17.4.0
+```
+
+**Note** - You must restart your terminal after changing versions of node for the change to take effect
+
+### Deploying locally
+
+To be able to preview your subjective evaluation locally, you must
+[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+and obtain a username and password. The default username is `root`.
+
+Run the following to store the username and password in
+`reseval.CACHE / '.env'`.
+
+```
+python -m reseval.credentials \
+    --mysql_local_user <mysql_user> \
+    --mysql_local_password <mysql_local_password>
+```
+
+The `.env` file is used to set local environment variables and is not pushed to
+GitHub or uploaded to any remote storage.
+
+
+## Configuration
+
+All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
+
+
+## Adding files
+
+The files to be evaluated must be organized in a directory structure according
+to the type of test being run. The directory structures for each test are as
+follows. Examples of valid directories of evaluation files can be found in
+`examples/`.
+
+
+### AB
+
+```
+ab
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### ABX
+
+```
+abx
+└── reference
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### MOS
+
+```
+mos
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### MUSHRA
+
+```
+mushra
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### WordSelect
+
+```
+wordselect
+├── <file-0>
+├── <words-0>
+├── <file-1>
+├── <words-1>
+├── <file-2>
+├── <words-2>
+├── ...
+```
+
+`<words-x>` is `<file-x>` with `-words.txt` extension.
+
+
+## Credentials
+
+API keys are required to use the third-party services that ReSEval depends on.
+These are not required for local development. Do not share these API keys.
+
+
+### Amazon Web Services
+
+Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
+
+<p align="center">
+    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
+    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
+</p>
+
+Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
+
+
+### Amazon Mechanical Turk
+
+Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
+
+
+### Heroku (Optional if you don't want to use AWS)
+
+Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
+
+<p align="center">
+    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
+    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
+</p>
+
+You will also need to enable billing. You can do so [here](https://heroku.com/verify).
+
+
+## Usage
+
+Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
+
+If you are not deploying locally, add your API keys.
+
+```
+python -m reseval.credentials \
+    --aws_api_key <aws_api_key> \
+    --aws_api_secret_key <aws_api_secret_key> \
+    --heroku_api_key <heroku_api_key>
+```
+
+ API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
+
+
+### Command-line interface
+
+ Arguments for the following command-line interfaces are as follows, unless otherwise specified.
+
+- `<config>` - The configuration file
+- `<directory>` - The directory of evaluation files
+- `<name>` - The name of the evaluation given in the configuration file
+
+
+#### Create
+
+Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
+
+**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
+
+```
+# Local development
+python -m reseval.create <config> <directory> --local
+
+# Remote development
+python -m reseval.create <config> <directory>
+
+# Production
+python -m reseval.create <config> <directory> --production
+```
+
+
+#### Monitor
+
+```
+# Monitor all subjective evaluations
+python -m reseval.monitor
+
+# Monitor one subjective evaluation
+# The name of the evaluation can be found in its configuration file
+python -m reseval.monitor --name <name>
+```
+
+**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
+
+```
+# Update the monitor once every ten seconds
+python -m reseval.monitor --interval 10
+```
+
+
+#### Results
+
+```
+# Get the results of a subjective evaluation.
+# Results are stored in <directory>/<name>.
+# <directory> defaults to the current directory.
+python -m reseval.results <name> --directory <directory>
+```
+
+
+#### Pay
+
+```
+# Pay participants
+python -m reseval.pay <name>
+```
+
+
+#### Destroy
+
+```
+# Destroy the compute resources of a subjective evaluation (e.g., any cloud
+# storage, databases, or servers)
+python -m reseval.destroy <name>
+
+# Destroy a subjective evaluation even if it is still active.
+# Participants who have taken the test so far will be paid.
+python -m reseval.destroy <name> --force
+```
+
+
+#### Extend
+
+```
+# Add <participants> additional participants to a finished evaluation
+python -m reseval.extend <name> <participants>
+```
+
+
+### Application programming interface
+
+Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
+
+
+## Advanced usage
+
+Once you feel comfortable with using ReSEval step-by-step from the
+command-line and after you have added your credentials with
+`reseval.credentials`, you can use the CLI or API to run your evaluation with
+only a single command.
+
+
+### CLI
+
+```
+# Local development
+python -m reseval <config> <directory> --local
+
+# Remote development
+python -m reseval <config> <directory>
+
+# Production
+python -m reseval <config> <directory> --production
+```
+
+
+### API
+
+```
+import reseval
+
+# Local development
+reseval.run(config, directory, local=True)
+
+# Remote development
+reseval.run(config, directory)
+
+# Production
+reseval.run(config, directory, production=True)
+```
+
+
+## Additional monitoring
+
+### AWS S3
+
+To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
+[AWS S3 console](https://s3.console.aws.amazon.com/s3).
+
+
+### AWS Elastic Beanstalk
+
+To monitor, edit, or delete the server compute, use the
+[AWS Elastic Beanstalk console](https://console.aws.amazon.com/elasticbeanstalk).
+
+
+### AWS Relational Database Service
+
+To monitor, edit, or delete the database, use the
+[AWS RDS console](https://console.aws.amazon.com/rds).
+
+
+### MTurk
+
+HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
+You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
+on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
+at the end of the billing period.
+
+
+### Heroku
+
+To monitor, edit, or delete Heroku databases and servers, use the
+[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
+any costs on the
+[billing dashboard](https://dashboard.heroku.com/account/billing).
```

### Comparing `reseval-0.0.3/README.md` & `reseval-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,417 +1,459 @@
-# Reproducible Subjective Evaluation (ReSEval)
-[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
-[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
-
-ReSEval is a framework for quickly building subjective evaluations that are
-deployed on crowdworker platforms like
-[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
-A/B, ABX, MOS, and MUSHRA tests on audio, image, text, and video data.
-
-<h3 align="center">
-    While our code is free to use, performing crowdsourced subjective
-    evaluation is not free.<br/>We are not responsible for costs incurred
-    while using our code.
-</h3>
-
-
-### Citation
-
-If you use ReSEval in an academic publication, please cite
-[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
-
-
-### IEEE
-
-M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
-
-
-### BibTex
-
-```
-@inproceedings{morrison2022reproducible,
-    title={Reproducible Subjective Evaluation},
-    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
-    booktitle={ICLR Workshop on ML Evaluation Standards},
-    month={April},
-    year={2022}
-}
-```
-
-
-## Table of contents
-- [Installation](#installation)
-    * [Deploying locally](#deploying-locally)
-- [Configuration](#configuration)
-- [Adding files](#adding-files)
-    * [AB](#ab)
-    * [ABX](#abx)
-    * [MOS](#mos)
-    * [MUSHRA](#mushra)
-- [Credentials](#credentials)
-    * [Heroku](#heroku)
-    * [Amazon Web Services](#amazon-web-services)
-    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
-- [Usage](#usage)
-    * [Command-line interface](#command-line-interface)
-        * [Create](#create)
-        * [Monitor](#monitor)
-        * [Results](#results)
-        * [Pay](#pay)
-        * [Destroy](#destroy)
-        * [Extend](#extend)
-    * [Application programming interface](#application-programming-interface)
-- [Advanced usage](#advanced-usage)
-    * [CLI](#cli)
-    * [API](#api)
-- [Additional monitoring](#additional-monitoring)
-
-
-## Installation
-
-First, install the Python module. ReSEval requires Python 3.9 or higher.
-
-`pip install reseval`
-
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
-
-```
-# Linux or OS X
-sudo npm install -g n
-sudo n 17.4.0
-
-# Windows
-# Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
-```
-
-**Note** - You must restart your terminal after changing versions of node for the change to take effect
-
-### Deploying locally
-
-To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
-and obtain a username and password. The default username is `root`.
-
-Run the following to store the username and password in
-`reseval.CACHE / '.env'`.
-
-```
-python -m reseval.credentials \
-    --mysql_local_user <mysql_user> \
-    --mysql_local_password <mysql_local_password>
-```
-
-The `.env` file is used to set local environment variables and is not pushed to
-GitHub or uploaded to any remote storage.
-
-
-## Configuration
-
-All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
-
-
-## Adding files
-
-The files to be evaluated must be organized in a directory structure according
-to the type of test being run. The directory structures for each test are as
-follows. Examples of valid directories of evaluation files can be found in
-`examples/`.
-
-
-### AB
-
-```
-ab
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### ABX
-
-```
-abx
-└── reference
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### MOS
-
-```
-mos
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-### MUSHRA
-
-```
-mushra
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-## Credentials
-
-API keys are required to use the third-party services that ReSEval depends on.
-These are not required for local development. Do not share these API keys.
-
-
-### Heroku
-
-Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
-
-<p align="center">
-    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
-    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
-</p>
-
-You will also need to enable billing. You can do so [here](https://heroku.com/verify).
-
-
-### Amazon Web Services
-
-Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
-
-<p align="center">
-    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
-    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
-</p>
-
-
-### Amazon Mechanical Turk
-
-Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
-
-
-## Usage
-
-Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
-
-If you are not deploying locally, add your API keys.
-
-```
-python -m reseval.credentials \
-    --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
-    --heroku_api_key <heroku_api_key>
-```
-
- API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
-
-
-### Command-line interface
-
- Arguments for the following command-line interfaces are as follows, unless otherwise specified.
-
-- `<config>` - The configuration file
-- `<directory>` - The directory of evaluation files
-- `<name>` - The name of the evaluation given in the configuration file
-
-
-#### Create
-
-Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
-
-**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
-
-```
-# Local development
-python -m reseval.create <config> <directory> --local
-
-# Remote development
-python -m reseval.create <config> <directory>
-
-# Production
-python -m reseval.create <config> <directory> --production
-```
-
-
-#### Monitor
-
-```
-# Monitor all subjective evaluations
-python -m reseval.monitor
-
-# Monitor one subjective evaluation
-# The name of the evaluation can be found in its configuration file
-python -m reseval.monitor --name <name>
-```
-
-**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
-
-```
-# Update the monitor once every ten seconds
-python -m reseval.monitor --interval 10
-```
-
-
-#### Results
-
-```
-# Get the results of a subjective evaluation.
-# Results are stored in <directory>/<name>.
-# <directory> defaults to the current directory.
-python -m reseval.results <name> --directory <directory>
-```
-
-
-#### Pay
-
-```
-# Pay participants
-python -m reseval.pay <name>
-```
-
-
-#### Destroy
-
-```
-# Destroy the compute resources of a subjective evaluation (e.g., any cloud
-# storage, databases, or servers)
-python -m reseval.destroy <name>
-
-# Destroy a subjective evaluation even if it is still active.
-# Participants who have taken the test so far will be paid.
-python -m reseval.destroy <name> --force
-```
-
-
-#### Extend
-
-```
-# Add <participants> additional participants to a finished evaluation
-python -m reseval.extend <name> <participants>
-```
-
-
-### Application programming interface
-
-Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
-
-
-## Advanced usage
-
-Once you feel comfortable with using ReSEval step-by-step from the
-command-line and after you have added your credentials with
-`reseval.credentials`, you can use the CLI or API to run your evaluation with
-only a single command.
-
-
-### CLI
-
-```
-# Local development
-python -m reseval <config> <directory> --local
-
-# Remote development
-python -m reseval <config> <directory>
-
-# Production
-python -m reseval <config> <directory> --production
-```
-
-
-### API
-
-```
-import reseval
-
-# Local development
-reseval.run(config, directory, local=True)
-
-# Remote development
-reseval.run(config, directory)
-
-# Production
-reseval.run(config, directory, production=True)
-```
-
-
-## Additional monitoring
-
-### Heroku
-
-To monitor, edit, or delete Heroku databases and servers, use the
-[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
-any costs on the
-[billing dashboard](https://dashboard.heroku.com/account/billing).
-
-
-### AWS S3
-
-To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
-[AWS S3 console](https://aws.amazon.com/s3/).
-
-
-### MTurk
-
-HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
-You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
-on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
-at the end of the billing period.
+Metadata-Version: 2.1
+Name: reseval
+Version: 0.1.0
+Summary: Reproducible Subjective Evaluation
+Home-page: https://github.com/reseval/reseval
+Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
+Author-email: maxrmorrison@gmail.com
+Keywords: annotation,audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Reproducible Subjective Evaluation (ReSEval)
+[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
+
+ReSEval is a framework for quickly building subjective evaluation and
+annotation tasks that are deployed on crowdworker platforms like
+[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
+A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
+
+<h3 align="center">
+    While our code is free to use, performing crowdsourced subjective
+    evaluation is not free.<br/>We are not responsible for costs incurred
+    while using our code.
+</h3>
+
+
+### Citation
+
+If you use ReSEval in an academic publication, please cite
+[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
+
+
+### IEEE
+
+M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
+
+
+### BibTex
+
+```
+@inproceedings{morrison2022reproducible,
+    title={Reproducible Subjective Evaluation},
+    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
+    booktitle={ICLR Workshop on ML Evaluation Standards},
+    month={April},
+    year={2022}
+}
+```
+
+
+## Table of contents
+- [Installation](#installation)
+    * [Deploying locally](#deploying-locally)
+- [Configuration](#configuration)
+- [Adding files](#adding-files)
+    * [AB](#ab)
+    * [ABX](#abx)
+    * [MOS](#mos)
+    * [MUSHRA](#mushra)
+    * [WordSelect](#wordselect)
+- [Credentials](#credentials)
+    * [Heroku](#heroku)
+    * [Amazon Web Services](#amazon-web-services)
+    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
+- [Usage](#usage)
+    * [Command-line interface](#command-line-interface)
+        * [Create](#create)
+        * [Monitor](#monitor)
+        * [Results](#results)
+        * [Pay](#pay)
+        * [Destroy](#destroy)
+        * [Extend](#extend)
+    * [Application programming interface](#application-programming-interface)
+- [Advanced usage](#advanced-usage)
+    * [CLI](#cli)
+    * [API](#api)
+- [Additional monitoring](#additional-monitoring)
+
+
+## Installation
+
+First, install the Python module. ReSEval requires Python 3.9 or higher.
+
+`pip install reseval`
+
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+
+```
+# Linux or OS X
+sudo npm install -g n
+sudo n 17.4.0
+
+# Windows
+# Must be run with administrator privileges
+nvm install 17.4.0
+nvm use 17.4.0
+```
+
+**Note** - You must restart your terminal after changing versions of node for the change to take effect
+
+### Deploying locally
+
+To be able to preview your subjective evaluation locally, you must
+[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+and obtain a username and password. The default username is `root`.
+
+Run the following to store the username and password in
+`reseval.CACHE / '.env'`.
+
+```
+python -m reseval.credentials \
+    --mysql_local_user <mysql_user> \
+    --mysql_local_password <mysql_local_password>
+```
+
+The `.env` file is used to set local environment variables and is not pushed to
+GitHub or uploaded to any remote storage.
+
+
+## Configuration
+
+All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
+
+
+## Adding files
+
+The files to be evaluated must be organized in a directory structure according
+to the type of test being run. The directory structures for each test are as
+follows. Examples of valid directories of evaluation files can be found in
+`examples/`.
+
+
+### AB
+
+```
+ab
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### ABX
+
+```
+abx
+└── reference
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### MOS
+
+```
+mos
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### MUSHRA
+
+```
+mushra
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### WordSelect
+
+```
+wordselect
+├── <file-0>
+├── <words-0>
+├── <file-1>
+├── <words-1>
+├── <file-2>
+├── <words-2>
+├── ...
+```
+
+`<words-x>` is `<file-x>` with `-words.txt` extension.
+
+
+## Credentials
+
+API keys are required to use the third-party services that ReSEval depends on.
+These are not required for local development. Do not share these API keys.
+
+
+### Amazon Web Services
+
+Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
+
+<p align="center">
+    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
+    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
+</p>
+
+Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
+
+
+### Amazon Mechanical Turk
+
+Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
+
+
+### Heroku (Optional if you don't want to use AWS)
+
+Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
+
+<p align="center">
+    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
+    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
+</p>
+
+You will also need to enable billing. You can do so [here](https://heroku.com/verify).
+
+
+## Usage
+
+Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
+
+If you are not deploying locally, add your API keys.
+
+```
+python -m reseval.credentials \
+    --aws_api_key <aws_api_key> \
+    --aws_api_secret_key <aws_api_secret_key> \
+    --heroku_api_key <heroku_api_key>
+```
+
+ API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
+
+
+### Command-line interface
+
+ Arguments for the following command-line interfaces are as follows, unless otherwise specified.
+
+- `<config>` - The configuration file
+- `<directory>` - The directory of evaluation files
+- `<name>` - The name of the evaluation given in the configuration file
+
+
+#### Create
+
+Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
+
+**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
+
+```
+# Local development
+python -m reseval.create <config> <directory> --local
+
+# Remote development
+python -m reseval.create <config> <directory>
+
+# Production
+python -m reseval.create <config> <directory> --production
+```
+
+
+#### Monitor
+
+```
+# Monitor all subjective evaluations
+python -m reseval.monitor
+
+# Monitor one subjective evaluation
+# The name of the evaluation can be found in its configuration file
+python -m reseval.monitor --name <name>
+```
+
+**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
+
+```
+# Update the monitor once every ten seconds
+python -m reseval.monitor --interval 10
+```
+
+
+#### Results
+
+```
+# Get the results of a subjective evaluation.
+# Results are stored in <directory>/<name>.
+# <directory> defaults to the current directory.
+python -m reseval.results <name> --directory <directory>
+```
+
+
+#### Pay
+
+```
+# Pay participants
+python -m reseval.pay <name>
+```
+
+
+#### Destroy
+
+```
+# Destroy the compute resources of a subjective evaluation (e.g., any cloud
+# storage, databases, or servers)
+python -m reseval.destroy <name>
+
+# Destroy a subjective evaluation even if it is still active.
+# Participants who have taken the test so far will be paid.
+python -m reseval.destroy <name> --force
+```
+
+
+#### Extend
+
+```
+# Add <participants> additional participants to a finished evaluation
+python -m reseval.extend <name> <participants>
+```
+
+
+### Application programming interface
+
+Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
+
+
+## Advanced usage
+
+Once you feel comfortable with using ReSEval step-by-step from the
+command-line and after you have added your credentials with
+`reseval.credentials`, you can use the CLI or API to run your evaluation with
+only a single command.
+
+
+### CLI
+
+```
+# Local development
+python -m reseval <config> <directory> --local
+
+# Remote development
+python -m reseval <config> <directory>
+
+# Production
+python -m reseval <config> <directory> --production
+```
+
+
+### API
+
+```
+import reseval
+
+# Local development
+reseval.run(config, directory, local=True)
+
+# Remote development
+reseval.run(config, directory)
+
+# Production
+reseval.run(config, directory, production=True)
+```
+
+
+## Additional monitoring
+
+### AWS S3
+
+To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
+[AWS S3 console](https://s3.console.aws.amazon.com/s3).
+
+
+### AWS Elastic Beanstalk
+
+To monitor, edit, or delete the server compute, use the
+[AWS Elastic Beanstalk console](https://console.aws.amazon.com/elasticbeanstalk).
+
+
+### AWS Relational Database Service
+
+To monitor, edit, or delete the database, use the
+[AWS RDS console](https://console.aws.amazon.com/rds).
+
+
+### MTurk
+
+HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
+You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
+on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
+at the end of the billing period.
+
+
+### Heroku
+
+To monitor, edit, or delete Heroku databases and servers, use the
+[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
+any costs on the
+[billing dashboard](https://dashboard.heroku.com/account/billing).
```

### Comparing `reseval-0.0.3/reseval/app/heroku.py` & `reseval-0.1.0/reseval/app/heroku.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,62 @@
-import json
-import os
-import string
-
-import heroku3
-
-import reseval
-
-
-def configure(name, key, value):
-    """Add an environment variable to a Heroku application"""
-    # Get Heroku application
-    app = get(name)
-
-    # Set environment variable
-    app.config()[key] = value
-
-
-def connect():
-    """Connect to Heroku"""
-    reseval.load.api_keys()
-    return heroku3.from_key(os.environ['HerokuAccessKey'])
-
-
-def create(config):
-    """Create a Heroku web application"""
-    # Create a globally unique name to prevent collision
-    name = (
-        reseval.random.string(1, string.ascii_lowercase) +
-        reseval.random.string(23))
-
-    # Create Heroku app
-    connect().create_app(name=name)
-
-    # Save name as application credentials
-    credentials_file = (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        'app.json')
-    credentials_file.parent.mkdir(exist_ok=True, parents=True)
-    with open(credentials_file, 'w') as file:
-        json.dump({'name': name}, file)
-
-
-def destroy(config):
-    """Destroy a Heroku app"""
-    try:
-
-        # Destroy app
-        get(config['name']).delete()
-
-    except (FileNotFoundError, KeyError):
-
-        # Handle app not existing
-        pass
-
-    # Delete credentials file
-    (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        'app.json'
-    ).unlink(missing_ok=True)
-
-
-def get(name):
-    """Retrieve a Heroku application"""
-    # Load application credentials
-    credentials = reseval.load.credentials_by_name(name, 'app')
-
-    # Get Heroku application
-    return connect().apps()[credentials['name']]
+import os
+
+import heroku3
+
+import reseval
+
+
+def configure(name, key, value):
+    """Add an environment variable to a Heroku application"""
+    # Get Heroku application
+    app = get(name)
+
+    # Set environment variable
+    app.config()[key] = value
+
+
+def connect():
+    """Connect to Heroku"""
+    reseval.load.api_keys()
+    return heroku3.from_key(os.environ['HerokuAccessKey'])
+
+
+def create(name):
+    """Create a Heroku web application"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Create Heroku app
+    connect().create_app(name=unique)
+
+
+def destroy(name):
+    """Destroy a Heroku app"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    try:
+
+        # Destroy app
+        get(unique).delete()
+
+    except (FileNotFoundError, KeyError):
+
+        # Handle app not existing
+        pass
+
+    # Delete credentials file
+    (
+        reseval.EVALUATION_DIRECTORY /
+        name /
+        'credentials' /
+        'app.json'
+    ).unlink(missing_ok=True)
+
+
+def get(name):
+    """Retrieve a Heroku application"""
+    # Load application credentials
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Get Heroku application
+    return connect().apps()[unique]
```

### Comparing `reseval-0.0.3/reseval/assets/client/public/favicon.ico` & `reseval-0.1.0/reseval/assets/client/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/client/public/index.html` & `reseval-0.1.0/reseval/assets/client/public/index.html`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-<!DOCTYPE html>
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
-    <meta name="viewport" content="width=device-width, initial-scale=1" />
-    <meta name="theme-color" content="#000000" />
-    <meta
-      name="description"
-      content="Reproducible Subjective Evaluation (ReSEval)"
-    />
-    <link rel="apple-touch-icon" href="%PUBLIC_URL%/logo192.png" />
-    <!--
-      manifest.json provides metadata used when your web app is installed on a
-      user's mobile device or desktop. See https://developers.google.com/web/fundamentals/web-app-manifest/
-    -->
-    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
-    <!--
-      Notice the use of %PUBLIC_URL% in the tags above.
-      It will be replaced with the URL of the `public` folder during the build.
-      Only files inside the `public` folder can be referenced from the HTML.
-
-      Unlike "/favicon.ico" or "favicon.ico", "%PUBLIC_URL%/favicon.ico" will
-      work correctly both with client-side routing and a non-root public URL.
-      Learn how to configure a non-root public URL by running `npm run build`.
-    -->
-
-    <title>ReSEval</title>
-  </head>
-  <body>
-    <noscript>You need to enable JavaScript to run this app.</noscript>
-    <div id="root"></div>
-    <!--
-      This HTML file is a template.
-      If you open it directly in the browser, you will see an empty page.
-
-      You can add webfonts, meta tags, or analytics to this file.
-      The build step will place the bundled scripts into the <body> tag.
-
-      To begin the development, run `npm start` or `yarn start`.
-      To create a production bundle, use `npm run build` or `yarn build`.
-    -->
-  </body>
-</html>
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8" />
+    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
+    <meta name="viewport" content="width=device-width, initial-scale=1" />
+    <meta name="theme-color" content="#000000" />
+    <meta
+      name="description"
+      content="Reproducible Subjective Evaluation (ReSEval)"
+    />
+    <link rel="apple-touch-icon" href="%PUBLIC_URL%/logo192.png" />
+    <!--
+      manifest.json provides metadata used when your web app is installed on a
+      user's mobile device or desktop. See https://developers.google.com/web/fundamentals/web-app-manifest/
+    -->
+    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
+    <!--
+      Notice the use of %PUBLIC_URL% in the tags above.
+      It will be replaced with the URL of the `public` folder during the build.
+      Only files inside the `public` folder can be referenced from the HTML.
+
+      Unlike "/favicon.ico" or "favicon.ico", "%PUBLIC_URL%/favicon.ico" will
+      work correctly both with client-side routing and a non-root public URL.
+      Learn how to configure a non-root public URL by running `npm run build`.
+    -->
+
+    <title>ReSEval</title>
+  </head>
+  <body>
+    <noscript>You need to enable JavaScript to run this app.</noscript>
+    <div id="root"></div>
+    <!--
+      This HTML file is a template.
+      If you open it directly in the browser, you will see an empty page.
+
+      You can add webfonts, meta tags, or analytics to this file.
+      The build step will place the bundled scripts into the <body> tag.
+
+      To begin the development, run `npm start` or `yarn start`.
+      To create a production bundle, use `npm run build` or `yarn build`.
+    -->
+  </body>
+</html>
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/Survey.js` & `reseval-0.1.0/reseval/assets/client/src/Survey.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,137 +1,137 @@
-import Chance from 'chance';
-import React, {
-    useState
-} from 'react';
-import {
-    useStep
-} from 'react-hooks-helper';
-
-import './css/components.css';
-
-import EndPage from './pages/EndPage';
-import FeedbackPage from './pages/FeedbackPage';
-import QualificationPage from './pages/QualificationPage';
-import TaskPage from './pages/TaskPage';
-import WelcomePage from './pages/WelcomePage';
-
-
-/******************************************************************************
- Constants
- ******************************************************************************/
-
-
-// Random number generator
-const chance = new Chance();
-
-// Completion code for participant
-const completionCode = chance.string({
-    length: 10
-});
-
-// Chronological ordering of pages visited by participants during evaluation
-const steps = [{
-    id: 'welcome'
-}, {
-    id: 'prescreen'
-}, {
-    id: 'task'
-}, {
-    id: 'feedback'
-}, {
-    id: 'end'
-}];
-
-
-/******************************************************************************
- Subjective evaluation survey
- ******************************************************************************/
-
-
-export default function Survey() {
-    /* Page navigation management for surveys */
-    // Start at the welcome page
-    const {
-        step,
-        navigation
-    } = useStep({
-        initialStep: 0,
-        steps
-    });
-
-    // Participant id
-    const [participant, setParticipant] = useState(undefined);
-
-    // Evaluation conditions
-    const [conditions, setConditions] = useState(undefined);
-
-    // Evaluation files
-    const [files, setFiles] = useState(undefined);
-    // Evaluator Id; this is an incremental integer id starts from 0
-    const [evaluatorId, setEvaluatorId] = useState(undefined);
-    // Render current page
-    switch (step.id) {
-        case 'welcome':
-            return < WelcomePage navigation = {
-                navigation
-            }
-            />;
-        case 'prescreen':
-            return < QualificationPage
-            participant = {
-                participant
-            }
-            setParticipant = {
-                setParticipant
-            }
-            completionCode = {
-                completionCode
-            }
-            setFiles = {
-                setFiles
-            }
-            setConditions = {
-                setConditions
-            }
-            setEvaluatorId = {
-                setEvaluatorId
-            }
-            navigation = {
-                navigation
-            }
-            />;
-        case 'task':
-            return < TaskPage
-            files = {
-                files
-            }
-            conditions = {
-                conditions
-            }
-            participant = {
-                participant
-            }
-            navigation = {
-                navigation
-            }
-            evaluatorId = {
-                evaluatorId
-            }
-            />;
-        case 'feedback':
-            return < FeedbackPage
-            navigation = {
-                navigation
-            }
-            participant = {
-                participant
-            }
-            />;
-        case 'end':
-            return < EndPage completionCode = {
-                completionCode
-            }
-            />;
-        default:
-            return
-    }
-};
+import Chance from 'chance';
+import React, {
+    useState
+} from 'react';
+import {
+    useStep
+} from 'react-hooks-helper';
+
+import './css/components.css';
+
+import EndPage from './pages/EndPage';
+import FeedbackPage from './pages/FeedbackPage';
+import QualificationPage from './pages/QualificationPage';
+import TaskPage from './pages/TaskPage';
+import WelcomePage from './pages/WelcomePage';
+
+
+/******************************************************************************
+ Constants
+ ******************************************************************************/
+
+
+// Random number generator
+const chance = new Chance();
+
+// Completion code for participant
+const completionCode = chance.string({
+    length: 10
+});
+
+// Chronological ordering of pages visited by participants during evaluation
+const steps = [{
+    id: 'welcome'
+}, {
+    id: 'prescreen'
+}, {
+    id: 'task'
+}, {
+    id: 'feedback'
+}, {
+    id: 'end'
+}];
+
+
+/******************************************************************************
+ Subjective evaluation survey
+ ******************************************************************************/
+
+
+export default function Survey() {
+    /* Page navigation management for surveys */
+    // Start at the welcome page
+    const {
+        step,
+        navigation
+    } = useStep({
+        initialStep: 0,
+        steps
+    });
+
+    // Participant id
+    const [participant, setParticipant] = useState(undefined);
+
+    // Evaluation conditions
+    const [conditions, setConditions] = useState(undefined);
+
+    // Evaluation files
+    const [files, setFiles] = useState(undefined);
+    // Evaluator Id; this is an incremental integer id starts from 0
+    const [evaluatorId, setEvaluatorId] = useState(undefined);
+    // Render current page
+    switch (step.id) {
+        case 'welcome':
+            return < WelcomePage navigation = {
+                navigation
+            }
+            />;
+        case 'prescreen':
+            return < QualificationPage
+            participant = {
+                participant
+            }
+            setParticipant = {
+                setParticipant
+            }
+            completionCode = {
+                completionCode
+            }
+            setFiles = {
+                setFiles
+            }
+            setConditions = {
+                setConditions
+            }
+            setEvaluatorId = {
+                setEvaluatorId
+            }
+            navigation = {
+                navigation
+            }
+            />;
+        case 'task':
+            return < TaskPage
+            files = {
+                files
+            }
+            conditions = {
+                conditions
+            }
+            participant = {
+                participant
+            }
+            navigation = {
+                navigation
+            }
+            evaluatorId = {
+                evaluatorId
+            }
+            />;
+        case 'feedback':
+            return < FeedbackPage
+            navigation = {
+                navigation
+            }
+            participant = {
+                participant
+            }
+            />;
+        case 'end':
+            return < EndPage completionCode = {
+                completionCode
+            }
+            />;
+        default:
+            return
+    }
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/components/Audio.js` & `reseval-0.1.0/reseval/assets/client/src/components/Video.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,43 +1,51 @@
-import React, {
-    useEffect
-} from 'react';
-
-import '../css/components.css';
-
-export default function Audio({
-    src,
-    reference,
-    onEnded,
-    onPlayed
-}) {
-    /* Create an HTML audio element */
-    // Reload audio when src changes
-    useEffect(() => {
-        if (typeof reference !== 'undefined' && reference.current) {
-            reference.current.pause();
-            reference.current.load();
-        }
-    }, [reference, src]);
-
-    // Render
-    return ( <
-        audio className = 'audio-single'
-        controls controlsList = 'nodownload'
-        ref = {
-            reference
-        }
-        onPlay = {
-            () => typeof(onPlayed) !== 'undefined' && onPlayed()
-        }
-        onEnded = {
-            () => typeof(onEnded) !== 'undefined' && onEnded()
-        } >
-        <
-        source src = {
-            src
-        }
-        type = 'audio/mpeg' / >
-        <
-        /audio>
-    );
-};
+import React, {
+    useEffect
+} from 'react';
+
+import '../css/components.css';
+
+export default function Video({
+    src,
+    reference,
+    onEnded,
+    onStarted,
+    onPlay
+}) {
+    /* Create an HTML video element */
+    // Reload video when src changes
+    useEffect(() => {
+        if (reference.current) {
+            reference.current.pause();
+            reference.current.load();
+        }
+    }, [reference, src]);
+
+    // Render
+    return ( <
+        video controls ref = {
+            reference
+        }
+        style = {
+            {
+                minWidth: '150px',
+                maxWidth: '750px'
+            }
+        }
+        onPlay = {
+            () => {
+                if (typeof(onStarted) !== 'undefined') onStarted();
+                if (typeof(onPlay) !== 'undefined') onPlay();
+            }
+        }
+        onEnded = {
+            () => typeof(onEnded) !== 'undefined' && onEnded()
+        } >
+        <
+        source src = {
+            src
+        }
+        type = 'video/mp4' / >
+        <
+        /video>
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/components/Media.js` & `reseval-0.1.0/reseval/assets/client/src/components/Media.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,114 +1,114 @@
-import React, {
-    useContext
-} from 'react';
-
-import Audio from './Audio';
-import Image from './Image';
-import Text from './Text';
-import Video from './Video';
-
-import config from '../json/config.json';
-import {
-    MediaContext
-} from "../pages/TaskPage";
-
-
-/******************************************************************************
- Render media objects (audio, image, etc.)
- ******************************************************************************/
-
-
-export default function Media(props) {
-    /* Render a media object (audio, image, etc.) */
-    // Retrieve the global state, which contains any currently playing media
-    let {
-        mediaRef,
-        setMediaRef
-    } = useContext(MediaContext);
-
-    function onPlayed() {
-        if (mediaRef !== props.reference) {
-
-            // Do nothing if it is the same media that is being played
-            if (mediaRef !== undefined && mediaRef.current !== undefined) {
-
-                // Pause old media to prevent both playing simultaneously
-                mediaRef.current.pause()
-
-                // Set the play head to the beginning
-                mediaRef.current.currentTime = 0
-            }
-
-            // Replace the media in the context
-            setMediaRef(props.reference)
-        }
-    }
-
-    // Add callback prop
-    const newProps = {
-        ...props
-    };
-    newProps.onPlayed = onPlayed;
-
-    // Update file source prop
-    if (config['local']) {
-        newProps.src = '/evaluation-files/' + newProps.src;
-    } else {
-        switch (config.storage) {
-            case 'aws':
-                newProps.src = `https://${config['bucket']}.s3.amazonaws.com/${newProps.src}`;
-                break;
-            default:
-                throw new Error(
-                    `Storage location ${config.storage} is not recognized`);
-        }
-    }
-
-    // Lock props
-    Object.preventExtensions(newProps);
-
-    // Get datatype
-    let media;
-    switch (config.datatype) {
-        case 'audio':
-            media = < Audio {
-                ...newProps
-            }
-            />;
-            break;
-        case 'image':
-            media = < Image {
-                ...newProps
-            }
-            />;
-            break;
-        case 'text':
-            media = < Text {
-                ...newProps
-            }
-            />;
-            break;
-        case 'video':
-            media = < Video {
-                ...newProps
-            }
-            />;
-            break;
-        default:
-            throw new Error(`Datatype ${config.datatype} is not recognized`);
-    }
-
-    return ( <
-        div style = {
-            {
-                display: 'flex',
-                justifyContent: 'center',
-                padding: '10px'
-            }
-        } >
-        {
-            media
-        } <
-        /div>
-    );
+import React, {
+    useContext
+} from 'react';
+
+import Audio from './Audio';
+import Image from './Image';
+import Text from './Text';
+import Video from './Video';
+
+import config from '../json/config.json';
+import {
+    MediaContext
+} from "../pages/TaskPage";
+
+
+/******************************************************************************
+ Render media objects (audio, image, etc.)
+ ******************************************************************************/
+
+
+export default function Media(props) {
+    /* Render a media object (audio, image, etc.) */
+    // Retrieve the global state, which contains any currently playing media
+    let {
+        mediaRef,
+        setMediaRef
+    } = useContext(MediaContext);
+
+    function onPlay() {
+        if (mediaRef !== props.reference) {
+
+            // Do nothing if it is the same media that is being played
+            if (mediaRef !== undefined && mediaRef.current !== undefined) {
+
+                // Pause old media to prevent both playing simultaneously
+                mediaRef.current.pause()
+
+                // Set the play head to the beginning
+                mediaRef.current.currentTime = 0
+            }
+
+            // Replace the media in the context
+            setMediaRef(props.reference)
+        }
+    }
+
+    // Add callback prop
+    const newProps = {
+        ...props
+    };
+    newProps.onPlay = onPlay;
+
+    // Update file source prop
+    if (config['local']) {
+        newProps.src = '/evaluation-files/' + newProps.src;
+    } else {
+        switch (config.storage) {
+            case 'aws':
+                newProps.src = `https://${config['bucket']}.s3.amazonaws.com/${newProps.src}`;
+                break;
+            default:
+                throw new Error(
+                    `Storage location ${config.storage} is not recognized`);
+        }
+    }
+
+    // Lock props
+    Object.preventExtensions(newProps);
+
+    // Get datatype
+    let media;
+    switch (config.datatype) {
+        case 'audio':
+            media = < Audio {
+                ...newProps
+            }
+            />;
+            break;
+        case 'image':
+            media = < Image {
+                ...newProps
+            }
+            />;
+            break;
+        case 'text':
+            media = < Text {
+                ...newProps
+            }
+            />;
+            break;
+        case 'video':
+            media = < Video {
+                ...newProps
+            }
+            />;
+            break;
+        default:
+            throw new Error(`Datatype ${config.datatype} is not recognized`);
+    }
+
+    return ( <
+        div style = {
+            {
+                display: 'flex',
+                justifyContent: 'center',
+                padding: '10px'
+            }
+        } >
+        {
+            media
+        } <
+        /div>
+    );
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/components/MediaRadioButtonGroup.js` & `reseval-0.1.0/reseval/assets/client/src/components/RadioButtonGroup.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,98 +1,90 @@
-import React from 'react';
-
-import Media from './Media';
-
-import '../css/components.css';
-
-
-/******************************************************************************
-Radio buttons with corresponding media (audio, image, etc.)
-******************************************************************************/
-
-
-function MediaRadioButton({
-    file,
-    condition,
-    response,
-    setResponse,
-    reference,
-    active,
-    onEnded
-}) {
-    /* Create a media element with a corresponding radio button */
-    // Get radio button state
-    let state = active ? 'active' : '';
-    if (active && condition === response) {
-        state = 'active selected';
-    }
-
-    // Render radio button and media
-    return ( <
-        li className = 'listitem grid grid-20-80' >
-        <
-        div className = {
-            `check col-1 ${state}`
-        }
-        onClick = {
-            () => active && setResponse(condition)
-        } >
-        <
-        div className = 'inside' / >
-        <
-        /div> <
-        Media src = {
-            condition + '/' + file
-        }
-        reference = {
-            reference
-        }
-        onEnded = {
-            onEnded
-        }
-        /> <
-        /li>
-    );
-};
-
-export default function MediaRadioButtonGroup({
-    file,
-    conditions,
-    response,
-    setResponse,
-    references,
-    active,
-    onEndeds
-}) {
-    /* Create a group of media elements with corresponding radio buttons */
-    const radioButtonGroup = conditions.map((condition, key) =>
-        <
-        MediaRadioButton file = {
-            file
-        }
-        condition = {
-            condition
-        }
-        key = {
-            key
-        }
-        response = {
-            response
-        }
-        setResponse = {
-            setResponse
-        }
-        reference = {
-            references[key]
-        }
-        active = {
-            active
-        }
-        onEnded = {
-            onEndeds[key]
-        }
-        />
-    );
-    return < ul > {
-        radioButtonGroup
-    } < /ul>;
-};
+import React from 'react';
+
+import '../css/components.css';
+
+
+/******************************************************************************
+Radio buttons
+******************************************************************************/
+
+
+export default function RadioButtonGroup({
+    response,
+    setResponse,
+    active
+}) {
+    /* Create a group of radio buttons */
+    const choices = 5;
+
+    // Radio buttons
+    const buttons = [...Array(choices).keys()].map(index => {
+
+        // Get radio button state
+        let state = active ? 'active' : '';
+        if (index + 1 === response) {
+            state = 'active selected';
+        }
+
+        // Render a button
+        return ( <
+            RadioButtonText onClick = {
+                () => active && setResponse(index + 1)
+            }
+            state = {
+                state
+            }
+            text = {
+                index + 1
+            }
+            />
+        );
+    });
+
+    // Render button group
+    return ( <
+        ul >
+        <
+        li className = ' listitem grid'
+        style = {
+            {
+                gridTemplateColumns: `repeat(${choices}, 1fr)`
+            }
+        } >
+        {
+            buttons
+        } <
+        /li> <
+        /ul>
+    );
+}
+
+function RadioButtonText({
+    onClick,
+    state,
+    text
+}) {
+    /* Render a radio button with corresponding text */
+    return ( <
+        div style = {
+            {
+                margin: 'auto',
+                textAlign: 'center'
+            }
+        } >
+        <
+        div className = {
+            `check col-1 ${state}`
+        }
+        onClick = {
+            onClick
+        } >
+        <
+        div className = 'inside' / >
+        <
+        /div> <
+        p > {
+            text
+        } < /p> <
+        /div>
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/components/MediaSliderGroup.js` & `reseval-0.1.0/reseval/assets/client/src/components/MediaSliderGroup.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,233 +1,233 @@
-import React from 'react';
-import Slider from 'rc-slider';
-
-import Media from './Media';
-
-import 'rc-slider/assets/index.css';
-
-import '../css/components.css';
-
-import config from '../json/config.json'
-
-
-/******************************************************************************
- Radio buttons with corresponding media (audio, image, etc.)
- ******************************************************************************/
-
-
-function MediaSlider({
-    file,
-    condition,
-    permutation,
-    index,
-    scores,
-    setScores,
-    setResponse,
-    reference,
-    endeds,
-    setEndeds,
-    toucheds,
-    setToucheds
-}) {
-    /* Create a media element with a corresponding slider */
-    function onChange(value) {
-        /* Update scores */
-        setScores(scores.map((score, i) => i === index ? value : score));
-
-        // Pad with leading zeros
-        const padded = scores.map(score => String(score).padStart(3, '0'));
-
-        // Undo permutation
-        const reverse_permutation = Array.from(
-                Array(permutation.length).keys())
-            .sort((a, b) => {
-                return (
-                    permutation[a] < permutation[b] ? -1 :
-                    (permutation[b] < permutation[a]) | 0
-                );
-            });
-
-        // Response is concatenation of zero-padded scores
-        setResponse(
-            reverse_permutation.map((index) => padded[index]).join(''));
-
-        // Set slider touchedness to be true
-        setToucheds(
-            toucheds.map((touched, i) => i === index ? true : touched));
-    }
-
-    function onEnded() {
-        /* Update what media has ended */
-        // If this is an image or text, they end immediately
-        const makeAllTrue = ['image', 'text'].includes(config.datatype);
-        setEndeds(endeds.map(
-            (ended, i) => i === index || makeAllTrue ? true : ended));
-    }
-
-    // Render slider and media
-    return ( <
-        div style = {
-            {
-                gridColumn: index + 1,
-                height: '500px',
-                justifyContent: 'center',
-                alignItems: 'center'
-            }
-        } >
-        <
-        div style = {
-            {
-                display: 'flex',
-                height: '300px',
-                justifyContent: 'center',
-                alignItems: 'center'
-            }
-        } >
-        <
-        Slider value = {
-            scores[index]
-        }
-        defaultValue = {
-            50
-        }
-        startPoint = {
-            50
-        }
-        marks = {
-            {
-                0: 0,
-                25: 25,
-                50: 50,
-                75: 75,
-                100: 100
-            }
-        }
-        vertical = {
-            true
-        }
-        disabled = {
-            !endeds[index]
-        }
-        onChange = {
-            onChange
-        }
-        railStyle = {
-            {
-                backgroundColor: 'black'
-            }
-        }
-        trackStyle = {
-            {
-                backgroundColor: 'black'
-            }
-        }
-        dotStyle = {
-            {
-                backgroundColor: 'black',
-                borderColor: 'black'
-            }
-        }
-        activeDotStyle = {
-            {
-                backgroundColor: 'black',
-                borderColor: 'black'
-            }
-        }
-        handleStyle = {
-            {
-                width: 20,
-                height: 20,
-                marginLeft: -8,
-                backgroundColor: 'black',
-                borderColor: 'white'
-            }
-        }
-        /> <
-        /div> <
-        Media src = {
-            condition + '/' + file
-        }
-        reference = {
-            reference
-        }
-        onEnded = {
-            onEnded
-        }
-        /> <
-        /div>
-    );
-};
-
-export default function MediaSliderGroup({
-    file,
-    conditions,
-    permutation,
-    scores,
-    setScores,
-    setResponse,
-    refs,
-    endeds,
-    setEndeds,
-    toucheds,
-    setToucheds
-}) {
-    /* Create a group of media elements with corresponding sliders */
-    const sliderGroup = conditions.map((condition, key) =>
-        <
-        MediaSlider file = {
-            file
-        }
-        condition = {
-            condition
-        }
-        permutation = {
-            permutation
-        }
-        index = {
-            key
-        }
-        key = {
-            key
-        }
-        scores = {
-            scores
-        }
-        setScores = {
-            setScores
-        }
-        setResponse = {
-            setResponse
-        }
-        reference = {
-            refs[key]
-        }
-        endeds = {
-            endeds
-        }
-        setEndeds = {
-            setEndeds
-        }
-        toucheds = {
-            toucheds
-        }
-        setToucheds = {
-            setToucheds
-        }
-        />
-    );
-    return ( <
-        div style = {
-            {
-                display: 'grid',
-                gridTemplateColumns: `repeat(${conditions.length}, 1fr)`,
-                height: '500px',
-                gridTemplateRows: '500px'
-            }
-        }
-        className = 'mediaSliderGrid' >
-        {
-            sliderGroup
-        } <
-        /div>
-    );
-};
+import React from 'react';
+import Slider from 'rc-slider';
+
+import Media from './Media';
+
+import 'rc-slider/assets/index.css';
+
+import '../css/components.css';
+
+import config from '../json/config.json'
+
+
+/******************************************************************************
+ Radio buttons with corresponding media (audio, image, etc.)
+ ******************************************************************************/
+
+
+function MediaSlider({
+    file,
+    condition,
+    permutation,
+    index,
+    scores,
+    setScores,
+    setResponse,
+    reference,
+    endeds,
+    setEndeds,
+    toucheds,
+    setToucheds
+}) {
+    /* Create a media element with a corresponding slider */
+    function onChange(value) {
+        /* Update scores */
+        setScores(scores.map((score, i) => i === index ? value : score));
+
+        // Pad with leading zeros
+        const padded = scores.map(score => String(score).padStart(3, '0'));
+
+        // Undo permutation
+        const reverse_permutation = Array.from(
+                Array(permutation.length).keys())
+            .sort((a, b) => {
+                return (
+                    permutation[a] < permutation[b] ? -1 :
+                    (permutation[b] < permutation[a]) | 0
+                );
+            });
+
+        // Response is concatenation of zero-padded scores
+        setResponse(
+            reverse_permutation.map((index) => padded[index]).join(''));
+
+        // Set slider touchedness to be true
+        setToucheds(
+            toucheds.map((touched, i) => i === index ? true : touched));
+    }
+
+    function onEnded() {
+        /* Update what media has ended */
+        // If this is an image or text, they end immediately
+        const makeAllTrue = ['image', 'text'].includes(config.datatype);
+        setEndeds(endeds.map(
+            (ended, i) => i === index || makeAllTrue ? true : ended));
+    }
+
+    // Render slider and media
+    return ( <
+        div style = {
+            {
+                gridColumn: index + 1,
+                height: '500px',
+                justifyContent: 'center',
+                alignItems: 'center'
+            }
+        } >
+        <
+        div style = {
+            {
+                display: 'flex',
+                height: '300px',
+                justifyContent: 'center',
+                alignItems: 'center'
+            }
+        } >
+        <
+        Slider value = {
+            scores[index]
+        }
+        defaultValue = {
+            50
+        }
+        startPoint = {
+            50
+        }
+        marks = {
+            {
+                0: 0,
+                25: 25,
+                50: 50,
+                75: 75,
+                100: 100
+            }
+        }
+        vertical = {
+            true
+        }
+        disabled = {
+            !endeds[index]
+        }
+        onChange = {
+            onChange
+        }
+        railStyle = {
+            {
+                backgroundColor: 'black'
+            }
+        }
+        trackStyle = {
+            {
+                backgroundColor: 'black'
+            }
+        }
+        dotStyle = {
+            {
+                backgroundColor: 'black',
+                borderColor: 'black'
+            }
+        }
+        activeDotStyle = {
+            {
+                backgroundColor: 'black',
+                borderColor: 'black'
+            }
+        }
+        handleStyle = {
+            {
+                width: 20,
+                height: 20,
+                marginLeft: -8,
+                backgroundColor: 'black',
+                borderColor: 'white'
+            }
+        }
+        /> <
+        /div> <
+        Media src = {
+            condition + '/' + file
+        }
+        reference = {
+            reference
+        }
+        onEnded = {
+            onEnded
+        }
+        /> <
+        /div>
+    );
+}
+
+export default function MediaSliderGroup({
+    file,
+    conditions,
+    permutation,
+    scores,
+    setScores,
+    setResponse,
+    refs,
+    endeds,
+    setEndeds,
+    toucheds,
+    setToucheds
+}) {
+    /* Create a group of media elements with corresponding sliders */
+    const sliderGroup = conditions.map((condition, key) =>
+        <
+        MediaSlider file = {
+            file
+        }
+        condition = {
+            condition
+        }
+        permutation = {
+            permutation
+        }
+        index = {
+            key
+        }
+        key = {
+            key
+        }
+        scores = {
+            scores
+        }
+        setScores = {
+            setScores
+        }
+        setResponse = {
+            setResponse
+        }
+        reference = {
+            refs[key]
+        }
+        endeds = {
+            endeds
+        }
+        setEndeds = {
+            setEndeds
+        }
+        toucheds = {
+            toucheds
+        }
+        setToucheds = {
+            setToucheds
+        }
+        />
+    );
+    return ( <
+        div style = {
+            {
+                display: 'grid',
+                gridTemplateColumns: `repeat(${conditions.length}, 1fr)`,
+                height: '500px',
+                gridTemplateRows: '500px'
+            }
+        }
+        className = 'mediaSliderGrid' >
+        {
+            sliderGroup
+        } <
+        /div>
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/components/Video.js` & `reseval-0.1.0/reseval/assets/client/src/components/Audio.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,47 +1,47 @@
-import React, {
-    useEffect
-} from 'react';
-
-import '../css/components.css';
-
-export default function Video({
-    src,
-    reference,
-    onEnded,
-    onPlayed
-}) {
-    /* Create an HTML video element */
-    // Reload video when src changes
-    useEffect(() => {
-        if (reference.current) {
-            reference.current.pause();
-            reference.current.load();
-        }
-    }, [reference, src]);
-
-    // Render
-    return ( <
-        video controls ref = {
-            reference
-        }
-        style = {
-            {
-                minWidth: '150px',
-                maxWidth: '750px'
-            }
-        }
-        onPlay = {
-            () => typeof(onPlayed) !== 'undefined' && onPlayed()
-        }
-        onEnded = {
-            () => typeof(onEnded) !== 'undefined' && onEnded()
-        } >
-        <
-        source src = {
-            src
-        }
-        type = 'video/mp4' / >
-        <
-        /video>
-    );
-};
+import React, {
+    useEffect
+} from 'react';
+
+import '../css/components.css';
+
+export default function Audio({
+    src,
+    reference,
+    onEnded,
+    onStarted,
+    onPlay
+}) {
+    /* Create an HTML audio element */
+    // Reload audio when src changes
+    useEffect(() => {
+        if (typeof reference !== 'undefined' && reference.current) {
+            reference.current.pause();
+            reference.current.load();
+        }
+    }, [reference, src]);
+
+    // Render
+    return ( <
+        audio className = 'audio-single'
+        controls controlsList = 'nodownload'
+        ref = {
+            reference
+        }
+        onPlay = {
+            () => {
+                if (typeof(onStarted) !== 'undefined') onStarted();
+                if (typeof(onPlay) !== 'undefined') onPlay();
+            }
+        }
+        onEnded = {
+            () => typeof(onEnded) !== 'undefined' && onEnded()
+        } >
+        <
+        source src = {
+            src
+        }
+        type = 'audio/mpeg' / >
+        <
+        /audio>
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/pages/EndPage.js` & `reseval-0.1.0/reseval/assets/client/src/pages/EndPage.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,33 @@
-import Markdown from '../components/Markdown';
-
-import config from '../json/config.json';
-
-export default function EndPage({
-    completionCode
-}) {
-    /* Display the final page with a completion code for the participant */
-    // Format platform string
-    let platform_string;
-    const platform = config.crowdsource.platform;
-    if (platform === 'mturk') {
-        platform_string = 'Amazon Mechanical Turk'
-    } else {
-        throw new Error(`Platform ${platform} is not recognized`);
-    }
-    const message =
-        `Thank you for your participation. Please copy and paste the ` +
-        `following code into ${platform_string}.`
-
-    // Render
-    return ( <
-        div className = 'container' >
-        <
-        Markdown > {
-            message
-        } < /Markdown> <
-        h1 > {
-            completionCode
-        } < /h1> <
-        /div>
-    );
+import Markdown from '../components/Markdown';
+
+import config from '../json/config.json';
+
+export default function EndPage({
+    completionCode
+}) {
+    /* Display the final page with a completion code for the participant */
+    // Format platform string
+    let platform_string;
+    const platform = config.crowdsource.platform;
+    if (platform === 'mturk') {
+        platform_string = 'Amazon Mechanical Turk'
+    } else {
+        throw new Error(`Platform ${platform} is not recognized`);
+    }
+    const message =
+        `Thank you for your participation. Please copy and paste the ` +
+        `following code into ${platform_string}.`
+
+    // Render
+    return ( <
+        div className = 'container' >
+        <
+        Markdown > {
+            message
+        } < /Markdown> <
+        h1 > {
+            completionCode
+        } < /h1> <
+        /div>
+    );
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/pages/FeedbackPage.js` & `reseval-0.1.0/reseval/assets/client/src/pages/FeedbackPage.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,106 +1,109 @@
-import {
-    useState
-} from 'react';
-
-import Button from '../components/Button';
-import Markdown from '../components/Markdown';
-import Question, {
-    validate
-} from '../questions/Question';
-
-import config from '../json/config.json';
-
-
-/******************************************************************************
-Constants
-******************************************************************************/
-
-
-const url = window.location.protocol + '//' + window.location.host;
-
-
-/******************************************************************************
-Follow-up Survey
-******************************************************************************/
-
-
-export default function FeedbackPage({
-    navigation,
-    participant
-}) {
-    /* Render the prescreening questions asked to the participant */
-    const [index, setIndex] = useState(0);
-    const [response, setResponse] = useState(undefined);
-
-    // Get the current question
-    const questions = config.followup_questions;
-    const question = questions[index];
-
-    function onClick() {
-        // Do not proceed if the respons is invalid
-        if (!validate(response)) return;
-
-        // Get the name of the question
-        const name = question.name;
-
-        // Upload response to database
-        fetch(url + '/api/participants/update', {
-            method: 'post',
-            headers: {
-                'Content-Type': 'application/json'
-            },
-            body: JSON.stringify({
-                ID: participant,
-                [name]: response
-            })
-        });
-
-        // If the response is wrong, end the survey
-        if ('correct_answer' in question &&
-            response !== question.correct_answer) {
-            navigation.go('end');
-        }
-
-        // Go to next question
-        else if (index + 1 < questions.length) {
-            setIndex(index + 1);
-            setResponse(undefined);
-        }
-
-        // Finished survey
-        else {
-            navigation.next();
-        }
-    }
-
-    // Render
-    return ( <
-        div className = 'container' >
-        <
-        Markdown > {
-            `## **Post-Evaluation Survey**\n` +
-            `**Question ${index + 1} of ${questions.length}**\n` +
-            question.text
-        } <
-        /Markdown> <
-        Question question = {
-            question
-        }
-        response = {
-            response
-        }
-        setResponse = {
-            setResponse
-        }
-        /> <
-        Button active = {
-            typeof response !== 'undefined' && response.trim()
-        }
-        onClick = {
-            onClick
-        } >
-        Submit <
-        /Button> <
-        /div>
-    );
+import {
+    useState
+} from 'react';
+
+import Button from '../components/Button';
+import Markdown from '../components/Markdown';
+import Question, {
+    validate
+} from '../questions/Question';
+
+import config from '../json/config.json';
+
+
+/******************************************************************************
+Constants
+******************************************************************************/
+
+
+const url = window.location.protocol + '//' + window.location.host;
+
+
+/******************************************************************************
+Follow-up Survey
+******************************************************************************/
+
+
+export default function FeedbackPage({
+    navigation,
+    participant
+}) {
+    /* Render the prescreening questions asked to the participant */
+    const [index, setIndex] = useState(0);
+    const [response, setResponse] = useState(undefined);
+
+    // Get the current question
+    const questions = config.followup_questions;
+    const question = questions[index];
+
+    function onClick() {
+        // Do not proceed if the respons is invalid
+        if (!validate(response)) return;
+
+        // Get the name of the question
+        const name = question.name;
+
+        // Upload response to database
+        fetch(url + '/api/participants/update', {
+            method: 'post',
+            headers: {
+                'Content-Type': 'application/json'
+            },
+            body: JSON.stringify({
+                ID: participant,
+                [name]: response
+            })
+        });
+
+        // If the response is wrong, end the survey
+        if ('correct_answer' in question &&
+            response !== question.correct_answer) {
+            window.scroll(0, 0);
+            navigation.go('end');
+        }
+
+        // Go to next question
+        else if (index + 1 < questions.length) {
+            setIndex(index + 1);
+            setResponse(undefined);
+            window.scroll(0, 0);
+        }
+
+        // Finished survey
+        else {
+            window.scroll(0, 0);
+            navigation.next();
+        }
+    }
+
+    // Render
+    return ( <
+        div className = 'container' >
+        <
+        Markdown > {
+            `## **Post-Evaluation Survey**\n` +
+            `**Question ${index + 1} of ${questions.length}**\n` +
+            question.text
+        } <
+        /Markdown> <
+        Question question = {
+            question
+        }
+        response = {
+            response
+        }
+        setResponse = {
+            setResponse
+        }
+        /> <
+        Button active = {
+            typeof response !== 'undefined' && response.trim()
+        }
+        onClick = {
+            onClick
+        } >
+        Submit <
+        /Button> <
+        /div>
+    );
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/pages/QualificationPage.js` & `reseval-0.1.0/reseval/assets/client/src/pages/QualificationPage.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,327 +1,338 @@
-import React, {
-    useMemo,
-    useRef,
-    useState
-} from 'react';
-import Chance from 'chance';
-
-import Button from '../components/Button';
-import Markdown from '../components/Markdown';
-import Media from "../components/Media";
-import ListeningTest from "../questions/ListeningTest";
-import Question, {
-    validate
-} from '../questions/Question';
-
-import assignments from '../json/assignments.json';
-import config from '../json/config.json';
-
-
-/******************************************************************************
- Constants
- ******************************************************************************/
-
-
-// Random number generator
-const chance = new Chance();
-
-// Valid characters for random participant ID
-const characters =
-    'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789';
-
-// Application URL
-const url = window.location.protocol + '//' + window.location.host;
-
-
-/******************************************************************************
- Prescreening survey
- ******************************************************************************/
-
-export default function QualificationPage({
-    navigation,
-    participant,
-    setParticipant,
-    completionCode,
-    setFiles,
-    setConditions,
-    setEvaluatorId
-}) {
-    /* Render the prescreening questions asked to the participant */
-    const [index, setIndex] = useState(0);
-    const [response, setResponse] = useState(undefined);
-
-    // Question type can be "prescreen" or "listening-test"
-    const [questionType, setQuestionType] = useState('prescreen')
-
-    // Whether the listening test has finished
-    let if_finish = false
-
-    // Get the current question
-    const questions = config.prescreen_questions;
-
-    // Listening test index
-    const [testIndex, setTestIndex] = useState(0);
-    const [audioEnded, setAudioEnded] = useState(false);
-
-    // Listening test retries
-    const [retries, setRetries] = useState(undefined);
-
-    // Listening test audio reference
-    const refTest = useRef();
-
-    // Number of listening test examples
-    let test_length = 0;
-    if ('listening_test' in config) {
-        test_length = config.listening_test.num_questions;
-        if (retries === undefined) {
-            setRetries(config.listening_test.retries);
-        }
-    }
-
-    // The listening test audio
-    const file = useMemo(getRandomSample, [test_length])
-
-    function getRandomSample() {
-        /* Retrieve a random audio files for listening test */
-        let file = []
-        let i = 0;
-        while (i < test_length) {
-            let idx = chance.integer({
-                min: 0,
-                max: 3
-            })
-            let tone = chance.integer({
-                min: 4,
-                max: 8
-            })
-            file.push(`tones${tone}_${idx}.wav`)
-            i += 1
-        }
-        return file
-    }
-
-    function listeningTest() {
-        /* Interaction logic for listening test */
-        // Skip if we are not performing a listening test
-        if (!('listening_test' in config)) {
-            if_finish = true;
-            return;
-        }
-
-        // Change question type for listening test
-        if (questionType !== 'listening-test') {
-            setQuestionType('listening-test');
-            return;
-        }
-
-        // Parse the true number of tones from the filename
-        let correct_response =
-            file[testIndex].split('.')[0].split('_')[0].slice(-1);
-
-        // Fail prescreening if the wrong answer is given
-        if (response !== correct_response) {
-            if (retries > 0) {
-                const plural = retries > 1 ? 's' : '';
-                const message = `Incorrect. Please put on headphones, move ` +
-                    `to a quiet location, and try again. You have ` +
-                    `${retries} attempt${plural} remaining.`
-                alert(message);
-                setRetries(retries - 1);
-                return;
-            } else {
-                navigation.go('end');
-            }
-        } else {
-            // End listening test if we've answered enough questions
-            if (testIndex + 1 >= test_length) {
-                if_finish = true
-                return
-            }
-        }
-
-        // Go to next question
-        if (testIndex + 1 < test_length) {
-            setAudioEnded(false)
-            setTestIndex(testIndex + 1);
-            setRetries(config.listening_test.retries);
-            setResponse(undefined);
-        }
-    }
-
-    function onClick() {
-        // Do not proceed if the response is invalid
-        if (questions.length > 0 && !validate(response)) return;
-
-        // Values to send to database
-        let values = {};
-
-        // Either use cached participant or create new participant
-        let route;
-        if (typeof participant === 'undefined') {
-            values['ID'] = chance.string({
-                length: 32,
-                pool: characters
-            });
-            values['CompletionCode'] = completionCode;
-            setParticipant(values['ID']);
-            route = 'insert';
-        } else {
-            values['ID'] = participant;
-            route = 'update';
-        }
-
-        // Add response
-        if (questions.length > 0) {
-            values[questions[index].name] = response;
-        }
-
-        // If the response is wrong, end the survey
-        if (questionType === 'prescreen' && questions.length > 0 &&
-            'correct_answer' in questions[index] &&
-            response !== questions[index].correct_answer) {
-
-            // Upload response to database
-            fetch(url + '/api/participants/' + route, {
-                method: 'post',
-                headers: {
-                    'Content-Type': 'application/json'
-                },
-                body: JSON.stringify(values)
-            });
-
-            // End survey
-            navigation.go('end');
-        } else {
-            // Upload response to database
-            fetch(url + '/api/participants/' + route, {
-                method: 'post',
-                headers: {
-                    'Content-Type': 'application/json'
-                },
-                body: JSON.stringify(values)
-            }).then(_ => {
-                if (index + 1 >= questions.length) {
-                    // enter listening test
-                    listeningTest()
-                    // do not proceed until listening test is finished
-                    if (!if_finish) {
-                        return
-                    }
-                    // Get evaluation files for this evaluator
-                    fetch(url + '/api/evaluators/')
-                        .then(response => response.json())
-                        .then(response => {
-                            setFiles(
-                                assignments[response % assignments.length]);
-                            setEvaluatorId(response);
-                        })
-
-                        // Get list of evaluation conditions
-                        .then(_ => {
-                            fetch(url + '/api/conditions')
-                                .then(response => response.json())
-                                .then(response => {
-                                    setConditions(
-                                        response.map(
-                                            cond => cond.Condition))
-
-                                    // Go to evaluation
-                                }).then(_ => navigation.next())
-                        });
-                }
-            });
-        }
-
-        // Go to next question
-        if (index + 1 < questions.length) {
-            setIndex(index + 1);
-            setResponse(undefined);
-        }
-    }
-
-    // Skip prescreening if there are no questions
-    if (questions.length === 0) {
-        if (!('listening_test' in config)) {
-            onClick();
-            return null
-        } else if (questionType === 'prescreen') {
-            setQuestionType('listening-test');
-        }
-    }
-
-    if (questionType === 'listening-test') {
-        // Render listening test
-        return ( <
-            div className = 'container' >
-            <
-            Markdown > {
-                `**Question ${testIndex + 1} of ${test_length}**\n` +
-                config.listening_test.instructions
-            } <
-            /Markdown> <
-            Media reference = {
-                refTest
-            }
-            onEnded = {
-                () => setAudioEnded(true)
-            }
-            src = {
-                'listening_test/' + file[testIndex]
-            }
-            /> <
-            ListeningTest response = {
-                response
-            }
-            setResponse = {
-                setResponse
-            }
-            active = {
-                audioEnded
-            }
-            /> <
-            Button active = {
-                audioEnded && typeof response !== 'undefined'
-            }
-            onClick = {
-                () => {
-                    typeof response !== 'undefined' &&
-                        audioEnded &&
-                        onClick()
-                }
-            } >
-            Next <
-            /Button> <
-            /div>
-        );
-    } else if (questions.length !== 0) {
-        // Render prescreening question
-        return ( <
-            div className = 'container' >
-            <
-            Markdown > {
-                `**Question ${index + 1}** ${questions[index].text}`
-            } <
-            /Markdown> <
-            Question question = {
-                questions[index]
-            }
-            response = {
-                response
-            }
-            setResponse = {
-                setResponse
-            }
-            /> <
-            Button active = {
-                typeof response !== 'undefined' && response.trim()
-            }
-            onClick = {
-                onClick
-            } >
-            Next <
-            /Button> <
-            /div>
-        );
-    } else {
-        return < > < />; }
+import React, {
+    useMemo,
+    useRef,
+    useState
+} from 'react';
+import Chance from 'chance';
+
+import Button from '../components/Button';
+import Markdown from '../components/Markdown';
+import Media from "../components/Media";
+import ListeningTest from "../questions/ListeningTest";
+import Question, {
+    validate
+} from '../questions/Question';
+
+import assignments from '../json/assignments.json';
+import config from '../json/config.json';
+
+
+/******************************************************************************
+ Constants
+ ******************************************************************************/
+
+
+// Random number generator
+const chance = new Chance();
+
+// Valid characters for random participant ID
+const characters =
+    'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789';
+
+// Application URL
+const url = window.location.protocol + '//' + window.location.host;
+
+
+/******************************************************************************
+ Prescreening survey
+ ******************************************************************************/
+
+export default function QualificationPage({
+    navigation,
+    participant,
+    setParticipant,
+    completionCode,
+    setFiles,
+    setConditions,
+    setEvaluatorId
+}) {
+    /* Render the prescreening questions asked to the participant */
+    const [index, setIndex] = useState(0);
+    const [response, setResponse] = useState(undefined);
+
+    // Question type can be "prescreen" or "listening-test"
+    const [questionType, setQuestionType] = useState('prescreen')
+
+    // Whether the listening test has finished
+    let if_finish = false
+
+    // Get the current question
+    const questions = config.prescreen_questions;
+
+    // Listening test index
+    const [testIndex, setTestIndex] = useState(0);
+    const [audioEnded, setAudioEnded] = useState(false);
+
+    // Listening test retries
+    const [retries, setRetries] = useState(undefined);
+
+    // Listening test audio reference
+    const refTest = useRef();
+
+    // Number of listening test examples
+    let test_length = 0;
+    if ('listening_test' in config) {
+        test_length = config.listening_test.num_questions;
+        if (retries === undefined) {
+            setRetries(config.listening_test.retries);
+        }
+    }
+
+    // The listening test audio
+    const file = useMemo(getRandomSample, [test_length])
+
+    function getRandomSample() {
+        /* Retrieve a random audio files for listening test */
+        let file = []
+        let i = 0;
+        while (i < test_length) {
+            let idx = chance.integer({
+                min: 0,
+                max: 3
+            })
+            let tone = chance.integer({
+                min: 4,
+                max: 8
+            })
+            file.push(`tones${tone}_${idx}.wav`)
+            i += 1
+        }
+        return file
+    }
+
+    function listeningTest() {
+        /* Interaction logic for listening test */
+        // Skip if we are not performing a listening test
+        if (!('listening_test' in config)) {
+            if_finish = true;
+            return;
+        }
+
+        // Change question type for listening test
+        if (questionType !== 'listening-test') {
+            setQuestionType('listening-test');
+            return;
+        }
+
+        // Parse the true number of tones from the filename
+        let correct_response =
+            file[testIndex].split('.')[0].split('_')[0].slice(-1);
+
+        // Fail prescreening if the wrong answer is given
+        if (response !== correct_response) {
+            if (retries > 0) {
+                const plural = retries > 1 ? 's' : '';
+                const message = `Incorrect. Please put on headphones, move ` +
+                    `to a quiet location, and try again. You have ` +
+                    `${retries} attempt${plural} remaining.`
+                alert(message);
+                setRetries(retries - 1);
+                return;
+            } else {
+                window.scroll(0, 0);
+                navigation.go('end');
+            }
+        } else {
+            // End listening test if we've answered enough questions
+            if (testIndex + 1 >= test_length) {
+                if_finish = true
+                return
+            }
+        }
+
+        // Go to next question
+        if (testIndex + 1 < test_length) {
+            setAudioEnded(false)
+            setTestIndex(testIndex + 1);
+            setRetries(config.listening_test.retries);
+            setResponse(undefined);
+            window.scroll(0, 0);
+        }
+    }
+
+    function onClick() {
+        // Do not proceed if the response is invalid
+        if (questions.length > 0 && !validate(response)) return;
+
+        // Values to send to database
+        let values = {};
+
+        // Either use cached participant or create new participant
+        let route;
+        if (typeof participant === 'undefined') {
+            values['ID'] = chance.string({
+                length: 32,
+                pool: characters
+            });
+            values['CompletionCode'] = completionCode;
+            setParticipant(values['ID']);
+            route = 'insert';
+        } else {
+            values['ID'] = participant;
+            route = 'update';
+        }
+
+        // Add response
+        if (questions.length > 0) {
+            values[questions[index].name] = response;
+        }
+
+        // If the response is wrong, end the survey
+        if (questionType === 'prescreen' && questions.length > 0 &&
+            'correct_answer' in questions[index] &&
+            response !== questions[index].correct_answer) {
+
+            // Upload response to database
+            fetch(url + '/api/participants/' + route, {
+                method: 'post',
+                headers: {
+                    'Content-Type': 'application/json'
+                },
+                body: JSON.stringify(values)
+            });
+
+            // End survey
+            navigation.go('end');
+        } else {
+            // Upload response to database
+            fetch(url + '/api/participants/' + route, {
+                method: 'post',
+                headers: {
+                    'Content-Type': 'application/json'
+                },
+                body: JSON.stringify(values)
+            }).then(_ => {
+                if (index + 1 >= questions.length) {
+                    // enter listening test
+                    listeningTest()
+                    // do not proceed until listening test is finished
+                    if (!if_finish) {
+                        return
+                    }
+                    // Get evaluation files for this evaluator
+                    fetch(url + '/api/participants/')
+                        .then(response => response.json())
+                        .then(response => {
+                            const evaluatorId = response.length - 1;
+                            setFiles(
+                                assignments[evaluatorId % assignments.length]);
+                            setEvaluatorId(evaluatorId);
+                        })
+
+                        // Get list of evaluation conditions
+                        .then(_ => {
+
+                            if (config.test === 'wordselect') {
+                                navigation.next();
+                            } else {
+                                fetch(url + '/api/conditions')
+                                    .then(response => response.json())
+                                    .then(response => {
+                                        setConditions(
+                                            response.map(
+                                                cond => cond.Condition))
+
+                                        // Go to evaluation
+                                    }).then(_ => {
+                                        window.scroll(0, 0);
+                                        navigation.next();
+                                    })
+                            }
+                        });
+                }
+            });
+        }
+
+        // Go to next question
+        if (index + 1 < questions.length) {
+            setIndex(index + 1);
+            setResponse(undefined);
+        }
+    }
+
+    // Skip prescreening if there are no questions
+    if (questions.length === 0) {
+        if (!('listening_test' in config)) {
+            onClick();
+            return null
+        } else if (questionType === 'prescreen') {
+            setQuestionType('listening-test');
+        }
+    }
+
+    if (questionType === 'listening-test') {
+        // Render listening test
+        return ( <
+            div className = 'container' >
+            <
+            Markdown > {
+                `**Question ${testIndex + 1} of ${test_length}**\n` +
+                config.listening_test.instructions
+            } <
+            /Markdown> <
+            Media reference = {
+                refTest
+            }
+            onEnded = {
+                () => setAudioEnded(true)
+            }
+            src = {
+                'listening_test/' + file[testIndex]
+            }
+            /> <
+            ListeningTest response = {
+                response
+            }
+            setResponse = {
+                setResponse
+            }
+            active = {
+                audioEnded
+            }
+            /> <
+            Button active = {
+                audioEnded && typeof response !== 'undefined'
+            }
+            onClick = {
+                () => {
+                    typeof response !== 'undefined' &&
+                        audioEnded &&
+                        onClick()
+                }
+            } >
+            Next <
+            /Button> <
+            /div>
+        );
+    } else if (questions.length !== 0) {
+        // Render prescreening question
+        return ( <
+            div className = 'container' >
+            <
+            Markdown > {
+                `**Question ${index + 1}** ${questions[index].text}`
+            } <
+            /Markdown> <
+            Question question = {
+                questions[index]
+            }
+            response = {
+                response
+            }
+            setResponse = {
+                setResponse
+            }
+            /> <
+            Button active = {
+                typeof response !== 'undefined' && response.trim()
+            }
+            onClick = {
+                onClick
+            } >
+            Next <
+            /Button> <
+            /div>
+        );
+    } else {
+        return < > < />; }
     }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/pages/TaskPage.js` & `reseval-0.1.0/reseval/assets/client/src/pages/TaskPage.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,161 +1,170 @@
-import React, {
-    createContext,
-    useMemo,
-    useState
-} from 'react';
-
-import AB from '../test/AB';
-import ABX from '../test/ABX';
-import MOS from '../test/MOS';
-import MUSHRA from '../test/MUSHRA';
-import Markdown from '../components/Markdown';
-
-import config from '../json/config.json';
-
-import '../css/components.css';
-
-
-/******************************************************************************
- Constants
- ******************************************************************************/
-
-
-// Application URL
-const url = window.location.protocol + '//' + window.location.host;
-
-// Global state of any currently playing media
-export const MediaContext = createContext({
-    mediaRef: '',
-    setMediaRef: () => {}
-});
-
-
-/******************************************************************************
- Prescreening survey
- ******************************************************************************/
-
-
-export default function TaskPage({
-    participant,
-    navigation,
-    files,
-    conditions,
-    evaluatorId
-}) {
-    /* Render the evaluation task */
-    // Current progress
-    const [index, setIndex] = useState(0);
-
-    // Update context value whenever media changes
-    const [mediaRef, setMediaRef] = useState(undefined);
-    const value = useMemo(
-        () => {
-            return {
-                mediaRef,
-                setMediaRef
-            }
-        },
-        [mediaRef]
-    );
-
-    // Response from the participant
-    const [response, setResponse] = useState(undefined);
-
-    // Don't render anything until we have files and conditions
-    if (typeof files === 'undefined' ||
-        typeof conditions === 'undefined') {
-        return null;
-    }
-
-    // Get current file to evaluate
-    const file = files[index];
-
-    function onClick() {
-
-        // Upload response
-        fetch(url + '/api/responses', {
-            method: 'post',
-            headers: {
-                'Content-Type': 'application/json'
-            },
-            body: JSON.stringify({
-                'Stem': file.replace(/\.[^/.]+$/, ''),
-                'Participant': participant,
-                'OrderAsked': index,
-                'Response': response
-            })
-        });
-
-        // Go to next question
-        if (index + 1 < files.length) {
-            setIndex(index + 1);
-            setResponse(undefined);
-        }
-
-        // Proceed to follow-up survey
-        else {
-            navigation.next();
-        }
-    }
-
-    // Bundle props
-    const props = {
-        file: file,
-        index: index,
-        conditions: conditions,
-        navigation: navigation,
-        response: response,
-        setResponse: setResponse,
-        evaluatorId: evaluatorId,
-        onClick: onClick
-    };
-
-    // Select test
-    let test;
-    switch (config.test) {
-        case 'ab':
-            test = < AB {
-                ...props
-            }
-            />;
-            break;
-        case 'abx':
-            test = < ABX {
-                ...props
-            }
-            />;
-            break;
-        case 'mos':
-            test = < MOS {
-                ...props
-            }
-            />;
-            break;
-        case 'mushra':
-            test = < MUSHRA {
-                ...props
-            }
-            />;
-            break;
-        default:
-            throw new Error(`Test type ${config.test} is not recognized`);
-    }
-
-    // Render
-    return ( <
-        div className = 'container' >
-        <
-        Markdown > {
-            `**Question ${index + 1} of ${files.length}**\n` +
-            config.survey_instructions
-        } <
-        /Markdown> <
-        MediaContext.Provider value = {
-            value
-        } > {
-            test
-        } <
-        /MediaContext.Provider> <
-        /div>
-    );
-};
+import React, {
+    createContext,
+    useMemo,
+    useState
+} from 'react';
+
+import AB from '../test/AB';
+import ABX from '../test/ABX';
+import MOS from '../test/MOS';
+import MUSHRA from '../test/MUSHRA';
+import WordSelect from '../test/WordSelect';
+import Markdown from '../components/Markdown';
+
+import config from '../json/config.json';
+
+import '../css/components.css';
+
+
+/******************************************************************************
+ Constants
+ ******************************************************************************/
+
+
+// Application URL
+const url = window.location.protocol + '//' + window.location.host;
+
+// Global state of any currently playing media
+export const MediaContext = createContext({
+    mediaRef: '',
+    setMediaRef: () => {}
+});
+
+
+/******************************************************************************
+ Prescreening survey
+ ******************************************************************************/
+
+
+export default function TaskPage({
+    participant,
+    navigation,
+    files,
+    conditions,
+    evaluatorId
+}) {
+    /* Render the evaluation task */
+    // Current progress
+    const [index, setIndex] = useState(0);
+
+    // Update context value whenever media changes
+    const [mediaRef, setMediaRef] = useState(undefined);
+    const value = useMemo(
+        () => {
+            return {
+                mediaRef,
+                setMediaRef
+            }
+        },
+        [mediaRef]
+    );
+
+    // Response from the participant
+    const [response, setResponse] = useState(undefined);
+
+    // Don't render anything until we have files and conditions
+    if (typeof files === 'undefined' ||
+        (typeof conditions === 'undefined' && !config.test === 'wordselect')) {
+        return null;
+    }
+
+    // Get current file to evaluate
+    const file = files[index];
+
+    function onClick() {
+
+        // Upload response
+        fetch(url + '/api/responses', {
+            method: 'post',
+            headers: {
+                'Content-Type': 'application/json'
+            },
+            body: JSON.stringify({
+                'Stem': file.replace(/\.[^/.]+$/, ''),
+                'Participant': participant,
+                'OrderAsked': index,
+                'Response': response
+            })
+        });
+
+        // Go to next question
+        if (index + 1 < files.length) {
+            setIndex(index + 1);
+            setResponse(undefined);
+            window.scroll(0, 0);
+        }
+
+        // Proceed to follow-up survey
+        else {
+            window.scroll(0, 0);
+            navigation.next();
+        }
+    }
+
+    // Bundle props
+    const props = {
+        file: file,
+        index: index,
+        conditions: conditions,
+        navigation: navigation,
+        response: response,
+        setResponse: setResponse,
+        evaluatorId: evaluatorId,
+        onClick: onClick
+    };
+
+    // Select test
+    let test;
+    switch (config.test) {
+        case 'ab':
+            test = < AB {
+                ...props
+            }
+            />;
+            break;
+        case 'abx':
+            test = < ABX {
+                ...props
+            }
+            />;
+            break;
+        case 'mos':
+            test = < MOS {
+                ...props
+            }
+            />;
+            break;
+        case 'mushra':
+            test = < MUSHRA {
+                ...props
+            }
+            />;
+            break;
+        case 'wordselect':
+            test = < WordSelect {
+                ...props
+            }
+            />;
+            break;
+        default:
+            throw new Error(`Test type ${config.test} is not recognized`);
+    }
+
+    // Render
+    return ( <
+        div className = 'container' >
+        <
+        Markdown > {
+            `**Question ${index + 1} of ${files.length}**\n` +
+            config.survey_instructions
+        } <
+        /Markdown> <
+        MediaContext.Provider value = {
+            value
+        } > {
+            test
+        } <
+        /MediaContext.Provider> <
+        /div>
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/questions/ListeningTest.js` & `reseval-0.1.0/reseval/assets/client/src/questions/ListeningTest.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,82 +1,82 @@
-export default function ListeningTest({
-    response,
-    setResponse,
-    active
-}) {
-    /* Render a multiple choice question for listening test */
-    // enumerated answers
-    let answers = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
-    return ( <
-        ul > {
-            answers.map((item, key) =>
-                <
-                Choice key = {
-                    key
-                }
-                response = {
-                    response
-                }
-                setResponse = {
-                    setResponse
-                }
-                label = {
-                    item
-                }
-                active = {
-                    active
-                }
-                />
-            )
-        } <
-        /ul>
-    )
-}
-
-function Choice({
-    response,
-    setResponse,
-    label,
-    active
-}) {
-    return ( <
-        li className = 'listitem grid grid-20-80' >
-        <
-        div style = {
-            {
-                display: 'flex',
-                justifyContent: 'center',
-                width: '100%'
-            }
-        } >
-        <
-        div className = {
-            `check col-1 ${active ? ' active' : ''}` +
-            `${label === response ? ' selected' : ''}`
-        }
-        onClick = {
-            () => active && setResponse(label)
-        } >
-        <
-        div className = 'inside' / >
-        <
-        /div> <
-        /div> <
-        div style = {
-            {
-                display: 'flex',
-                width: '100%'
-            }
-        } >
-        <
-        label className = 'choices'
-        onClick = {
-            () => active && setResponse(label)
-        } >
-        {
-            label
-        } <
-        /label> <
-        /div> <
-        /li>
-    )
+export default function ListeningTest({
+    response,
+    setResponse,
+    active
+}) {
+    /* Render a multiple choice question for listening test */
+    // enumerated answers
+    let answers = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
+    return ( <
+        ul > {
+            answers.map((item, key) =>
+                <
+                Choice key = {
+                    key
+                }
+                response = {
+                    response
+                }
+                setResponse = {
+                    setResponse
+                }
+                label = {
+                    item
+                }
+                active = {
+                    active
+                }
+                />
+            )
+        } <
+        /ul>
+    )
+}
+
+function Choice({
+    response,
+    setResponse,
+    label,
+    active
+}) {
+    return ( <
+        li className = 'listitem grid grid-20-80' >
+        <
+        div style = {
+            {
+                display: 'flex',
+                justifyContent: 'center',
+                width: '100%'
+            }
+        } >
+        <
+        div className = {
+            `check col-1 ${active ? ' active' : ''}` +
+            `${label === response ? ' selected' : ''}`
+        }
+        onClick = {
+            () => active && setResponse(label)
+        } >
+        <
+        div className = 'inside' / >
+        <
+        /div> <
+        /div> <
+        div style = {
+            {
+                display: 'flex',
+                width: '100%'
+            }
+        } >
+        <
+        label className = 'choices'
+        onClick = {
+            () => active && setResponse(label)
+        } >
+        {
+            label
+        } <
+        /label> <
+        /div> <
+        /li>
+    )
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/questions/MultipleChoice.js` & `reseval-0.1.0/reseval/assets/client/src/questions/MultipleChoice.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,76 +1,76 @@
-export default function MultipleChoice({
-    response,
-    setResponse,
-    answers
-}) {
-    /* Render a multiple choice question */
-    return ( <
-        ul > {
-            answers.map((item, key) =>
-                <
-                Choice key = {
-                    key
-                }
-                response = {
-                    response
-                }
-                setResponse = {
-                    setResponse
-                }
-                label = {
-                    item
-                }
-                />
-            )
-        } <
-        /ul>
-    )
-}
-
-function Choice({
-    response,
-    setResponse,
-    label
-}) {
-    /* Render one choice of a multiple choice question */
-    return ( <
-        li className = 'listitem grid grid-20-80' >
-        <
-        div style = {
-            {
-                display: 'flex',
-                justifyContent: 'center',
-                width: '100%'
-            }
-        } >
-        <
-        div className = {
-            `check active col-1 ${label === response ? 'selected' : ''}`
-        }
-        onClick = {
-            () => setResponse(label)
-        } >
-        <
-        div className = 'inside' / >
-        <
-        /div> <
-        /div> <
-        div style = {
-            {
-                display: 'flex',
-                width: '100%'
-            }
-        } >
-        <
-        label className = 'choices'
-        onClick = {
-            () => setResponse(label)
-        } >
-        {
-            label
-        } <
-        /label> <
-        /div> <
-        /li>
-    )
+export default function MultipleChoice({
+    response,
+    setResponse,
+    answers
+}) {
+    /* Render a multiple choice question */
+    return ( <
+        ul > {
+            answers.map((item, key) =>
+                <
+                Choice key = {
+                    key
+                }
+                response = {
+                    response
+                }
+                setResponse = {
+                    setResponse
+                }
+                label = {
+                    item
+                }
+                />
+            )
+        } <
+        /ul>
+    )
+}
+
+function Choice({
+    response,
+    setResponse,
+    label
+}) {
+    /* Render one choice of a multiple choice question */
+    return ( <
+        li className = 'listitem grid grid-20-80' >
+        <
+        div style = {
+            {
+                display: 'flex',
+                justifyContent: 'center',
+                width: '100%'
+            }
+        } >
+        <
+        div className = {
+            `check active col-1 ${label === response ? 'selected' : ''}`
+        }
+        onClick = {
+            () => setResponse(label)
+        } >
+        <
+        div className = 'inside' / >
+        <
+        /div> <
+        /div> <
+        div style = {
+            {
+                display: 'flex',
+                width: '100%'
+            }
+        } >
+        <
+        label className = 'choices'
+        onClick = {
+            () => setResponse(label)
+        } >
+        {
+            label
+        } <
+        /label> <
+        /div> <
+        /li>
+    )
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/questions/Question.js` & `reseval-0.1.0/reseval/assets/client/src/questions/Question.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,50 +1,50 @@
-import FreeResponse from './FreeResponse';
-import MultipleChoice from './MultipleChoice';
-
-export default function Question({
-    question,
-    response,
-    setResponse
-}) {
-    /* Render a question */
-    // Maybe render multiple choice
-    if (question.type === 'multiple-choice') {
-        return < MultipleChoice
-        response = {
-            response
-        }
-        setResponse = {
-            setResponse
-        }
-        answers = {
-            question.answers
-        }
-        />;
-    }
-
-    // Maybe render free response
-    if (question.type === 'free-response') {
-        return < FreeResponse
-        placeholder = {
-            question.placeholder
-        }
-        setResponse = {
-            setResponse
-        }
-        />;
-    }
-
-    // Unrecognized question type
-    throw new Error(`Question type ${question.type} is not recognized`);
-}
-
-
-export function validate(response) {
-    /* Error check question response */
-    // Require input to be non-empty
-    if (typeof response === 'undefined' || !response.trim()) {
-        alert('Please leave a response.');
-        return false;
-    }
-    return true;
+import FreeResponse from './FreeResponse';
+import MultipleChoice from './MultipleChoice';
+
+export default function Question({
+    question,
+    response,
+    setResponse
+}) {
+    /* Render a question */
+    // Maybe render multiple choice
+    if (question.type === 'multiple-choice') {
+        return < MultipleChoice
+        response = {
+            response
+        }
+        setResponse = {
+            setResponse
+        }
+        answers = {
+            question.answers
+        }
+        />;
+    }
+
+    // Maybe render free response
+    if (question.type === 'free-response') {
+        return < FreeResponse
+        placeholder = {
+            question.placeholder
+        }
+        setResponse = {
+            setResponse
+        }
+        />;
+    }
+
+    // Unrecognized question type
+    throw new Error(`Question type ${question.type} is not recognized`);
+}
+
+
+export function validate(response) {
+    /* Error check question response */
+    // Require input to be non-empty
+    if (typeof response === 'undefined' || !response.trim()) {
+        alert('Please leave a response.');
+        return false;
+    }
+    return true;
 }
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/test/AB.js` & `reseval-0.1.0/reseval/assets/client/src/test/MOS.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,99 +1,90 @@
-import Chance from 'chance';
-import React, {
-    useRef,
-    useState
-} from 'react';
-
-import MediaRadioButtonGroup from '../components/MediaRadioButtonGroup';
-
-import '../css/components.css';
-
-import Button from '../components/Button';
-
-
-/******************************************************************************
-Constants
-******************************************************************************/
-
-
-// Random number generator
-const chance = new Chance();
-
-
-/******************************************************************************
-AB test
-******************************************************************************/
-
-
-export default function AB({
-    file,
-    conditions,
-    response,
-    setResponse,
-    onClick
-}) {
-    /* Render an AB evaluation task */
-    const refA = useRef();
-    const refB = useRef();
-
-    // Whether file has ended
-    const [AEnded, setAEnded] = useState(false);
-    const [BEnded, setBEnded] = useState(false);
-
-    // Non-deterministic ordering of media elements
-    const [permutation, setPermutation] = useState(
-        chance.shuffle([...Array(conditions.length).keys()]));
-    const permuted_conditions = permutation.map(index => conditions[index]);
-
-    function clickHandler() {
-        // Send response and update index
-        onClick();
-
-        // Reset media components
-        setAEnded(false);
-        setBEnded(false);
-
-        // Get a new permutation
-        setPermutation(chance.shuffle([...Array(conditions.length).keys()]));
-    }
-
-    // Can we advance?
-    const advance = typeof response !== 'undefined' && AEnded && BEnded;
-
-    // Render
-    return ( <
-        >
-        <
-        MediaRadioButtonGroup file = {
-            file
-        }
-        conditions = {
-            permuted_conditions
-        }
-        response = {
-            response
-        }
-        setResponse = {
-            setResponse
-        }
-        references = {
-            [refA, refB]
-        }
-        active = {
-            AEnded && BEnded
-        }
-        onEndeds = {
-            [() => setAEnded(true), () => setBEnded(true)]
-        }
-        /> <
-        Button active = {
-            advance
-        }
-        onClick = {
-            () => advance && clickHandler()
-        } >
-        Next <
-        /Button> <
-        />
-    );
-};
+import React, {
+    useRef,
+    useState
+} from 'react';
+
+import Media from '../components/Media';
+import RadioButtonGroup from '../components/RadioButtonGroup';
+import conditions from '../json/conditions.json';
+
+import '../css/components.css';
+
+import Button from '../components/Button';
+
+
+/******************************************************************************
+ Mean opinion score evaluation
+ ******************************************************************************/
+
+
+export default function MOS({
+    file,
+    index,
+    response,
+    setResponse,
+    evaluatorId,
+    onClick
+}) {
+    /* Render a MOS evaluation task */
+    const reference = useRef();
+
+    // Conditions to use for this evaluator
+    const conditionList = conditions[evaluatorId % conditions.length]
+
+    // Condition of the current file
+    const [condition, setCondition] = useState(conditionList[index]);
+
+    // Whether the media has ended
+    const [ended, setEnded] = useState(false);
+
+    function clickHandler() {
+        // Send response to database and go to next question
+        onClick();
+
+        // Reset media files
+        setEnded(false);
+
+        // Update condition
+        setCondition(conditionList[index + 1])
+    }
+
+    // Can we advance?
+    const advance = typeof response !== 'undefined' && ended;
+
+    // Render
+    return ( <
+        >
+        <
+        Media src = {
+            condition + '/' + file
+        }
+        reference = {
+            reference
+        }
+        onEnded = {
+            () => setEnded(true)
+        }
+        /> <
+        RadioButtonGroup response = {
+            typeof response === 'undefined' ? response : Number(response.slice(-1))
+        }
+        setResponse = {
+            index => setResponse(`${condition}-${index}`)
+        }
+        active = {
+            ended
+        }
+        /> <
+        Button active = {
+            advance
+        }
+        onClick = {
+            () => {
+                advance && clickHandler()
+            }
+        } >
+        Next <
+        /Button> <
+        />
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/test/ABX.js` & `reseval-0.1.0/reseval/assets/client/src/test/ABX.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,129 +1,129 @@
-import Chance from 'chance';
-import React, {
-    useRef,
-    useState
-} from 'react';
-
-import Media from '../components/Media';
-import MediaRadioButtonGroup from '../components/MediaRadioButtonGroup';
-
-import '../css/components.css';
-
-import Button from '../components/Button';
-
-
-/******************************************************************************
-Constants
-******************************************************************************/
-
-
-// Random number generator
-const chance = new Chance();
-
-
-/******************************************************************************
-ABX test
-******************************************************************************/
-
-
-export default function ABX({
-    file,
-    conditions,
-    response,
-    setResponse,
-    onClick
-}) {
-    /* Render an ABX evaluation task */
-    const refX = useRef();
-    const refA = useRef();
-    const refB = useRef();
-
-    // Whether the audio has ended
-    const [XEnded, setXEnded] = useState(false);
-    const [AEnded, setAEnded] = useState(false);
-    const [BEnded, setBEnded] = useState(false);
-
-    // Non-deterministic ordering of media elements
-    const conditions_no_reference = conditions.filter(
-        condition => condition !== 'reference')
-    const [permutation, setPermutation] = useState(
-        chance.shuffle([...Array(conditions_no_reference.length).keys()]));
-    const permuted_conditions = permutation.map(
-        index => conditions_no_reference[index]);
-
-    function clickHandler() {
-        // Send response to database and go to next question
-        onClick();
-
-        // Reset audio files
-        setXEnded(false);
-        setAEnded(false);
-        setBEnded(false);
-
-        // Get a new permutation
-        setPermutation(
-            chance.shuffle([...Array(conditions_no_reference.length).keys()]));
-    }
-
-    // Can we advance?
-    const advance =
-        typeof response !== 'undefined' && XEnded && AEnded && BEnded;
-
-    // Render
-    return ( <
-        >
-        <
-        div className = 'grid grid-20-80' >
-        <
-        div style = {
-            {
-                width: '100%'
-            }
-        }
-        /> <
-        Media src = {
-            'reference/' + file
-        }
-        reference = {
-            refX
-        }
-        onEnded = {
-            () => setXEnded(true)
-        }
-        /> <
-        /div> <
-        MediaRadioButtonGroup file = {
-            file
-        }
-        conditions = {
-            permuted_conditions
-        }
-        response = {
-            response
-        }
-        setResponse = {
-            setResponse
-        }
-        references = {
-            [refA, refB]
-        }
-        active = {
-            XEnded && AEnded && BEnded
-        }
-        onEndeds = {
-            [() => setAEnded(true), () => setBEnded(true)]
-        }
-        /> <
-        Button active = {
-            advance
-        }
-        onClick = {
-            () => {
-                advance && clickHandler()
-            }
-        } >
-        Next <
-        /Button> <
-        />
-    );
-};
+import Chance from 'chance';
+import React, {
+    useRef,
+    useState
+} from 'react';
+
+import Media from '../components/Media';
+import MediaRadioButtonGroup from '../components/MediaRadioButtonGroup';
+
+import '../css/components.css';
+
+import Button from '../components/Button';
+
+
+/******************************************************************************
+Constants
+******************************************************************************/
+
+
+// Random number generator
+const chance = new Chance();
+
+
+/******************************************************************************
+ABX test
+******************************************************************************/
+
+
+export default function ABX({
+    file,
+    conditions,
+    response,
+    setResponse,
+    onClick
+}) {
+    /* Render an ABX evaluation task */
+    const refX = useRef();
+    const refA = useRef();
+    const refB = useRef();
+
+    // Whether the media has ended
+    const [XEnded, setXEnded] = useState(false);
+    const [AEnded, setAEnded] = useState(false);
+    const [BEnded, setBEnded] = useState(false);
+
+    // Non-deterministic ordering of media elements
+    const conditions_no_reference = conditions.filter(
+        condition => condition !== 'reference')
+    const [permutation, setPermutation] = useState(
+        chance.shuffle([...Array(conditions_no_reference.length).keys()]));
+    const permuted_conditions = permutation.map(
+        index => conditions_no_reference[index]);
+
+    function clickHandler() {
+        // Send response to database and go to next question
+        onClick();
+
+        // Reset media files
+        setXEnded(false);
+        setAEnded(false);
+        setBEnded(false);
+
+        // Get a new permutation
+        setPermutation(
+            chance.shuffle([...Array(conditions_no_reference.length).keys()]));
+    }
+
+    // Can we advance?
+    const advance =
+        typeof response !== 'undefined' && XEnded && AEnded && BEnded;
+
+    // Render
+    return ( <
+        >
+        <
+        div className = 'grid grid-20-80' >
+        <
+        div style = {
+            {
+                width: '100%'
+            }
+        }
+        /> <
+        Media src = {
+            'reference/' + file
+        }
+        reference = {
+            refX
+        }
+        onEnded = {
+            () => setXEnded(true)
+        }
+        /> <
+        /div> <
+        MediaRadioButtonGroup file = {
+            file
+        }
+        conditions = {
+            permuted_conditions
+        }
+        response = {
+            response
+        }
+        setResponse = {
+            setResponse
+        }
+        references = {
+            [refA, refB]
+        }
+        active = {
+            XEnded && AEnded && BEnded
+        }
+        onEndeds = {
+            [() => setAEnded(true), () => setBEnded(true)]
+        }
+        /> <
+        Button active = {
+            advance
+        }
+        onClick = {
+            () => {
+                advance && clickHandler()
+            }
+        } >
+        Next <
+        /Button> <
+        />
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/client/src/test/MUSHRA.js` & `reseval-0.1.0/reseval/assets/client/src/test/MUSHRA.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,128 +1,128 @@
-import Chance from 'chance';
-import React, {
-    createRef,
-    useMemo,
-    useState
-} from 'react';
-
-import MediaSliderGroup from '../components/MediaSliderGroup';
-
-import '../css/components.css';
-
-import Button from '../components/Button';
-
-
-/******************************************************************************
- Constants
- ******************************************************************************/
-
-
-// Random number generator
-const chance = new Chance();
-
-
-/******************************************************************************
- MUSHRA test
- ******************************************************************************/
-
-
-export default function MUSHRA({
-    file,
-    conditions,
-    setResponse,
-    onClick
-}) {
-    /* Render a MUSHRA evaluation task */
-    // Create a ref for each media object
-    const refs = useMemo(
-        () => conditions.map(() => createRef()), [conditions]);
-
-    // Whether file has ended
-    const [endeds, setEndeds] = useState(Array(conditions.length).fill(false));
-
-    // Whether sliders have been touched
-    const [toucheds, setToucheds] = useState(
-        Array(conditions.length).fill(false));
-
-    // Non-deterministic ordering of media elements
-    const [permutation, setPermutation] = useState(
-        chance.shuffle([...Array(conditions.length).keys()]));
-    const permuted_conditions = permutation.map(index => conditions[index]);
-
-    // Responses corresponding to each slider
-    const [scores, setScores] = useState(Array(conditions.length).fill(50));
-
-    function clickHandler() {
-
-        // Send response to database and go to next question
-        onClick();
-
-        // Reset media files
-        setEndeds(Array(conditions.length).fill(false));
-
-        // Reset Slider if_touched flag
-        setToucheds(Array(conditions.length).fill(false));
-
-        // Reset scores
-        setScores(Array(conditions.length).fill(50));
-
-        // Get a new permutation
-        setPermutation(chance.shuffle([...Array(conditions.length).keys()]));
-    }
-
-    // Can we advance?
-    const advance =
-        endeds.every(item => item === true) &&
-        toucheds.some(item => item === true);
-
-    // Render
-    return ( <
-        >
-        <
-        MediaSliderGroup file = {
-            file
-        }
-        conditions = {
-            permuted_conditions
-        }
-        permutation = {
-            permutation
-        }
-        scores = {
-            scores
-        }
-        setScores = {
-            setScores
-        }
-        setResponse = {
-            setResponse
-        }
-        refs = {
-            refs
-        }
-        endeds = {
-            endeds
-        }
-        setEndeds = {
-            setEndeds
-        }
-        toucheds = {
-            toucheds
-        }
-        setToucheds = {
-            setToucheds
-        }
-        /> <
-        Button active = {
-            advance
-        }
-        onClick = {
-            () => {
-                advance && clickHandler()
-            }
-        } >
-        Next <
-        /Button> <
-        />
-    );
-};
+import Chance from 'chance';
+import React, {
+    createRef,
+    useMemo,
+    useState
+} from 'react';
+
+import MediaSliderGroup from '../components/MediaSliderGroup';
+
+import '../css/components.css';
+
+import Button from '../components/Button';
+
+
+/******************************************************************************
+ Constants
+ ******************************************************************************/
+
+
+// Random number generator
+const chance = new Chance();
+
+
+/******************************************************************************
+ MUSHRA test
+ ******************************************************************************/
+
+
+export default function MUSHRA({
+    file,
+    conditions,
+    setResponse,
+    onClick
+}) {
+    /* Render a MUSHRA evaluation task */
+    // Create a ref for each media object
+    const refs = useMemo(
+        () => conditions.map(() => createRef()), [conditions]);
+
+    // Whether file has ended
+    const [endeds, setEndeds] = useState(Array(conditions.length).fill(false));
+
+    // Whether sliders have been touched
+    const [toucheds, setToucheds] = useState(
+        Array(conditions.length).fill(false));
+
+    // Non-deterministic ordering of media elements
+    const [permutation, setPermutation] = useState(
+        chance.shuffle([...Array(conditions.length).keys()]));
+    const permuted_conditions = permutation.map(index => conditions[index]);
+
+    // Responses corresponding to each slider
+    const [scores, setScores] = useState(Array(conditions.length).fill(50));
+
+    function clickHandler() {
+
+        // Send response to database and go to next question
+        onClick();
+
+        // Reset media files
+        setEndeds(Array(conditions.length).fill(false));
+
+        // Reset Slider if_touched flag
+        setToucheds(Array(conditions.length).fill(false));
+
+        // Reset scores
+        setScores(Array(conditions.length).fill(50));
+
+        // Get a new permutation
+        setPermutation(chance.shuffle([...Array(conditions.length).keys()]));
+    }
+
+    // Can we advance?
+    const advance =
+        endeds.every(item => item === true) &&
+        toucheds.some(item => item === true);
+
+    // Render
+    return ( <
+        >
+        <
+        MediaSliderGroup file = {
+            file
+        }
+        conditions = {
+            permuted_conditions
+        }
+        permutation = {
+            permutation
+        }
+        scores = {
+            scores
+        }
+        setScores = {
+            setScores
+        }
+        setResponse = {
+            setResponse
+        }
+        refs = {
+            refs
+        }
+        endeds = {
+            endeds
+        }
+        setEndeds = {
+            setEndeds
+        }
+        toucheds = {
+            toucheds
+        }
+        setToucheds = {
+            setToucheds
+        }
+        /> <
+        Button active = {
+            advance
+        }
+        onClick = {
+            () => {
+                advance && clickHandler()
+            }
+        } >
+        Next <
+        /Button> <
+        />
+    );
+}
```

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones4_0.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones4_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones4_1.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones4_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones4_2.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones4_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones4_3.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones4_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones5_0.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones5_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones5_1.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones5_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones5_2.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones5_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones5_3.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones5_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones6_0.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones6_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones6_1.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones6_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones6_2.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones6_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones6_3.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones6_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones7_0.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones7_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones7_1.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones7_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones7_2.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones7_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones7_3.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones7_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones8_0.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones8_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones8_1.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones8_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones8_2.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones8_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/listening_test/tones8_3.wav` & `reseval-0.1.0/reseval/assets/listening_test/tones8_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.0.3/reseval/assets/server/db/index.ts` & `reseval-0.1.0/reseval/assets/server/db/index.ts`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import * as mysql from 'mysql2';
-
-// Load database credentials
-require('dotenv').config();
-const pool = mysql.createPool({
-    host: process.env.MYSQL_HOST,
-    user: process.env.MYSQL_USER,
-    password: process.env.MYSQL_PASS,
-    database: process.env.MYSQL_DBNAME
-})
-
-export const Query = (query: string, values?: any) => {
-    return new Promise((resolve, reject) => {
-        pool.query(query, values, (err, results) => {
-            if (err) {
-                console.log("process.env.MYSQL_HOST:", process.env.MYSQL_HOST);
-                reject(err);
-            } else {
-                resolve(results);
-            }
-        })
-    })
-}
-
-import conditions from './queries/conditions';
-import files from './queries/files';
-import participants from './queries/participants';
-import responses from './queries/responses';
-
-export default { conditions, files, participants, responses, }
+import * as mysql from 'mysql2';
+
+// Load database credentials
+require('dotenv').config();
+const pool = mysql.createPool({
+    host: process.env.RDS_HOSTNAME || process.env.MYSQL_HOST,
+    user: process.env.RDS_USERNAME || process.env.MYSQL_USER,
+    password: process.env.RDS_PASSWORD || process.env.MYSQL_PASS,
+    database: process.env.RDS_DB_NAME || process.env.MYSQL_DBNAME
+})
+
+export const Query = (query: string, values?: any) => {
+    return new Promise((resolve, reject) => {
+        pool.query(query, values, (err, results) => {
+            if (err) {
+                reject(err);
+            } else {
+                resolve(results);
+            }
+        })
+    })
+}
+
+import conditions from './queries/conditions';
+import files from './queries/files';
+import participants from './queries/participants';
+import responses from './queries/responses';
+
+export default { conditions, files, participants, responses, }
```

### Comparing `reseval-0.0.3/reseval/assets/server/db/queries/participants.ts` & `reseval-0.1.0/reseval/assets/server/db/queries/participants.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-import { Query } from '..';
-
-function insert(participant: any) {
-    /* Insert into the participant table */
-    const keys = Object.keys(participant)
-    const values = Object.values(participant);
-    const query =
-        `INSERT INTO participants (${keys.join(', ')})` +
-        ` VALUES (${'?, '.repeat(keys.length - 1) + '?'})`;
-    return Query(query, values);
-}
-
-function update(participant: any) {
-    /* Insert into the participant table */
-    // Get participant ID
-    const ID = participant.ID;
-    delete participant.ID;
-
-    // Get update command
-    const keys = Object.keys(participant);
-    const set = keys.map((key: any, index: Number) =>
-        key +
-        ' = "' +
-        participant[key] +
-        (index == keys.length - 1 ? '"' : '", ')
-    );
-
-    // Don't update if there are no contents
-    if (set.length === 0) return null;
-
-    // Create MySQL query
-    const query = `UPDATE participants SET ${set} WHERE ID="${ID}"`
-    return Query(query);
-}
-
-export default { insert, update };
+import { Query } from '..';
+
+const all = () => Query('SELECT * FROM participants');
+
+function insert(participant: any) {
+    /* Insert into the participant table */
+    const keys = Object.keys(participant);
+    const values = Object.values(participant);
+    const query =
+        `INSERT INTO participants (${keys.join(', ')})` +
+        ` VALUES (${'?, '.repeat(keys.length - 1) + '?'})`;
+    return Query(query, values);
+}
+
+function update(participant: any) {
+    /* Insert into the participant table */
+    // Get participant ID
+    const ID = participant.ID;
+    delete participant.ID;
+
+    // Get update command
+    const keys = Object.keys(participant);
+    const set = keys.map((key: any, index: Number) =>
+        key +
+        ' = "' +
+        participant[key] +
+        (index == keys.length - 1 ? '"' : '", ')
+    );
+
+    // Don't update if there are no contents
+    if (set.length === 0) return null;
+
+    // Create MySQL query
+    const query = `UPDATE participants SET ${set} WHERE ID="${ID}"`
+    return Query(query);
+}
+
+export default { all, insert, update };
```

### Comparing `reseval-0.0.3/reseval/assets/server/routes/api/participants.ts` & `reseval-0.1.0/reseval/assets/server/routes/api/participants.ts`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,50 @@
-import * as express from 'express';
-import db from '../../db';
-
-const router = express.Router();
-
-router.post('/insert', async (request, response) => {
-    const participant = request.body;
-    try {
-        const result = await db.participants.insert(participant);
-        response.json(result);
-    } catch (err) {
-        console.log(err);
-        let err_message = "";
-        if (err instanceof Error) {
-            err_message = err.message;
-        }
-        response.status(500).json({ err: err_message });
-    }
-});
-
-router.post('/update', async (request, response) => {
-    const participant = request.body;
-    try {
-        const result = await db.participants.update(participant);
-        response.json(result);
-    } catch (err) {
-        console.log(err);
-        let err_message = "";
-        if (err instanceof Error) {
-            err_message = err.message;
-        }
-        response.status(500).json({ err: err_message });
-    }
-});
-
-export default router;
+import * as express from 'express';
+import db from '../../db';
+
+const router = express.Router();
+
+router.get('/', async (_, response) => {
+    try {
+        const participants = await db.participants.all();
+        response.json(participants);
+    } catch (err: unknown) {
+        console.log(err);
+        let err_message = "";
+        if (err instanceof Error) {
+            err_message = err.message;
+        }
+        response.status(500).json({ err: err_message });
+    }
+});
+
+router.post('/insert', async (request, response) => {
+    const participant = request.body;
+    try {
+        const result = await db.participants.insert(participant);
+        response.json(result);
+    } catch (err) {
+        console.log(err);
+        let err_message = "";
+        if (err instanceof Error) {
+            err_message = err.message;
+        }
+        response.status(500).json({ err: err_message });
+    }
+});
+
+router.post('/update', async (request, response) => {
+    const participant = request.body;
+    try {
+        const result = await db.participants.update(participant);
+        response.json(result);
+    } catch (err) {
+        console.log(err);
+        let err_message = "";
+        if (err instanceof Error) {
+            err_message = err.message;
+        }
+        response.status(500).json({ err: err_message });
+    }
+});
+
+export default router;
```

### Comparing `reseval-0.0.3/reseval/assets/survey.xml` & `reseval-0.1.0/reseval/assets/survey.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: HTML document, ASCII text, with CRLF line terminators*

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 00000000: 3c48 544d 4c51 7565 7374 696f 6e20 786d  <HTMLQuestion xm
 00000010: 6c6e 733d 2268 7474 703a 2f2f 6d65 6368  lns="http://mech
 00000020: 616e 6963 616c 7475 726b 2e61 6d61 7a6f  anicalturk.amazo
 00000030: 6e61 7773 2e63 6f6d 2f41 5753 4d65 6368  naws.com/AWSMech
 00000040: 616e 6963 616c 5475 726b 4461 7461 5363  anicalTurkDataSc
 00000050: 6865 6d61 732f 3230 3131 2d31 312d 3131  hemas/2011-11-11
 00000060: 2f48 544d 4c51 7565 7374 696f 6e2e 7873  /HTMLQuestion.xs
-00000070: 6422 3e0d 0a20 2020 203c 4854 4d4c 436f  d">..    <HTMLCo
-00000080: 6e74 656e 743e 3c21 5b43 4441 5441 5b0d  ntent><![CDATA[.
-00000090: 0a3c 212d 2d20 594f 5552 2048 544d 4c20  .<!-- YOUR HTML 
-000000a0: 4245 4749 4e53 202d 2d3e 0d0a 3c21 444f  BEGINS -->..<!DO
-000000b0: 4354 5950 4520 6874 6d6c 3e0d 0a3c 6874  CTYPE html>..<ht
-000000c0: 6d6c 3e0d 0a3c 6865 6164 3e0d 0a3c 6d65  ml>..<head>..<me
-000000d0: 7461 2068 7474 702d 6571 7569 763d 2743  ta http-equiv='C
-000000e0: 6f6e 7465 6e74 2d54 7970 6527 2063 6f6e  ontent-Type' con
-000000f0: 7465 6e74 3d27 7465 7874 2f68 746d 6c3b  tent='text/html;
-00000100: 2063 6861 7273 6574 3d55 5446 2d38 272f   charset=UTF-8'/
-00000110: 3e0d 0a3c 7363 7269 7074 2074 7970 653d  >..<script type=
-00000120: 2774 6578 742f 6a61 7661 7363 7269 7074  'text/javascript
-00000130: 2720 7372 633d 2768 7474 7073 3a2f 2f73  ' src='https://s
-00000140: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
-00000150: 6d74 7572 6b2d 7075 626c 6963 2f65 7874  mturk-public/ext
-00000160: 6572 6e61 6c48 4954 5f76 312e 6a73 273e  ernalHIT_v1.js'>
-00000170: 3c2f 7363 7269 7074 3e0d 0a3c 2f68 6561  </script>..</hea
-00000180: 643e 0d0a 3c62 6f64 793e 0d0a 3c66 6f72  d>..<body>..<for
-00000190: 6d20 6e61 6d65 3d27 6d74 7572 6b5f 666f  m name='mturk_fo
-000001a0: 726d 2720 6d65 7468 6f64 3d27 706f 7374  rm' method='post
-000001b0: 2720 6964 3d27 6d74 7572 6b5f 666f 726d  ' id='mturk_form
-000001c0: 2720 6163 7469 6f6e 3d27 6874 7470 733a  ' action='https:
-000001d0: 2f2f 7777 772e 6d74 7572 6b2e 636f 6d2f  //www.mturk.com/
-000001e0: 6d74 7572 6b2f 6578 7465 726e 616c 5375  mturk/externalSu
-000001f0: 626d 6974 273e 3c69 6e70 7574 2074 7970  bmit'><input typ
-00000200: 653d 2768 6964 6465 6e27 2076 616c 7565  e='hidden' value
-00000210: 3d27 2720 6e61 6d65 3d27 6173 7369 676e  ='' name='assign
-00000220: 6d65 6e74 4964 2720 6964 3d27 6173 7369  mentId' id='assi
-00000230: 676e 6d65 6e74 4964 272f 3e0d 0a3c 6832  gnmentId'/>..<h2
-00000240: 3e43 6c69 636b 2074 6865 206c 696e 6b20  >Click the link 
-00000250: 746f 2066 696e 6973 6820 7468 6520 7375  to finish the su
-00000260: 7276 6579 2c20 7468 656e 2070 6173 7465  rvey, then paste
-00000270: 2074 6865 2073 7572 7665 795f 6964 2068   the survey_id h
-00000280: 6572 653a 3c2f 6832 3e0d 0a3c 6833 3e20  ere:</h2>..<h3> 
-00000290: 3c61 2074 6172 6765 743d 225f 626c 616e  <a target="_blan
-000002a0: 6b22 2072 656c 3d22 6e6f 6f70 656e 6572  k" rel="noopener
-000002b0: 206e 6f72 6566 6572 7265 7222 2068 7265   noreferrer" hre
-000002c0: 663d 227b 7d22 3e4c 696e 6b3c 2f61 3e3c  f="{}">Link</a><
-000002d0: 2f68 333e 0d0a 0d0a 3c64 6976 3e0d 0a20  /h3>....<div>.. 
-000002e0: 203c 696e 7075 7420 7479 7065 3d27 7465   <input type='te
-000002f0: 7874 2720 6e61 6d65 3d27 7375 7276 6579  xt' name='survey
-00000300: 5f69 6427 2070 6c61 6365 686f 6c64 6572  _id' placeholder
-00000310: 3d27 5479 7065 2069 6e20 796f 7572 2061  ='Type in your a
-00000320: 6e73 7765 7220 6865 7265 273e 0d0a 3c2f  nswer here'>..</
-00000330: 6469 763e 0d0a 3c70 3e3c 696e 7075 7420  div>..<p><input 
-00000340: 7479 7065 3d27 7375 626d 6974 2720 6964  type='submit' id
-00000350: 3d27 7375 626d 6974 4275 7474 6f6e 2720  ='submitButton' 
-00000360: 7661 6c75 653d 2753 7562 6d69 7427 202f  value='Submit' /
-00000370: 3e3c 2f70 3e3c 2f66 6f72 6d3e 0d0a 3c73  ></p></form>..<s
-00000380: 6372 6970 7420 6c61 6e67 7561 6765 3d27  cript language='
-00000390: 4a61 7661 7363 7269 7074 273e 7475 726b  Javascript'>turk
-000003a0: 5365 7441 7373 6967 6e6d 656e 7449 4428  SetAssignmentID(
-000003b0: 293b 3c2f 7363 7269 7074 3e0d 0a3c 2f62  );</script>..</b
-000003c0: 6f64 793e 3c2f 6874 6d6c 3e0d 0a3c 212d  ody></html>..<!-
-000003d0: 2d20 594f 5552 2048 544d 4c20 454e 4453  - YOUR HTML ENDS
-000003e0: 202d 2d3e 0d0a 5d5d 3e0d 0a20 2020 203c   -->..]]>..    <
-000003f0: 2f48 544d 4c43 6f6e 7465 6e74 3e0d 0a20  /HTMLContent>.. 
-00000400: 2020 203c 4672 616d 6548 6569 6768 743e     <FrameHeight>
-00000410: 3630 303c 2f46 7261 6d65 4865 6967 6874  600</FrameHeight
-00000420: 3e0d 0a3c 2f48 544d 4c51 7565 7374 696f  >..</HTMLQuestio
-00000430: 6e3e 0d0a 0d0a 0d0a 0d0a                 n>........
+00000070: 6422 3e0a 2020 2020 3c48 544d 4c43 6f6e  d">.    <HTMLCon
+00000080: 7465 6e74 3e3c 215b 4344 4154 415b 0a3c  tent><![CDATA[.<
+00000090: 212d 2d20 594f 5552 2048 544d 4c20 4245  !-- YOUR HTML BE
+000000a0: 4749 4e53 202d 2d3e 0a3c 2144 4f43 5459  GINS -->.<!DOCTY
+000000b0: 5045 2068 746d 6c3e 0a3c 6874 6d6c 3e0a  PE html>.<html>.
+000000c0: 3c68 6561 643e 0a3c 6d65 7461 2068 7474  <head>.<meta htt
+000000d0: 702d 6571 7569 763d 2743 6f6e 7465 6e74  p-equiv='Content
+000000e0: 2d54 7970 6527 2063 6f6e 7465 6e74 3d27  -Type' content='
+000000f0: 7465 7874 2f68 746d 6c3b 2063 6861 7273  text/html; chars
+00000100: 6574 3d55 5446 2d38 272f 3e0a 3c73 6372  et=UTF-8'/>.<scr
+00000110: 6970 7420 7479 7065 3d27 7465 7874 2f6a  ipt type='text/j
+00000120: 6176 6173 6372 6970 7427 2073 7263 3d27  avascript' src='
+00000130: 6874 7470 733a 2f2f 7333 2e61 6d61 7a6f  https://s3.amazo
+00000140: 6e61 7773 2e63 6f6d 2f6d 7475 726b 2d70  naws.com/mturk-p
+00000150: 7562 6c69 632f 6578 7465 726e 616c 4849  ublic/externalHI
+00000160: 545f 7631 2e6a 7327 3e3c 2f73 6372 6970  T_v1.js'></scrip
+00000170: 743e 0a3c 2f68 6561 643e 0a3c 626f 6479  t>.</head>.<body
+00000180: 3e0a 3c66 6f72 6d20 6e61 6d65 3d27 6d74  >.<form name='mt
+00000190: 7572 6b5f 666f 726d 2720 6d65 7468 6f64  urk_form' method
+000001a0: 3d27 706f 7374 2720 6964 3d27 6d74 7572  ='post' id='mtur
+000001b0: 6b5f 666f 726d 2720 6163 7469 6f6e 3d27  k_form' action='
+000001c0: 6874 7470 733a 2f2f 7777 772e 6d74 7572  https://www.mtur
+000001d0: 6b2e 636f 6d2f 6d74 7572 6b2f 6578 7465  k.com/mturk/exte
+000001e0: 726e 616c 5375 626d 6974 273e 3c69 6e70  rnalSubmit'><inp
+000001f0: 7574 2074 7970 653d 2768 6964 6465 6e27  ut type='hidden'
+00000200: 2076 616c 7565 3d27 2720 6e61 6d65 3d27   value='' name='
+00000210: 6173 7369 676e 6d65 6e74 4964 2720 6964  assignmentId' id
+00000220: 3d27 6173 7369 676e 6d65 6e74 4964 272f  ='assignmentId'/
+00000230: 3e0a 3c68 323e 436c 6963 6b20 7468 6520  >.<h2>Click the 
+00000240: 6c69 6e6b 2074 6f20 6669 6e69 7368 2074  link to finish t
+00000250: 6865 2073 7572 7665 792c 2074 6865 6e20  he survey, then 
+00000260: 7061 7374 6520 7468 6520 7375 7276 6579  paste the survey
+00000270: 5f69 6420 6865 7265 3a3c 2f68 323e 0a3c  _id here:</h2>.<
+00000280: 6833 3e20 3c61 2074 6172 6765 743d 225f  h3> <a target="_
+00000290: 626c 616e 6b22 2072 656c 3d22 6e6f 6f70  blank" rel="noop
+000002a0: 656e 6572 206e 6f72 6566 6572 7265 7222  ener noreferrer"
+000002b0: 2068 7265 663d 227b 7d22 3e4c 696e 6b3c   href="{}">Link<
+000002c0: 2f61 3e3c 2f68 333e 0a0a 3c64 6976 3e0a  /a></h3>..<div>.
+000002d0: 2020 3c69 6e70 7574 2074 7970 653d 2774    <input type='t
+000002e0: 6578 7427 206e 616d 653d 2773 7572 7665  ext' name='surve
+000002f0: 795f 6964 2720 706c 6163 6568 6f6c 6465  y_id' placeholde
+00000300: 723d 2754 7970 6520 696e 2079 6f75 7220  r='Type in your 
+00000310: 616e 7377 6572 2068 6572 6527 3e0a 3c2f  answer here'>.</
+00000320: 6469 763e 0a3c 703e 3c69 6e70 7574 2074  div>.<p><input t
+00000330: 7970 653d 2773 7562 6d69 7427 2069 643d  ype='submit' id=
+00000340: 2773 7562 6d69 7442 7574 746f 6e27 2076  'submitButton' v
+00000350: 616c 7565 3d27 5375 626d 6974 2720 2f3e  alue='Submit' />
+00000360: 3c2f 703e 3c2f 666f 726d 3e0a 3c73 6372  </p></form>.<scr
+00000370: 6970 7420 6c61 6e67 7561 6765 3d27 4a61  ipt language='Ja
+00000380: 7661 7363 7269 7074 273e 7475 726b 5365  vascript'>turkSe
+00000390: 7441 7373 6967 6e6d 656e 7449 4428 293b  tAssignmentID();
+000003a0: 3c2f 7363 7269 7074 3e0a 3c2f 626f 6479  </script>.</body
+000003b0: 3e3c 2f68 746d 6c3e 0a3c 212d 2d20 594f  ></html>.<!-- YO
+000003c0: 5552 2048 544d 4c20 454e 4453 202d 2d3e  UR HTML ENDS -->
+000003d0: 0a5d 5d3e 0a20 2020 203c 2f48 544d 4c43  .]]>.    </HTMLC
+000003e0: 6f6e 7465 6e74 3e0a 2020 2020 3c46 7261  ontent>.    <Fra
+000003f0: 6d65 4865 6967 6874 3e36 3030 3c2f 4672  meHeight>600</Fr
+00000400: 616d 6548 6569 6768 743e 0a3c 2f48 544d  ameHeight>.</HTM
+00000410: 4c51 7565 7374 696f 6e3e 0a0a 0a0a       LQuestion>....
```

### Comparing `reseval-0.0.3/reseval/assets/tsconfig.json` & `reseval-0.1.0/reseval/assets/tsconfig.json`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-{
-  "compilerOptions": {
-    /* Visit https://aka.ms/tsconfig.json to read more about this file */
-
-    /* Projects */
-    // "incremental": true,                              /* Enable incremental compilation */
-    // "composite": true,                                /* Enable constraints that allow a TypeScript project to be used with project references. */
-    // "tsBuildInfoFile": "./",                          /* Specify the folder for .tsbuildinfo incremental compilation files. */
-    // "disableSourceOfProjectReferenceRedirect": true,  /* Disable preferring source files instead of declaration files when referencing composite projects */
-    // "disableSolutionSearching": true,                 /* Opt a project out of multi-project reference checking when editing. */
-    // "disableReferencedProjectLoad": true,             /* Reduce the number of projects loaded automatically by TypeScript. */
-
-    /* Language and Environment */
-    "target": "es6",                                     /* Set the JavaScript language version for emitted JavaScript and include compatible library declarations. */
-    // "lib": [],                                        /* Specify a set of bundled library declaration files that describe the target runtime environment. */
-    // "jsx": "preserve",                                /* Specify what JSX code is generated. */
-    // "experimentalDecorators": true,                   /* Enable experimental support for TC39 stage 2 draft decorators. */
-    // "emitDecoratorMetadata": true,                    /* Emit design-type metadata for decorated declarations in source files. */
-    // "jsxFactory": "",                                 /* Specify the JSX factory function used when targeting React JSX emit, e.g. 'React.createElement' or 'h' */
-    // "jsxFragmentFactory": "",                         /* Specify the JSX Fragment reference used for fragments when targeting React JSX emit e.g. 'React.Fragment' or 'Fragment'. */
-    // "jsxImportSource": "",                            /* Specify module specifier used to import the JSX factory functions when using `jsx: react-jsx*`.` */
-    // "reactNamespace": "",                             /* Specify the object invoked for `createElement`. This only applies when targeting `react` JSX emit. */
-    // "noLib": true,                                    /* Disable including any library files, including the default lib.d.ts. */
-    // "useDefineForClassFields": true,                  /* Emit ECMAScript-standard-compliant class fields. */
-
-    /* Modules */
-    "module": "commonjs",                                /* Specify what module code is generated. */
-    // "rootDir": "./src",                                  /* Specify the root folder within your source files. */
-    // "moduleResolution": "node",                       /* Specify how TypeScript looks up a file from a given module specifier. */
-    // "baseUrl": "./",                                  /* Specify the base directory to resolve non-relative module names. */
-    // "paths": {},                                      /* Specify a set of entries that re-map imports to additional lookup locations. */
-    // "rootDirs": [],                                   /* Allow multiple folders to be treated as one when resolving modules. */
-    // "typeRoots": [],                                  /* Specify multiple folders that act like `./node_modules/@types`. */
-    // "types": [],                                      /* Specify type package names to be included without being referenced in a source file. */
-    // "allowUmdGlobalAccess": true,                     /* Allow accessing UMD globals from modules. */
-    // "resolveJsonModule": true,                        /* Enable importing .json files */
-    // "noResolve": true,                                /* Disallow `import`s, `require`s or `<reference>`s from expanding the number of files TypeScript should add to a project. */
-
-    /* JavaScript Support */
-    // "allowJs": true,                                  /* Allow JavaScript files to be a part of your program. Use the `checkJS` option to get errors from these files. */
-    // "checkJs": true,                                  /* Enable error reporting in type-checked JavaScript files. */
-    // "maxNodeModuleJsDepth": 1,                        /* Specify the maximum folder depth used for checking JavaScript files from `node_modules`. Only applicable with `allowJs`. */
-
-    /* Emit */
-    // "declaration": true,                              /* Generate .d.ts files from TypeScript and JavaScript files in your project. */
-    // "declarationMap": true,                           /* Create sourcemaps for d.ts files. */
-    // "emitDeclarationOnly": true,                      /* Only output d.ts files and not JavaScript files. */
-    // "sourceMap": true,                                /* Create source map files for emitted JavaScript files. */
-    // "outFile": "./",                                  /* Specify a file that bundles all outputs into one JavaScript file. If `declaration` is true, also designates a file that bundles all .d.ts output. */
-    // "outDir": "./dist",                                   /* Specify an output folder for all emitted files. */
-    // "removeComments": true,                           /* Disable emitting comments. */
-    // "noEmit": true,                                   /* Disable emitting files from a compilation. */
-    // "importHelpers": true,                            /* Allow importing helper functions from tslib once per project, instead of including them per-file. */
-    // "importsNotUsedAsValues": "remove",               /* Specify emit/checking behavior for imports that are only used for types */
-    // "downlevelIteration": true,                       /* Emit more compliant, but verbose and less performant JavaScript for iteration. */
-    // "sourceRoot": "",                                 /* Specify the root path for debuggers to find the reference source code. */
-    // "mapRoot": "",                                    /* Specify the location where debugger should locate map files instead of generated locations. */
-    // "inlineSourceMap": true,                          /* Include sourcemap files inside the emitted JavaScript. */
-    // "inlineSources": true,                            /* Include source code in the sourcemaps inside the emitted JavaScript. */
-    // "emitBOM": true,                                  /* Emit a UTF-8 Byte Order Mark (BOM) in the beginning of output files. */
-    // "newLine": "crlf",                                /* Set the newline character for emitting files. */
-    // "stripInternal": true,                            /* Disable emitting declarations that have `@internal` in their JSDoc comments. */
-    // "noEmitHelpers": true,                            /* Disable generating custom helper functions like `__extends` in compiled output. */
-    // "noEmitOnError": true,                            /* Disable emitting files if any type checking errors are reported. */
-    // "preserveConstEnums": true,                       /* Disable erasing `const enum` declarations in generated code. */
-    // "declarationDir": "./",                           /* Specify the output directory for generated declaration files. */
-
-    /* Interop Constraints */
-    // "isolatedModules": true,                          /* Ensure that each file can be safely transpiled without relying on other imports. */
-    // "allowSyntheticDefaultImports": true,             /* Allow 'import x from y' when a module doesn't have a default export. */
-    "esModuleInterop": true,                             /* Emit additional JavaScript to ease support for importing CommonJS modules. This enables `allowSyntheticDefaultImports` for type compatibility. */
-    // "preserveSymlinks": true,                         /* Disable resolving symlinks to their realpath. This correlates to the same flag in node. */
-    "forceConsistentCasingInFileNames": true,            /* Ensure that casing is correct in imports. */
-
-    /* Type Checking */
-    "strict": true,                                      /* Enable all strict type-checking options. */
-    // "noImplicitAny": true,                            /* Enable error reporting for expressions and declarations with an implied `any` type.. */
-    // "strictNullChecks": true,                         /* When type checking, take into account `null` and `undefined`. */
-    // "strictFunctionTypes": true,                      /* When assigning functions, check to ensure parameters and the return values are subtype-compatible. */
-    // "strictBindCallApply": true,                      /* Check that the arguments for `bind`, `call`, and `apply` methods match the original function. */
-    // "strictPropertyInitialization": true,             /* Check for class properties that are declared but not set in the constructor. */
-    // "noImplicitThis": true,                           /* Enable error reporting when `this` is given the type `any`. */
-    // "useUnknownInCatchVariables": true,               /* Type catch clause variables as 'unknown' instead of 'any'. */
-    // "alwaysStrict": true,                             /* Ensure 'use strict' is always emitted. */
-    // "noUnusedLocals": true,                           /* Enable error reporting when a local variables aren't read. */
-    // "noUnusedParameters": true,                       /* Raise an error when a function parameter isn't read */
-    // "exactOptionalPropertyTypes": true,               /* Interpret optional property types as written, rather than adding 'undefined'. */
-    // "noImplicitReturns": true,                        /* Enable error reporting for codepaths that do not explicitly return in a function. */
-    // "noFallthroughCasesInSwitch": true,               /* Enable error reporting for fallthrough cases in switch statements. */
-    // "noUncheckedIndexedAccess": true,                 /* Include 'undefined' in index signature results */
-    // "noImplicitOverride": true,                       /* Ensure overriding members in derived classes are marked with an override modifier. */
-    // "noPropertyAccessFromIndexSignature": true,       /* Enforces using indexed accessors for keys declared using an indexed type */
-    // "allowUnusedLabels": true,                        /* Disable error reporting for unused labels. */
-    // "allowUnreachableCode": true,                     /* Disable error reporting for unreachable code. */
-
-    /* Completeness */
-    // "skipDefaultLibCheck": true,                      /* Skip type checking .d.ts files that are included with TypeScript. */
-    "skipLibCheck": true                                 /* Skip type checking all .d.ts files. */
-  },
-  "exclude": [
-    "./node_modules"
-  ]
-}
+{
+  "compilerOptions": {
+    /* Visit https://aka.ms/tsconfig.json to read more about this file */
+
+    /* Projects */
+    // "incremental": true,                              /* Enable incremental compilation */
+    // "composite": true,                                /* Enable constraints that allow a TypeScript project to be used with project references. */
+    // "tsBuildInfoFile": "./",                          /* Specify the folder for .tsbuildinfo incremental compilation files. */
+    // "disableSourceOfProjectReferenceRedirect": true,  /* Disable preferring source files instead of declaration files when referencing composite projects */
+    // "disableSolutionSearching": true,                 /* Opt a project out of multi-project reference checking when editing. */
+    // "disableReferencedProjectLoad": true,             /* Reduce the number of projects loaded automatically by TypeScript. */
+
+    /* Language and Environment */
+    "target": "es6",                                     /* Set the JavaScript language version for emitted JavaScript and include compatible library declarations. */
+    // "lib": [],                                        /* Specify a set of bundled library declaration files that describe the target runtime environment. */
+    // "jsx": "preserve",                                /* Specify what JSX code is generated. */
+    // "experimentalDecorators": true,                   /* Enable experimental support for TC39 stage 2 draft decorators. */
+    // "emitDecoratorMetadata": true,                    /* Emit design-type metadata for decorated declarations in source files. */
+    // "jsxFactory": "",                                 /* Specify the JSX factory function used when targeting React JSX emit, e.g. 'React.createElement' or 'h' */
+    // "jsxFragmentFactory": "",                         /* Specify the JSX Fragment reference used for fragments when targeting React JSX emit e.g. 'React.Fragment' or 'Fragment'. */
+    // "jsxImportSource": "",                            /* Specify module specifier used to import the JSX factory functions when using `jsx: react-jsx*`.` */
+    // "reactNamespace": "",                             /* Specify the object invoked for `createElement`. This only applies when targeting `react` JSX emit. */
+    // "noLib": true,                                    /* Disable including any library files, including the default lib.d.ts. */
+    // "useDefineForClassFields": true,                  /* Emit ECMAScript-standard-compliant class fields. */
+
+    /* Modules */
+    "module": "commonjs",                                /* Specify what module code is generated. */
+    // "rootDir": "./src",                                  /* Specify the root folder within your source files. */
+    // "moduleResolution": "node",                       /* Specify how TypeScript looks up a file from a given module specifier. */
+    // "baseUrl": "./",                                  /* Specify the base directory to resolve non-relative module names. */
+    // "paths": {},                                      /* Specify a set of entries that re-map imports to additional lookup locations. */
+    // "rootDirs": [],                                   /* Allow multiple folders to be treated as one when resolving modules. */
+    // "typeRoots": [],                                  /* Specify multiple folders that act like `./node_modules/@types`. */
+    // "types": [],                                      /* Specify type package names to be included without being referenced in a source file. */
+    // "allowUmdGlobalAccess": true,                     /* Allow accessing UMD globals from modules. */
+    // "resolveJsonModule": true,                        /* Enable importing .json files */
+    // "noResolve": true,                                /* Disallow `import`s, `require`s or `<reference>`s from expanding the number of files TypeScript should add to a project. */
+
+    /* JavaScript Support */
+    // "allowJs": true,                                  /* Allow JavaScript files to be a part of your program. Use the `checkJS` option to get errors from these files. */
+    // "checkJs": true,                                  /* Enable error reporting in type-checked JavaScript files. */
+    // "maxNodeModuleJsDepth": 1,                        /* Specify the maximum folder depth used for checking JavaScript files from `node_modules`. Only applicable with `allowJs`. */
+
+    /* Emit */
+    // "declaration": true,                              /* Generate .d.ts files from TypeScript and JavaScript files in your project. */
+    // "declarationMap": true,                           /* Create sourcemaps for d.ts files. */
+    // "emitDeclarationOnly": true,                      /* Only output d.ts files and not JavaScript files. */
+    // "sourceMap": true,                                /* Create source map files for emitted JavaScript files. */
+    // "outFile": "./",                                  /* Specify a file that bundles all outputs into one JavaScript file. If `declaration` is true, also designates a file that bundles all .d.ts output. */
+    // "outDir": "./dist",                                   /* Specify an output folder for all emitted files. */
+    // "removeComments": true,                           /* Disable emitting comments. */
+    // "noEmit": true,                                   /* Disable emitting files from a compilation. */
+    // "importHelpers": true,                            /* Allow importing helper functions from tslib once per project, instead of including them per-file. */
+    // "importsNotUsedAsValues": "remove",               /* Specify emit/checking behavior for imports that are only used for types */
+    // "downlevelIteration": true,                       /* Emit more compliant, but verbose and less performant JavaScript for iteration. */
+    // "sourceRoot": "",                                 /* Specify the root path for debuggers to find the reference source code. */
+    // "mapRoot": "",                                    /* Specify the location where debugger should locate map files instead of generated locations. */
+    // "inlineSourceMap": true,                          /* Include sourcemap files inside the emitted JavaScript. */
+    // "inlineSources": true,                            /* Include source code in the sourcemaps inside the emitted JavaScript. */
+    // "emitBOM": true,                                  /* Emit a UTF-8 Byte Order Mark (BOM) in the beginning of output files. */
+    // "newLine": "crlf",                                /* Set the newline character for emitting files. */
+    // "stripInternal": true,                            /* Disable emitting declarations that have `@internal` in their JSDoc comments. */
+    // "noEmitHelpers": true,                            /* Disable generating custom helper functions like `__extends` in compiled output. */
+    // "noEmitOnError": true,                            /* Disable emitting files if any type checking errors are reported. */
+    // "preserveConstEnums": true,                       /* Disable erasing `const enum` declarations in generated code. */
+    // "declarationDir": "./",                           /* Specify the output directory for generated declaration files. */
+
+    /* Interop Constraints */
+    // "isolatedModules": true,                          /* Ensure that each file can be safely transpiled without relying on other imports. */
+    // "allowSyntheticDefaultImports": true,             /* Allow 'import x from y' when a module doesn't have a default export. */
+    "esModuleInterop": true,                             /* Emit additional JavaScript to ease support for importing CommonJS modules. This enables `allowSyntheticDefaultImports` for type compatibility. */
+    // "preserveSymlinks": true,                         /* Disable resolving symlinks to their realpath. This correlates to the same flag in node. */
+    "forceConsistentCasingInFileNames": true,            /* Ensure that casing is correct in imports. */
+
+    /* Type Checking */
+    "strict": true,                                      /* Enable all strict type-checking options. */
+    // "noImplicitAny": true,                            /* Enable error reporting for expressions and declarations with an implied `any` type.. */
+    // "strictNullChecks": true,                         /* When type checking, take into account `null` and `undefined`. */
+    // "strictFunctionTypes": true,                      /* When assigning functions, check to ensure parameters and the return values are subtype-compatible. */
+    // "strictBindCallApply": true,                      /* Check that the arguments for `bind`, `call`, and `apply` methods match the original function. */
+    // "strictPropertyInitialization": true,             /* Check for class properties that are declared but not set in the constructor. */
+    // "noImplicitThis": true,                           /* Enable error reporting when `this` is given the type `any`. */
+    // "useUnknownInCatchVariables": true,               /* Type catch clause variables as 'unknown' instead of 'any'. */
+    // "alwaysStrict": true,                             /* Ensure 'use strict' is always emitted. */
+    // "noUnusedLocals": true,                           /* Enable error reporting when a local variables aren't read. */
+    // "noUnusedParameters": true,                       /* Raise an error when a function parameter isn't read */
+    // "exactOptionalPropertyTypes": true,               /* Interpret optional property types as written, rather than adding 'undefined'. */
+    // "noImplicitReturns": true,                        /* Enable error reporting for codepaths that do not explicitly return in a function. */
+    // "noFallthroughCasesInSwitch": true,               /* Enable error reporting for fallthrough cases in switch statements. */
+    // "noUncheckedIndexedAccess": true,                 /* Include 'undefined' in index signature results */
+    // "noImplicitOverride": true,                       /* Ensure overriding members in derived classes are marked with an override modifier. */
+    // "noPropertyAccessFromIndexSignature": true,       /* Enforces using indexed accessors for keys declared using an indexed type */
+    // "allowUnusedLabels": true,                        /* Disable error reporting for unused labels. */
+    // "allowUnreachableCode": true,                     /* Disable error reporting for unreachable code. */
+
+    /* Completeness */
+    // "skipDefaultLibCheck": true,                      /* Skip type checking .d.ts files that are included with TypeScript. */
+    "skipLibCheck": true                                 /* Skip type checking all .d.ts files. */
+  },
+  "exclude": [
+    "./node_modules"
+  ]
+}
```

### Comparing `reseval-0.0.3/reseval/convert/audio.py` & `reseval-0.1.0/reseval/convert/audio.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import argparse
-import glob
-import os
-import shutil
-import subprocess
-from pathlib import Path
-
-
-###############################################################################
-# Convert audio to mp3
-###############################################################################
-
-
-def from_file_to_file(input_file, output_file=None, verbose=True):
-    """Convert audio file to mp3"""
-    # Handle input files starting with hyphen
-    clean_input = False
-    if input_file.stem.startswith('-'):
-        dummy_file = input_file.parent / input_file.name[1:]
-        shutil.copyfile(input_file, dummy_file)
-        input_file = dummy_file
-        clean_input = True
-
-    # Handle output files starting with hyphen
-    clean_output = False
-    if output_file.stem.startswith('-'):
-        output_file = output_file.parent / output_file.name[1:]
-        clean_output = True
-
-    # Default output filename is same as input but with MP3 extension
-    if output_file is None:
-        output_file = input_file.with_suffix('.mp3')
-
-    # Ensure output directory exists
-    output_file.parent.mkdir(exist_ok=True, parents=True)
-
-    # Convert
-    args = [
-        'ffmpeg',
-        '-y',
-        '-i',
-        str(input_file),
-        '-b:a',
-         '320k',
-        str(output_file)]
-    process = subprocess.Popen(
-        args,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        universal_newlines=True)
-    stdout, stderr = process.communicate()
-
-    # Maybe print
-    if verbose or process.returncode != 0:
-        print(stdout)
-        print(stderr)
-
-    # Clean-up input files starting with hyphen
-    if clean_input:
-        os.remove(input_file)
-
-    # Clean-up output files starting with hyphen
-    if clean_output:
-        os.replace(output_file, output_file.parent / ('-' + output_file.name))
-
-
-def from_files_to_files(input_files, output_files=None):
-    """Convert audio files to mp3"""
-    # Convert to paths
-    input_files = [Path(file) for file in input_files]
-
-    # Default output filename is same as input but with MP3 extension
-    if output_files is None:
-        output_files = [file.with_suffix('.mp3') for file in input_files]
-
-    # Multiprocess conversion
-    # with mp.Pool() as pool:
-    #     pool.starmap(from_file_to_file, zip(input_files, output_files))
-
-    for input_file, output_file in zip(input_files, output_files):
-        from_file_to_file(input_file, output_file)
-
-
-###############################################################################
-# Entry point
-###############################################################################
-
-
-def expand_files(files):
-    """Expands a wildcard to a list of paths for Windows compatibility"""
-    # Split at whitespace
-    files = files.split()
-
-    # Handle wildcard expansion
-    if len(files) == 1 and '*' in files[0]:
-        files = glob.glob(files[0])
-
-    # Convert to Path objects
-    return files
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(description='Convert audio to MP3')
-
-    # Handle wildcards across platforms
-    if os.name == 'nt':
-        parser.add_argument(
-            '--input_files',
-            type=expand_files,
-            help='The audio files to convert to mp3')
-    else:
-        parser.add_argument(
-            '--input_files',
-            nargs='+',
-            help='The audio files to convert to mp3')
-
-    parser.add_argument(
-        '--output_files',
-        type=Path,
-        nargs='+',
-        help='The corresponding output files. ' + \
-             'Uses same filename with mp3 extension by default')
-    return parser.parse_args()
-
-
-if __name__ == '__main__':
-    from_files_to_files(**vars(parse_args()))
+import argparse
+import glob
+import os
+import shutil
+import subprocess
+from pathlib import Path
+
+
+###############################################################################
+# Convert audio to mp3
+###############################################################################
+
+
+def from_file_to_file(input_file, output_file=None, verbose=True):
+    """Convert audio file to mp3"""
+    # Handle input files starting with hyphen
+    clean_input = False
+    if input_file.stem.startswith('-'):
+        dummy_file = input_file.parent / input_file.name[1:]
+        shutil.copyfile(input_file, dummy_file)
+        input_file = dummy_file
+        clean_input = True
+
+    # Handle output files starting with hyphen
+    clean_output = False
+    if output_file.stem.startswith('-'):
+        output_file = output_file.parent / output_file.name[1:]
+        clean_output = True
+
+    # Default output filename is same as input but with MP3 extension
+    if output_file is None:
+        output_file = input_file.with_suffix('.mp3')
+
+    # Ensure output directory exists
+    output_file.parent.mkdir(exist_ok=True, parents=True)
+
+    # Convert
+    args = [
+        'ffmpeg',
+        '-y',
+        '-i',
+        str(input_file),
+        '-b:a',
+         '320k',
+        str(output_file)]
+    process = subprocess.Popen(
+        args,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        universal_newlines=True)
+    stdout, stderr = process.communicate()
+
+    # Maybe print
+    if verbose or process.returncode != 0:
+        print(stdout)
+        print(stderr)
+
+    # Clean-up input files starting with hyphen
+    if clean_input:
+        os.remove(input_file)
+
+    # Clean-up output files starting with hyphen
+    if clean_output:
+        os.replace(output_file, output_file.parent / ('-' + output_file.name))
+
+
+def from_files_to_files(input_files, output_files=None):
+    """Convert audio files to mp3"""
+    # Convert to paths
+    input_files = [Path(file) for file in input_files]
+
+    # Default output filename is same as input but with MP3 extension
+    if output_files is None:
+        output_files = [file.with_suffix('.mp3') for file in input_files]
+
+    # Multiprocess conversion
+    # with mp.Pool() as pool:
+    #     pool.starmap(from_file_to_file, zip(input_files, output_files))
+
+    for input_file, output_file in zip(input_files, output_files):
+        from_file_to_file(input_file, output_file)
+
+
+###############################################################################
+# Entry point
+###############################################################################
+
+
+def expand_files(files):
+    """Expands a wildcard to a list of paths for Windows compatibility"""
+    # Split at whitespace
+    files = files.split()
+
+    # Handle wildcard expansion
+    if len(files) == 1 and '*' in files[0]:
+        files = glob.glob(files[0])
+
+    # Convert to Path objects
+    return files
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(description='Convert audio to MP3')
+
+    # Handle wildcards across platforms
+    if os.name == 'nt':
+        parser.add_argument(
+            '--input_files',
+            type=expand_files,
+            help='The audio files to convert to mp3')
+    else:
+        parser.add_argument(
+            '--input_files',
+            nargs='+',
+            help='The audio files to convert to mp3')
+
+    parser.add_argument(
+        '--output_files',
+        type=Path,
+        nargs='+',
+        help='The corresponding output files. ' + \
+             'Uses same filename with mp3 extension by default')
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    from_files_to_files(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/convert/image.py` & `reseval-0.1.0/reseval/convert/image.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import argparse
-import glob
-import io
-import multiprocessing as mp
-import os
-from pathlib import Path
-
-from PIL import Image
-
-
-###############################################################################
-# Convert image to jpeg
-###############################################################################
-
-
-def from_file_to_file(input_file, output_file=None):
-    """Convert image file to jpeg"""
-    # Default output filename is same as input but with JPEG extension
-    if output_file is None:
-        output_file = input_file.with_suffix('.jpg')
-
-    # Open image file
-    image = Image.open(input_file)
-
-    # Create raw byte buffer
-    buffer = io.BytesIO()
-
-    # Perform compression to 25% of the original file size
-    image.save(buffer, 'JPEG', quality=25)
-
-    # Write the buffer to a file
-    with open(output_file, 'w') as file:
-        file.write(buffer.contents())
-
-
-def from_files_to_files(input_files, output_files=None):
-    """Convert audio files to mp3"""
-    # Convert to paths
-    input_files = [Path(file) for file in input_files]
-
-    # Default output filename is same as input but with MP3 extension
-    if output_files is None:
-        output_files = [file.with_suffix('.jpg') for file in input_files]
-
-    # Multiprocess conversion
-    with mp.Pool() as pool:
-        pool.starmap(from_file_to_file, zip(input_files, output_files))
-
-    # for input_file, output_file in zip(input_files, output_files):
-    #     from_file_to_file(input_file, output_file)
-
-
-###############################################################################
-# Entry point
-###############################################################################
-
-
-def expand_files(files):
-    """Expands a wildcard to a list of paths for Windows compatibility"""
-    # Split at whitespace
-    files = files.split()
-
-    # Handle wildcard expansion
-    if len(files) == 1 and '*' in files[0]:
-        files = glob.glob(files[0])
-
-    # Convert to Path objects
-    return files
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(description='Convert images to JPEG')
-
-    # Handle wildcards across platforms
-    if os.name == 'nt':
-        parser.add_argument(
-            '--input_files',
-            type=expand_files,
-            help='The image files to convert to jpeg')
-    else:
-        parser.add_argument(
-            '--input_files',
-            nargs='+',
-            help='The image files to convert to jpeg')
-
-    parser.add_argument(
-        '--output_files',
-        type=Path,
-        nargs='+',
-        help='The corresponding output files. ' +
-             'Uses same filename with jpg extension by default')
-    return parser.parse_args()
-
-
-if __name__ == '__main__':
-    from_files_to_files(**vars(parse_args()))
+import argparse
+import glob
+import io
+import multiprocessing as mp
+import os
+from pathlib import Path
+
+from PIL import Image
+
+
+###############################################################################
+# Convert image to jpeg
+###############################################################################
+
+
+def from_file_to_file(input_file, output_file=None):
+    """Convert image file to jpeg"""
+    # Default output filename is same as input but with JPEG extension
+    if output_file is None:
+        output_file = input_file.with_suffix('.jpg')
+
+    # Open image file
+    image = Image.open(input_file)
+
+    # Create raw byte buffer
+    buffer = io.BytesIO()
+
+    # Perform compression to 25% of the original file size
+    image.save(buffer, 'JPEG', quality=25)
+
+    # Write the buffer to a file
+    with open(output_file, 'w') as file:
+        file.write(buffer.contents())
+
+
+def from_files_to_files(input_files, output_files=None):
+    """Convert audio files to mp3"""
+    # Convert to paths
+    input_files = [Path(file) for file in input_files]
+
+    # Default output filename is same as input but with MP3 extension
+    if output_files is None:
+        output_files = [file.with_suffix('.jpg') for file in input_files]
+
+    # Multiprocess conversion
+    with mp.Pool() as pool:
+        pool.starmap(from_file_to_file, zip(input_files, output_files))
+
+    # for input_file, output_file in zip(input_files, output_files):
+    #     from_file_to_file(input_file, output_file)
+
+
+###############################################################################
+# Entry point
+###############################################################################
+
+
+def expand_files(files):
+    """Expands a wildcard to a list of paths for Windows compatibility"""
+    # Split at whitespace
+    files = files.split()
+
+    # Handle wildcard expansion
+    if len(files) == 1 and '*' in files[0]:
+        files = glob.glob(files[0])
+
+    # Convert to Path objects
+    return files
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(description='Convert images to JPEG')
+
+    # Handle wildcards across platforms
+    if os.name == 'nt':
+        parser.add_argument(
+            '--input_files',
+            type=expand_files,
+            help='The image files to convert to jpeg')
+    else:
+        parser.add_argument(
+            '--input_files',
+            nargs='+',
+            help='The image files to convert to jpeg')
+
+    parser.add_argument(
+        '--output_files',
+        type=Path,
+        nargs='+',
+        help='The corresponding output files. ' +
+             'Uses same filename with jpg extension by default')
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    from_files_to_files(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/core.py` & `reseval-0.1.0/reseval/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,81 @@
-import contextlib
-import os
-import typing
-from pathlib import Path
-
-import reseval
-
-
-###############################################################################
-# Run subjective evaluation pipeline
-###############################################################################
-
-
-def run(
-    config: str,
-    directory: typing.Union[str, bytes, os.PathLike],
-    results_directory: typing.Union[str, bytes, os.PathLike] = Path(),
-    local: bool = False,
-    production: bool = False,
-    interval: int = 120) -> dict:
-    """Perform subjective evaluation
-
-    Args:
-        config: The configuration file
-        directory: The directory containing the files to evaluate
-        local: Run subjective evaluation locally
-        production: Deploy the subjective evaluation to crowdsource
-            participants
-        interval: The time between monitoring updates in seconds
-
-    Returns:
-        dict: Evaluation results
-    """
-    # Setup evaluation
-    name = reseval.create(config, directory, local, production, detach=True)
-
-    try:
-
-        # Monitor evaluation until completion
-        reseval.monitor([name], interval, exit_on_finish=True)
-
-    except (Exception, KeyboardInterrupt) as exception:
-
-        # Perform clean-up only if evaluation is local
-        if not local:
-            raise exception
-
-    # Pay participants
-    reseval.pay(name)
-
-    # Get results
-    results = reseval.results(name, results_directory)
-
-    # Cleanup database, server, storage, and crowdsource task
-    reseval.destroy(name, force=True)
-
-    return results
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-@contextlib.contextmanager
-def chdir(directory):
-    """Change working directory"""
-    curr_dir = os.getcwd()
-    try:
-        os.chdir(directory)
-        yield
-    finally:
-        os.chdir(curr_dir)
-
-
-def is_local(name):
-    """Returns true if the evaluation is hosted locally"""
-    return (reseval.EVALUATION_DIRECTORY / name / '.local').exists()
+import contextlib
+import os
+import typing
+from pathlib import Path
+
+import reseval
+
+
+###############################################################################
+# Run subjective evaluation pipeline
+###############################################################################
+
+
+def run(
+    config: str,
+    directory: typing.Union[str, bytes, os.PathLike],
+    results_directory: typing.Union[str, bytes, os.PathLike] = Path(),
+    local: bool = False,
+    production: bool = False,
+    interval: int = 120) -> dict:
+    """Perform subjective evaluation
+
+    Args:
+        config: The configuration file
+        directory: The directory containing the files to evaluate
+        results_directory: The directory to save results
+        local: Run subjective evaluation locally
+        production: Deploy the subjective evaluation to crowdsource
+            participants
+        interval: The time between monitoring updates in seconds
+
+    Returns:
+        dict: Evaluation results
+    """
+    # Setup evaluation
+    name = reseval.create(config, directory, local, production, detach=True)
+
+    try:
+
+        # Monitor evaluation until completion
+        reseval.monitor([name], interval, exit_on_finish=True)
+
+    except (Exception, KeyboardInterrupt) as exception:
+
+        # Perform clean-up only if evaluation is local
+        if local:
+            print(exception)
+        else:
+            raise exception
+
+    # Pay participants
+    reseval.pay(name)
+
+    # Get results
+    results = reseval.results(name, results_directory)
+
+    # Cleanup database, server, storage, and crowdsource task
+    reseval.destroy(name, force=True)
+
+    return results
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+@contextlib.contextmanager
+def chdir(directory):
+    """Change working directory"""
+    curr_dir = os.getcwd()
+    try:
+        os.chdir(directory)
+        yield
+    finally:
+        os.chdir(curr_dir)
+
+
+def is_local(name):
+    """Returns true if the evaluation is hosted locally"""
+    return (reseval.EVALUATION_DIRECTORY / name / '.local').exists()
```

### Comparing `reseval-0.0.3/reseval/credentials/__main__.py` & `reseval-0.1.0/reseval/credentials/__main__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import argparse
-
-import reseval
-
-
-###############################################################################
-# Entry point for adding or updating credentials
-###############################################################################
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(
-        description='Stop a subjective evaluation without ' +
-                    'destroying resources')
-    parser.add_argument('--aws_api_key', help='The public API key for AWS')
-    parser.add_argument(
-        '--aws_api_secret_key',
-        help='The private API key for AWS')
-    parser.add_argument('--heroku_api_key', help='The API key for Heroku')
-    parser.add_argument(
-        '--mysql_local_user',
-        help='The username of the local MySQL database',
-        default='root')
-    parser.add_argument(
-        '--mysql_local_password',
-        help='The corresponding password of the local MySQL database')
-    return parser.parse_args()
-
-
-reseval.credentials(**vars(parse_args()))
+import argparse
+
+import reseval
+
+
+###############################################################################
+# Entry point for adding or updating credentials
+###############################################################################
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(
+        description='Stop a subjective evaluation without ' +
+                    'destroying resources')
+    parser.add_argument('--aws_api_key', help='The public API key for AWS')
+    parser.add_argument(
+        '--aws_api_secret_key',
+        help='The private API key for AWS')
+    parser.add_argument('--heroku_api_key', help='The API key for Heroku')
+    parser.add_argument(
+        '--mysql_local_user',
+        help='The username of the local MySQL database',
+        default='root')
+    parser.add_argument(
+        '--mysql_local_password',
+        help='The corresponding password of the local MySQL database')
+    return parser.parse_args()
+
+
+reseval.credentials(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/crowdsource/core.py` & `reseval-0.1.0/reseval/crowdsource/core.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import json
-
-import reseval
-
-
-###############################################################################
-# Crowdsourcing interface
-###############################################################################
-
-
-def active(name):
-    """Returns True if the evaluation is still running"""
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    # Local dev is active until we have enough participants and responses
-    if reseval.is_local(name):
-        try:
-            reseval.database.download(
-                name,
-                reseval.EVALUATION_DIRECTORY / name / 'tables',
-                ['responses'])
-            responses = reseval.load.responses(name)
-            participants = len(set(
-                response['Participant'] for response in responses))
-            samples = \
-                config['participants'] * config['samples_per_participant']
-            return (
-                len(responses) < samples or
-                participants < config['participants'])
-        except FileNotFoundError:
-            return True
-
-    # Get credentials
-    try:
-        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-    except FileNotFoundError:
-        return False
-
-    # Check if the evaluation is active
-    return module(config).active(config, credentials)
-
-
-def assignments(name):
-    """Get the assignment results"""
-    # Skip if performing local development
-    if reseval.is_local(name):
-        return []
-
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    # Get credentials
-    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    # Extend task
-    return module(config).assignments(credentials)
-
-
-def create(config, url, local=False, production=False):
-    """Create a subjective evaluation"""
-    # Skip if performing local development
-    if local:
-        return
-
-    # Skip if evaluation exists
-    if exists(config['name']):
-        raise ValueError('Not overwriting existing evaluation')
-
-    print('Creating crowdsource task...')
-
-    # Create crowdsource task
-    credentials = module(config).create(config, url, production)
-
-    # Save crowdsource credentials
-    file = (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        'crowdsource.json')
-    file.parent.mkdir(exist_ok=True, parents=True)
-    with open(file, 'w') as file:
-        json.dump(credentials, file, indent=4, sort_keys=True)
-
-
-def destroy(name):
-    """Delete a subjective evaluation"""
-    try:
-
-        # Skip if performing local development
-        if reseval.is_local(name):
-            return
-
-        # Get config
-        config = reseval.load.config_by_name(name)
-
-        # Get credentials
-        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-        # Destroy crowdsource task
-        module(config).destroy(config, credentials)
-
-    except FileNotFoundError:
-
-        pass
-
-    # Clean-up credentials
-    (
-        reseval.EVALUATION_DIRECTORY /
-        name /
-        'credentials' /
-        'crowdsource.json'
-    ).unlink(missing_ok=True)
-
-
-def extend(name, participants):
-    """Extend a subjectve evaluation"""
-    # Skip if performing local development
-    if reseval.is_local(name):
-        return
-
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    # Get credentials
-    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    # Extend task
-    module(config).extend(credentials, participants, name)
-
-
-def exists(name):
-    """Returns true if the evaluation exists"""
-    if reseval.is_local(name):
-        return False
-
-    try:
-
-        # Get config
-        config = reseval.load.config_by_name(name)
-
-        # Get credentials
-        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    except FileNotFoundError:
-
-        return False
-
-    # Check if evaluation exists
-    return module(config).exists(config, credentials)
-
-
-def paid(name):
-    """Check if all participants have been paid"""
-    # Skip if performing local development
-    if reseval.is_local(name):
-        return True
-
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    try:
-
-        # Get credentials
-        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    except FileNotFoundError:
-
-        # We assume that the evaluation was never started or already finished
-        # if we do not have the credentials
-        return True
-
-    # Check if participants have been paid
-    return module(config).paid(credentials)
-
-
-def pay(name):
-    """Pay participants"""
-    # Skip if performing local development
-    if reseval.is_local(name):
-        return
-
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    # Get credentials
-    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    # Pay participants
-    module(config).pay(config, credentials)
-
-
-def progress(name):
-    """Retrieve the number of participants who have taken the evaluation"""
-    # Skip if performing local development
-    if reseval.is_local(name):
-        return
-
-    # Get config
-    config = reseval.load.config_by_name(name)
-
-    # Get credentials
-    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
-
-    # Check current progress
-    return module(config).progress(credentials)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def module(config):
-    """Get the crowdsourcing module to use"""
-    platform = config['crowdsource']['platform']
-    if platform == 'mturk':
-        return reseval.crowdsource.mturk
-    raise ValueError(f'Crowdsource platform {platform} not recognized')
+import json
+
+import reseval
+
+
+###############################################################################
+# Crowdsourcing interface
+###############################################################################
+
+
+def active(name):
+    """Returns True if the evaluation is still running"""
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    # Local dev is active until we have enough participants and responses
+    if reseval.is_local(name):
+        try:
+            reseval.database.download(
+                name,
+                reseval.EVALUATION_DIRECTORY / name / 'tables',
+                ['responses'])
+            responses = reseval.load.responses(name)
+            participants = len(set(
+                response['Participant'] for response in responses))
+            samples = \
+                config['participants'] * config['samples_per_participant']
+            return (
+                len(responses) < samples or
+                participants < config['participants'])
+        except FileNotFoundError:
+            return True
+
+    # Get credentials
+    try:
+        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+    except FileNotFoundError:
+        return False
+
+    # Check if the evaluation is active
+    return module(config).active(config, credentials)
+
+
+def assignments(name):
+    """Get the assignment results"""
+    # Skip if performing local development
+    if reseval.is_local(name):
+        return []
+
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    # Get credentials
+    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    # Extend task
+    return module(config).assignments(credentials)
+
+
+def create(config, url, local=False, production=False):
+    """Create a subjective evaluation"""
+    # Skip if performing local development
+    if local:
+        return
+
+    # Skip if evaluation exists
+    if exists(config['name']):
+        raise ValueError('Not overwriting existing evaluation')
+
+    print('Creating crowdsource task...')
+
+    # Create crowdsource task
+    credentials = module(config).create(config, url, production)
+
+    # Save crowdsource credentials
+    file = (
+        reseval.EVALUATION_DIRECTORY /
+        config['name'] /
+        'credentials' /
+        'crowdsource.json')
+    file.parent.mkdir(exist_ok=True, parents=True)
+    with open(file, 'w') as file:
+        json.dump(credentials, file, indent=4, sort_keys=True)
+
+
+def destroy(name):
+    """Delete a subjective evaluation"""
+    try:
+
+        # Skip if performing local development
+        if reseval.is_local(name):
+            return
+
+        # Get config
+        config = reseval.load.config_by_name(name)
+
+        # Get credentials
+        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+        # Destroy crowdsource task
+        module(config).destroy(config, credentials)
+
+    except FileNotFoundError:
+
+        pass
+
+    # Clean-up credentials
+    (
+        reseval.EVALUATION_DIRECTORY /
+        name /
+        'credentials' /
+        'crowdsource.json'
+    ).unlink(missing_ok=True)
+
+
+def extend(name, participants):
+    """Extend a subjectve evaluation"""
+    # Skip if performing local development
+    if reseval.is_local(name):
+        return
+
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    # Get credentials
+    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    # Extend task
+    module(config).extend(credentials, participants, name)
+
+
+def exists(name):
+    """Returns true if the evaluation exists"""
+    if reseval.is_local(name):
+        return False
+
+    try:
+
+        # Get config
+        config = reseval.load.config_by_name(name)
+
+        # Get credentials
+        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    except FileNotFoundError:
+
+        return False
+
+    # Check if evaluation exists
+    return module(config).exists(config, credentials)
+
+
+def paid(name):
+    """Check if all participants have been paid"""
+    # Skip if performing local development
+    if reseval.is_local(name):
+        return True
+
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    try:
+
+        # Get credentials
+        credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    except FileNotFoundError:
+
+        # We assume that the evaluation was never started or already finished
+        # if we do not have the credentials
+        return True
+
+    # Check if participants have been paid
+    return module(config).paid(credentials)
+
+
+def pay(name):
+    """Pay participants"""
+    # Skip if performing local development
+    if reseval.is_local(name):
+        return
+
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    # Get credentials
+    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    # Pay participants
+    module(config).pay(config, credentials)
+
+
+def progress(name):
+    """Retrieve the number of participants who have taken the evaluation"""
+    # Skip if performing local development
+    if reseval.is_local(name):
+        return
+
+    # Get config
+    config = reseval.load.config_by_name(name)
+
+    # Get credentials
+    credentials = reseval.load.credentials_by_name(name, 'crowdsource')
+
+    # Check current progress
+    return module(config).progress(credentials)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def module(config):
+    """Get the crowdsourcing module to use"""
+    platform = config['crowdsource']['platform']
+    if platform == 'mturk':
+        return reseval.crowdsource.mturk
+    raise ValueError(f'Crowdsource platform {platform} not recognized')
```

### Comparing `reseval-0.0.3/reseval/crowdsource/mturk.py` & `reseval-0.1.0/reseval/crowdsource/mturk.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,392 +1,392 @@
-import datetime
-import itertools
-import json
-import os
-import re
-from hashlib import md5
-from pathlib import Path
-import time
-
-import boto3
-import xmltodict as xmltodict
-import uuid
-
-import reseval
-
-
-###############################################################################
-# Constants
-###############################################################################
-
-
-# HIT preview URL
-PREVIEW_URL = {
-    'development': 'https://workersandbox.mturk.com/mturk/preview?groupId={}',
-    'production': 'https://worker.mturk.com/mturk/preview?groupId={}'}
-
-# HIT creation URL
-URL = {
-    'development': 'https://mturk-requester-sandbox.us-east-1.amazonaws.com',
-    'production': 'https://mturk-requester.us-east-1.amazonaws.com'}
-
-# Survey XML
-XML_FILE = reseval.ASSETS_DIR / 'survey.xml'
-
-
-###############################################################################
-# Amazon Mechanical Turk crowdsourcing interface
-###############################################################################
-
-
-def active(config, credentials):
-    """Returns True if the evaluation is still running"""
-    return status(config, credentials) not in ['Reviewing', 'Reviewable']
-
-
-def create(config, url, production=False):
-    """Create a HIT"""
-    # Connect to MTurk
-    mturk = connect(production)
-
-    # Get survey XML and link to our external survey
-    with open(reseval.ASSETS_DIR / 'survey.xml') as file:
-        question = file.read().format(url)
-
-    # Create HIT
-    cfg = config['crowdsource']
-    hit = mturk.create_hit(
-        Title=cfg['title'],
-        Description=cfg['description'],
-        Keywords=cfg['keywords'],
-        Reward=str(cfg['payment']['base']),
-        MaxAssignments=config['participants'],
-        LifetimeInSeconds=cfg['duration']['total'],
-        AssignmentDurationInSeconds=cfg['duration']['assignment'],
-        AutoApprovalDelayInSeconds=cfg['duration']['autoapprove'],
-        QualificationRequirements=qualifications(config),
-        Question=question)
-
-    # Log HIT
-    hit_id = hit['HIT']['HITId']
-    url_key = 'production' if production else 'development'
-    preview_url = PREVIEW_URL[url_key].format(hit['HIT']['HITGroupId'])
-    print(f'Created HIT {hit_id}. You can view your HIT at {preview_url}')
-
-    # Return crowdsource credentials
-    return {'HIT_ID': hit_id, 'PRODUCTION': production}
-
-
-def destroy(config, credentials):
-    """Delete a HIT"""
-    if credentials['HIT_ID'] in list_hits(credentials):
-        # Connect to MTurk
-        mturk = connect(credentials['PRODUCTION'])
-
-        # Stop HIT
-        mturk.update_expiration_for_hit(
-            HITId=credentials['HIT_ID'],
-            ExpireAt=datetime.datetime(2000, 1, 1).timestamp())
-
-        # The HIT can only be deleted once the status is one of 'Reviewing' or
-        # 'Reviewable'. Otherwise, an error will be thrown. Sometimes, it takes
-        # a couple of seconds after the update call above for the status to
-        # change to 'Reviewable'. This loop is a time buffer that gives MTurk
-        # 90 seconds to update the status. If the status doesn't change, the
-        # most likely explanation is that someone is still taking the
-        # evaluation.
-        start = datetime.datetime.now()
-        while (datetime.datetime.now() - start).total_seconds() < 90:
-            if not active(config, credentials):
-                break
-            time.sleep(5)
-
-        # Delete HIT
-        mturk.delete_hit(HITId=credentials['HIT_ID'])
-
-
-def extend(credentials, participants, name):
-    """Extend a HIT with additional assignments"""
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Location to save unique response token
-    token_file = Path(reseval.EVALUATION_DIRECTORY / name / 'tokens.json')
-
-    try:
-
-        # Last response was bad. Retry using same token.
-        with open(token_file) as json_file:
-            unique_token = json.load(json_file)['extend_token']
-
-    except FileNotFoundError:
-
-        # Create and save a new unique token
-        unique_token = str(uuid.uuid4())
-        data = {'extend_token': unique_token}
-        with open(token_file, 'w') as json_file:
-            json.dump(data, json_file)
-
-    try:
-
-        # Extend HIT
-        mturk.create_additional_assignments_for_hit(
-            HITId=credentials['HIT_ID'],
-            UniqueRequestToken=unique_token,
-            NumberOfAdditionalAssignments=participants)
-
-    except Exception as exception:
-
-        # If the token is in the exception args, we assume the token has been
-        # used and delete the token
-        if re.search(re.escape(unique_token), exception.args[0]) is not None:
-            token_file.unlink(True)
-
-        else:
-            raise exception
-
-
-def exists(config, credentials):
-    """Returns true if the evaluation exists"""
-    return credentials['HIT_ID'] in list_hits(credentials)
-
-
-def paid(credentials):
-    """Returns True if all participants have been paid"""
-    return not assignments(credentials, ['Submitted'])
-
-
-def pay(config, credentials):
-    """Evaluate and pay participants"""
-    # Get assignment IDs and completion codes
-    mturk_results = results(credentials)
-
-    # Get participants and responses from database
-    reseval.database.download(
-        config['name'],
-        reseval.EVALUATION_DIRECTORY / config['name'] / 'tables',
-        ['participants', 'responses'])
-    participants = reseval.load.participants(config['name'])
-    responses = reseval.load.responses(config['name'])
-
-    # Match participants with responses
-    participant_responses = {}
-    for participant in participants:
-        pid = participant['ID']
-        participant_responses[pid] = (
-                participant |
-                {'responses': list(filter(
-                    lambda x: x['Participant'] == pid,
-                    responses))})
-
-    # Iterate over participants
-    for result in mturk_results:
-
-        # Find matching completion code
-        match = None
-        for pid in participant_responses:
-            if (participant_responses[pid]['CompletionCode'] ==
-                    result['completion_code']):
-                match = pid
-
-        # Only process payment if the participant has not already been paid
-        if result['status'] == 'Submitted':
-
-            # Reject work if the completion codes do not match
-            if match is None and result['status'] == 'Submitted':
-                reject(
-                    credentials,
-                    result['assignment_id'],
-                    'Survey completion code does not match')
-                continue
-
-            # Approve work
-            approve(credentials, result['assignment_id'])
-
-            # If they passed prescreening and completed evaluation, give
-            # the participant a bonus
-            if (len(participant_responses[pid]['responses']) ==
-                    config['samples_per_participant']):
-                bonus(config, credentials, result['assignment_id'])
-
-
-def progress(credentials):
-    """Retrieve the number of participants that have taken the evaluation"""
-    return len(assignments(credentials))
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def approve(credentials, assignment_id):
-    """Approve an assignment"""
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Skip if already processed
-    assignment = mturk.get_assignment(AssignmentId=assignment_id)
-    if assignment['Assignment']['AssignmentStatus'] == 'Submitted':
-        # Approve assignment
-        mturk.approve_assignment(AssignmentId=assignment_id)
-
-
-def assignments(credentials, statuses=None):
-    """Retrieve a list of all assignments for a HIT"""
-    # Default to all statuses
-    statuses = (
-        ['Submitted', 'Approved', 'Rejected']
-        if statuses is None else statuses)
-
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Download results
-    paginator = mturk.get_paginator('list_assignments_for_hit')
-    iterator = paginator.paginate(
-        HITId=credentials['HIT_ID'],
-        AssignmentStatuses=statuses)
-
-    # Get assignments
-    return list(itertools.chain.from_iterable(
-        page['Assignments'] for page in iterator))
-
-
-def bonus(config, credentials, assignment_id):
-    """Give a participant a bonus"""
-    # We only send one bonus per assignment, so we use the assignment ID to
-    # generate the unique token
-    unique_token = md5(assignment_id.encode('utf-8')).hexdigest()
-
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Get worker ID
-    assignment = mturk.get_assignment(AssignmentId=assignment_id)
-    worker_id = assignment['Assignment']['WorkerId']
-
-    try:
-
-        # Approve assignment
-        mturk.send_bonus(
-            WorkerId=worker_id,
-            BonusAmount=str(config['crowdsource']['payment']['completion']),
-            AssignmentId=assignment_id,
-            UniqueRequestToken=unique_token,
-            Reason='Passed prescreening and completed evaluation. Thank you!')
-
-    except Exception as exception:
-
-        # If the token is in the exception args, we assume the worker has
-        # already been given a bonus
-        if re.search(re.escape(unique_token), exception.args[0]) is None:
-            raise exception
-
-
-def connect(production=False):
-    """Connect to MTurk"""
-    # Load API keys
-    reseval.load.api_keys()
-
-    # Connect to MTurk
-    return boto3.Session(
-        aws_access_key_id=os.environ['AWSAccessKeyId'],
-        aws_secret_access_key=os.environ['AWSSecretKey']
-    ).client(
-        'mturk',
-        region_name='us-east-1',
-        endpoint_url=URL['production' if production else 'development'])
-
-
-def list_hits(credentials):
-    """List the IDs of all HITs on MTurk"""
-    # Connect to S3
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Get list of HITs
-    iterator = mturk.get_paginator('list_hits').paginate()
-    responses = list(iterator)
-
-    # Extract HIT Ids
-    if responses:
-        return list(itertools.chain.from_iterable([
-            [hit['HITId'] for hit in response['HITs']]
-            for response in responses]))
-
-    return []
-
-
-def qualifications(config):
-    """Format participant qualificiations"""
-    qualifications = []
-
-    # Country of origin
-    cfg = config['crowdsource']['filter']
-    if 'countries' in cfg:
-        locales = [{'Country': country} for country in cfg['countries']]
-        qualifications.append({
-            'QualificationTypeId': '00000000000000000071',
-            'Comparator': 'In',
-            'LocaleValues': locales,
-            'RequiredToPreview': True})
-
-    # Number of approved tasks
-    if 'approved_tasks' in cfg and cfg['approved_tasks'] > 0:
-        qualifications.append({
-            'QualificationTypeId': '00000000000000000040',
-            'Comparator': 'GreaterThan',
-            'IntegerValues': [cfg['approved_tasks']],
-            'RequiredToPreview': True})
-
-    # Approval rating
-    if 'approval_rating' in cfg and cfg['approval_rating'] > 0:
-        qualifications.append({
-            'QualificationTypeId': '000000000000000000L0',
-            'Comparator': 'GreaterThanOrEqualTo',
-            'IntegerValues': [cfg['approval_rating']],
-            'RequiredToPreview': True})
-
-    return qualifications
-
-
-def reject(credentials, assignment_id, reason):
-    """Reject assignment by ID"""
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Skip if already processed
-    assignment = mturk.get_assignment(AssignmentId=assignment_id)
-    if assignment['Assignment']['AssignmentStatus'] == 'Submitted':
-        # Reject assignment
-        mturk.reject_assignment(
-            AssignmentId=assignment_id,
-            RequesterFeedback=reason)
-
-
-def results(credentials):
-    """Get a list of all assignment IDs and completion codes"""
-    result = []
-    for assignment in assignments(credentials):
-        # Parse XML
-        xml_doc = xmltodict.parse(assignment['Answer'])
-
-        # Get completion code
-        completion_code = xml_doc['QuestionFormAnswers']['Answer']['FreeText']
-
-        # Format result
-        result.append({
-            'assignment_id': assignment['AssignmentId'],
-            'completion_code': completion_code,
-            'status': assignment['AssignmentStatus'],
-            'worker_id': assignment['WorkerId']})
-
-    return result
-
-
-def status(config, credentials):
-    """Get the status of the current HIT"""
-    # Connect to MTurk
-    mturk = connect(credentials['PRODUCTION'])
-
-    # Get HIT status
-    return mturk.get_hit(HITId=credentials['HIT_ID'])['HIT']['HITStatus']
+import datetime
+import itertools
+import json
+import os
+import re
+from hashlib import md5
+from pathlib import Path
+import time
+
+import boto3
+import xmltodict as xmltodict
+import uuid
+
+import reseval
+
+
+###############################################################################
+# Constants
+###############################################################################
+
+
+# HIT preview URL
+PREVIEW_URL = {
+    'development': 'https://workersandbox.mturk.com/mturk/preview?groupId={}',
+    'production': 'https://worker.mturk.com/mturk/preview?groupId={}'}
+
+# HIT creation URL
+URL = {
+    'development': 'https://mturk-requester-sandbox.us-east-1.amazonaws.com',
+    'production': 'https://mturk-requester.us-east-1.amazonaws.com'}
+
+# Survey XML
+XML_FILE = reseval.ASSETS_DIR / 'survey.xml'
+
+
+###############################################################################
+# Amazon Mechanical Turk crowdsourcing interface
+###############################################################################
+
+
+def active(config, credentials):
+    """Returns True if the evaluation is still running"""
+    return status(config, credentials) not in ['Reviewing', 'Reviewable']
+
+
+def create(config, url, production=False):
+    """Create a HIT"""
+    # Connect to MTurk
+    mturk = connect(production)
+
+    # Get survey XML and link to our external survey
+    with open(reseval.ASSETS_DIR / 'survey.xml') as file:
+        question = file.read().format(url)
+
+    # Create HIT
+    cfg = config['crowdsource']
+    hit = mturk.create_hit(
+        Title=cfg['title'],
+        Description=cfg['description'],
+        Keywords=cfg['keywords'],
+        Reward=str(cfg['payment']['base']),
+        MaxAssignments=config['participants'],
+        LifetimeInSeconds=cfg['duration']['total'],
+        AssignmentDurationInSeconds=cfg['duration']['assignment'],
+        AutoApprovalDelayInSeconds=cfg['duration']['autoapprove'],
+        QualificationRequirements=qualifications(config),
+        Question=question)
+
+    # Log HIT
+    hit_id = hit['HIT']['HITId']
+    url_key = 'production' if production else 'development'
+    preview_url = PREVIEW_URL[url_key].format(hit['HIT']['HITGroupId'])
+    print(f'Created HIT {hit_id}. You can view your HIT at {preview_url}')
+
+    # Return crowdsource credentials
+    return {'HIT_ID': hit_id, 'PRODUCTION': production}
+
+
+def destroy(config, credentials):
+    """Delete a HIT"""
+    if credentials['HIT_ID'] in list_hits(credentials):
+        # Connect to MTurk
+        mturk = connect(credentials['PRODUCTION'])
+
+        # Stop HIT
+        mturk.update_expiration_for_hit(
+            HITId=credentials['HIT_ID'],
+            ExpireAt=datetime.datetime(2000, 1, 1).timestamp())
+
+        # The HIT can only be deleted once the status is one of 'Reviewing' or
+        # 'Reviewable'. Otherwise, an error will be thrown. Sometimes, it takes
+        # a couple of seconds after the update call above for the status to
+        # change to 'Reviewable'. This loop is a time buffer that gives MTurk
+        # 90 seconds to update the status. If the status doesn't change, the
+        # most likely explanation is that someone is still taking the
+        # evaluation.
+        start = datetime.datetime.now()
+        while (datetime.datetime.now() - start).total_seconds() < 90:
+            if not active(config, credentials):
+                break
+            time.sleep(5)
+
+        # Delete HIT
+        mturk.delete_hit(HITId=credentials['HIT_ID'])
+
+
+def extend(credentials, participants, name):
+    """Extend a HIT with additional assignments"""
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Location to save unique response token
+    token_file = Path(reseval.EVALUATION_DIRECTORY / name / 'tokens.json')
+
+    try:
+
+        # Last response was bad. Retry using same token.
+        with open(token_file) as json_file:
+            unique_token = json.load(json_file)['extend_token']
+
+    except FileNotFoundError:
+
+        # Create and save a new unique token
+        unique_token = str(uuid.uuid4())
+        data = {'extend_token': unique_token}
+        with open(token_file, 'w') as json_file:
+            json.dump(data, json_file)
+
+    try:
+
+        # Extend HIT
+        mturk.create_additional_assignments_for_hit(
+            HITId=credentials['HIT_ID'],
+            UniqueRequestToken=unique_token,
+            NumberOfAdditionalAssignments=participants)
+
+    except Exception as exception:
+
+        # If the token is in the exception args, we assume the token has been
+        # used and delete the token
+        if re.search(re.escape(unique_token), exception.args[0]) is not None:
+            token_file.unlink(True)
+
+        else:
+            raise exception
+
+
+def exists(config, credentials):
+    """Returns true if the evaluation exists"""
+    return credentials['HIT_ID'] in list_hits(credentials)
+
+
+def paid(credentials):
+    """Returns True if all participants have been paid"""
+    return not assignments(credentials, ['Submitted'])
+
+
+def pay(config, credentials):
+    """Evaluate and pay participants"""
+    # Get assignment IDs and completion codes
+    mturk_results = results(credentials)
+
+    # Get participants and responses from database
+    reseval.database.download(
+        config['name'],
+        reseval.EVALUATION_DIRECTORY / config['name'] / 'tables',
+        ['participants', 'responses'])
+    participants = reseval.load.participants(config['name'])
+    responses = reseval.load.responses(config['name'])
+
+    # Match participants with responses
+    participant_responses = {}
+    for participant in participants:
+        pid = participant['ID']
+        participant_responses[pid] = (
+                participant |
+                {'responses': list(filter(
+                    lambda x: x['Participant'] == pid,
+                    responses))})
+
+    # Iterate over participants
+    for result in mturk_results:
+
+        # Find matching completion code
+        match = None
+        for pid in participant_responses:
+            if (participant_responses[pid]['CompletionCode'] ==
+                    result['completion_code']):
+                match = pid
+
+        # Only process payment if the participant has not already been paid
+        if result['status'] == 'Submitted':
+
+            # Reject work if the completion codes do not match
+            if match is None and result['status'] == 'Submitted':
+                reject(
+                    credentials,
+                    result['assignment_id'],
+                    'Survey completion code does not match')
+                continue
+
+            # Approve work
+            approve(credentials, result['assignment_id'])
+
+            # If they passed prescreening and completed evaluation, give
+            # the participant a bonus
+            if (len(participant_responses[pid]['responses']) ==
+                    config['samples_per_participant']):
+                bonus(config, credentials, result['assignment_id'])
+
+
+def progress(credentials):
+    """Retrieve the number of participants that have taken the evaluation"""
+    return len(assignments(credentials))
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def approve(credentials, assignment_id):
+    """Approve an assignment"""
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Skip if already processed
+    assignment = mturk.get_assignment(AssignmentId=assignment_id)
+    if assignment['Assignment']['AssignmentStatus'] == 'Submitted':
+        # Approve assignment
+        mturk.approve_assignment(AssignmentId=assignment_id)
+
+
+def assignments(credentials, statuses=None):
+    """Retrieve a list of all assignments for a HIT"""
+    # Default to all statuses
+    statuses = (
+        ['Submitted', 'Approved', 'Rejected']
+        if statuses is None else statuses)
+
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Download results
+    paginator = mturk.get_paginator('list_assignments_for_hit')
+    iterator = paginator.paginate(
+        HITId=credentials['HIT_ID'],
+        AssignmentStatuses=statuses)
+
+    # Get assignments
+    return list(itertools.chain.from_iterable(
+        page['Assignments'] for page in iterator))
+
+
+def bonus(config, credentials, assignment_id):
+    """Give a participant a bonus"""
+    # We only send one bonus per assignment, so we use the assignment ID to
+    # generate the unique token
+    unique_token = md5(assignment_id.encode('utf-8')).hexdigest()
+
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Get worker ID
+    assignment = mturk.get_assignment(AssignmentId=assignment_id)
+    worker_id = assignment['Assignment']['WorkerId']
+
+    try:
+
+        # Approve assignment
+        mturk.send_bonus(
+            WorkerId=worker_id,
+            BonusAmount=str(config['crowdsource']['payment']['completion']),
+            AssignmentId=assignment_id,
+            UniqueRequestToken=unique_token,
+            Reason='Passed prescreening and completed evaluation. Thank you!')
+
+    except Exception as exception:
+
+        # If the token is in the exception args, we assume the worker has
+        # already been given a bonus
+        if re.search(re.escape(unique_token), exception.args[0]) is None:
+            raise exception
+
+
+def connect(production=False):
+    """Connect to MTurk"""
+    # Load API keys
+    reseval.load.api_keys()
+
+    # Connect to MTurk
+    return boto3.Session(
+        aws_access_key_id=os.environ['AWSAccessKeyId'],
+        aws_secret_access_key=os.environ['AWSSecretKey']
+    ).client(
+        'mturk',
+        region_name='us-east-1',
+        endpoint_url=URL['production' if production else 'development'])
+
+
+def list_hits(credentials):
+    """List the IDs of all HITs on MTurk"""
+    # Connect to S3
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Get list of HITs
+    iterator = mturk.get_paginator('list_hits').paginate()
+    responses = list(iterator)
+
+    # Extract HIT Ids
+    if responses:
+        return list(itertools.chain.from_iterable([
+            [hit['HITId'] for hit in response['HITs']]
+            for response in responses]))
+
+    return []
+
+
+def qualifications(config):
+    """Format participant qualificiations"""
+    qualifications = []
+
+    # Country of origin
+    cfg = config['crowdsource']['filter']
+    if 'countries' in cfg:
+        locales = [{'Country': country} for country in cfg['countries']]
+        qualifications.append({
+            'QualificationTypeId': '00000000000000000071',
+            'Comparator': 'In',
+            'LocaleValues': locales,
+            'RequiredToPreview': True})
+
+    # Number of approved tasks
+    if 'approved_tasks' in cfg and cfg['approved_tasks'] > 0:
+        qualifications.append({
+            'QualificationTypeId': '00000000000000000040',
+            'Comparator': 'GreaterThan',
+            'IntegerValues': [cfg['approved_tasks']],
+            'RequiredToPreview': True})
+
+    # Approval rating
+    if 'approval_rating' in cfg and cfg['approval_rating'] > 0:
+        qualifications.append({
+            'QualificationTypeId': '000000000000000000L0',
+            'Comparator': 'GreaterThanOrEqualTo',
+            'IntegerValues': [cfg['approval_rating']],
+            'RequiredToPreview': True})
+
+    return qualifications
+
+
+def reject(credentials, assignment_id, reason):
+    """Reject assignment by ID"""
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Skip if already processed
+    assignment = mturk.get_assignment(AssignmentId=assignment_id)
+    if assignment['Assignment']['AssignmentStatus'] == 'Submitted':
+        # Reject assignment
+        mturk.reject_assignment(
+            AssignmentId=assignment_id,
+            RequesterFeedback=reason)
+
+
+def results(credentials):
+    """Get a list of all assignment IDs and completion codes"""
+    result = []
+    for assignment in assignments(credentials):
+        # Parse XML
+        xml_doc = xmltodict.parse(assignment['Answer'])
+
+        # Get completion code
+        completion_code = xml_doc['QuestionFormAnswers']['Answer']['FreeText']
+
+        # Format result
+        result.append({
+            'assignment_id': assignment['AssignmentId'],
+            'completion_code': completion_code,
+            'status': assignment['AssignmentStatus'],
+            'worker_id': assignment['WorkerId']})
+
+    return result
+
+
+def status(config, credentials):
+    """Get the status of the current HIT"""
+    # Connect to MTurk
+    mturk = connect(credentials['PRODUCTION'])
+
+    # Get HIT status
+    return mturk.get_hit(HITId=credentials['HIT_ID'])['HIT']['HITStatus']
```

### Comparing `reseval-0.0.3/reseval/database/core.py` & `reseval-0.1.0/reseval/database/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,311 +1,315 @@
-import contextlib
-import csv
-import os
-
-import mysql.connector
-
-import reseval
-
-
-###############################################################################
-# Constants
-###############################################################################
-
-
-# MySQL database schema
-SCHEMA = [
-    # Evaluation conditions. For example, for an AB test, these are the
-    # names of the conditions corresponding to the "A" and "B" choices.
-    #
-    # Condition - The name of the condition
-    'CREATE TABLE `conditions` ('
-    '  `Condition` varchar(255) UNIQUE,'
-    '  PRIMARY KEY (`Condition`)'
-    ')',
-
-    # Tables of files to be evaluated, split into stem and extension.
-    # Exact file paths depend on the test being performed. See README for
-    # details.
-    #
-    # Stem - The file stem
-    # Extension - The file extension
-    # Uses - The number of times this stem has been selected for evaluation
-    'CREATE TABLE `files` ('
-    '  `Stem` varchar(255) UNIQUE,'
-    '  `Extension` varchar(16) NOT NULL,'
-    '  `Uses` int DEFAULT 0,'
-    '  PRIMARY KEY (`Stem`)'
-    ')',
-
-    # Participant information
-    # This assumes each participant only takes the survey once.
-    # Prescreening questions from the configuration file are included
-    # as well. These questions are formatted as
-    # f' `{name}` varchar({length}) NOT NULL,', where "name" is the
-    # name given to the question in the configuration file, and "length"
-    # is automatically computed from the longest allowed answer.
-    #
-    # ID - The participant ID
-    # CompletionCode - The random code the participant recieves upon completion
-    # DateTaken - The time at which the participant took the survey
-    'CREATE TABLE `participants` ('
-    '  `ID` char(32) UNIQUE,'
-    '{}'
-    '  `CompletionCode` char(10) DEFAULT \'INCOMPLETE\','
-    '  `DateTaken` timestamp DEFAULT CURRENT_TIMESTAMP,'
-    '  PRIMARY KEY (`ID`)'
-    ')',
-
-    # Participant's responses
-    # The format of the response depends on the test being taken. For example,
-    # an ABX test has as responses a character A, B, or X, and an MOS test has
-    # as responses numbers 1-5.
-    #
-    # Stem - The file stem
-    # Participant - The participant ID
-    # OrderAsked - The chronological ordering of the survey
-    # Response - The response given by the participant
-    'CREATE TABLE `responses` ('
-    '  `Stem` varchar(255),'
-    '  `Participant` char(32),'
-    '  `OrderAsked` int,'
-    '  `Response` {},'
-    '  FOREIGN KEY (`Stem`) REFERENCES `files`(`Stem`),'
-    '  FOREIGN KEY (`Participant`) REFERENCES `participants`(`ID`)'
-    ')']
-
-# Names of tables in the database
-TABLES = ['conditions', 'files', 'participants', 'responses']
-
-
-###############################################################################
-# Database management
-###############################################################################
-
-
-def create(config, test, local=False):
-    """Write database environment variable file and initialize the database"""
-    print('Creating database...')
-
-    # Create new database and retrieve credentials
-    credentials = module(config, local).create(config)
-
-    # Load environment variables
-    for key, value in credentials.items():
-        os.environ[key] = value
-
-    # Connect to MySQL database
-    with connect() as (_, cursor):
-
-        # Create database tables
-        for table, command in zip(TABLES, SCHEMA):
-
-            # Add prescreen questions from configuration file
-            if table == 'participants':
-                questions = ''
-                all_questions = (
-                    config['prescreen_questions'] +
-                    config['followup_questions'])
-                for question in all_questions:
-                    name = question['name']
-
-                    # Get maximum answer length
-                    question_type = question['type']
-                    if question_type == 'free-response':
-                        max_length = 1024
-                    elif question_type == 'multiple-choice':
-                        answers = question['answers']
-                        max_length = max([len(answer) for answer in answers])
-                    else:
-                        raise ValueError(
-                            f'Question type {question_type} is not recognized')
-
-                    # Add database row
-                    questions += f'  `{name}` varchar({max_length}),'
-
-                # Update MySQL command with prescreen questions
-                command = command.format(questions)
-
-            # Response type is unique to the test
-            if table == 'responses':
-                command = command.format(test.response_type())
-
-            # Communicate with database
-            cursor.execute(command)
-
-    # Upload conditions and filenames
-    upload_test(test)
-
-    # Upload any previous results from this evaluation
-    upload_previous(config['name'])
-
-    # Write credentials to environment file
-    environment_file = (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        '.env')
-    environment_file.parent.mkdir(exist_ok=True, parents=True)
-    with open(environment_file, 'w') as file:
-        for key, value in credentials.items():
-            file.write(f'{key}={value}\n')
-
-
-def destroy(name):
-    """Destroy a database"""
-    # Load database credentials
-    try:
-        reseval.load.environment_variables_by_name(name)
-    except FileNotFoundError:
-        return
-
-    # Destroy database
-    local = reseval.is_local(name)
-    config = reseval.load.config_by_name(name)
-    module(config, local).destroy(config)
-
-    # Cleanup credentials
-    (
-        reseval.EVALUATION_DIRECTORY /
-        name /
-        'credentials' /
-        '.env'
-    ).unlink(missing_ok=True)
-
-
-def download(name, directory, tables=TABLES):
-    """Download the contents of the MySQL database"""
-    # Load database credentials
-    reseval.load.environment_variables_by_name(name)
-
-    # Create directory to store results
-    directory.mkdir(exist_ok=True, parents=True)
-
-    with connect() as (_, cursor):
-
-        # Download each table to a csv file
-        for name in tables:
-
-            # Download table
-            cursor.execute('SELECT * FROM ' + name)
-            table = cursor.fetchall()
-
-            # Get table header
-            cursor.execute(f'SHOW COLUMNS FROM {name}')
-            header = [column[0] for column in cursor.fetchall()]
-
-            # Write table to CSV
-            with open(directory / f'{name}.csv', 'w') as file:
-                file = csv.writer(file)
-                file.writerow(header)
-                file.writerows(table)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-@contextlib.contextmanager
-def connect():
-    """Connect to a MySQL database"""
-    try:
-
-        # Connect to the database
-        connection = mysql.connector.connect(
-            database=os.environ['MYSQL_DBNAME'],
-            host=os.environ['MYSQL_HOST'],
-            user=os.environ['MYSQL_USER'],
-            password=os.environ['MYSQL_PASS'])
-
-        # Create cursor to execute commands
-        cursor = connection.cursor()
-
-        # Execute user code
-        yield connection, cursor
-
-    finally:
-
-        # Close database connection
-        if 'cursor' in locals():
-            cursor.close()
-        if 'connection' in locals():
-            connection.close()
-
-
-def upload_previous(name):
-    """Upload previous results from this evaluation to database"""
-    # Check if we have previous results to upload
-    tables = ['participants', 'responses']
-    directory = reseval.EVALUATION_DIRECTORY / name / 'tables'
-    if not all((directory / f'{table}.csv').exists() for table in tables):
-        return
-
-    # Connect to MySQL database
-    with reseval.database.connect() as (connection, cursor):
-
-        # Upload previous results
-        for table in tables:
-
-            # Read CSV
-            with open(directory / f'{table}.csv') as file:
-                rows = [row for row in csv.DictReader(file)]
-
-            # Skip if table is empty
-            if len(rows) == 0:
-                return
-
-            # Format MySQL command
-            keys = list(rows[0].keys())
-            columns, values, update = '', '', ''
-            for i, key in enumerate(keys):
-                columns += f'`{key}`'
-                values += '%s'
-                update += f'`{key}`=`{key}`'
-                if i != len(keys) - 1:
-                    columns += ', '
-                    values += ', '
-                    update += ', '
-            command = (
-                f'INSERT INTO {table} ({columns}) VALUES ({values}) '
-                f'ON DUPLICATE KEY UPDATE {update}')
-
-            # Specify data order
-            items = [tuple(row[key] for key in keys) for row in rows]
-
-            # Execute insertions
-            cursor.executemany(command, items)
-
-        # Communicate with database
-        connection.commit()
-
-
-def upload_test(test):
-    """Upload test information to database"""
-    # Connect to MySQL database
-    with reseval.database.connect() as (connection, cursor):
-
-        # Add conditions to the database
-        command = (
-            'INSERT INTO conditions (`Condition`) VALUES (%s) '
-            'ON DUPLICATE KEY UPDATE `Condition`=`Condition`')
-        cursor.executemany(command, [(c,) for c in test.conditions])
-
-        # Add filenames and extensions to database
-        command = (
-            'INSERT INTO files (Stem, Extension) VALUES (%s, %s) ' +
-            'ON DUPLICATE KEY UPDATE Stem=Stem, Extension=Extension')
-
-        stems_and_extensions = test.stems_and_extensions()
-        cursor.executemany(command, stems_and_extensions)
-        connection.commit()
-
-
-def module(config, local=False):
-    """Get the database module to use"""
-    if local:
-        return reseval.database.localhost
-    database = config['database']
-    if database == 'heroku':
-        return reseval.database.heroku
-    raise ValueError(f'Database service {database} is not recognized')
+import contextlib
+import csv
+import os
+
+import mysql.connector
+
+import reseval
+
+
+###############################################################################
+# Constants
+###############################################################################
+
+
+# MySQL database schema
+SCHEMA = [
+    # Evaluation conditions. For example, for an AB test, these are the
+    # names of the conditions corresponding to the "A" and "B" choices.
+    #
+    # Condition - The name of the condition
+    'CREATE TABLE `conditions` ('
+    '  `Condition` varchar(255) UNIQUE,'
+    '  PRIMARY KEY (`Condition`)'
+    ')',
+
+    # Tables of files to be evaluated, split into stem and extension.
+    # Exact file paths depend on the test being performed. See README for
+    # details.
+    #
+    # Stem - The file stem
+    # Extension - The file extension
+    # Uses - The number of times this stem has been selected for evaluation
+    'CREATE TABLE `files` ('
+    '  `Stem` varchar(255) UNIQUE,'
+    '  `Extension` varchar(16) NOT NULL,'
+    '  `Uses` int DEFAULT 0,'
+    '  PRIMARY KEY (`Stem`)'
+    ')',
+
+    # Participant information
+    # This assumes each participant only takes the survey once.
+    # Prescreening questions from the configuration file are included
+    # as well. These questions are formatted as
+    # f' `{name}` varchar({length}) NOT NULL,', where "name" is the
+    # name given to the question in the configuration file, and "length"
+    # is automatically computed from the longest allowed answer.
+    #
+    # ID - The participant ID
+    # CompletionCode - The random code the participant recieves upon completion
+    # DateTaken - The time at which the participant took the survey
+    'CREATE TABLE `participants` ('
+    '  `ID` char(32) UNIQUE,'
+    '{}'
+    '  `CompletionCode` char(10) DEFAULT \'INCOMPLETE\','
+    '  `DateTaken` timestamp DEFAULT CURRENT_TIMESTAMP,'
+    '  PRIMARY KEY (`ID`)'
+    ')',
+
+    # Participant's responses
+    # The format of the response depends on the test being taken. For example,
+    # an ABX test has as responses a character A, B, or X, and an MOS test has
+    # as responses numbers 1-5.
+    #
+    # Stem - The file stem
+    # Participant - The participant ID
+    # OrderAsked - The chronological ordering of the survey
+    # Response - The response given by the participant
+    'CREATE TABLE `responses` ('
+    '  `Stem` varchar(255),'
+    '  `Participant` char(32),'
+    '  `OrderAsked` int,'
+    '  `Response` {},'
+    '  FOREIGN KEY (`Stem`) REFERENCES `files`(`Stem`),'
+    '  FOREIGN KEY (`Participant`) REFERENCES `participants`(`ID`)'
+    ')']
+
+# Names of tables in the database
+TABLES = ['conditions', 'files', 'participants', 'responses']
+
+
+###############################################################################
+# Database management
+###############################################################################
+
+
+def create(config, test, local=False):
+    """Write database environment variable file and initialize the database"""
+    print('Creating database...')
+
+    # Create new database and retrieve credentials
+    credentials = module(config, local).create(config['name'])
+
+    # Save environment variables
+    for key, value in credentials.items():
+        os.environ[key] = value
+
+    # Connect to MySQL database
+    with connect() as (_, cursor):
+
+        # Create database tables
+        for table, command in zip(TABLES, SCHEMA):
+
+            # Add prescreen questions from configuration file
+            if table == 'participants':
+                questions = ''
+                all_questions = (
+                    config['prescreen_questions'] +
+                    config['followup_questions'])
+                for question in all_questions:
+                    name = question['name']
+
+                    # Get maximum answer length
+                    question_type = question['type']
+                    if question_type == 'free-response':
+                        max_length = 1024
+                    elif question_type == 'multiple-choice':
+                        answers = question['answers']
+                        max_length = max([len(answer) for answer in answers])
+                    else:
+                        raise ValueError(
+                            f'Question type {question_type} is not recognized')
+
+                    # Add database row
+                    questions += f'  `{name}` varchar({max_length}),'
+
+                # Update MySQL command with prescreen questions
+                command = command.format(questions)
+
+            # Response type is unique to the test
+            if table == 'responses':
+                command = command.format(test.response_type())
+
+            # Communicate with database
+            cursor.execute(command)
+
+    # Upload conditions and filenames
+    upload_test(test)
+
+    # Upload any previous results from this evaluation
+    upload_previous(config['name'])
+
+    # Write credentials to environment file
+    environment_file = (
+        reseval.EVALUATION_DIRECTORY /
+        config['name'] /
+        'credentials' /
+        '.env')
+    environment_file.parent.mkdir(exist_ok=True, parents=True)
+    with open(environment_file, 'w') as file:
+        for key, value in credentials.items():
+            file.write(f'{key}={value}\n')
+
+    return credentials
+
+
+def destroy(name):
+    """Destroy a database"""
+    # Load database credentials
+    try:
+        reseval.load.environment_variables_by_name(name)
+    except FileNotFoundError:
+        return
+
+    # Destroy database
+    local = reseval.is_local(name)
+    config = reseval.load.config_by_name(name)
+    module(config, local).destroy(name)
+
+    # Cleanup credentials
+    (
+        reseval.EVALUATION_DIRECTORY /
+        name /
+        'credentials' /
+        '.env'
+    ).unlink(missing_ok=True)
+
+
+def download(name, directory, tables=TABLES):
+    """Download the contents of the MySQL database"""
+    # Load database credentials
+    reseval.load.environment_variables_by_name(name)
+
+    # Create directory to store results
+    directory.mkdir(exist_ok=True, parents=True)
+
+    with connect() as (_, cursor):
+
+        # Download each table to a csv file
+        for name in tables:
+
+            # Download table
+            cursor.execute('SELECT * FROM ' + name)
+            table = cursor.fetchall()
+
+            # Get table header
+            cursor.execute(f'SHOW COLUMNS FROM {name}')
+            header = [column[0] for column in cursor.fetchall()]
+
+            # Write table to CSV
+            with open(directory / f'{name}.csv', 'w') as file:
+                file = csv.writer(file)
+                file.writerow(header)
+                file.writerows(table)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+@contextlib.contextmanager
+def connect():
+    """Connect to a MySQL database"""
+    try:
+
+        # Connect to the database
+        connection = mysql.connector.connect(
+            database=os.environ['MYSQL_DBNAME'],
+            host=os.environ['MYSQL_HOST'],
+            user=os.environ['MYSQL_USER'],
+            password=os.environ['MYSQL_PASS'])
+
+        # Create cursor to execute commands
+        cursor = connection.cursor()
+
+        # Execute user code
+        yield connection, cursor
+
+    finally:
+
+        # Close database connection
+        if 'cursor' in locals():
+            cursor.close()
+        if 'connection' in locals():
+            connection.close()
+
+
+def upload_previous(name):
+    """Upload previous results from this evaluation to database"""
+    # Check if we have previous results to upload
+    tables = ['participants', 'responses']
+    directory = reseval.EVALUATION_DIRECTORY / name / 'tables'
+    if not all((directory / f'{table}.csv').exists() for table in tables):
+        return
+
+    # Connect to MySQL database
+    with connect() as (connection, cursor):
+
+        # Upload previous results
+        for table in tables:
+
+            # Read CSV
+            with open(directory / f'{table}.csv') as file:
+                rows = [row for row in csv.DictReader(file)]
+
+            # Skip if table is empty
+            if len(rows) == 0:
+                return
+
+            # Format MySQL command
+            keys = list(rows[0].keys())
+            columns, values, update = '', '', ''
+            for i, key in enumerate(keys):
+                columns += f'`{key}`'
+                values += '%s'
+                update += f'`{key}`=`{key}`'
+                if i != len(keys) - 1:
+                    columns += ', '
+                    values += ', '
+                    update += ', '
+            command = (
+                f'INSERT INTO {table} ({columns}) VALUES ({values}) '
+                f'ON DUPLICATE KEY UPDATE {update}')
+
+            # Specify data order
+            items = [tuple(row[key] for key in keys) for row in rows]
+
+            # Execute insertions
+            cursor.executemany(command, items)
+
+        # Communicate with database
+        connection.commit()
+
+
+def upload_test(test):
+    """Upload test information to database"""
+    # Connect to MySQL database
+    with connect() as (connection, cursor):
+
+        # Add conditions to the database
+        command = (
+            'INSERT INTO conditions (`Condition`) VALUES (%s) '
+            'ON DUPLICATE KEY UPDATE `Condition`=`Condition`')
+        cursor.executemany(command, [(c,) for c in test.conditions])
+
+        # Add filenames and extensions to database
+        command = (
+            'INSERT INTO files (Stem, Extension) VALUES (%s, %s) ' +
+            'ON DUPLICATE KEY UPDATE Stem=Stem, Extension=Extension')
+
+        stems_and_extensions = test.stems_and_extensions()
+        cursor.executemany(command, stems_and_extensions)
+        connection.commit()
+
+
+def module(config, local=False):
+    """Get the database module to use"""
+    if local:
+        return reseval.database.localhost
+    database = config['database']
+    if database == 'aws':
+        return reseval.database.aws
+    if database == 'heroku':
+        return reseval.database.heroku
+    raise ValueError(f'Database service {database} is not recognized')
```

### Comparing `reseval-0.0.3/reseval/database/localhost.py` & `reseval-0.1.0/reseval/database/localhost.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-import contextlib
-import os
-
-import dotenv
-import mysql.connector
-
-import reseval
-
-
-def create(config):
-    """Create a local MySQL database"""
-    # Load environment variables
-    dotenv.load_dotenv(reseval.ENVIRONMENT_FILE)
-
-    # Create connection
-    with connect() as (_, cursor):
-
-        # Create database
-        cursor.execute(f'CREATE DATABASE `{config["name"]}`')
-
-        # Return credentials
-        return {
-            'MYSQL_DBNAME': config['name'],
-            'MYSQL_HOST': os.environ['MYSQL_HOST'],
-            'MYSQL_USER': os.environ['MYSQL_USER'],
-            'MYSQL_PASS': os.environ['MYSQL_PASS']}
-
-
-def destroy(config):
-    """Destroy a local MySQL database"""
-    # Create connection
-    with connect() as (_, cursor):
-
-        # Destroy database
-        try:
-            cursor.execute(f'DROP DATABASE `{config["name"]}`')
-        except mysql.connector.errors.DatabaseError:
-
-            # Database doesn't exist
-            pass
-
-
-###############################################################################
-# Constants
-###############################################################################
-
-
-@contextlib.contextmanager
-def connect():
-    """Connect to a local MySQL database"""
-    try:
-
-        # Connect to the database
-        connection = mysql.connector.connect(
-            host=os.environ['MYSQL_HOST'],
-            user=os.environ['MYSQL_USER'],
-            password=os.environ['MYSQL_PASS'])
-
-        # Create cursor to execute commands
-        cursor = connection.cursor()
-
-        # Execute user code
-        yield connection, cursor
-
-    finally:
-
-        # Close database connection
-        if 'cursor' in locals():
-            cursor.close()
-        if 'connection' in locals():
-            connection.close()
+import contextlib
+import os
+
+import dotenv
+import mysql.connector
+
+import reseval
+
+
+def create(name):
+    """Create a local MySQL database"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Load environment variables
+    dotenv.load_dotenv(reseval.ENVIRONMENT_FILE)
+
+    # Create connection
+    with connect() as (_, cursor):
+
+        # Create database
+        cursor.execute(f'CREATE DATABASE `{unique}`')
+
+        # Return credentials
+        return {
+            'MYSQL_DBNAME': unique,
+            'MYSQL_HOST': os.environ['MYSQL_HOST'],
+            'MYSQL_USER': os.environ['MYSQL_USER'],
+            'MYSQL_PASS': os.environ['MYSQL_PASS']}
+
+
+def destroy(name):
+    """Destroy a local MySQL database"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Create connection
+    with connect() as (_, cursor):
+
+        # Destroy database
+        try:
+            cursor.execute(f'DROP DATABASE `{unique}`')
+        except mysql.connector.errors.DatabaseError:
+
+            # Database doesn't exist
+            pass
+
+
+###############################################################################
+# Constants
+###############################################################################
+
+
+@contextlib.contextmanager
+def connect():
+    """Connect to a local MySQL database"""
+    try:
+
+        # Connect to the database
+        connection = mysql.connector.connect(
+            host=os.environ['MYSQL_HOST'],
+            user=os.environ['MYSQL_USER'],
+            password=os.environ['MYSQL_PASS'])
+
+        # Create cursor to execute commands
+        cursor = connection.cursor()
+
+        # Execute user code
+        yield connection, cursor
+
+    finally:
+
+        # Close database connection
+        if 'cursor' in locals():
+            cursor.close()
+        if 'connection' in locals():
+            connection.close()
```

### Comparing `reseval-0.0.3/reseval/destroy/__main__.py` & `reseval-0.1.0/reseval/pay/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import argparse
-
-import reseval
-
-
-###############################################################################
-# Entry point for destroying subjective evaluation compute resources
-###############################################################################
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(
-        description='Clean-up database, server, and storage resources')
-    parser.add_argument('name', help='The name of the evaluation to destroy')
-    parser.add_argument(
-        '--force',
-        action='store_true',
-        help='Destroy evaluation resources even if it is still running. ' +
-             'Pays all participants who have taken the evaluation.')
-    return parser.parse_args()
-
-
-reseval.destroy(**vars(parse_args()))
+import argparse
+
+import reseval
+
+
+###############################################################################
+# Entry point for paying participants
+###############################################################################
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(
+        description='Pay participants of a subjective evaluation')
+    parser.add_argument('name', help='The name of the evaluation to pay for')
+    return parser.parse_args()
+
+
+reseval.pay(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/destroy/core.py` & `reseval-0.1.0/reseval/destroy/core.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import shutil
-import reseval
-
-
-###############################################################################
-# Cleanup subjective evaluation compute resources
-###############################################################################
-
-
-def destroy(name: str, force: bool = False):
-    """Destroys an evaluation's storage, database, server, and crowdsource task
-
-    Args:
-        name: The name of the evaluation to destroy
-        force: Destroy evaluation resources even if it is still running. Pays
-            all participants who have taken the evaluation.
-    """
-    # Evaluation doesn't exist
-    if not (reseval.EVALUATION_DIRECTORY / name).exists():
-        return
-
-    # Is the evaluation currently active?
-    try:
-        active = reseval.crowdsource.active(name)
-    except Exception:
-        if force:
-            active = False
-
-    paid = reseval.crowdsource.paid(name)
-    if active or not paid:
-
-        if not force:
-            tag = (
-                ('active ' if active else '') +
-                ('unpaid ' if not paid else ''))
-            raise ValueError(
-                f'Not destroying {tag}subjective evaluation {name}')
-
-        else:
-
-            # Pay participants
-            if not paid:
-                reseval.crowdsource.pay(name)
-
-    # Maybe destroy crowdsource task
-    reseval.crowdsource.destroy(name)
-
-    # Destroy server
-    reseval.server.destroy(name)
-
-    # Destroy database
-    reseval.database.destroy(name)
-
-    # Destroy storage
-    reseval.storage.destroy(name)
-
-    # Clean-up cache
-    shutil.rmtree(reseval.EVALUATION_DIRECTORY / name)
+import shutil
+import reseval
+
+
+###############################################################################
+# Cleanup subjective evaluation compute resources
+###############################################################################
+
+
+def destroy(name: str, force: bool = False):
+    """Destroys an evaluation's storage, database, server, and crowdsource task
+
+    Args:
+        name: The name of the evaluation to destroy
+        force: Destroy evaluation resources even if it is still running. Pays
+            all participants who have taken the evaluation.
+    """
+    # Evaluation doesn't exist
+    if not (reseval.EVALUATION_DIRECTORY / name).exists():
+        return
+
+    # Is the evaluation currently active?
+    try:
+        active = reseval.crowdsource.active(name)
+    except Exception:
+        if force:
+            active = False
+
+    paid = reseval.crowdsource.paid(name)
+    if active or not paid:
+
+        if not force:
+            tag = (
+                ('active ' if active else '') +
+                ('unpaid ' if not paid else ''))
+            raise ValueError(
+                f'Not destroying {tag}subjective evaluation {name}')
+
+        else:
+
+            # Pay participants
+            if not paid:
+                reseval.crowdsource.pay(name)
+
+    # Maybe destroy crowdsource task
+    reseval.crowdsource.destroy(name)
+
+    # Destroy database
+    reseval.database.destroy(name)
+
+    # Destroy server
+    reseval.server.destroy(name)
+
+    # Destroy storage
+    reseval.storage.destroy(name)
+
+    # Clean-up cache
+    shutil.rmtree(reseval.EVALUATION_DIRECTORY / name)
```

### Comparing `reseval-0.0.3/reseval/extend/core.py` & `reseval-0.1.0/reseval/extend/core.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import re
-
-import reseval
-
-
-def extend(
-    name: str,
-    participants: int,
-    local: bool = False,
-    production: bool = False):
-    """Extend a subjective evaluation
-
-    Args:
-        name: The name of the evaluation to extend
-        participants: The number of new participants to add to the evaluation
-        local: Run subjective evaluation locally
-        production: Deploy the subjective evaluation to crowdsource
-            participants
-    """
-    if not (reseval.EVALUATION_DIRECTORY / name).exists():
-        raise ValueError(f'Cannot extend non-existant evaluation {name}')
-
-    if production and local:
-        raise ValueError('Cannot deploy production build locally')
-
-    # We can only restart evaluations that have been run in the same mode
-    prod_file = reseval.EVALUATION_DIRECTORY / name / '.prod'
-    if not production and prod_file.exists():
-        raise ValueError(
-            f'Cannot extend production evaluation {name} '
-            'in non-production mode')
-    local_file = reseval.EVALUATION_DIRECTORY / name / '.local'
-    if not local and local_file.exists():
-        raise ValueError(
-            f'Cannot extend local evaluation {name} '
-            'in non-local mode')
-
-    # Extend crowdsourcing task
-    reseval.crowdsource.extend(name, participants)
-
-    # Get saved configuration
-    config_file = reseval.EVALUATION_DIRECTORY / name / 'config.yaml'
-    with open(config_file, encoding='utf-8') as file:
-        lines = file.readlines()
-
-    # Replace number of participants
-    for i in range(len(lines)):
-        if lines[i].startswith('participants: '):
-            previous = re.findall(r'\d+', lines[i])[0]
-            current = int(previous) + participants
-            lines[i] = re.sub(r'\d+', str(current), lines[i])
-
-    # Save new configuration
-    with open(config_file, 'w', encoding='utf-8') as file:
-        for line in lines:
-            file.write(line)
+import re
+
+import reseval
+
+
+def extend(
+    name: str,
+    participants: int,
+    local: bool = False,
+    production: bool = False):
+    """Extend a subjective evaluation
+
+    Args:
+        name: The name of the evaluation to extend
+        participants: The number of new participants to add to the evaluation
+        local: Run subjective evaluation locally
+        production: Deploy the subjective evaluation to crowdsource
+            participants
+    """
+    if not (reseval.EVALUATION_DIRECTORY / name).exists():
+        raise ValueError(f'Cannot extend non-existant evaluation {name}')
+
+    if production and local:
+        raise ValueError('Cannot deploy production build locally')
+
+    # We can only restart evaluations that have been run in the same mode
+    prod_file = reseval.EVALUATION_DIRECTORY / name / '.prod'
+    if not production and prod_file.exists():
+        raise ValueError(
+            f'Cannot extend production evaluation {name} '
+            'in non-production mode')
+    local_file = reseval.EVALUATION_DIRECTORY / name / '.local'
+    if not local and local_file.exists():
+        raise ValueError(
+            f'Cannot extend local evaluation {name} '
+            'in non-local mode')
+
+    # Extend crowdsourcing task
+    reseval.crowdsource.extend(name, participants)
+
+    # Get saved configuration
+    config_file = reseval.EVALUATION_DIRECTORY / name / 'config.yaml'
+    with open(config_file, encoding='utf-8') as file:
+        lines = file.readlines()
+
+    # Replace number of participants
+    for i in range(len(lines)):
+        if lines[i].startswith('participants: '):
+            previous = re.findall(r'\d+', lines[i])[0]
+            current = int(previous) + participants
+            lines[i] = re.sub(r'\d+', str(current), lines[i])
+
+    # Save new configuration
+    with open(config_file, 'w', encoding='utf-8') as file:
+        for line in lines:
+            file.write(line)
```

### Comparing `reseval-0.0.3/reseval/filter.py` & `reseval-0.1.0/reseval/filter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-def anchors(responses, conditions, low_anchor, high_anchor):
-    """Removes participants that rate the low anchor above the high anchor"""
-    low_index = conditions.index(low_anchor)
-    high_index = conditions.index(high_anchor)
-
-    # Make blacklist of bad participants
-    blacklist = set()
-    for response in responses:
-        scores = response['Response']
-        scores = [scores[i:i + 3] for i in range(0, len(scores), 3)]
-        if scores[low_index] > scores[high_index]:
-            blacklist.add(response['Participant'])
-
-    # Filter out bad participants
-    filtered = []
-    for response in responses:
-        if response['Participant'] not in blacklist:
-            filtered.append(response)
-
-    return filtered
+def anchors(responses, conditions, low_anchor, high_anchor):
+    """Removes participants that rate the low anchor above the high anchor"""
+    low_index = conditions.index(low_anchor)
+    high_index = conditions.index(high_anchor)
+
+    # Make blacklist of bad participants
+    blacklist = set()
+    for response in responses:
+        scores = response['Response']
+        scores = [scores[i:i + 3] for i in range(0, len(scores), 3)]
+        if scores[low_index] > scores[high_index]:
+            blacklist.add(response['Participant'])
+
+    # Filter out bad participants
+    filtered = []
+    for response in responses:
+        if response['Participant'] not in blacklist:
+            filtered.append(response)
+
+    return filtered
```

### Comparing `reseval-0.0.3/reseval/monitor/__main__.py` & `reseval-0.1.0/reseval/monitor/__main__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import argparse
-
-import reseval
-
-
-###############################################################################
-# Entry point for monitoring subjective evaluations
-###############################################################################
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(
-        description='Monitor subjective evaluations')
-    parser.add_argument(
-        '--names',
-        nargs='+',
-        help='The names of the evaluations to monitor. ' +
-             'If not provided, monitors all evaluations.')
-    parser.add_argument(
-        '--interval',
-        type=int,
-        default=60,
-        help='The time between monitoring updates in seconds')
-    return parser.parse_args()
-
-
-reseval.monitor(**vars(parse_args()))
+import argparse
+
+import reseval
+
+
+###############################################################################
+# Entry point for monitoring subjective evaluations
+###############################################################################
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(
+        description='Monitor subjective evaluations')
+    parser.add_argument(
+        '--names',
+        nargs='+',
+        help='The names of the evaluations to monitor. ' +
+             'If not provided, monitors all evaluations.')
+    parser.add_argument(
+        '--interval',
+        type=int,
+        default=60,
+        help='The time between monitoring updates in seconds')
+    return parser.parse_args()
+
+
+reseval.monitor(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/npm.py` & `reseval-0.1.0/reseval/npm.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import subprocess
-
-
-###############################################################################
-# Npm server management
-
-# NOTE - shell=True is often not considered best practice. This is for two
-#     reasons:
-#         1) It assumes the binary is the program you expect it to be. In
-#            this case, npm.
-#         2) If parameterized, it can run malicious code. For example,
-#            f'npm run {user_input}' where
-#            user_input = 'nonexistant_arg; rm -rf /'.
-#     In our use case, we've asked users to install npm and we do not
-#     parameterize the commands. The alternative is to set shell=False and
-#     require the user to provide the path to the npm executable.
-###############################################################################
-
-
-def build(verbose=False):
-    """Build the optimized front-end client code"""
-    stdout = None if verbose else subprocess.DEVNULL
-    return subprocess.Popen('npm run build', shell=True, stdout=stdout)
-
-
-def install():
-    """Installs an npm package in the current directory"""
-    return subprocess.Popen('npm install', shell=True)
-
-
-def start():
-    """Start the server process"""
-    return subprocess.Popen('npm run dev', shell=True)
+import subprocess
+
+
+###############################################################################
+# Npm server management
+
+# NOTE - shell=True is often not considered best practice. This is for two
+#     reasons:
+#         1) It assumes the binary is the program you expect it to be. In
+#            this case, npm.
+#         2) If parameterized, it can run malicious code. For example,
+#            f'npm run {user_input}' where
+#            user_input = 'nonexistant_arg; rm -rf /'.
+#     In our use case, we've asked users to install npm and we do not
+#     parameterize the commands. The alternative is to set shell=False and
+#     require the user to provide the path to the npm executable.
+###############################################################################
+
+
+def build(verbose=False):
+    """Build the optimized front-end client code"""
+    stdout = None if verbose else subprocess.DEVNULL
+    return subprocess.Popen('npm run build', shell=True, stdout=stdout)
+
+
+def install():
+    """Installs an npm package in the current directory"""
+    return subprocess.Popen('npm install', shell=True)
+
+
+def start():
+    """Start the server process"""
+    return subprocess.Popen('npm run dev', shell=True)
```

### Comparing `reseval-0.0.3/reseval/pay/__main__.py` & `reseval-0.1.0/reseval/results/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-import argparse
-
-import reseval
-
-
-###############################################################################
-# Entry point for paying participants
-###############################################################################
-
-
-def parse_args():
-    """Parse command-line arguments"""
-    parser = argparse.ArgumentParser(
-        description='Pay participants of a subjective evaluation')
-    parser.add_argument('name', help='The name of the evaluation to pay for')
-    return parser.parse_args()
-
-
-reseval.pay(**vars(parse_args()))
+import argparse
+from pathlib import Path
+
+import reseval
+
+
+###############################################################################
+# Get the results of a subjective evaluation
+###############################################################################
+
+
+def parse_args():
+    """Parse command-line arguments"""
+    parser = argparse.ArgumentParser(
+        description='Get the results of a subjective evaluation')
+    parser.add_argument(
+        'name',
+        help='The name of the subjective evaluation to retrieve results for')
+    parser.add_argument(
+        '--directory',
+        type=Path,
+        default=Path(),
+        help='The directory to save results')
+    return parser.parse_args()
+
+
+reseval.results(**vars(parse_args()))
```

### Comparing `reseval-0.0.3/reseval/plot.py` & `reseval-0.1.0/reseval/plot.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import matplotlib
-import matplotlib.pyplot as plt
-import numpy as np
-
-
-###############################################################################
-# Statistical plots
-###############################################################################
-
-
-def barh(results, file):
-    """Create a barh plot"""
-    # TODO
-    pass
-
-
-def violin(results, file, yticks):
-    """Create a violin plot"""
-    # Set font size
-    matplotlib.rcParams.update({'font.size': 18})
-
-    # Organize data by condition
-    data = {}
-    for _, values in results.items():
-        for condition, scores in values.items():
-            if condition not in data:
-                data[condition] = scores
-            else:
-                data[condition].extend(scores)
-    keys = np.array(list(data.keys()))
-    values = np.array(
-        [np.array(sorted(value), dtype=np.int) for value in data.values()])
-
-    # Order data by average value
-    means = np.nan_to_num([value.mean() for value in values])
-    indices = np.argsort(means)
-    means, keys, values = means[indices], list(keys[indices]), values[indices]
-
-    # No data
-    if not all(len(value) for value in values):
-        return
-
-    # Create violin plot
-    figure, ax = plt.subplots(1, 1, squeeze=True, figsize=(16, 6))
-    ax.violinplot(
-        values,
-        showmeans=False,
-        showmedians=False,
-        showextrema=False)
-
-    # Get locations of start and ends of violins
-    _, medians, _ = np.percentile(
-        values,
-        [25, 50, 75],
-        axis=values.ndim - 1)
-
-    # Style axes
-    inds = np.arange(1, len(medians) + 1)
-    ax.scatter(inds, means, marker='o', color='black', s=80, zorder=3)
-    ax.scatter(inds, medians, marker='o', color='white', s=80, zorder=3)
-
-    # Style axes
-    ax.spines['top'].set_visible(False)
-    ax.spines['right'].set_visible(False)
-    ax.spines['bottom'].set_visible(False)
-    ax.spines['left'].set_visible(False)
-    ax.xaxis.set_ticks_position('none')
-    ax.yaxis.set_ticks_position('none')
-    for y in yticks:
-        ax.hlines(
-            y=y,
-            xmin=0,
-            xmax=5.3,
-            linewidth=1,
-            color='#666666',
-            alpha=.3)
-
-    # Add labels
-    ax.set_xticks(np.arange(1, len(keys) + 1), labels=keys)
-    ax.set_xlim(0.25, len(keys) + 0.75)
-
-    # Save figure
-    figure.savefig(file, bbox_inches='tight', pad_inches=0)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def adjacent_values(vals, q1, q3):
-    upper_adjacent_value = q3 + (q3 - q1) * 1.5
-    upper_adjacent_value = np.clip(upper_adjacent_value, q3, vals[-1])
-    lower_adjacent_value = q1 - (q3 - q1) * 1.5
-    lower_adjacent_value = np.clip(lower_adjacent_value, vals[0], q1)
-    return lower_adjacent_value, upper_adjacent_value
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+
+
+###############################################################################
+# Statistical plots
+###############################################################################
+
+
+def barh(results, file):
+    """Create a barh plot"""
+    # TODO
+    pass
+
+
+def violin(results, file, yticks):
+    """Create a violin plot"""
+    # Set font size
+    matplotlib.rcParams.update({'font.size': 18})
+
+    # Organize data by condition
+    data = {}
+    for _, values in results.items():
+        for condition, scores in values.items():
+            if condition not in data:
+                data[condition] = scores
+            else:
+                data[condition].extend(scores)
+    keys = np.array(list(data.keys()))
+    values = np.array(
+        [np.array(sorted(value), dtype=np.int) for value in data.values()])
+
+    # Order data by average value
+    means = np.nan_to_num([value.mean() for value in values])
+    indices = np.argsort(means)
+    means, keys, values = means[indices], list(keys[indices]), values[indices]
+
+    # No data
+    if not all(len(value) for value in values):
+        return
+
+    # Create violin plot
+    figure, ax = plt.subplots(1, 1, squeeze=True, figsize=(16, 6))
+    ax.violinplot(
+        values,
+        showmeans=False,
+        showmedians=False,
+        showextrema=False)
+
+    # Get locations of start and ends of violins
+    _, medians, _ = np.percentile(
+        values,
+        [25, 50, 75],
+        axis=values.ndim - 1)
+
+    # Style axes
+    inds = np.arange(1, len(medians) + 1)
+    ax.scatter(inds, means, marker='o', color='black', s=80, zorder=3)
+    ax.scatter(inds, medians, marker='o', color='white', s=80, zorder=3)
+
+    # Style axes
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['bottom'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.xaxis.set_ticks_position('none')
+    ax.yaxis.set_ticks_position('none')
+    for y in yticks:
+        ax.hlines(
+            y=y,
+            xmin=0,
+            xmax=5.3,
+            linewidth=1,
+            color='#666666',
+            alpha=.3)
+
+    # Add labels
+    ax.set_xticks(np.arange(1, len(keys) + 1), labels=keys)
+    ax.set_xlim(0.25, len(keys) + 0.75)
+
+    # Save figure
+    figure.savefig(file, bbox_inches='tight', pad_inches=0)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def adjacent_values(vals, q1, q3):
+    upper_adjacent_value = q3 + (q3 - q1) * 1.5
+    upper_adjacent_value = np.clip(upper_adjacent_value, q3, vals[-1])
+    lower_adjacent_value = q1 - (q3 - q1) * 1.5
+    lower_adjacent_value = np.clip(lower_adjacent_value, vals[0], q1)
+    return lower_adjacent_value, upper_adjacent_value
```

### Comparing `reseval-0.0.3/reseval/results/core.py` & `reseval-0.1.0/reseval/results/core.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import json
-import os
-import typing
-from pathlib import Path
-
-import reseval
-
-
-###############################################################################
-# Get subjective evaluation results
-###############################################################################
-
-
-def results(
-    name: str,
-    directory: typing.Union[str, bytes, os.PathLike] = Path()) -> dict:
-    """Get the results of a subjective evaluation
-
-    Args:
-        name: The name of the subjective evaluation to retrieve results for
-        directory: The directory to save results
-
-    Returns:
-        dict: Evaluation results
-    """
-    # Download and save crowdsource results
-    crowdsource = reseval.crowdsource.assignments(name)
-    crowdsource_file = directory / name / 'crowdsource' / 'crowdsource.json'
-    crowdsource_file.parent.mkdir(exist_ok=True, parents=True)
-    with open(crowdsource_file, 'w') as file:
-        json.dump(crowdsource, file, indent=4, default=str)
-
-    # Download database tables
-    reseval.database.download(
-        name,
-        reseval.EVALUATION_DIRECTORY / name / 'tables')
-    if directory is not None:
-        reseval.database.download(name, directory / name / 'tables')
-
-    # Load responses
-    config = reseval.load.config_by_name(name)
-    conditions = reseval.load.conditions(name)
-    responses = reseval.load.responses(name)
-
-    # No responses yet
-    if len(responses) == 0:
-        results = {'samples': 0, 'conditions': {}}
-
-        # Save results
-        with open(directory / name / 'results.json', 'w') as file:
-            json.dump(results, file, indent=4)
-
-        return results
-
-    # Get condition names
-    conditions = [condition['Condition'] for condition in conditions]
-
-    # Group results by file stems
-    responses_by_stem = {}
-    for response in responses:
-        stem = response['Stem']
-        if stem in responses_by_stem:
-            responses_by_stem[stem].append(response['Response'])
-        else:
-            responses_by_stem[stem] = [response['Response']]
-
-    # Get test
-    test = reseval.test.get(config)
-
-    # Analyze results
-    analysis, stem_scores = test.analyze(
-        conditions,
-        responses_by_stem,
-        config['random_seed'])
-
-    # Save results
-    with open(directory / name / 'results.json', 'w') as file:
-        json.dump(analysis | {'stems': stem_scores}, file, indent=4)
-
-    # Create and save figure
-    test.plot(stem_scores, directory / name / 'results.jpg')
-
-    return analysis
+import json
+import os
+import typing
+from pathlib import Path
+
+import reseval
+
+
+###############################################################################
+# Get subjective evaluation results
+###############################################################################
+
+
+def results(
+    name: str,
+    directory: typing.Union[str, bytes, os.PathLike] = Path()) -> dict:
+    """Get the results of a subjective evaluation
+
+    Args:
+        name: The name of the subjective evaluation to retrieve results for
+        directory: The directory to save results
+
+    Returns:
+        dict: Evaluation results
+    """
+    # Download and save crowdsource results
+    crowdsource = reseval.crowdsource.assignments(name)
+    crowdsource_file = directory / name / 'crowdsource' / 'crowdsource.json'
+    crowdsource_file.parent.mkdir(exist_ok=True, parents=True)
+    with open(crowdsource_file, 'w') as file:
+        json.dump(crowdsource, file, indent=4, default=str)
+
+    # Download database tables
+    reseval.database.download(
+        name,
+        reseval.EVALUATION_DIRECTORY / name / 'tables')
+    if directory is not None:
+        reseval.database.download(name, directory / name / 'tables')
+
+    # Load responses
+    config = reseval.load.config_by_name(name)
+    conditions = reseval.load.conditions(name)
+    responses = reseval.load.responses(name)
+
+    # No responses yet
+    if len(responses) == 0:
+        results = {'samples': 0, 'conditions': {}}
+
+        # Save results
+        with open(directory / name / 'results.json', 'w') as file:
+            json.dump(results, file, indent=4)
+
+        return results
+
+    # Get condition names
+    conditions = [condition['Condition'] for condition in conditions]
+
+    # Group results by file stems
+    responses_by_stem = {}
+    for response in responses:
+        stem = response['Stem']
+        if stem in responses_by_stem:
+            responses_by_stem[stem].append(response['Response'])
+        else:
+            responses_by_stem[stem] = [response['Response']]
+
+    # Get test
+    test = reseval.test.get(config)
+
+    # Analyze results
+    analysis, stem_scores = test.analyze(
+        conditions,
+        responses_by_stem,
+        config['random_seed'])
+
+    # Save results
+    with open(directory / name / 'results.json', 'w') as file:
+        json.dump(analysis | {'stems': stem_scores}, file, indent=4)
+
+    # Create and save figure
+    test.plot(stem_scores, directory / name / 'results.jpg')
+
+    return analysis
```

### Comparing `reseval-0.0.3/reseval/server/core.py` & `reseval-0.1.0/reseval/server/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-import json
-
-import reseval
-
-
-###############################################################################
-# Server management
-###############################################################################
-
-
-def create(config, local=False, detach=False):
-    """Create a server"""
-    print('Creating server...')
-
-    # Create server
-    credentials = module(config, local).create(
-        config | {'detach': detach})
-
-    # Save server credentials
-    file = (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        'server.json')
-    file.parent.mkdir(exist_ok=True, parents=True)
-    with open(file, 'w') as file:
-        json.dump(credentials, file, indent=4, sort_keys=True)
-
-    # Return the application URL
-    return credentials['URL']
-
-
-def destroy(name):
-    """Destroy a server"""
-    local = reseval.is_local(name)
-
-    # Load config
-    config = reseval.load.config_by_name(name)
-
-    try:
-
-        # Load credentials
-        credentials = reseval.load.credentials_by_name(name, 'server')
-
-    except FileNotFoundError:
-
-        # We assume the server does not exist if we don't have credentials
-        return
-
-    # Destroy server
-    module(config, local).destroy(config, credentials)
-
-    # Cleanup credentials
-    (
-        reseval.EVALUATION_DIRECTORY /
-        name /
-        'credentials' /
-        'server.json'
-    ).unlink(missing_ok=True)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def module(config, local=False):
-    """Get the crowdsourcing module to use"""
-    if local:
-        return reseval.server.local
-    server = config['server']
-    if server == 'heroku':
-        return reseval.server.heroku
-    raise ValueError(f'Server hosting service {server} not recognized')
+import json
+
+import reseval
+
+
+###############################################################################
+# Server management
+###############################################################################
+
+
+def create(config, local=False, detach=False):
+    """Create a server"""
+    print('Creating server...')
+
+    # Create server
+    name = config['name']
+    credentials = module(config, local).create(name, detach=detach)
+
+    # Save server credentials
+    file = reseval.EVALUATION_DIRECTORY / name / 'credentials' / 'server.json'
+    file.parent.mkdir(exist_ok=True, parents=True)
+    with open(file, 'w') as file:
+        json.dump(credentials, file, indent=4, sort_keys=True)
+
+    # Return the application URL
+    return credentials['URL']
+
+
+def destroy(name):
+    """Destroy a server"""
+    local = reseval.is_local(name)
+
+    # Load config
+    config = reseval.load.config_by_name(name)
+
+    try:
+
+        # Load credentials
+        credentials = reseval.load.credentials_by_name(name, 'server')
+
+    except FileNotFoundError:
+
+        # We assume the server does not exist if we don't have credentials
+        return
+
+    # Destroy server
+    module(config, local).destroy(name, credentials)
+
+    # Cleanup credentials
+    (
+        reseval.EVALUATION_DIRECTORY /
+        name /
+        'credentials' /
+        'server.json'
+    ).unlink(missing_ok=True)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def module(config, local=False):
+    """Get the crowdsourcing module to use"""
+    if local:
+        return reseval.server.local
+    server = config['server']
+    if server == 'aws':
+        return reseval.server.aws
+    if server == 'heroku':
+        return reseval.server.heroku
+    raise ValueError(f'Server hosting service {server} not recognized')
```

### Comparing `reseval-0.0.3/reseval/server/heroku.py` & `reseval-0.1.0/reseval/server/heroku.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,124 @@
-import http.client
-import json
-import os
-import tarfile
-import tempfile
-import time
-from pathlib import Path
-
-import reseval
-
-
-###############################################################################
-# Heroku server management
-###############################################################################
-
-
-def create(config):
-    """Create a Heroku server"""
-    # Connect to Heroku
-    connection = http.client.HTTPSConnection('api.heroku.com')
-
-    # Maybe install client
-    client_directory = reseval.CACHE / 'client'
-    if not (client_directory / 'node_modules').exists():
-        with reseval.chdir(client_directory):
-            reseval.npm.install().wait()
-
-    # Build client
-    with reseval.chdir(reseval.CACHE / 'client'):
-        reseval.npm.build().wait()
-
-    # Create a tarball of all files needed by the Heroku server
-    with tempfile.TemporaryDirectory() as directory:
-        tarball = Path(directory) / 'reseval.tar.gz'
-        files = [
-            'client/build',
-            'server',
-            'package-lock.json',
-            'package.json',
-            'Procfile',
-            'server.ts',
-            'tsconfig.json']
-        with tarfile.open(tarball, 'w:gz') as tar:
-            for file in files:
-                tar.add(reseval.CACHE / file)
-
-        # Upload tarball and get a URL
-        tarball_url = reseval.storage.upload(config['name'], tarball)
-
-        # Server configuration
-        data = {
-            'source_blob': {'url': tarball_url},
-            'buildpacks': [{
-                'url': 'https://github.com/heroku/heroku-buildpack-nodejs',
-                'name': 'heroku/nodejs'}]}
-        headers = {
-            'Accept': 'application/vnd.heroku+json; version=3',
-            'Authorization': f'Bearer {os.environ["HerokuAccessKey"]}'}
-
-        # Create server
-        name = reseval.load.credentials_by_name(config['name'], 'app')['name']
-        connection.request(
-            'POST',
-            f'/apps/{name}/builds',
-            json.dumps(data),
-            headers=headers)
-
-        # Get response from server
-        response = json.loads(connection.getresponse().read().decode())
-
-        # if app doesn't exist, raise error
-        if response['id'] == 'not_found':
-            raise ValueError(f'app name: {config["name"]} does not exist')
-
-    # Close the connection
-    connection.close()
-
-    # Wait until server is setup
-    while status(config['name']) == 'pending':
-        time.sleep(3)
-
-    if status(config['name']) == 'failure':
-        raise ValueError('Heroku server failed to start')
-
-    # Return application URL
-    return {'URL': f'http://{name}.herokuapp.com/'}
-
-
-def destroy(config, credentials):
-    """Destroy a Heroku server"""
-    reseval.app.heroku.destroy(config)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def status(name):
-    """Get current build status. One of ['succeeded', 'failed', 'pending']"""
-    # Connect to Heroku
-    connection = http.client.HTTPSConnection('api.heroku.com')
-
-    # Send request
-    reseval.load.api_keys()
-    headers = {
-        'Accept': 'application/vnd.heroku+json; version=3',
-        'Authorization': f'Bearer {os.environ["HerokuAccessKey"]}'}
-    unique_name = reseval.load.credentials_by_name(name, 'app')['name']
-    connection.request('GET', f'/apps/{unique_name}/builds', headers=headers)
-
-    # Get response
-    data = json.loads(connection.getresponse().read().decode())
-
-    # Close connection
-    connection.close()
-
-    # Get most recent build status from response
-    status = list(map(lambda x: x['status'], data))
-    return status[-1]
+import http.client
+import json
+import os
+import tarfile
+import tempfile
+import time
+from pathlib import Path
+
+import reseval
+
+
+###############################################################################
+# Heroku server management
+###############################################################################
+
+
+def create(name, detach=True):
+    """Create a Heroku server"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Connect to Heroku
+    connection = http.client.HTTPSConnection('api.heroku.com')
+
+    # Maybe install client
+    client_directory = reseval.CACHE / 'client'
+    if not (client_directory / 'node_modules').exists():
+        with reseval.chdir(client_directory):
+            reseval.npm.install().wait()
+
+    # Build client
+    with reseval.chdir(reseval.CACHE / 'client'):
+        reseval.npm.build().wait()
+
+    # Create a tarball of all files needed by the Heroku server
+    with tempfile.TemporaryDirectory() as directory:
+        tarball = Path(directory) / 'reseval.tar.gz'
+        files = [
+            'client/build',
+            'server',
+            'package-lock.json',
+            'package.json',
+            'Procfile',
+            'server.ts',
+            'tsconfig.json']
+        with tarfile.open(tarball, 'w:gz') as tar:
+            for file in files:
+                tar.add(reseval.CACHE / file)
+
+        # Upload tarball and get a URL
+        tarball_url = reseval.storage.upload(name, tarball)
+
+        # Server configuration
+        data = {
+            'source_blob': {'url': tarball_url},
+            'buildpacks': [{
+                'url': 'https://github.com/heroku/heroku-buildpack-nodejs',
+                'name': 'heroku/nodejs'}]}
+        headers = {
+            'Accept': 'application/vnd.heroku+json; version=3',
+            'Authorization': f'Bearer {os.environ["HerokuAccessKey"]}'}
+
+        # Create server
+        connection.request(
+            'POST',
+            f'/apps/{unique}/builds',
+            json.dumps(data),
+            headers=headers)
+
+        # Get response from server
+        response = json.loads(connection.getresponse().read().decode())
+
+        # if app doesn't exist, raise error
+        if response['id'] == 'not_found':
+            raise ValueError(f'app name: {unique} does not exist')
+
+    # Close the connection
+    connection.close()
+
+    # Wait until server is setup
+    while status(name) == 'pending':
+        time.sleep(3)
+
+    if status(name) == 'failure':
+        raise ValueError('Heroku server failed to start')
+
+    # Return application URL
+    return {'URL': f'http://{name}.herokuapp.com/'}
+
+
+def destroy(name, credentials):
+    """Destroy a Heroku server"""
+    reseval.app.heroku.destroy(name)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def status(name):
+    """Get current build status. One of ['succeeded', 'failed', 'pending']"""
+    # Get unique identifier
+    unique = reseval.load.credentials_by_name(name, 'unique')['unique']
+
+    # Connect to Heroku
+    connection = http.client.HTTPSConnection('api.heroku.com')
+
+    # Send request
+    reseval.load.api_keys()
+    headers = {
+        'Accept': 'application/vnd.heroku+json; version=3',
+        'Authorization': f'Bearer {os.environ["HerokuAccessKey"]}'}
+    connection.request('GET', f'/apps/{unique}/builds', headers=headers)
+
+    # Get response
+    data = json.loads(connection.getresponse().read().decode())
+
+    # Close connection
+    connection.close()
+
+    # Get most recent build status from response
+    status = list(map(lambda x: x['status'], data))
+    return status[-1]
```

### Comparing `reseval-0.0.3/reseval/server/local.py` & `reseval-0.1.0/reseval/server/local.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import json
-import psutil
-import webbrowser
-
-import requests
-from requests.adapters import HTTPAdapter, Retry
-
-import reseval
-
-
-###############################################################################
-# Local server management
-###############################################################################
-
-
-def create(config):
-    """Deploy a local server"""
-    # Maybe install server
-    if not (reseval.CACHE / 'node_modules').exists():
-        with reseval.chdir(reseval.CACHE):
-            reseval.npm.install().wait()
-
-    # Maybe install client
-    client_directory = reseval.CACHE / 'client'
-    if not (client_directory / 'node_modules').exists():
-        with reseval.chdir(client_directory):
-            reseval.npm.install().wait()
-
-    # Launch server process
-    with reseval.chdir(reseval.CACHE):
-        process = reseval.npm.start()
-
-    # Ping server until we get a response
-    session = requests.Session()
-    retries = Retry(total=11,
-                    backoff_factor=0.1,
-                    status_forcelist=[500, 502, 503, 504])
-    session.mount('http://', HTTPAdapter(max_retries=retries))
-    session.get(reseval.LOCALHOST_URL)
-
-    # Open web browser to evaluation
-    webbrowser.open(reseval.LOCALHOST_URL)
-
-    # Save server credentials
-    credentials = {'URL': reseval.LOCALHOST_URL, 'PID': process.pid}
-    file = (
-        reseval.EVALUATION_DIRECTORY /
-        config['name'] /
-        'credentials' /
-        'server.json')
-    file.parent.mkdir(exist_ok=True, parents=True)
-    with open(file, 'w') as file:
-        json.dump(credentials, file, indent=4, sort_keys=True)
-
-    # Maybe wait for process to finish
-    if not config['detach']:
-        process.wait()
-
-    return credentials
-
-
-def destroy(config, credentials):
-    """Shutdown a local server"""
-    try:
-        parent = psutil.Process(credentials['PID'])
-        for child in parent.children(recursive=True):
-            child.kill()
-        parent.kill()
-    except psutil.NoSuchProcess:
-        pass
+import json
+import psutil
+import webbrowser
+
+import requests
+from requests.adapters import HTTPAdapter, Retry
+
+import reseval
+
+
+###############################################################################
+# Local server management
+###############################################################################
+
+
+def create(name, detach=False):
+    """Deploy a local server"""
+    # Maybe install server
+    if not (reseval.CACHE / 'node_modules').exists():
+        with reseval.chdir(reseval.CACHE):
+            reseval.npm.install().wait()
+
+    # Maybe install client
+    client_directory = reseval.CACHE / 'client'
+    if not (client_directory / 'node_modules').exists():
+        with reseval.chdir(client_directory):
+            reseval.npm.install().wait()
+
+    # Launch server process
+    with reseval.chdir(reseval.CACHE):
+        process = reseval.npm.start()
+
+    # Ping server until we get a response
+    session = requests.Session()
+    retries = Retry(total=11,
+                    backoff_factor=0.1,
+                    status_forcelist=[500, 502, 503, 504])
+    session.mount('http://', HTTPAdapter(max_retries=retries))
+    session.get(reseval.LOCALHOST_URL)
+
+    # Open web browser to evaluation
+    webbrowser.open(reseval.LOCALHOST_URL)
+
+    # Save server credentials
+    credentials = {'URL': reseval.LOCALHOST_URL, 'PID': process.pid}
+    file = (
+        reseval.EVALUATION_DIRECTORY /
+        name /
+        'credentials' /
+        'server.json')
+    file.parent.mkdir(exist_ok=True, parents=True)
+    with open(file, 'w') as file:
+        json.dump(credentials, file, indent=4, sort_keys=True)
+
+    # Maybe wait for process to finish
+    if not detach:
+        process.wait()
+
+    return credentials
+
+
+def destroy(name, credentials):
+    """Shutdown a local server"""
+    try:
+        parent = psutil.Process(credentials['PID'])
+        for child in parent.children(recursive=True):
+            child.kill()
+        parent.kill()
+    except psutil.NoSuchProcess:
+        pass
```

### Comparing `reseval-0.0.3/reseval/stats.py` & `reseval-0.1.0/reseval/stats.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import math
-import scipy.stats
-
-
-###############################################################################
-# Statistical tests
-###############################################################################
-
-
-def binomial(counts):
-    """Performs a two-sided Binomial t-test"""
-    result = scipy.stats.binomtest(counts[0], sum(counts))
-    return {
-        'Sample mean': result.proportion_estimate,
-        'p-value': result.pvalue}
-
-
-def student_ttest(x, y, random_seed=0):
-    """Performs a two-sided Student t-test"""
-    result = scipy.stats.ttest_ind(x, y, random_state=random_seed)
-    return {
-        'Test statistic': result.statistic,
-        'p-value': result.pvalue}
-
-
-def mannwhitney(x, y):
-    """Performs a two-sided Mann-Whitney test"""
-    # Handle no data
-    if len(x) == 0 or len(y) == 0:
-        return {'Test statistic': math.nan, 'p-value': math.nan}
-
-    # Perform test
-    result = scipy.stats.mannwhitneyu(x, y)
-
-    return {
-        'Test statistic': result.statistic,
-        'p-value': result.pvalue}
-
-
-def welchs_ttest(x, y, random_seed=0):
-    """Performs a two-sided Welch's t-test"""
-    result = scipy.stats.ttest_ind(
-        x,
-        y,
-        equal_var=False,
-        random_state=random_seed)
-    return {
-        'Test statistic': result.statistic,
-        'p-value': result.pvalue}
-
-
-def wilcoxon(x, y):
-    """Performs a two-sided Wilcoxon signed-rank test"""
-    # Handle no data
-    if len(x) == 0:
-        return
-
-    # Perform test
-    result = scipy.stats.wilcoxon(x, y)
-
-    return {
-        'Test statistic': result.statistic,
-        'p-value': result.pvalue}
+import math
+import scipy.stats
+
+
+###############################################################################
+# Statistical tests
+###############################################################################
+
+
+def binomial(counts):
+    """Performs a two-sided Binomial t-test"""
+    result = scipy.stats.binomtest(counts[0], sum(counts))
+    return {
+        'Sample mean': result.proportion_estimate,
+        'p-value': result.pvalue}
+
+
+def student_ttest(x, y, random_seed=0):
+    """Performs a two-sided Student t-test"""
+    result = scipy.stats.ttest_ind(x, y, random_state=random_seed)
+    return {
+        'Test statistic': result.statistic,
+        'p-value': result.pvalue}
+
+
+def mannwhitney(x, y):
+    """Performs a two-sided Mann-Whitney test"""
+    # Handle no data
+    if len(x) == 0 or len(y) == 0:
+        return {'Test statistic': math.nan, 'p-value': math.nan}
+
+    # Perform test
+    result = scipy.stats.mannwhitneyu(x, y)
+
+    return {
+        'Test statistic': result.statistic,
+        'p-value': result.pvalue}
+
+
+def welchs_ttest(x, y, random_seed=0):
+    """Performs a two-sided Welch's t-test"""
+    result = scipy.stats.ttest_ind(
+        x,
+        y,
+        equal_var=False,
+        random_state=random_seed)
+    return {
+        'Test statistic': result.statistic,
+        'p-value': result.pvalue}
+
+
+def wilcoxon(x, y):
+    """Performs a two-sided Wilcoxon signed-rank test"""
+    # Handle no data
+    if len(x) == 0:
+        return
+
+    # Perform test
+    result = scipy.stats.wilcoxon(x, y)
+
+    return {
+        'Test statistic': result.statistic,
+        'p-value': result.pvalue}
```

### Comparing `reseval-0.0.3/reseval/storage/client.py` & `reseval-0.1.0/reseval/storage/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-import shutil
-from pathlib import Path
-
-import reseval
-
-
-###############################################################################
-# Client file storage management
-###############################################################################
-
-
-def create(config, directory):
-    """Add evaluation files to client storage"""
-    for path in directory.iterdir():
-        upload(config['name'], path)
-
-    # Add listening test files to client storage
-    if 'listening_test' in config:
-        upload(config['name'], reseval.LISTENING_TEST_DIRECTORY)
-
-
-def destroy(config):
-    """Remove all evaluation files in client public directory"""
-    try:
-        for path in reseval.CLIENT_PUBLIC_DIRECTORY.iterdir():
-            if path.name != '.gitkeep':
-                try:
-                    shutil.rmtree(path)
-                except NotADirectoryError:
-                    path.unlink()
-    except FileNotFoundError:
-        pass
-
-
-def upload(name, file_or_directory):
-    """Upload a file or directory to client storage"""
-    destination = reseval.CLIENT_PUBLIC_DIRECTORY / file_or_directory.name
-    reseval.CLIENT_PUBLIC_DIRECTORY.mkdir(exist_ok=True, parents=True)
-
-    # Upload directory
-    if file_or_directory.is_dir():
-        shutil.copytree(file_or_directory, destination)
-
-    # Upload file
-    else:
-        shutil.copyfile(file_or_directory, destination)
-
-    # Return URL
-    return f'/evaluation-files/{file_or_directory}'
+import shutil
+
+import reseval
+
+
+###############################################################################
+# Client file storage management
+###############################################################################
+
+
+def create(config, directory):
+    """Add evaluation files to client storage"""
+    for path in directory.iterdir():
+        upload(config['name'], path)
+
+    # Add listening test files to client storage
+    if 'listening_test' in config:
+        upload(config['name'], reseval.LISTENING_TEST_DIRECTORY)
+
+
+def destroy(name):
+    """Remove all evaluation files in client public directory"""
+    try:
+        for path in reseval.CLIENT_PUBLIC_DIRECTORY.iterdir():
+            if path.name != '.gitkeep':
+                try:
+                    shutil.rmtree(path)
+                except NotADirectoryError:
+                    path.unlink()
+    except FileNotFoundError:
+        pass
+
+
+def upload(name, file_or_directory):
+    """Upload a file or directory to client storage"""
+    destination = reseval.CLIENT_PUBLIC_DIRECTORY / file_or_directory.name
+    reseval.CLIENT_PUBLIC_DIRECTORY.mkdir(exist_ok=True, parents=True)
+
+    # Upload directory
+    if file_or_directory.is_dir():
+        shutil.copytree(file_or_directory, destination)
+
+    # Upload file
+    else:
+        shutil.copyfile(file_or_directory, destination)
+
+    # Return URL
+    return f'/evaluation-files/{file_or_directory.name}'
```

### Comparing `reseval-0.0.3/reseval/storage/core.py` & `reseval-0.1.0/reseval/storage/core.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import reseval
-
-
-###############################################################################
-# Evaluation file storage
-###############################################################################
-
-
-def create(config, directory, local=False):
-    """Create file storage and upload files"""
-    print('Creating storage...')
-
-    # Make sure client public storage doesn't have old evaluation files
-    reseval.storage.client.destroy(config)
-
-    # Create and upload
-    module(config, local).create(config, directory)
-
-
-def destroy(name):
-    """Destroy file storage"""
-    local = reseval.is_local(name)
-    config = reseval.load.config_by_name(name)
-    module(config, local).destroy(config['name'])
-
-
-def upload(name, file_or_directory):
-    """Upload a file or directory to storage"""
-    local = reseval.is_local(name)
-    config = reseval.load.config_by_name(name)
-    return module(config, local).upload(name, file_or_directory)
-
-
-###############################################################################
-# Utilities
-###############################################################################
-
-
-def module(config, local=False):
-    """Get the storage module to use"""
-    if local:
-        return reseval.storage.client
-    storage = config['storage']
-    if storage == 'aws':
-        return reseval.storage.aws
-    raise ValueError(f'Storage method {storage} is not recognized')
+import reseval
+
+
+###############################################################################
+# Evaluation file storage
+###############################################################################
+
+
+def create(config, directory, local=False):
+    """Create file storage and upload files"""
+    print('Creating storage...')
+
+    # Make sure client public storage doesn't have old evaluation files
+    reseval.storage.client.destroy(config)
+
+    # Create and upload
+    module(config, local).create(config, directory)
+
+
+def destroy(name):
+    """Destroy file storage"""
+    local = reseval.is_local(name)
+    config = reseval.load.config_by_name(name)
+    module(config, local).destroy(config['name'])
+
+
+def upload(name, file_or_directory):
+    """Upload a file or directory to storage"""
+    local = reseval.is_local(name)
+    config = reseval.load.config_by_name(name)
+    return module(config, local).upload(name, file_or_directory)
+
+
+###############################################################################
+# Utilities
+###############################################################################
+
+
+def module(config, local=False):
+    """Get the storage module to use"""
+    if local:
+        return reseval.storage.client
+    storage = config['storage']
+    if storage == 'aws':
+        return reseval.storage.aws
+    raise ValueError(f'Storage method {storage} is not recognized')
```

### Comparing `reseval-0.0.3/reseval/test/ab.py` & `reseval-0.1.0/reseval/test/ab.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import reseval
-from .base import Base
-
-
-###############################################################################
-# AB test
-###############################################################################
-
-
-class AB(Base):
-
-    @classmethod
-    def analyze(cls, conditions, responses, random_seed=0):
-        """Perform statistical analysis on evaluation results"""
-        # Get counts of responses for each condition and for each stem
-        condition_counts, stem_counts = cls.counts(conditions, responses)
-
-        # Two-sided Binomial test
-        results = {
-            'binomial': reseval.stats.binomial(
-                [condition_counts[condition] for condition in conditions])}
-
-        # Format results
-        results = {
-            'samples': sum(condition_counts.values()),
-            'conditions': {f'{conditions[0]}-{conditions[1]}': results}}
-
-        return results, stem_counts
-
-    @classmethod
-    def counts(cls, conditions, responses):
-        """Get counts from participant responses"""
-        condition_counts = {cond: 0 for cond in conditions}
-        stem_counts = {
-            stem: {cond: 0 for cond in conditions} for stem in responses}
-        for stem, results in responses.items():
-            for result in results:
-                condition_counts[result] += 1
-                stem_counts[stem][result] += 1
-        return condition_counts, stem_counts
-
-    @classmethod
-    def plot(self, results, file):
-        """Create a plot of the results and save to disk"""
-        reseval.plot.barh(results, file)
+import reseval
+from .base import Base
+
+
+###############################################################################
+# AB test
+###############################################################################
+
+
+class AB(Base):
+
+    @classmethod
+    def analyze(cls, conditions, responses, random_seed=0):
+        """Perform statistical analysis on evaluation results"""
+        # Get counts of responses for each condition and for each stem
+        condition_counts, stem_counts = cls.counts(conditions, responses)
+
+        # Two-sided Binomial test
+        results = {
+            'binomial': reseval.stats.binomial(
+                [condition_counts[condition] for condition in conditions])}
+
+        # Format results
+        results = {
+            'samples': sum(condition_counts.values()),
+            'conditions': {f'{conditions[0]}-{conditions[1]}': results}}
+
+        return results, stem_counts
+
+    @classmethod
+    def counts(cls, conditions, responses):
+        """Get counts from participant responses"""
+        condition_counts = {cond: 0 for cond in conditions}
+        stem_counts = {
+            stem: {cond: 0 for cond in conditions} for stem in responses}
+        for stem, results in responses.items():
+            for result in results:
+                condition_counts[result] += 1
+                stem_counts[stem][result] += 1
+        return condition_counts, stem_counts
+
+    @classmethod
+    def plot(cls, results, file):
+        """Create a plot of the results and save to disk"""
+        reseval.plot.barh(results, file)
```

### Comparing `reseval-0.0.3/reseval/test/abx.py` & `reseval-0.1.0/reseval/test/abx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import reseval
-from .base import Base
-
-
-###############################################################################
-# ABX test
-###############################################################################
-
-
-class ABX(Base):
-
-    @classmethod
-    def analyze(cls, conditions, responses, random_seed=0):
-        """Perform statistical analysis on evaluation results"""
-        conditions = [cond for cond in conditions if cond != 'reference']
-        return reseval.test.AB.analyze(conditions, responses, random_seed)
-
-    @classmethod
-    def plot(self, results, file):
-        """Create a plot of the results and save to disk"""
-        reseval.plot.barh(results, file)
+import reseval
+from .base import Base
+
+
+###############################################################################
+# ABX test
+###############################################################################
+
+
+class ABX(Base):
+
+    @classmethod
+    def analyze(cls, conditions, responses, random_seed=0):
+        """Perform statistical analysis on evaluation results"""
+        conditions = [cond for cond in conditions if cond != 'reference']
+        return reseval.test.AB.analyze(conditions, responses, random_seed)
+
+    @classmethod
+    def plot(cls, results, file):
+        """Create a plot of the results and save to disk"""
+        reseval.plot.barh(results, file)
```

### Comparing `reseval-0.0.3/reseval/test/base.py` & `reseval-0.1.0/reseval/test/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,115 @@
-import os
-import random
-from abc import ABC, abstractmethod
-
-import reseval
-
-
-###############################################################################
-# Abstract base test class
-###############################################################################
-
-
-class Base(ABC):
-
-    def __init__(self, config, directory):
-        self.directory = directory
-        self.random_seed = config['random_seed']
-        self.participants = config['participants']
-        self.samples_per_participant = config['samples_per_participant']
-
-        # Get all files in directory relative to the directory
-        self.files = [
-            file.relative_to(directory)
-            for file in directory.rglob('*') if file.is_file()]
-
-        # Get the set of conditions
-        self.conditions = sorted([
-            path.name for path in directory.iterdir() if path.is_dir()])
-
-    @classmethod
-    @abstractmethod
-    def analyze(cls, conditions, responses, random_seed=0):
-        """Perform statistical analysis on evaluation results"""
-        pass
-
-    def assign(self, random_seed=0):
-        """Randomly assign files to each participant"""
-        # Seed random number generation
-        random.seed(random_seed)
-
-        # Get shuffled files
-        files = [
-            stem.replace("\\", "/") + extension
-            for stem, extension in self.stems_and_extensions()]
-        random.shuffle(files)
-
-        # Assign stems to participants
-        index = 0
-        samples = self.samples_per_participant
-        assignments, residual = [], []
-
-        # We generate more assignments than the expected number of participants
-        # in case participants leave during the test or we extend the test
-        while len(assignments) < 10 * self.participants:
-
-            # Shuffle and reset index whenever we reach the end
-            while index + samples - len(residual) >= len(files):
-                residual.extend(files[index:])
-                random.shuffle(files)
-                index = 0
-
-            # Add assignment
-            end = index + samples - len(residual)
-            assignments.append(residual + files[index:end])
-            index = end
-
-            # Reset residual
-            residual = []
-
-        return assignments
-
-    @classmethod
-    @abstractmethod
-    def plot(self, results, file):
-        """Create a plot of the results and save to disk"""
-        pass
-
-    def response_type(self):
-        """Retrieve the MySQL datatype of a participant response"""
-        # By default, the response type is the name of the winning condition.
-        max_length = max([len(condition) for condition in self.conditions])
-        return f'varchar({max_length})'
-
-    def stems(self):
-        """Retrieve the file stems to be uploaded to the database"""
-        return [stem for stem, _ in self.stems_and_extensions()]
-
-    def stems_and_extensions(self):
-        """Retrieve file stems and extensions to be updated to the database"""
-        cond = sorted([
-            file for file in self.files
-            if file.parts[0] == self.conditions[0]])
-        return [os.path.splitext('/'.join(file.parts[1:])) for file in cond]
-
-    def validate(self):
-        """Perform validation on the directory of files to evaluate"""
-        # Use first condition as reference
-        common = sorted([
-            file for file in self.files
-            if file.parts[0] == self.conditions[0]])
-
-        # All subsequent conditions must match
-        for condition in self.conditions[1:]:
-            files = sorted([
-                file for file in self.files if file.parts[0] == condition])
-
-            # Check lengths
-            if len(files) != len(common):
-                raise reseval.ValidationError()
-
-            # Check file matches
-            for a, b in zip(files, common):
-                if a.parts[1:].join('/') != b.parts[1:].join('/'):
-                    raise reseval.ValidationError()
+import os
+import random
+from abc import ABC, abstractmethod
+
+import reseval
+
+
+###############################################################################
+# Abstract base test class
+###############################################################################
+
+
+class Base(ABC):
+
+    def __init__(self, config, directory):
+        self.directory = directory
+        self.random_seed = config['random_seed']
+        self.participants = config['participants']
+        self.samples_per_participant = config['samples_per_participant']
+
+        # Get all files in directory relative to the directory
+        self.files = [
+            file.relative_to(directory)
+            for file in directory.rglob('*') if file.is_file()]
+
+        # Get the set of conditions
+        self.conditions = sorted([
+            path.name for path in directory.iterdir() if path.is_dir()])
+
+    @classmethod
+    @abstractmethod
+    def analyze(cls, conditions, responses, random_seed=0):
+        """Perform statistical analysis on evaluation results"""
+        pass
+
+    def assign(self, random_seed=0):
+        """Randomly assign files to each participant"""
+        # Seed random number generation
+        random.seed(random_seed)
+
+        # Get shuffled files
+        files = [
+            stem.replace("\\", "/") + extension
+            for stem, extension in self.stems_and_extensions()]
+        random.shuffle(files)
+
+        # Assign stems to participants
+        index = 0
+        samples = self.samples_per_participant
+        assignments, residual = [], []
+
+        # We generate more assignments than the expected number of participants
+        # in case participants leave during the test or we extend the test
+        while len(assignments) < 10 * self.participants:
+
+            # Shuffle and reset index whenever we reach the end
+            while index + samples - len(residual) >= len(files):
+                residual.extend(files[index:])
+                random.shuffle(files)
+                index = 0
+
+            # Add assignment
+            end = index + samples - len(residual)
+            assignments.append(residual + files[index:end])
+            index = end
+
+            # Reset residual
+            residual = []
+
+        return assignments
+
+    @classmethod
+    def plot(cls, results, file):
+        """Create a plot of the results and save to disk"""
+        pass
+
+    def response_type(self):
+        """Retrieve the MySQL datatype of a participant response"""
+        # By default, the response type is the name of the winning condition.
+        max_length = max([len(condition) for condition in self.conditions])
+        return f'varchar({max_length})'
+
+    def stems(self):
+        """Retrieve the file stems to be uploaded to the database"""
+        return [stem for stem, _ in self.stems_and_extensions()]
+
+    def stems_and_extensions(self):
+        """Retrieve file stems and extensions to be updated to the database"""
+        if self.conditions:
+            cond = sorted([
+                file for file in self.files
+                if file.parts[0] == self.conditions[0]])
+            return [os.path.splitext('/'.join(file.parts[1:])) for file in cond]
+        return [(file.stem, file.suffix) for file in self.files]
+
+    def validate(self):
+        """Perform validation on the directory of files to evaluate"""
+        # Use first condition as reference
+        common = sorted([
+            file for file in self.files
+            if file.parts[0] == self.conditions[0]])
+
+        # All subsequent conditions must match
+        for condition in self.conditions[1:]:
+            files = sorted([
+                file for file in self.files if file.parts[0] == condition])
+
+            # Check lengths
+            if len(files) != len(common):
+                raise reseval.ValidationError()
+
+            # Check file matches
+            for a, b in zip(files, common):
+                if a.parts[1:].join('/') != b.parts[1:].join('/'):
+                    raise reseval.ValidationError()
```

### Comparing `reseval-0.0.3/reseval/test/mos.py` & `reseval-0.1.0/reseval/test/mos.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import itertools
-import random
-
-import reseval
-from .base import Base
-
-
-###############################################################################
-# MOS test
-###############################################################################
-
-
-class MOS(Base):
-
-    @classmethod
-    def analyze(cls, conditions, responses, random_seed=0):
-        """Perform statistical analysis on evaluation results"""
-        # Get MOS ratings
-        condition_scores, stem_scores = cls.scores(conditions, responses)
-
-        # Iterate over unique pairs of conditions
-        samples = sum(len(scores) for scores in condition_scores.values())
-        all_results = {'samples': samples, 'conditions': {}}
-        for condition_a, condition_b in itertools.combinations(conditions, 2):
-            results = {}
-
-            # Two-sided t-test assuming equal variance
-            results['student_ttest'] = reseval.stats.student_ttest(
-                condition_scores[condition_a],
-                condition_scores[condition_b],
-                random_seed)
-
-            # Two-sided t-test assuming unequal variance
-            results['welchs_ttest'] = reseval.stats.welchs_ttest(
-                condition_scores[condition_a],
-                condition_scores[condition_b],
-                random_seed)
-
-            # Two-sided Wilcoxon test with no distribution assumptions
-            results['mannwhitney'] = reseval.stats.mannwhitney(
-                condition_scores[condition_a],
-                condition_scores[condition_b])
-
-            all_results['conditions'][f'{condition_a}-{condition_b}'] = results
-
-        return all_results, stem_scores
-
-    @classmethod
-    def plot(self, results, file):
-        """Create a plot of the results and save to disk"""
-        reseval.plot.violin(results, file, range(0, 6))
-
-    def response_type(self):
-        """Retrieve the MySQL datatype of a participant response"""
-        # For MOS, we store the condition of the file presented to the
-        # participant as well as the score given to the file by the participant
-        # (an integer 1-5 inclusive). The format is "<condition>-<score>".
-        max_length = max([len(condition) for condition in self.conditions])
-        return f'varchar({max_length + 2})'
-
-    @classmethod
-    def scores(cls, conditions, responses):
-        """Get scores from participant responses"""
-        condition_scores = {cond: [] for cond in conditions}
-        stem_scores = {
-            stem: {cond: [] for cond in conditions} for stem in responses}
-        for stem, results in responses.items():
-            for result in results:
-                parts = result.split('-')
-                condition, score = '-'.join(parts[:-1]), int(parts[-1])
-                condition_scores[condition].append(score)
-                stem_scores[stem][condition].append(score)
-        return condition_scores, stem_scores
-
-    def assign_conditions(self, random_seed=0):
-        """Randomly assign conditions to each participant"""
-        # Seed random number generation
-        random.seed(random_seed)
-
-        # Get shuffled conditions
-        all_conditions = self.conditions
-        random.shuffle(all_conditions)
-
-        # Assign conditions to participants
-        index = 0
-        samples = self.samples_per_participant
-        assigned_conditions, residual = [], []
-
-        # We generate more conditions than the expected number of participants
-        # in case participants leave during the test or we extend the test
-        while len(assigned_conditions) < 10 * self.participants:
-
-            # Shuffle and reset index whenever we reach the end
-            while index + samples - len(residual) >= len(all_conditions):
-                residual.extend(all_conditions[index:])
-                random.shuffle(all_conditions)
-                index = 0
-
-            # Add conditions
-            end = index + samples - len(residual)
-            assigned_conditions.append(residual + all_conditions[index:end])
-            index = end
-
-            # Reset residual
-            residual = []
-
-        return assigned_conditions
+import itertools
+import random
+
+import reseval
+from .base import Base
+
+
+###############################################################################
+# MOS test
+###############################################################################
+
+
+class MOS(Base):
+
+    @classmethod
+    def analyze(cls, conditions, responses, random_seed=0):
+        """Perform statistical analysis on evaluation results"""
+        # Get MOS ratings
+        condition_scores, stem_scores = cls.scores(conditions, responses)
+
+        # Iterate over unique pairs of conditions
+        samples = sum(len(scores) for scores in condition_scores.values())
+        all_results = {'samples': samples, 'conditions': {}}
+        for condition_a, condition_b in itertools.combinations(conditions, 2):
+            results = {}
+
+            # Two-sided t-test assuming equal variance
+            results['student_ttest'] = reseval.stats.student_ttest(
+                condition_scores[condition_a],
+                condition_scores[condition_b],
+                random_seed)
+
+            # Two-sided t-test assuming unequal variance
+            results['welchs_ttest'] = reseval.stats.welchs_ttest(
+                condition_scores[condition_a],
+                condition_scores[condition_b],
+                random_seed)
+
+            # Two-sided Wilcoxon test with no distribution assumptions
+            results['mannwhitney'] = reseval.stats.mannwhitney(
+                condition_scores[condition_a],
+                condition_scores[condition_b])
+
+            all_results['conditions'][f'{condition_a}-{condition_b}'] = results
+
+        return all_results, stem_scores
+
+    @classmethod
+    def plot(cls, results, file):
+        """Create a plot of the results and save to disk"""
+        reseval.plot.violin(results, file, range(0, 6))
+
+    def response_type(self):
+        """Retrieve the MySQL datatype of a participant response"""
+        # For MOS, we store the condition of the file presented to the
+        # participant as well as the score given to the file by the participant
+        # (an integer 1-5 inclusive). The format is "<condition>-<score>".
+        max_length = max([len(condition) for condition in self.conditions])
+        return f'varchar({max_length + 2})'
+
+    @classmethod
+    def scores(cls, conditions, responses):
+        """Get scores from participant responses"""
+        condition_scores = {cond: [] for cond in conditions}
+        stem_scores = {
+            stem: {cond: [] for cond in conditions} for stem in responses}
+        for stem, results in responses.items():
+            for result in results:
+                parts = result.split('-')
+                condition, score = '-'.join(parts[:-1]), int(parts[-1])
+                condition_scores[condition].append(score)
+                stem_scores[stem][condition].append(score)
+        return condition_scores, stem_scores
+
+    def assign_conditions(self, random_seed=0):
+        """Randomly assign conditions to each participant"""
+        # Seed random number generation
+        random.seed(random_seed)
+
+        # Get shuffled conditions
+        all_conditions = self.conditions
+        random.shuffle(all_conditions)
+
+        # Assign conditions to participants
+        index = 0
+        samples = self.samples_per_participant
+        assigned_conditions, residual = [], []
+
+        # We generate more conditions than the expected number of participants
+        # in case participants leave during the test or we extend the test
+        while len(assigned_conditions) < 10 * self.participants:
+
+            # Shuffle and reset index whenever we reach the end
+            while index + samples - len(residual) >= len(all_conditions):
+                residual.extend(all_conditions[index:])
+                random.shuffle(all_conditions)
+                index = 0
+
+            # Add conditions
+            end = index + samples - len(residual)
+            assigned_conditions.append(residual + all_conditions[index:end])
+            index = end
+
+            # Reset residual
+            residual = []
+
+        return assigned_conditions
```

### Comparing `reseval-0.0.3/reseval/test/mushra.py` & `reseval-0.1.0/reseval/test/mushra.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,74 @@
-import itertools
-
-import reseval
-from .base import Base
-
-
-###############################################################################
-# MUSHRA test
-###############################################################################
-
-
-class MUSHRA(Base):
-
-    @classmethod
-    def analyze(cls, conditions, responses, random_seed=0):
-        """Perform statistical analysis on evaluation results"""
-        import pdb; pdb.set_trace()
-
-        # Get MUSHRA ratings
-        condition_scores, stem_scores = cls.scores(conditions, responses)
-
-        # Iterate over unique pairs of conditions
-        samples = len(condition_scores[conditions[0]])
-        all_results = {'samples': samples, 'conditions': {}}
-        for condition_a, condition_b in itertools.combinations(conditions, 2):
-            results = {}
-
-            # Two-sided t-test assuming equal variance
-            results['student_ttest'] = reseval.stats.student_ttest(
-                condition_scores[condition_a],
-                condition_scores[condition_b],
-                random_seed)
-
-            # Two-sided t-test assuming unequal variance
-            results['welchs_ttest'] = reseval.stats.welchs_ttest(
-                condition_scores[condition_a],
-                condition_scores[condition_b],
-                random_seed)
-
-            # Two-sided Wilcoxon test with no distribution assumptions
-            results['wilcoxon'] = reseval.stats.wilcoxon(
-                condition_scores[condition_a],
-                condition_scores[condition_b])
-
-            all_results['conditions'][f'{condition_a}-{condition_b}'] = results
-
-        return all_results, stem_scores
-
-    @classmethod
-    def plot(self, results, file):
-        """Create a plot of the results and save to disk"""
-        reseval.plot.violin(results, file, range(0, 101, 20))
-
-    def response_type(self):
-        """Retrieve the MySQL datatype of a participant response"""
-        # For the MUSHRA test, the response is a string of concatenated
-        # three-digit numbers, where each number is a value between 000 and
-        # 100, inclusive. For example, if your MUSHRA test has four conditions
-        # and the conditions, in alphabetical order, are given scores 67, 72,
-        # 95, and 23, respectively, the response will be "067072095023".
-        return f'varchar({3 * len(self.conditions)})'
-
-    @classmethod
-    def scores(cls, conditions, responses):
-        """Get scores from participant responses"""
-        condition_scores = {cond: [] for cond in conditions}
-        stem_scores = {
-            stem: {cond: [] for cond in conditions} for stem in responses}
-        for stem, results in responses.items():
-            for result in results:
-                scores = [
-                    int(result[i:i + 3]) for i in range(0, len(result), 3)]
-                for condition, score in zip(sorted(conditions), scores):
-                    condition_scores[condition].append(score)
-                    stem_scores[stem][condition].append(score)
-        return condition_scores, stem_scores
+import itertools
+
+import reseval
+from .base import Base
+
+
+###############################################################################
+# MUSHRA test
+###############################################################################
+
+
+class MUSHRA(Base):
+
+    @classmethod
+    def analyze(cls, conditions, responses, random_seed=0):
+        """Perform statistical analysis on evaluation results"""
+        # Get MUSHRA ratings
+        condition_scores, stem_scores = cls.scores(conditions, responses)
+
+        # Iterate over unique pairs of conditions
+        samples = len(condition_scores[conditions[0]])
+        all_results = {'samples': samples, 'conditions': {}}
+        for condition_a, condition_b in itertools.combinations(conditions, 2):
+            results = {}
+
+            # Two-sided t-test assuming equal variance
+            results['student_ttest'] = reseval.stats.student_ttest(
+                condition_scores[condition_a],
+                condition_scores[condition_b],
+                random_seed)
+
+            # Two-sided t-test assuming unequal variance
+            results['welchs_ttest'] = reseval.stats.welchs_ttest(
+                condition_scores[condition_a],
+                condition_scores[condition_b],
+                random_seed)
+
+            # Two-sided Wilcoxon test with no distribution assumptions
+            results['wilcoxon'] = reseval.stats.wilcoxon(
+                condition_scores[condition_a],
+                condition_scores[condition_b])
+
+            all_results['conditions'][f'{condition_a}-{condition_b}'] = results
+
+        return all_results, stem_scores
+
+    @classmethod
+    def plot(cls, results, file):
+        """Create a plot of the results and save to disk"""
+        reseval.plot.violin(results, file, range(0, 101, 20))
+
+    def response_type(self):
+        """Retrieve the MySQL datatype of a participant response"""
+        # For the MUSHRA test, the response is a string of concatenated
+        # three-digit numbers, where each number is a value between 000 and
+        # 100, inclusive. For example, if your MUSHRA test has four conditions
+        # and the conditions, in alphabetical order, are given scores 67, 72,
+        # 95, and 23, respectively, the response will be "067072095023".
+        return f'varchar({3 * len(self.conditions)})'
+
+    @classmethod
+    def scores(cls, conditions, responses):
+        """Get scores from participant responses"""
+        condition_scores = {cond: [] for cond in conditions}
+        stem_scores = {
+            stem: {cond: [] for cond in conditions} for stem in responses}
+        for stem, results in responses.items():
+            for result in results:
+                scores = [
+                    int(result[i:i + 3]) for i in range(0, len(result), 3)]
+                for condition, score in zip(sorted(conditions), scores):
+                    condition_scores[condition].append(score)
+                    stem_scores[stem][condition].append(score)
+        return condition_scores, stem_scores
```

### Comparing `reseval-0.0.3/reseval.egg-info/PKG-INFO` & `reseval-0.1.0/reseval.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,428 +1,459 @@
-Metadata-Version: 2.1
-Name: reseval
-Version: 0.0.3
-Summary: Reproducible Subjective Evaluation
-Home-page: https://github.com/reseval/reseval
-Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
-Author-email: maxrmorrison@gmail.com
-Keywords: audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Reproducible Subjective Evaluation (ReSEval)
-[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
-[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
-[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
-
-ReSEval is a framework for quickly building subjective evaluations that are
-deployed on crowdworker platforms like
-[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
-A/B, ABX, MOS, and MUSHRA tests on audio, image, text, and video data.
-
-<h3 align="center">
-    While our code is free to use, performing crowdsourced subjective
-    evaluation is not free.<br/>We are not responsible for costs incurred
-    while using our code.
-</h3>
-
-
-### Citation
-
-If you use ReSEval in an academic publication, please cite
-[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
-
-
-### IEEE
-
-M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
-
-
-### BibTex
-
-```
-@inproceedings{morrison2022reproducible,
-    title={Reproducible Subjective Evaluation},
-    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
-    booktitle={ICLR Workshop on ML Evaluation Standards},
-    month={April},
-    year={2022}
-}
-```
-
-
-## Table of contents
-- [Installation](#installation)
-    * [Deploying locally](#deploying-locally)
-- [Configuration](#configuration)
-- [Adding files](#adding-files)
-    * [AB](#ab)
-    * [ABX](#abx)
-    * [MOS](#mos)
-    * [MUSHRA](#mushra)
-- [Credentials](#credentials)
-    * [Heroku](#heroku)
-    * [Amazon Web Services](#amazon-web-services)
-    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
-- [Usage](#usage)
-    * [Command-line interface](#command-line-interface)
-        * [Create](#create)
-        * [Monitor](#monitor)
-        * [Results](#results)
-        * [Pay](#pay)
-        * [Destroy](#destroy)
-        * [Extend](#extend)
-    * [Application programming interface](#application-programming-interface)
-- [Advanced usage](#advanced-usage)
-    * [CLI](#cli)
-    * [API](#api)
-- [Additional monitoring](#additional-monitoring)
-
-
-## Installation
-
-First, install the Python module. ReSEval requires Python 3.9 or higher.
-
-`pip install reseval`
-
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
-
-```
-# Linux or OS X
-sudo npm install -g n
-sudo n 17.4.0
-
-# Windows
-# Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
-```
-
-**Note** - You must restart your terminal after changing versions of node for the change to take effect
-
-### Deploying locally
-
-To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
-and obtain a username and password. The default username is `root`.
-
-Run the following to store the username and password in
-`reseval.CACHE / '.env'`.
-
-```
-python -m reseval.credentials \
-    --mysql_local_user <mysql_user> \
-    --mysql_local_password <mysql_local_password>
-```
-
-The `.env` file is used to set local environment variables and is not pushed to
-GitHub or uploaded to any remote storage.
-
-
-## Configuration
-
-All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
-
-
-## Adding files
-
-The files to be evaluated must be organized in a directory structure according
-to the type of test being run. The directory structures for each test are as
-follows. Examples of valid directories of evaluation files can be found in
-`examples/`.
-
-
-### AB
-
-```
-ab
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### ABX
-
-```
-abx
-└── reference
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-```
-
-
-### MOS
-
-```
-mos
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-### MUSHRA
-
-```
-mushra
-├── <condition-0>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-1>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-2>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-├── <condition-3>
-│   ├── <file-0>
-│   ├── <file-1>
-│   ├── <file-2>
-│   ├── ...
-└── ...
-```
-
-
-## Credentials
-
-API keys are required to use the third-party services that ReSEval depends on.
-These are not required for local development. Do not share these API keys.
-
-
-### Heroku
-
-Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
-
-<p align="center">
-    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
-    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
-</p>
-
-You will also need to enable billing. You can do so [here](https://heroku.com/verify).
-
-
-### Amazon Web Services
-
-Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
-
-<p align="center">
-    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
-    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
-</p>
-
-
-### Amazon Mechanical Turk
-
-Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
-
-
-## Usage
-
-Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
-
-If you are not deploying locally, add your API keys.
-
-```
-python -m reseval.credentials \
-    --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
-    --heroku_api_key <heroku_api_key>
-```
-
- API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
-
-
-### Command-line interface
-
- Arguments for the following command-line interfaces are as follows, unless otherwise specified.
-
-- `<config>` - The configuration file
-- `<directory>` - The directory of evaluation files
-- `<name>` - The name of the evaluation given in the configuration file
-
-
-#### Create
-
-Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
-
-**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
-
-```
-# Local development
-python -m reseval.create <config> <directory> --local
-
-# Remote development
-python -m reseval.create <config> <directory>
-
-# Production
-python -m reseval.create <config> <directory> --production
-```
-
-
-#### Monitor
-
-```
-# Monitor all subjective evaluations
-python -m reseval.monitor
-
-# Monitor one subjective evaluation
-# The name of the evaluation can be found in its configuration file
-python -m reseval.monitor --name <name>
-```
-
-**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
-
-```
-# Update the monitor once every ten seconds
-python -m reseval.monitor --interval 10
-```
-
-
-#### Results
-
-```
-# Get the results of a subjective evaluation.
-# Results are stored in <directory>/<name>.
-# <directory> defaults to the current directory.
-python -m reseval.results <name> --directory <directory>
-```
-
-
-#### Pay
-
-```
-# Pay participants
-python -m reseval.pay <name>
-```
-
-
-#### Destroy
-
-```
-# Destroy the compute resources of a subjective evaluation (e.g., any cloud
-# storage, databases, or servers)
-python -m reseval.destroy <name>
-
-# Destroy a subjective evaluation even if it is still active.
-# Participants who have taken the test so far will be paid.
-python -m reseval.destroy <name> --force
-```
-
-
-#### Extend
-
-```
-# Add <participants> additional participants to a finished evaluation
-python -m reseval.extend <name> <participants>
-```
-
-
-### Application programming interface
-
-Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
-
-
-## Advanced usage
-
-Once you feel comfortable with using ReSEval step-by-step from the
-command-line and after you have added your credentials with
-`reseval.credentials`, you can use the CLI or API to run your evaluation with
-only a single command.
-
-
-### CLI
-
-```
-# Local development
-python -m reseval <config> <directory> --local
-
-# Remote development
-python -m reseval <config> <directory>
-
-# Production
-python -m reseval <config> <directory> --production
-```
-
-
-### API
-
-```
-import reseval
-
-# Local development
-reseval.run(config, directory, local=True)
-
-# Remote development
-reseval.run(config, directory)
-
-# Production
-reseval.run(config, directory, production=True)
-```
-
-
-## Additional monitoring
-
-### Heroku
-
-To monitor, edit, or delete Heroku databases and servers, use the
-[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
-any costs on the
-[billing dashboard](https://dashboard.heroku.com/account/billing).
-
-
-### AWS S3
-
-To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
-[AWS S3 console](https://aws.amazon.com/s3/).
-
-
-### MTurk
-
-HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
-You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
-on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
-at the end of the billing period.
+Metadata-Version: 2.1
+Name: reseval
+Version: 0.1.0
+Summary: Reproducible Subjective Evaluation
+Home-page: https://github.com/reseval/reseval
+Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
+Author-email: maxrmorrison@gmail.com
+Keywords: annotation,audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Reproducible Subjective Evaluation (ReSEval)
+[![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
+[![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
+
+ReSEval is a framework for quickly building subjective evaluation and
+annotation tasks that are deployed on crowdworker platforms like
+[Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
+A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
+
+<h3 align="center">
+    While our code is free to use, performing crowdsourced subjective
+    evaluation is not free.<br/>We are not responsible for costs incurred
+    while using our code.
+</h3>
+
+
+### Citation
+
+If you use ReSEval in an academic publication, please cite
+[our paper](https://www.maxrmorrison.com/pdfs/morrison2022reproducible.pdf).
+
+
+### IEEE
+
+M. Morrison, B. Tang, G. Tan, and B. Pardo, "Reproducible Subjective Evaluation," ICLR Workshop on ML Evaluation Standards, April 2022.
+
+
+### BibTex
+
+```
+@inproceedings{morrison2022reproducible,
+    title={Reproducible Subjective Evaluation},
+    author={Morrison, Max and Tang, Brian and Tan, Gefei and Pardo, Bryan},
+    booktitle={ICLR Workshop on ML Evaluation Standards},
+    month={April},
+    year={2022}
+}
+```
+
+
+## Table of contents
+- [Installation](#installation)
+    * [Deploying locally](#deploying-locally)
+- [Configuration](#configuration)
+- [Adding files](#adding-files)
+    * [AB](#ab)
+    * [ABX](#abx)
+    * [MOS](#mos)
+    * [MUSHRA](#mushra)
+    * [WordSelect](#wordselect)
+- [Credentials](#credentials)
+    * [Heroku](#heroku)
+    * [Amazon Web Services](#amazon-web-services)
+    * [Amazon Mechanical Turk](#amazon-mechanical-turk)
+- [Usage](#usage)
+    * [Command-line interface](#command-line-interface)
+        * [Create](#create)
+        * [Monitor](#monitor)
+        * [Results](#results)
+        * [Pay](#pay)
+        * [Destroy](#destroy)
+        * [Extend](#extend)
+    * [Application programming interface](#application-programming-interface)
+- [Advanced usage](#advanced-usage)
+    * [CLI](#cli)
+    * [API](#api)
+- [Additional monitoring](#additional-monitoring)
+
+
+## Installation
+
+First, install the Python module. ReSEval requires Python 3.9 or higher.
+
+`pip install reseval`
+
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+
+```
+# Linux or OS X
+sudo npm install -g n
+sudo n 17.4.0
+
+# Windows
+# Must be run with administrator privileges
+nvm install 17.4.0
+nvm use 17.4.0
+```
+
+**Note** - You must restart your terminal after changing versions of node for the change to take effect
+
+### Deploying locally
+
+To be able to preview your subjective evaluation locally, you must
+[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+and obtain a username and password. The default username is `root`.
+
+Run the following to store the username and password in
+`reseval.CACHE / '.env'`.
+
+```
+python -m reseval.credentials \
+    --mysql_local_user <mysql_user> \
+    --mysql_local_password <mysql_local_password>
+```
+
+The `.env` file is used to set local environment variables and is not pushed to
+GitHub or uploaded to any remote storage.
+
+
+## Configuration
+
+All configuration is performed in a YAML configuration file. See `examples/*.yaml` for examples and documentation of parameters.
+
+
+## Adding files
+
+The files to be evaluated must be organized in a directory structure according
+to the type of test being run. The directory structures for each test are as
+follows. Examples of valid directories of evaluation files can be found in
+`examples/`.
+
+
+### AB
+
+```
+ab
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### ABX
+
+```
+abx
+└── reference
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+```
+
+
+### MOS
+
+```
+mos
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### MUSHRA
+
+```
+mushra
+├── <condition-0>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-1>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-2>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+├── <condition-3>
+│   ├── <file-0>
+│   ├── <file-1>
+│   ├── <file-2>
+│   ├── ...
+└── ...
+```
+
+
+### WordSelect
+
+```
+wordselect
+├── <file-0>
+├── <words-0>
+├── <file-1>
+├── <words-1>
+├── <file-2>
+├── <words-2>
+├── ...
+```
+
+`<words-x>` is `<file-x>` with `-words.txt` extension.
+
+
+## Credentials
+
+API keys are required to use the third-party services that ReSEval depends on.
+These are not required for local development. Do not share these API keys.
+
+
+### Amazon Web Services
+
+Sign up for an AWS account. Go to `Security Credentials`. Under `Access keys`, click `Create New Access Key`.
+
+<p align="center">
+    <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
+    <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
+</p>
+
+Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
+
+
+### Amazon Mechanical Turk
+
+Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
+
+
+### Heroku (Optional if you don't want to use AWS)
+
+Sign up for a Heroku account. Go to `Account Settings`. At the bottom of the page in the `API Key` section is a `Reveal` button.
+
+<p align="center">
+    <img src="docs/images/heroku-00.png" width="400" alt="Heroku API key instructions">
+    <img src="docs/images/heroku-01.png" width="400" alt="Heroku API key instructions">
+</p>
+
+You will also need to enable billing. You can do so [here](https://heroku.com/verify).
+
+
+## Usage
+
+Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
+
+If you are not deploying locally, add your API keys.
+
+```
+python -m reseval.credentials \
+    --aws_api_key <aws_api_key> \
+    --aws_api_secret_key <aws_api_secret_key> \
+    --heroku_api_key <heroku_api_key>
+```
+
+ API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
+
+
+### Command-line interface
+
+ Arguments for the following command-line interfaces are as follows, unless otherwise specified.
+
+- `<config>` - The configuration file
+- `<directory>` - The directory of evaluation files
+- `<name>` - The name of the evaluation given in the configuration file
+
+
+#### Create
+
+Create a subjective evaluation either locally, in remote development mode (e.g., MTurk Sandbox), or in production mode.
+
+**Note** - `reseval.create` is not currently thread-safe. Wait until the first call has finished before calling it again. See [this GitHub issue](https://github.com/reseval/reseval/issues/5).
+
+```
+# Local development
+python -m reseval.create <config> <directory> --local
+
+# Remote development
+python -m reseval.create <config> <directory>
+
+# Production
+python -m reseval.create <config> <directory> --production
+```
+
+
+#### Monitor
+
+```
+# Monitor all subjective evaluations
+python -m reseval.monitor
+
+# Monitor one subjective evaluation
+# The name of the evaluation can be found in its configuration file
+python -m reseval.monitor --name <name>
+```
+
+**Note** - By default, the monitor updates once every minute. You can update the monitor more or less often by providing an update interval in seconds.
+
+```
+# Update the monitor once every ten seconds
+python -m reseval.monitor --interval 10
+```
+
+
+#### Results
+
+```
+# Get the results of a subjective evaluation.
+# Results are stored in <directory>/<name>.
+# <directory> defaults to the current directory.
+python -m reseval.results <name> --directory <directory>
+```
+
+
+#### Pay
+
+```
+# Pay participants
+python -m reseval.pay <name>
+```
+
+
+#### Destroy
+
+```
+# Destroy the compute resources of a subjective evaluation (e.g., any cloud
+# storage, databases, or servers)
+python -m reseval.destroy <name>
+
+# Destroy a subjective evaluation even if it is still active.
+# Participants who have taken the test so far will be paid.
+python -m reseval.destroy <name> --force
+```
+
+
+#### Extend
+
+```
+# Add <participants> additional participants to a finished evaluation
+python -m reseval.extend <name> <participants>
+```
+
+
+### Application programming interface
+
+Documentation for our API can be found [here](https://reseval.github.io/reseval/html/index.html).
+
+
+## Advanced usage
+
+Once you feel comfortable with using ReSEval step-by-step from the
+command-line and after you have added your credentials with
+`reseval.credentials`, you can use the CLI or API to run your evaluation with
+only a single command.
+
+
+### CLI
+
+```
+# Local development
+python -m reseval <config> <directory> --local
+
+# Remote development
+python -m reseval <config> <directory>
+
+# Production
+python -m reseval <config> <directory> --production
+```
+
+
+### API
+
+```
+import reseval
+
+# Local development
+reseval.run(config, directory, local=True)
+
+# Remote development
+reseval.run(config, directory)
+
+# Production
+reseval.run(config, directory, production=True)
+```
+
+
+## Additional monitoring
+
+### AWS S3
+
+To monitor, edit, or delete AWS S3 storage buckets, or see any costs, use the
+[AWS S3 console](https://s3.console.aws.amazon.com/s3).
+
+
+### AWS Elastic Beanstalk
+
+To monitor, edit, or delete the server compute, use the
+[AWS Elastic Beanstalk console](https://console.aws.amazon.com/elasticbeanstalk).
+
+
+### AWS Relational Database Service
+
+To monitor, edit, or delete the database, use the
+[AWS RDS console](https://console.aws.amazon.com/rds).
+
+
+### MTurk
+
+HITs not created on the MTurk dashboard are not visible on the MTurk dashboard.
+You can use the MTurk CLI to monitor, edit, or delete HITs. MTurk costs appear
+on the [AWS billing dashboard](https://console.aws.amazon.com/billing/home)
+at the end of the billing period.
+
+
+### Heroku
+
+To monitor, edit, or delete Heroku databases and servers, use the
+[Heroku application dashboard](https://dashboard.heroku.com/apps). You can see
+any costs on the
+[billing dashboard](https://dashboard.heroku.com/account/billing).
```

### Comparing `reseval-0.0.3/reseval.egg-info/SOURCES.txt` & `reseval-0.1.0/reseval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 reseval.egg-info/requires.txt
 reseval.egg-info/top_level.txt
 reseval/app/__init__.py
 reseval/app/heroku.py
 reseval/assets/Procfile
 reseval/assets/package-lock.json
 reseval/assets/package.json
-reseval/assets/policy.json
 reseval/assets/server.ts
 reseval/assets/survey.xml
 reseval/assets/tsconfig.json
 reseval/assets/client/package-lock.json
 reseval/assets/client/package.json
 reseval/assets/client/static.json
 reseval/assets/client/public/favicon.ico
@@ -42,14 +41,15 @@
 reseval/assets/client/src/components/Markdown.js
 reseval/assets/client/src/components/Media.js
 reseval/assets/client/src/components/MediaRadioButtonGroup.js
 reseval/assets/client/src/components/MediaSliderGroup.js
 reseval/assets/client/src/components/RadioButtonGroup.js
 reseval/assets/client/src/components/Text.js
 reseval/assets/client/src/components/Video.js
+reseval/assets/client/src/components/WordSelection.js
 reseval/assets/client/src/css/components.css
 reseval/assets/client/src/css/index.css
 reseval/assets/client/src/json/.gitkeep
 reseval/assets/client/src/pages/EndPage.js
 reseval/assets/client/src/pages/FeedbackPage.js
 reseval/assets/client/src/pages/QualificationPage.js
 reseval/assets/client/src/pages/TaskPage.js
@@ -58,14 +58,15 @@
 reseval/assets/client/src/questions/ListeningTest.js
 reseval/assets/client/src/questions/MultipleChoice.js
 reseval/assets/client/src/questions/Question.js
 reseval/assets/client/src/test/AB.js
 reseval/assets/client/src/test/ABX.js
 reseval/assets/client/src/test/MOS.js
 reseval/assets/client/src/test/MUSHRA.js
+reseval/assets/client/src/test/WordSelect.js
 reseval/assets/listening_test/tones4_0.wav
 reseval/assets/listening_test/tones4_1.wav
 reseval/assets/listening_test/tones4_2.wav
 reseval/assets/listening_test/tones4_3.wav
 reseval/assets/listening_test/tones5_0.wav
 reseval/assets/listening_test/tones5_1.wav
 reseval/assets/listening_test/tones5_2.wav
@@ -85,15 +86,14 @@
 reseval/assets/server/db/index.ts
 reseval/assets/server/db/queries/conditions.ts
 reseval/assets/server/db/queries/files.ts
 reseval/assets/server/db/queries/participants.ts
 reseval/assets/server/db/queries/responses.ts
 reseval/assets/server/routes/index.ts
 reseval/assets/server/routes/api/conditions.ts
-reseval/assets/server/routes/api/evaluators.ts
 reseval/assets/server/routes/api/files.ts
 reseval/assets/server/routes/api/index.ts
 reseval/assets/server/routes/api/participants.ts
 reseval/assets/server/routes/api/responses.ts
 reseval/convert/__init__.py
 reseval/convert/__main__.py
 reseval/convert/audio.py
@@ -104,14 +104,15 @@
 reseval/credentials/__init__.py
 reseval/credentials/__main__.py
 reseval/credentials/core.py
 reseval/crowdsource/__init__.py
 reseval/crowdsource/core.py
 reseval/crowdsource/mturk.py
 reseval/database/__init__.py
+reseval/database/aws.py
 reseval/database/core.py
 reseval/database/download.py
 reseval/database/heroku.py
 reseval/database/localhost.py
 reseval/destroy/__init__.py
 reseval/destroy/__main__.py
 reseval/destroy/core.py
@@ -124,21 +125,23 @@
 reseval/pay/__init__.py
 reseval/pay/__main__.py
 reseval/pay/core.py
 reseval/results/__init__.py
 reseval/results/__main__.py
 reseval/results/core.py
 reseval/server/__init__.py
+reseval/server/aws.py
 reseval/server/core.py
 reseval/server/heroku.py
 reseval/server/local.py
 reseval/storage/__init__.py
 reseval/storage/aws.py
 reseval/storage/client.py
 reseval/storage/core.py
 reseval/test/__init__.py
 reseval/test/ab.py
 reseval/test/abx.py
 reseval/test/base.py
 reseval/test/core.py
 reseval/test/mos.py
-reseval/test/mushra.py
+reseval/test/mushra.py
+reseval/test/wordselect.py
```

### Comparing `reseval-0.0.3/setup.py` & `reseval-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-from pathlib import Path
-from setuptools import find_packages, setup
-
-
-def long_description():
-    """Generate description to post on PyPi"""
-    with open('README.md', encoding='utf8') as file:
-        return file.read()
-
-
-def package_data():
-    """Get the non-python files that should be included in release"""
-    module_directory = Path(__file__).parent / 'reseval'
-    assets_directory = module_directory / 'assets'
-
-    # Package data should be paths relative to package
-    return {'reseval': [
-        str(path.relative_to(module_directory))
-        for path in assets_directory.rglob('*')]}
-
-
-# Setup
-setup(
-    name='reseval',
-    description='Reproducible Subjective Evaluation',
-    version='0.0.3',
-    author='Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo',
-    author_email='maxrmorrison@gmail.com',
-    url='https://github.com/reseval/reseval',
-    install_requires=[
-        'appdirs>=1.4.4',
-        'boto3>=1.21.3',
-        'matplotlib>=3.5.2',
-        'mysql-connector-python>=8.0.28',
-        'psutil>=5.9.0',
-        'python-dotenv>=0.19.2',
-        'pyyaml>=6.0',
-        'rich>=11.2.0',
-        'scipy>=1.8.0',
-        'xmltodict>=0.12.0',
-        'heroku3>=5.1.4'],
-    packages=find_packages(),
-    package_data=package_data(),
-    long_description=long_description(),
-    long_description_content_type='text/markdown',
-    keywords=[
-        'audio',
-        'ab',
-        'abx',
-        'crowdsourcing',
-        'evaluation',
-        'image',
-        'mos',
-        'mushra',
-        'speech',
-        'subjective'])
+from pathlib import Path
+from setuptools import find_packages, setup
+
+
+def long_description():
+    """Generate description to post on PyPi"""
+    with open('README.md', encoding='utf8') as file:
+        return file.read()
+
+
+def package_data():
+    """Get the non-python files that should be included in release"""
+    module_directory = Path(__file__).parent / 'reseval'
+    assets_directory = module_directory / 'assets'
+
+    # Package data should be paths relative to package
+    return {'reseval': [
+        str(path.relative_to(module_directory))
+        for path in assets_directory.rglob('*')]}
+
+
+# Setup
+setup(
+    name='reseval',
+    description='Reproducible Subjective Evaluation',
+    version='0.1.0',
+    author='Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo',
+    author_email='maxrmorrison@gmail.com',
+    url='https://github.com/reseval/reseval',
+    install_requires=[
+        'appdirs>=1.4.4',
+        'boto3>=1.21.3',
+        'matplotlib>=3.5.2',
+        'mysql-connector-python>=8.0.28',
+        'psutil>=5.9.0',
+        'python-dotenv>=0.19.2',
+        'pyyaml>=6.0',
+        'rich>=11.2.0',
+        'scipy>=1.8.0',
+        'xmltodict>=0.12.0',
+        'heroku3>=5.1.4'],
+    packages=find_packages(),
+    package_data=package_data(),
+    long_description=long_description(),
+    long_description_content_type='text/markdown',
+    keywords=[
+        'annotation',
+        'audio',
+        'ab',
+        'abx',
+        'crowdsourcing',
+        'evaluation',
+        'image',
+        'mos',
+        'mushra',
+        'speech',
+        'subjective'])
```

