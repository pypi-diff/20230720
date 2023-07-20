# Comparing `tmp/neon-skill-user_settings-1.0.1a1.tar.gz` & `tmp/neon-skill-user_settings-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-user_settings-1.0.1a1.tar", last modified: Wed Jul 12 02:14:41 2023, max compression
+gzip compressed data, was "neon-skill-user_settings-1.0.2a1.tar", last modified: Thu Jul 20 20:22:45 2023, max compression
```

## Comparing `neon-skill-user_settings-1.0.1a1.tar` & `neon-skill-user_settings-1.0.2a1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.581867 neon-skill-user_settings-1.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.581867 neon-skill-user_settings-1.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.589867 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/also_change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/birthday_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/birthday_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/birthday_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/birthday_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/change_location_tz.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/date_format_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/date_format_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/dialog_mode_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/dialog_mode_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_already_set_same.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_overwrite.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/email_set_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/error_change_username.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/happy_birthday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/hesitation_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/hesitation_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_change_confirmation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_not_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_not_recognized.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/language_setting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/location_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/location_not_found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/location_uknown_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/location_unknown_online.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_no_username.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_not_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_not_known.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_set_full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/name_set_part.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/only_one_language.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/speech_speed_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/speech_speed_limit.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/speech_speed_normal.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/speech_speed_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/time_format_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/time_format_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/transcription_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/transcription_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/units_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/units_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_at.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_audio.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_faster.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_female.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_first_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_full_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_imperial.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_last_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_limited.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_male.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_metric.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_middle_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_preferred_name.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_primary.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_random.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_secondary.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_slower.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_speak.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_stt.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_text.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_timezone.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_understand.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/dialog/word_username.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.589867 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/language_settings.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/language_stt.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/language_tts.intent
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/when_is_my_birthday.intent
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/where_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/intent/who_am_i.intent
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.589867 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/language.rx
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/name.rx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/place.rx
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/primary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/secondary_tts.rx
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/regex/setting.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/at.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/audio.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/birthday.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/deny.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/dialog_mode.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/dmy.voc
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/dot.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/email.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/faster.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/first_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/full.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/full_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/half.voc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/hesitation.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/imperial.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/language.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/language_settings.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/language_stt.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/language_tts.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/last_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/limited.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/location.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/mdy.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/metric.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/middle_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/my.voc
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/my_name_is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/name.voc
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/no_secondary_language.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/normally.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/permit.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/preferred.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/preferred_name.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/random.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/retention.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/second.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/slower.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/speak_to_me.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/tell_me_my.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/text.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/timezone.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/units.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/username.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/locale/en-us/vocab/ymd.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 02:14:41.000000 neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    77788 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:14:41.593867 neon-skill-user_settings-1.0.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/ui/SYSTEM_InputBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-12 02:14:37.000000 neon-skill-user_settings-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    52846 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.694170 neon-skill-user_settings-1.0.2a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.698170 neon-skill-user_settings-1.0.2a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.710170 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/also_change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/birthday_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/birthday_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/birthday_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/birthday_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/change_location_tz.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/date_format_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/date_format_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/dialog_mode_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/dialog_mode_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_already_set_same.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_overwrite.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/email_set_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/error_change_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/happy_birthday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/hesitation_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/hesitation_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_change_confirmation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_not_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_not_recognized.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/language_setting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/location_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/location_not_found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/location_uknown_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/location_unknown_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_no_username.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_not_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_not_known.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_set_full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/name_set_part.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/only_one_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/speech_speed_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/speech_speed_limit.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/speech_speed_normal.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/speech_speed_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/time_format_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/time_format_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/transcription_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/transcription_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/units_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/units_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_at.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_audio.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_faster.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_female.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_first_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_full_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_imperial.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_last_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_limited.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_male.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_metric.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_middle_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_preferred_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_primary.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_random.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_secondary.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_slower.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_speak.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_stt.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_text.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_timezone.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_understand.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/dialog/word_username.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.710170 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/language_settings.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/language_stt.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/language_tts.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/when_is_my_birthday.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/where_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/intent/who_am_i.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.710170 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/language.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/name.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/place.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/primary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/secondary_tts.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/regex/setting.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.714170 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/at.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/audio.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/birthday.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/deny.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/dialog_mode.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/dmy.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/dot.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/email.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/faster.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/first_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/full.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/full_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/half.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/hesitation.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/imperial.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/language.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/language_settings.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/language_stt.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/language_tts.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/last_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/limited.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/location.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/mdy.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/metric.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/middle_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/my.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/my_name_is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/no_secondary_language.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/normally.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/permit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/preferred.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/preferred_name.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/random.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/retention.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/second.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/slower.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/speak_to_me.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/tell_me_my.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/text.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/timezone.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/units.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/username.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/locale/en-us/vocab/ymd.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 20:22:45.000000 neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    77788 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:22:45.718170 neon-skill-user_settings-1.0.2a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/ui/SYSTEM_InputBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-20 20:22:41.000000 neon-skill-user_settings-1.0.2a1/version.py
```

### Comparing `neon-skill-user_settings-1.0.1a1/LICENSE.md` & `neon-skill-user_settings-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/PKG-INFO` & `neon-skill-user_settings-1.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user_settings
-Version: 1.0.1a1
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-1.0.1a1/README.md` & `neon-skill-user_settings-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/__init__.py` & `neon-skill-user_settings-1.0.2a1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,16 +96,28 @@
         updated_location = message.data.get('location')
         if not updated_location:
             LOG.warning(f"No geolocation returned by plugin")
             return
         from neon_utils.user_utils import apply_local_user_profile_updates
         from neon_utils.configuration_utils import NGIConfig
         user_config = NGIConfig("ngi_user_info")
-        if not all((user_config.get('location', {}).get('lat'),
-                    user_config.get('location', {}).get('lng'))):
+        # default_coords = (
+        #     str(self.config_core.default.get('location',
+        #                                      {}).get('coordinate',
+        #                                              {}).get('latitude')),
+        #     str(self.config_core.default.get('location',
+        #                                      {}).get('coordinate',
+        #                                              {}).get('longitude')))
+        # TODO: Figure out why default config doesn't match real default values
+        default_coords = ("38.971669", "-95.23525")
+        user_coords = (
+            user_config.get('location', {}).get('lat'),
+            user_config.get('location', {}).get('lng')
+        )
+        if not all(user_coords) or user_coords == default_coords:
             LOG.info(f'Updating default user config from ip geolocation')
             new_loc = {
                     'lat': str(updated_location['coordinate']['latitude']),
                     'lon': str(updated_location['coordinate']['longitude']),
                     'city': updated_location['city']['name'],
                     'state': updated_location['city']['state']['name'],
                     'country': updated_location['city']['state']['country']['name'],
@@ -115,14 +127,16 @@
             new_loc['tz'] = name
             new_loc['utc'] = str(round(offset, 1))
             apply_local_user_profile_updates({'location': new_loc}, user_config)
             self._emit_weather_update(message)
         else:
             LOG.debug(f'Ignoring IP location for already defined user location:'
                       f'{user_config["location"]}')
+            LOG.debug(f'default={default_coords}')
+            LOG.debug(f'user={user_coords}')
         # Remove listener after a successful update
         self.remove_event('ovos.ipgeo.update.response')
 
     @property
     def stt_languages(self) -> Optional[set]:
         self._get_supported_languages()
         if not all((self._languages.skills, self._languages.stt)):
```

### Comparing `neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/PKG-INFO` & `neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-user-settings
-Version: 1.0.1a1
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-user_settings
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-user_settings-1.0.1a1/neon_skill_user_settings.egg-info/SOURCES.txt` & `neon-skill-user_settings-1.0.2a1/neon_skill_user_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/setup.py` & `neon-skill-user_settings-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/skill.json` & `neon-skill-user_settings-1.0.2a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/test/test_skill.py` & `neon-skill-user_settings-1.0.2a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/ui/SYSTEM_InputBox.qml` & `neon-skill-user_settings-1.0.2a1/ui/SYSTEM_InputBox.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-user_settings-1.0.1a1/version.py` & `neon-skill-user_settings-1.0.2a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.2a1"
```

