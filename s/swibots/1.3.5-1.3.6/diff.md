# Comparing `tmp/swibots-1.3.5.tar.gz` & `tmp/swibots-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.3.5.tar", last modified: Mon Jul 17 15:13:55 2023, max compression
+gzip compressed data, was "swibots-1.3.6.tar", last modified: Thu Jul 20 06:32:24 2023, max compression
```

## Comparing `swibots-1.3.5.tar` & `swibots-1.3.6.tar`

### file list

```diff
@@ -1,237 +1,238 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.288450 swibots-1.3.5/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-17 15:13:55.288450 swibots-1.3.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1538 2023-07-15 16:34:05.000000 swibots-1.3.5/README.md
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2023-07-17 15:13:55.288450 swibots-1.3.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      688 2023-07-17 15:13:45.000000 swibots-1.3.5/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      236 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      140 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2236 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/api_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/auth/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       85 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1220 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/auth_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/auth/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       73 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/controllers/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1518 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/controllers/user_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/auth/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       94 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      650 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/methods/get_me.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      837 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/methods/login.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/auth/models/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       56 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4642 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/auth/models/auth_user.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/bot/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1141 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/bot_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots/api/bot/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       71 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/controllers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1790 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/controllers/bot_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.268450 swibots-1.3.5/swibots/api/bot/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      209 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/methods/delete_bot_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      582 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/methods/get_bot_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      615 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/methods/update_bot_info.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.268450 swibots-1.3.5/swibots/api/bot/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      116 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/models/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      955 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/models/bot_command_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1585 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/bot/models/bot_info.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.268450 swibots-1.3.5/swibots/api/chat/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      107 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5372 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/chat_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.268450 swibots-1.3.5/swibots/api/chat/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/controllers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    22522 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/controllers/message_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.268450 swibots-1.3.5/swibots/api/chat/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      326 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2073 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/callback_query_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2731 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/chat_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2095 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/command_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2103 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/inline_query_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2434 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/events/message_event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/chat/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1709 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      654 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/answer_inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/clear_conversation.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      705 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/delete_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/delete_messages_from_user.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1358 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/download_media.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      750 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/edit_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/edit_message_text.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/flag_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1222 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/methods/forward_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1139 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_channel_chat_history.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      725 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_community_media_files.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      883 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_community_media_files_by_status.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      636 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_flag_messages.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1090 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_group_chat_history.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      649 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_messages.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1102 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_messages_between_users.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      560 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_unread_messages_count.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      785 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/get_user_media_files.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      912 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/methods/reply_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1063 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/methods/reply_message_text.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      880 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/methods/send_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1136 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/methods/send_text.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/chat/models/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      305 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      920 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/group_chat_history.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/chat/models/inline/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      565 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1371 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2533 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1871 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_answer.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      991 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1158 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1273 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1620 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1760 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_video.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      581 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/input_message_content.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline/types.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline_keyboard_button.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      170 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline_keyboard_color.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      146 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline_keyboard_size.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2864 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/chat/models/inline_markup.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13436 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/chat/models/message.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/common/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       44 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/common/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/common/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       46 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/common/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2789 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/common/events/event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/common/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      191 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/common/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      562 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/common/models/embed_inline_field.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3248 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/common/models/embedded_media.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2004 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/common/models/media.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1603 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/common/models/media_upload_request.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1725 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/common/models/user.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.272450 swibots-1.3.5/swibots/api/community/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       90 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6445 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/community_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.276450 swibots-1.3.5/swibots/api/community/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      273 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1005 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/ban_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      978 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/channel_controller.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1867 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/controllers/community_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      576 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/group_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2221 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/permissions_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2126 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/controllers/restrict_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1981 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/rolemember_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1860 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/controllers/roles_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.276450 swibots-1.3.5/swibots/api/community/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      566 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/channel_created_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/channel_deleted_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/channel_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2404 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/events/community_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1383 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/community_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/group_created_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/group_deleted_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/group_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1380 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/member_joined_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1377 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/member_left_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1373 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/events/user_banned_event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.280450 swibots-1.3.5/swibots/api/community/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      719 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/methods/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      450 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/ban_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/create_channel.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      815 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/deduct_xp.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      643 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/get_channel.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      866 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/get_community.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      522 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/methods/get_community_member.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      619 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/get_group.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2946 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/permission.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2195 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/restrict_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2259 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/rolemember.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2222 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/roles.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/unban_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/methods/update_channel.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.280450 swibots-1.3.5/swibots/api/community/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      378 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      733 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/baninfo.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3563 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/channel.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2954 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/community.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2998 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/api/community/models/community_member.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2720 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/group.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1218 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/role.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1464 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/rolemember.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3176 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/api/community/models/rolepermission.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9347 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/app.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.280450 swibots-1.3.5/swibots/base/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      262 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       69 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/rest_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      370 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/rest_request.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      644 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/rest_response.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4261 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/switch_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1180 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/switch_object.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/base/switch_ws_async_client.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4598 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bot_app.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.280450 swibots-1.3.5/swibots/bots/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4646 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/bot.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1646 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/bot_context.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      109 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/constants.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/bots/decorators/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      999 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_callback_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      510 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_channel_created.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_channel_deleted.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      541 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_channel_updated.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      574 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_community_updated.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_group_created.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_group_deleted.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_group_updated.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      537 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_member_joined.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      529 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_member_left.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      503 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_unknown_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      509 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/decorators/on_user_banned.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/bots/filters/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       22 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/filters/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     7785 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/filters/filter.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/bots/handlers/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1300 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1048 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/base_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      985 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/callback_query_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      681 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/channel_created_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      688 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/channel_deleted_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      734 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/channel_updated_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1514 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/command_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/community_updated_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1325 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/event_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      680 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/group_created_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/group_deleted_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/group_updated_handler.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      867 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/inline_query_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      679 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/member_joined_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      674 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/member_left_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      960 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/message_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      885 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/unknown_command_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      670 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/handlers/user_banned_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      285 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/bots/register_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1645 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/config.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1333 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/error.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      854 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/types.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/utils/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       75 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5883 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/rest_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2684 2023-07-17 15:05:23.000000 swibots-1.3.5/swibots/utils/types.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/utils/ws/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       48 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.284450 swibots-1.3.5/swibots/utils/ws/asyncstomp/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      150 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9787 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      980 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.288450 swibots-1.3.5/swibots/utils/ws/common/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      100 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/common/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/common/ws_frame.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      430 2023-07-15 16:34:05.000000 swibots-1.3.5/swibots/utils/ws/common/ws_message.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-17 15:13:55.264450 swibots-1.3.5/swibots.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-17 15:13:55.000000 swibots-1.3.5/swibots.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8326 2023-07-17 15:13:55.000000 swibots-1.3.5/swibots.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-07-17 15:13:55.000000 swibots-1.3.5/swibots.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2023-07-17 15:13:55.000000 swibots-1.3.5/swibots.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2023-07-17 15:13:55.000000 swibots-1.3.5/swibots.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.867862 swibots-1.3.6/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-20 06:32:24.867862 swibots-1.3.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1538 2023-07-15 16:34:05.000000 swibots-1.3.6/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2023-07-20 06:32:24.867862 swibots-1.3.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      809 2023-07-20 06:32:08.000000 swibots-1.3.6/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      236 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      140 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2236 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/api_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/auth/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       85 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1220 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/auth_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/auth/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       73 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/controllers/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1518 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/controllers/user_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/auth/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       94 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      650 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/methods/get_me.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      837 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/methods/login.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/auth/models/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       56 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4642 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/auth/models/auth_user.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/bot/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1141 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/bot_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/bot/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       71 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/controllers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1790 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/controllers/bot_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots/api/bot/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      209 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/methods/delete_bot_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      582 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/methods/get_bot_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      615 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/methods/update_bot_info.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.847862 swibots-1.3.6/swibots/api/bot/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      116 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/models/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      955 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/models/bot_command_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1585 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/bot/models/bot_info.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.847862 swibots-1.3.6/swibots/api/chat/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      107 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5372 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/chat_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.847862 swibots-1.3.6/swibots/api/chat/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/controllers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    22522 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/controllers/message_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.847862 swibots-1.3.6/swibots/api/chat/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      326 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2073 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/callback_query_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2731 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/chat_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2095 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/command_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2103 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/inline_query_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2434 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/events/message_event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/chat/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1709 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      654 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/answer_inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/clear_conversation.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      705 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/delete_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/delete_messages_from_user.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1358 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/download_media.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      750 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/edit_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/edit_message_text.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/flag_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1222 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/methods/forward_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1139 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_channel_chat_history.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      725 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_community_media_files.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      883 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      636 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_flag_messages.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1090 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_group_chat_history.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      649 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_messages.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1102 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_messages_between_users.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      560 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_unread_messages_count.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      785 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/get_user_media_files.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      912 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/methods/reply_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1063 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/methods/reply_message_text.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      880 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/methods/send_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1136 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/methods/send_text.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/chat/models/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      305 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      920 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/group_chat_history.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/chat/models/inline/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      565 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1371 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2533 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1871 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_answer.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      991 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1158 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1273 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1620 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1760 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_video.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      581 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/input_message_content.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline/types.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline_keyboard_button.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      170 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline_keyboard_color.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      146 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline_keyboard_size.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2864 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/chat/models/inline_markup.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13436 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/chat/models/message.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/common/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       44 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/common/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/common/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       46 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/common/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2922 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/common/events/event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.851862 swibots-1.3.6/swibots/api/common/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      191 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/common/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      562 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/common/models/embed_inline_field.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3248 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/common/models/embedded_media.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2004 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/common/models/media.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1603 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/common/models/media_upload_request.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1725 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/common/models/user.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.855862 swibots-1.3.6/swibots/api/community/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       90 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6693 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/community_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.855862 swibots-1.3.6/swibots/api/community/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      273 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1005 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/ban_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      978 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/channel_controller.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1867 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/community/controllers/community_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      576 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/group_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2221 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/permissions_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1633 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/controllers/restrict_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1981 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/rolemember_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1860 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/controllers/roles_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.855862 swibots-1.3.6/swibots/api/community/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      566 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/channel_created_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/channel_deleted_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/channel_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2404 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/community/events/community_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1383 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/community_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/group_created_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/group_deleted_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/group_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1380 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/member_joined_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1377 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/member_left_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1373 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/events/user_banned_event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.859862 swibots-1.3.6/swibots/api/community/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      765 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/methods/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      450 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/ban_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/create_channel.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      815 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/deduct_xp.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      643 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/get_channel.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      866 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/get_community.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      522 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/community/methods/get_community_member.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      619 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/get_group.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2946 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/permission.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2418 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/methods/restrict_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2259 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/rolemember.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2222 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/roles.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/unban_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/methods/update_channel.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.859862 swibots-1.3.6/swibots/api/community/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      439 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      733 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/baninfo.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3563 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/channel.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2954 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/community.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2998 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/api/community/models/community_member.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2720 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/group.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1460 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/api/community/models/restricteduser.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1218 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/role.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1464 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/rolemember.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3176 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/api/community/models/rolepermission.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9347 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/app.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.859862 swibots-1.3.6/swibots/base/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      262 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       69 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/rest_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      370 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/rest_request.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      644 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/rest_response.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4261 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/switch_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1180 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/switch_object.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/base/switch_ws_async_client.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4598 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bot_app.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.859862 swibots-1.3.6/swibots/bots/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4646 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/bot.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1646 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/bot_context.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      109 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/constants.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.863862 swibots-1.3.6/swibots/bots/decorators/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      999 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_callback_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      510 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_channel_created.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_channel_deleted.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      541 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_channel_updated.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      574 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_community_updated.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_group_created.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_group_deleted.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_group_updated.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      537 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_member_joined.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      529 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_member_left.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      503 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_unknown_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      509 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/decorators/on_user_banned.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.863862 swibots-1.3.6/swibots/bots/filters/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       22 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/filters/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     7785 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/filters/filter.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.863862 swibots-1.3.6/swibots/bots/handlers/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1300 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1048 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/base_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      985 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/callback_query_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      681 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/channel_created_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      688 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/channel_deleted_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      734 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/channel_updated_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1514 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/command_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/community_updated_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1325 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/event_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      680 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/group_created_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/group_deleted_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      867 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/inline_query_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      679 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/member_joined_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      674 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/member_left_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      960 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/message_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      885 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/unknown_command_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      670 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/handlers/user_banned_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      285 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/bots/register_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1645 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/config.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1333 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/error.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      973 2023-07-20 06:32:08.000000 swibots-1.3.6/swibots/types.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.863862 swibots-1.3.6/swibots/utils/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       75 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5883 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/rest_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2684 2023-07-17 15:05:23.000000 swibots-1.3.6/swibots/utils/types.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.863862 swibots-1.3.6/swibots/utils/ws/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       48 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.867862 swibots-1.3.6/swibots/utils/ws/asyncstomp/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      150 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9787 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      980 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.867862 swibots-1.3.6/swibots/utils/ws/common/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      100 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/common/ws_frame.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      430 2023-07-15 16:34:05.000000 swibots-1.3.6/swibots/utils/ws/common/ws_message.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 06:32:24.843862 swibots-1.3.6/swibots.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-20 06:32:24.000000 swibots-1.3.6/swibots.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8373 2023-07-20 06:32:24.000000 swibots-1.3.6/swibots.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-07-20 06:32:24.000000 swibots-1.3.6/swibots.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2023-07-20 06:32:24.000000 swibots-1.3.6/swibots.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2023-07-20 06:32:24.000000 swibots-1.3.6/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.3.5/PKG-INFO` & `swibots-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.5
+Version: 1.3.6
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.5/README.md` & `swibots-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/setup.py` & `swibots-1.3.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 
-requires = ['httpx==0.23.3', 'websockets==10.4']
+try:
+    with open("requirements.txt", encoding="utf-8") as r:
+        requires = [i.strip() for i in r]
+except:
+        requires = ["httpx==0.23.3", "websockets==10.4"]
 
 try:
     import pypandoc
 
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.3.5",
+    version="1.3.6",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.3.5/swibots/api/api_client.py` & `swibots-1.3.6/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/auth/auth_client.py` & `swibots-1.3.6/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/auth/controllers/user_controller.py` & `swibots-1.3.6/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/auth/methods/get_me.py` & `swibots-1.3.6/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/auth/methods/login.py` & `swibots-1.3.6/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/auth/models/auth_user.py` & `swibots-1.3.6/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/bot_client.py` & `swibots-1.3.6/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.3.6/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.3.6/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.3.6/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.3.6/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/models/bot_command_info.py` & `swibots-1.3.6/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/bot/models/bot_info.py` & `swibots-1.3.6/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/chat_client.py` & `swibots-1.3.6/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/controllers/message_controller.py` & `swibots-1.3.6/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/events/callback_query_event.py` & `swibots-1.3.6/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/events/chat_event.py` & `swibots-1.3.6/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/events/command_event.py` & `swibots-1.3.6/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/events/inline_query_event.py` & `swibots-1.3.6/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/events/message_event.py` & `swibots-1.3.6/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/__init__.py` & `swibots-1.3.6/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.3.6/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.3.6/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/delete_message.py` & `swibots-1.3.6/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.3.6/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/download_media.py` & `swibots-1.3.6/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/edit_message.py` & `swibots-1.3.6/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.3.6/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/flag_message.py` & `swibots-1.3.6/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/forward_message.py` & `swibots-1.3.6/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.3.6/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.3.6/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.3.6/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.3.6/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.3.6/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_message.py` & `swibots-1.3.6/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_messages.py` & `swibots-1.3.6/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.3.6/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.3.6/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.3.6/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/reply_message.py` & `swibots-1.3.6/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.3.6/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/send_message.py` & `swibots-1.3.6/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/methods/send_text.py` & `swibots-1.3.6/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/group_chat_history.py` & `swibots-1.3.6/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/__init__.py` & `swibots-1.3.6/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.3.6/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.3.6/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.3.6/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.3.6/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/inline_markup.py` & `swibots-1.3.6/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/chat/models/message.py` & `swibots-1.3.6/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/common/events/event.py` & `swibots-1.3.6/swibots/api/common/events/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,24 +38,28 @@
 
     def from_json(self, data: swibots.JSONDict) -> "Event":
         if data is not None:
             details = data.get("details") or {}
             self.type = swibots.EventType(data.get("type"))
             self.action_by_id = data.get("actionById")
             self.action_by = swibots.User.build_from_json(
-                data.get("actionBy"), self.app)
+                data.get("actionBy"), self.app
+            )
             self.community_id = details.get("communityId")
             self.community = swibots.Community.build_from_json(
-                details.get("community"), self.app)
+                details.get("community"), self.app
+            )
+            if not self.community_id and self.community:
+                self.community_id = self.community.id
             self.group_id = details.get("groupId")
-            self.group = swibots.Group.build_from_json(
-                details.get("group"), self.app)
+            self.group = swibots.Group.build_from_json(details.get("group"), self.app)
             self.channel_id = details.get("channelId")
             self.channel = swibots.Channel.build_from_json(
-                details.get("channel"), self.app)
+                details.get("channel"), self.app
+            )
             self.data = details
         return self
 
     def to_json(self) -> swibots.JSONDict:
         return {
             "type": self.type,
             "details": self.data,
```

### Comparing `swibots-1.3.5/swibots/api/common/models/embed_inline_field.py` & `swibots-1.3.6/swibots/api/common/models/embed_inline_field.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/common/models/embedded_media.py` & `swibots-1.3.6/swibots/api/common/models/embedded_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/common/models/media.py` & `swibots-1.3.6/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/common/models/media_upload_request.py` & `swibots-1.3.6/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/common/models/user.py` & `swibots-1.3.6/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/community_client.py` & `swibots-1.3.6/swibots/api/community/community_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from swibots.api.auth.models.auth_user import AuthUser
 from swibots.api.community.events import *
 from swibots.base import SwitchRestClient, SwitchWSAsyncClient
 from swibots.config import get_config
 from swibots.error import SwitchError
+from logging import getLogger
 from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
 from swibots.utils.ws.common.ws_message import WsMessage
 from swibots.types import EventType
 from .controllers import (
     ChannelController,
     GroupController,
     CommunityController,
@@ -15,14 +16,16 @@
     PermissionController,
     RoleMemberController,
     RestrictController,
     BanController
 )
 import swibots
 
+Logger = getLogger(__name__)
+
 
 class CommunityClient(SwitchRestClient):
     def __init__(
         self,
         app: "swibots.App" = None,
         base_url: str = None,
         ws_url: str = None,
@@ -111,17 +114,23 @@
         if callback is None:
             raise SwitchError("Callback is not set")
         return await self.ws.subscribe(endpoint, callback=callback)
 
     async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
         subscription = await self.ws.subscribe(
             "/user/queue/events",
-            callback=lambda event: callback(self._parse_event(event)) if callback else None,
+            callback=lambda event: callback(self.__parseEvent(event)),
         )
         return subscription
+    
+    def __parseEvent(self, raw_message: WsMessage) -> CommunityEvent | None:
+        try:
+            return self._parse_event(raw_message)
+        except Exception as er:
+            Logger.exception(er)
 
     def _parse_event(self, raw_message: WsMessage) -> CommunityEvent:
         json_data = json.loads(raw_message.body)
         type = json_data.get("type", "COMMUNITY")
         evt = None
         if type == EventType.COMMUNITY_CHANNEL_CREATE.value:
             evt = self.build_object(ChannelCreatedEvent, json_data)
```

### Comparing `swibots-1.3.5/swibots/api/community/controllers/ban_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/ban_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/channel_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/community_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/group_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/permissions_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/permissions_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/rolemember_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/rolemember_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/controllers/roles_controller.py` & `swibots-1.3.6/swibots/api/community/controllers/roles_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/__init__.py` & `swibots-1.3.6/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/channel_created_event.py` & `swibots-1.3.6/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.3.6/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/channel_updated_event.py` & `swibots-1.3.6/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/community_event.py` & `swibots-1.3.6/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/community_updated_event.py` & `swibots-1.3.6/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/group_created_event.py` & `swibots-1.3.6/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/group_deleted_event.py` & `swibots-1.3.6/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/group_updated_event.py` & `swibots-1.3.6/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/member_joined_event.py` & `swibots-1.3.6/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/member_left_event.py` & `swibots-1.3.6/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/events/user_banned_event.py` & `swibots-1.3.6/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/__init__.py` & `swibots-1.3.6/swibots/api/community/methods/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from .rolemember import RoleMemberMethods
 from .ban_user import BanUser
 from .unban_user import UnbanUser
 from .create_channel import CreateChannel
 from .update_channel import UpdateChannel
 from .restrict_user import RestrictUser
 from .get_community_member import GetCommunityMember
+from .deduct_xp import DeductXP
 
 class CommunityMethods(
     GetChannel,
     GetCommunity,
     GetCommunityMember,
     GetGroup,
     RoleMethods,
     PermissionMethods,
     RoleMemberMethods,
     BanUser,
     UnbanUser,
     CreateChannel,
     UpdateChannel,
-    RestrictUser
+    RestrictUser,
+    DeductXP
 ):
     pass
```

### Comparing `swibots-1.3.5/swibots/api/community/methods/create_channel.py` & `swibots-1.3.6/swibots/api/community/methods/create_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/deduct_xp.py` & `swibots-1.3.6/swibots/api/community/methods/deduct_xp.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/get_channel.py` & `swibots-1.3.6/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/get_community.py` & `swibots-1.3.6/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/get_community_member.py` & `swibots-1.3.6/swibots/api/community/methods/get_community_member.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/get_group.py` & `swibots-1.3.6/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/permission.py` & `swibots-1.3.6/swibots/api/community/methods/permission.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/restrict_user.py` & `swibots-1.3.6/swibots/api/community/methods/restrict_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,24 @@
     """
 
     async def restrict_user(
         self: "swibots.ApiClient",
         community_id: str,
         restricted: bool,
         user_id: int,
-        until_date: float | datetime,
+        until_date: int = 0,
     ) -> bool:
         """
         Restricts a user in a community.
 
         Args:
             community_id (str): The ID of the community.
             restricted (bool): Whether the user should be restricted.
             user_id (int): The ID of the user to restrict.
-            until_date (float | datetime): The date until which the user should be restricted.
+            until_date (int): The timestamp until which the user should be restricted.
 
         Returns:
             bool: Whether the restriction was successful.
         """
 
         return await self.community_service.restrict.restrict_user(
             community_id=community_id,
@@ -46,25 +46,29 @@
         )
 
     async def update_restricted_user(
         self: "swibots.ApiClient",
         community_id: str,
         restricted: bool,
         user_id: int,
-        until_date: datetime | float,
+        until_date: int = 0,
     ) -> bool:
         """
         Updates the restriction status of a user in a community.
 
         Args:
             community_id (str): The ID of the community.
             restricted (bool): Whether the user should be restricted.
             user_id (int): The ID of the user to restrict.
-            until_date (datetime | float): The date until which the user should be restricted.
+            until_date (float | int): The date until which the user should be restricted.
 
         Returns:
             bool: Whether the restriction update was successful.
         """
 
         return await self.community_service.restrict.update_restricted_user(
             community_id, restricted, user_id, until_date
         )
+
+    async def get_restricted_user(self: "swibots.ApiClient", community_id: str, user_id:int):
+        """get restricted user from community_id and user_id"""
+        return await self.community_service.restrict.get_restricted_user(community_id, user_id)
```

### Comparing `swibots-1.3.5/swibots/api/community/methods/rolemember.py` & `swibots-1.3.6/swibots/api/community/methods/rolemember.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/roles.py` & `swibots-1.3.6/swibots/api/community/methods/roles.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/unban_user.py` & `swibots-1.3.6/swibots/api/community/methods/unban_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/methods/update_channel.py` & `swibots-1.3.6/swibots/api/community/methods/update_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/baninfo.py` & `swibots-1.3.6/swibots/api/community/models/baninfo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/channel.py` & `swibots-1.3.6/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/community.py` & `swibots-1.3.6/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/community_member.py` & `swibots-1.3.6/swibots/api/community/models/community_member.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/group.py` & `swibots-1.3.6/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/role.py` & `swibots-1.3.6/swibots/api/community/models/role.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/rolemember.py` & `swibots-1.3.6/swibots/api/community/models/rolemember.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/api/community/models/rolepermission.py` & `swibots-1.3.6/swibots/api/community/models/rolepermission.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/app.py` & `swibots-1.3.6/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/base/rest_response.py` & `swibots-1.3.6/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/base/switch_client.py` & `swibots-1.3.6/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/base/switch_object.py` & `swibots-1.3.6/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/base/switch_ws_async_client.py` & `swibots-1.3.6/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bot_app.py` & `swibots-1.3.6/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/bot.py` & `swibots-1.3.6/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/bot_context.py` & `swibots-1.3.6/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/__init__.py` & `swibots-1.3.6/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_callback_query.py` & `swibots-1.3.6/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.3.6/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.3.6/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_command.py` & `swibots-1.3.6/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_community_updated.py` & `swibots-1.3.6/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_group_created.py` & `swibots-1.3.6/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.3.6/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_group_updated.py` & `swibots-1.3.6/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_inline_query.py` & `swibots-1.3.6/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_member_joined.py` & `swibots-1.3.6/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_member_left.py` & `swibots-1.3.6/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.3.6/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/filters/filter.py` & `swibots-1.3.6/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/__init__.py` & `swibots-1.3.6/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/base_handler.py` & `swibots-1.3.6/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.3.6/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.3.6/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.3.6/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.3.6/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/command_handler.py` & `swibots-1.3.6/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.3.6/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/event_handler.py` & `swibots-1.3.6/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/group_created_handler.py` & `swibots-1.3.6/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.3.6/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.3.6/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.3.6/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.3.6/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/member_left_handler.py` & `swibots-1.3.6/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/message_handler.py` & `swibots-1.3.6/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.3.6/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.3.6/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/config.py` & `swibots-1.3.6/swibots/config.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/error.py` & `swibots-1.3.6/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/types.py` & `swibots-1.3.6/swibots/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,24 @@
     """Represents the type of a event."""
 
     # Chat
     MESSAGE = "MESSAGE"
     COMMAND = "COMMAND"
     CALLBACK_QUERY = "CALLBACK_QUERY"
     INLINE_QUERY = "INLINE_QUERY"
+
     # Community
     COMMUNITY_CHANNEL_CREATE = "COMMUNITY_CHANNEL_CREATE"
     COMMUNITY_CHANNEL_UPDATE = "COMMUNITY_CHANNEL_UPDATE"
     COMMUNITY_CHANNEL_DELETE = "COMMUNITY_CHANNEL_DELETE"
     COMMUNITY_GROUP_CREATE = "COMMUNITY_GROUP_CREATE"
     COMMUNITY_GROUP_UPDATE = "COMMUNITY_GROUP_UPDATE"
     COMMUNITY_GROUP_DELETE = "COMMUNITY_GROUP_DELETE"
     COMMUNITY_USER_BAN = "COMMUNITY_USER_BAN"
     COMMUNITY_USER_UNBAN = "COMMUNITY_USER_UNBAN"
     COMMUNITY_MEMBER_JOIN = "COMMUNITY_MEMBER_JOIN"
     COMMUNITY_MEMBER_LEAVE = "COMMUNITY_MEMBER_LEAVE"
     COMMUNITY_UPDATE = "COMMUNITY_UPDATE"
     COMMUNITY_DELETE = "COMMUNITY_DELETE"
+
+    COMMUNITY_UNRESTRICT_USER = "COMMUNITY_UN_RESTRICT_USER"
+    COMMUNITY_RESTRICT_USER = "COMMUNITY_RESTRICT_USER"
```

### Comparing `swibots-1.3.5/swibots/utils/rest_client.py` & `swibots-1.3.6/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/utils/types.py` & `swibots-1.3.6/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.3.6/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.3.6/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots/utils/ws/common/ws_frame.py` & `swibots-1.3.6/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.5/swibots.egg-info/PKG-INFO` & `swibots-1.3.6/swibots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.5
+Version: 1.3.6
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.5/swibots.egg-info/SOURCES.txt` & `swibots-1.3.6/swibots.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 swibots/api/community/methods/update_channel.py
 swibots/api/community/models/__init__.py
 swibots/api/community/models/baninfo.py
 swibots/api/community/models/channel.py
 swibots/api/community/models/community.py
 swibots/api/community/models/community_member.py
 swibots/api/community/models/group.py
+swibots/api/community/models/restricteduser.py
 swibots/api/community/models/role.py
 swibots/api/community/models/rolemember.py
 swibots/api/community/models/rolepermission.py
 swibots/base/__init__.py
 swibots/base/rest_controller.py
 swibots/base/rest_request.py
 swibots/base/rest_response.py
```

