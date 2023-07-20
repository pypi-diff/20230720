# Comparing `tmp/autosrt-1.4.7.tar.gz` & `tmp/autosrt-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.4.7.tar", last modified: Sun Jul 16 11:56:02 2023, max compression
+gzip compressed data, was "autosrt-1.4.8.tar", last modified: Thu Jul 20 11:19:18 2023, max compression
```

## Comparing `autosrt-1.4.7.tar` & `autosrt-1.4.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:56:02.061192 autosrt-1.4.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-07-16 11:56:02.061942 autosrt-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 11:56:01.958885 autosrt-1.4.7/autosrt/
--rw-rw-rw-   0        0        0   168204 2023-07-16 11:52:40.000000 autosrt-1.4.7/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:56:01.992361 autosrt-1.4.7/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 11:56:01.000000 autosrt-1.4.7/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-07-16 11:56:02.064943 autosrt-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:56:02.058195 autosrt-1.4.7/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.7/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.7/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.7/test/test3.py
--rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.7/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:19:18.234128 autosrt-1.4.8/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-07-20 11:19:18.234128 autosrt-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 11:19:18.197457 autosrt-1.4.8/autosrt/
+-rw-rw-rw-   0        0        0   169418 2023-07-20 11:18:26.000000 autosrt-1.4.8/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:19:18.219895 autosrt-1.4.8/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-20 11:19:17.000000 autosrt-1.4.8/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-20 11:19:18.000000 autosrt-1.4.8/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 11:19:17.000000 autosrt-1.4.8/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-20 11:19:17.000000 autosrt-1.4.8/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-20 11:19:17.000000 autosrt-1.4.8/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-20 11:19:17.000000 autosrt-1.4.8/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-20 11:19:18.237126 autosrt-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:19:18.231881 autosrt-1.4.8/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.8/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.8/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.8/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.8/test/test4.py
```

### Comparing `autosrt-1.4.7/LICENSE` & `autosrt-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/PKG-INFO` & `autosrt-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.7
+Version: 1.4.8
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.7/README.md` & `autosrt-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/autosrt/__init__.py` & `autosrt-1.4.8/autosrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
 
-VERSION = "1.4.7"
+VERSION = "1.4.8"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -2997,14 +2997,16 @@
     ffmpeg_src_language_code = None
     ffmpeg_dst_language_code = None
     embedded_media_filepath = None
 
     subtitle_format = args.format
 
     removed_media_filepaths = []
+    processed_list = []
+
 
     # CHECK SUBTITLE STREAM PART IF args.force_recognize == False
     if args.force_recognize == False:
 
         print("CHECKING EXISTING SUBTITLES STREAMS")
         print("===================================")
 
@@ -3016,15 +3018,15 @@
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
                 print(f"Checking '{media_filepath}'")
 
                 media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
                 if media_type == "audio":
-                    print("Audio file won't have subtitles streams, skip checking")
+                    print("Audio file won't has subtitles streams, skip checking")
                     continue
 
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                 subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
                 if subtitle_streams_data and subtitle_streams_data != []:
 
@@ -3085,15 +3087,15 @@
             for media_filepath in media_filepaths:
 
                 print(f"Checking '{media_filepath}'")
 
                 media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
                 if media_type == "audio":
-                    print("Audio file won't have subtitles streams, skip checking")
+                    print("Audio file won't has subtitles streams, skip checking")
                     continue
 
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                 ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
                 subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
                 subtitle_streams_data = subtitle_stream_parser(media_filepath)
@@ -3312,379 +3314,384 @@
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
                 msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
                 print(msg)
                 sys.exit(0)
 
 
-    # SUBTITLES STREAMS REMOVER PART (IF args.force_recognize == True)
-    print("FORCE RECOGNIZE FLAG CHECK")
-    print("==========================")
+    if args.force_recognize == True:
+        # SUBTITLES STREAMS REMOVER PART (IF args.force_recognize == True)
+        print("FORCE RECOGNIZE FLAG CHECK")
+        print("==========================")
 
-    processed_list = []
+        # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to processed with transcribe
+        for media_filepath in media_filepaths:
 
-    # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to processed with transcribe
-    for media_filepath in media_filepaths:
+            print(f"Checking '{media_filepath}'")
 
-        print(f"Checking '{media_filepath}'")
+            media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+            if media_type == "video" and args.force_recognize == True:
 
-        if media_type == "video" and args.force_recognize == True:
+                force_recognize_media_file_format = None
 
-            force_recognize_media_file_format = None
+                base, ext = os.path.splitext(media_filepath)
+                if ext[1:] == "ts":
+                    force_recognize_media_file_format = "mp4"
+                else:
+                    force_recognize_media_file_format = ext[1:]
 
-            base, ext = os.path.splitext(media_filepath)
-            if ext[1:] == "ts":
-                force_recognize_media_file_format = "mp4"
-            else:
-                force_recognize_media_file_format = ext[1:]
+                #print(f"media_filepath = {media_filepath}")
+                subtitle_stream_parser = SubtitleStreamParser()
+                subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                #print(f"subtitle_streams_data = {subtitle_streams_data}")
+                #print(f"subtitle_stream_parser.timed_subtitles_of_index(1) = {subtitle_stream_parser.timed_subtitles_of_index(1)}")
 
-            #print(f"media_filepath = {media_filepath}")
-            subtitle_stream_parser = SubtitleStreamParser()
-            subtitle_streams_data = subtitle_stream_parser(media_filepath)
-            #print(f"subtitle_streams_data = {subtitle_streams_data}")
-            #print(f"subtitle_stream_parser.timed_subtitles_of_index(1) = {subtitle_stream_parser.timed_subtitles_of_index(1)}")
+                if subtitle_streams_data and subtitle_stream_parser.timed_subtitles_of_index(1) != []:
 
-            if subtitle_streams_data and subtitle_stream_parser.timed_subtitles_of_index(1) != []:
+                    tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{force_recognize_media_file_format}"
+                    subtitle_removed_media_filepath = f"{base}.force.recognize.{force_recognize_media_file_format}"
 
-                tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{force_recognize_media_file_format}"
-                subtitle_removed_media_filepath = f"{base}.force.recognize.{force_recognize_media_file_format}"
+                    widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                    subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    tmp_output = subtitle_remover(media_filepath)
+                    pbar.finish()
 
-                widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                tmp_output = subtitle_remover(media_filepath)
-                pbar.finish()
+                    if os.path.isfile(tmp_output):
+                        shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                        os.remove(tmp_output)
 
-                if os.path.isfile(tmp_output):
-                    shutil.copy(tmp_output, subtitle_removed_media_filepath)
-                    os.remove(tmp_output)
+                        processed_list.append(subtitle_removed_media_filepath)
 
-                    processed_list.append(subtitle_removed_media_filepath)
+                    print(f"Subtitles removed {media_type} file saved as   : '{subtitle_removed_media_filepath}'")
 
-                print(f"Subtitles removed {media_type} file saved as   : '{subtitle_removed_media_filepath}'")
+                else:
+                    print("Nothing to remove")
+                    if media_filepath not in processed_list and media_filepath not in removed_media_filepaths:
+                        processed_list.append(media_filepath)
 
             else:
-                print("Nothing to remove")
+                if media_type == "video":
+                    print("force_recognize is false")
+
+                if media_type == "audio":
+                    print(f"'{media_filepath}' is audio file, nothing to remove")
+
                 if media_filepath not in processed_list and media_filepath not in removed_media_filepaths:
                     processed_list.append(media_filepath)
 
-        else:
-            if media_type == "video":
-                print("force_recognize is false")
-
-            if media_type == "audio":
-                print(f"'{media_filepath}' is audio file, nothing to remove")
+            print("")
 
-            if media_filepath not in processed_list and media_filepath not in removed_media_filepaths:
+    if args.force_recognize == False and processed_list == []:
+        for media_filepath in media_filepaths:
+            if media_filepath not in removed_media_filepaths:
                 processed_list.append(media_filepath)
 
-        print("")
 
+    if processed_list:
+        # START THE TRANSCRIBE PROCESS
+        print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RECOGNIZED")
+        print("=========================================================================================================")
 
-    # START THE TRANSCRIBE PROCESS
-    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RECOGNIZED")
-    print("=========================================================================================================")
+        for media_filepath in processed_list:
+            print(f"Processing '{media_filepath}'")
 
-    for media_filepath in processed_list:
-        print(f"Processing '{media_filepath}'")
-
-        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
-
-        try:
-            widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
-            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-            wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
-            wav_filepath, sample_rate = wav_converter(media_filepath)
-            pbar.finish()
+            media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-            region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
-            regions = region_finder(wav_filepath)
+            try:
+                widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+                wav_filepath, sample_rate = wav_converter(media_filepath)
+                pbar.finish()
 
-            converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
-            recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
+                region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+                regions = region_finder(wav_filepath)
 
-            if regions:
-                widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
-                pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
-                extracted_regions = []
-                for i, extracted_region in enumerate(pool.imap(converter, regions)):
-                    extracted_regions.append(extracted_region)
-                    pbar.update(i)
-                pbar.finish()
+                converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+                recognizer = SpeechRecognizer(language=args.src_language, rate=sample_rate, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", error_messages_callback=show_error_messages)
 
-                widgets = ["Performing speech recognition           : ", Percentage(), ' ', Bar(), ' ', ETA()]
-                pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
-                transcripts = []
-                for i, transcript in enumerate(pool.imap(recognizer, extracted_regions)):
-                    transcripts.append(transcript)
-                    pbar.update(i)
-                pbar.finish()
+                if regions:
+                    widgets = ["Converting speech regions to FLAC files : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
+                    extracted_regions = []
+                    for i, extracted_region in enumerate(pool.imap(converter, regions)):
+                        extracted_regions.append(extracted_region)
+                        pbar.update(i)
+                    pbar.finish()
 
-                base, ext = os.path.splitext(media_filepath)
-                src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
-                writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                writer.write(src_subtitle_filepath)
-
-                if do_translate == True:
-                    # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
-                    # NO NEED TO TRANSLATE ALL transcript IN transcripts
-                    # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
-                    # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
-                    timed_subtitles = writer.timed_subtitles
-                    created_regions = []
-                    created_subtitles = []
-                    for entry in timed_subtitles:
-                        created_regions.append(entry[0])
-                        created_subtitles.append(entry[1])
-
-                    prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
-                    widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
-
-                    transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
-
-                    translated_subtitles = []
-                    for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
-                        translated_subtitles.append(translated_subtitle)
+                    widgets = ["Performing speech recognition           : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=len(regions)).start()
+                    transcripts = []
+                    for i, transcript in enumerate(pool.imap(recognizer, extracted_regions)):
+                        transcripts.append(transcript)
                         pbar.update(i)
                     pbar.finish()
 
                     base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
-                    translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
-                    translation_writer.write(dst_subtitle_filepath)
+                    src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
+                    writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                    writer.write(src_subtitle_filepath)
 
-                    print(f"Original subtitles file saved as        : '{src_subtitle_filepath}'")
-                    print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
 
-                    if media_type == "audio":
-                        completed_tasks += 1
-                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
 
-                    elif media_type == "video" and args.embed_src == False and args.embed_dst == False:
-                        completed_tasks += 1
-                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
+                    if do_translate == True:
+                        # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
+                        # NO NEED TO TRANSLATE ALL transcript IN transcripts
+                        # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
+                        # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
+                        timed_subtitles = writer.timed_subtitles
+                        created_regions = []
+                        created_subtitles = []
+                        for entry in timed_subtitles:
+                            created_regions.append(entry[0])
+                            created_subtitles.append(entry[1])
+
+                        prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
+                        widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
+
+                        transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
+
+                        translated_subtitles = []
+                        for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
+                            translated_subtitles.append(translated_subtitle)
+                            pbar.update(i)
+                        pbar.finish()
 
-                elif do_translate == False:
-                    print(f"Subtitles file saved as                 : '{src_subtitle_filepath}'")
+                        base, ext = os.path.splitext(media_filepath)
+                        dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
+                        translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
+                        translation_writer.write(dst_subtitle_filepath)
 
-                    if media_type == "audio":
-                        completed_tasks += 1
-                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
+                        print(f"Original subtitles file saved as        : '{src_subtitle_filepath}'")
+                        print(f"Translated subtitles file saved as      : '{dst_subtitle_filepath}'")
 
-                    elif media_type == "video" and args.embed_src == False:
-                        completed_tasks += 1
-                        #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'video', args.embed_src == False : completed_tasks = {completed_tasks}\n")
+                        if media_type == "audio":
+                            completed_tasks += 1
+                            #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
 
+                        elif media_type == "video" and args.embed_src == False and args.embed_dst == False:
+                            completed_tasks += 1
+                            #print(f"\nmedia_filepath = {media_filepath}, do_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
 
-                # EMBEDDING SUBTITLES FILE
+                    elif do_translate == False:
+                        print(f"Subtitles file saved as                 : '{src_subtitle_filepath}'")
 
-                embedded_media_filepath = None
+                        if media_type == "audio":
+                            completed_tasks += 1
+                            #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'audio' : completed_tasks = {completed_tasks}\n")
 
-                if do_translate == False:
+                        elif media_type == "video" and args.embed_src == False:
+                            completed_tasks += 1
+                            #print(f"\nmedia_filepath = {media_filepath}, do_translate == False, media_type == 'video', args.embed_src == False : completed_tasks = {completed_tasks}\n")
 
-                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-                    if media_type == "audio" and args.embed_src == True:
-                        print("Subtitles can only be embedded into video file, not audio file")
+                    # EMBEDDING SUBTITLES FILE
 
-                    if media_type == "video" and args.embed_src == True:
+                    embedded_media_filepath = None
 
-                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+                    if do_translate == False:
 
-                        base, ext = os.path.splitext(media_filepath)
+                        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-                        if ext[1:] == "ts":
-                            media_format = "mp4"
-                        else:
-                            media_format = ext[1:]
-
-                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
-
-                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        src_tmp_output = subtitle_embedder(media_filepath)
-                        pbar.finish()
+                        if media_type == "audio" and args.embed_src == True:
+                            print("Subtitles can only be embedded into video file, not audio file")
 
-                        if os.path.isfile(src_tmp_output):
-                            shutil.copy(src_tmp_output, embedded_media_filepath)
-                            os.remove(src_tmp_output)
-                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                        if media_type == "video" and args.embed_src == True:
 
-                    if media_type == "video" and args.embed_src == False:
-                        completed_tasks += 1
-                        #print(f"\ndo_translate == False, media_type == 'video' : completed_tasks = {completed_tasks}\n")
+                            ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
+                            base, ext = os.path.splitext(media_filepath)
 
-                elif do_translate == True:
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
 
-                    media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                            embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
-                    if media_type == "audio" and (args.embed_src == True or args.embed_src == True):
-                        print("Subtitles can only be embedded into video file, not audio file")
+                            widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            src_tmp_output = subtitle_embedder(media_filepath)
+                            pbar.finish()
 
-                    if media_type == "video" and args.embed_src == True and args.embed_dst == True:
+                            if os.path.isfile(src_tmp_output):
+                                shutil.copy(src_tmp_output, embedded_media_filepath)
+                                os.remove(src_tmp_output)
+                                print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                                completed_tasks += 1
+                                #print(f"\ndo_translate == False, media_type == 'video', args.embed_src == True: completed_tasks = {completed_tasks}\n")
 
-                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
-                        base, ext = os.path.splitext(media_filepath)
+                    elif do_translate == True:
 
-                        if ext[1:] == "ts":
-                            media_format = "mp4"
-                        else:
-                            media_format = ext[1:]
-
-                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                        src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
-                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
-
-                        '''
-                        # USING FUNCTION
-                        src_tmp_output = embed_subtitle_into_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
-                        if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
-                            src_dst_tmp_output = embed_subtitle_into_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
-                        '''
-
-                        # USING CLASS
-                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        src_tmp_output = subtitle_embedder(media_filepath)
-                        pbar.finish()
+                        media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
 
-                        if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
-                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        if media_type == "audio" and (args.embed_src == True or args.embed_src == True):
+                            print("Subtitles can only be embedded into video file, not audio file")
+
+                        if media_type == "video" and args.embed_src == True and args.embed_dst == True:
+
+                            ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+                            ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+
+                            base, ext = os.path.splitext(media_filepath)
+
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
+
+                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                            src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                            embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{media_format}"
+
+                            '''
+                            # USING FUNCTION
+                            src_tmp_output = embed_subtitle_into_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
+                            if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                                src_dst_tmp_output = embed_subtitle_into_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
+                            '''
+
+                            # USING CLASS
+                            widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            src_dst_tmp_output = subtitle_embedder(src_tmp_output)
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            src_tmp_output = subtitle_embedder(media_filepath)
                             pbar.finish()
 
-                        if os.path.isfile(src_dst_tmp_output):
-                            shutil.copy(src_dst_tmp_output, embedded_media_filepath)
-                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
-                            completed_tasks += 1
-                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
-                        else:
-                            print("Unknown error!")
-
-                        if os.path.isfile(src_dst_tmp_output):
-                            os.remove(src_dst_tmp_output)
-                        if os.path.isfile(src_tmp_output):
-                            os.remove(src_tmp_output)
+                            if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                                widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                src_dst_tmp_output = subtitle_embedder(src_tmp_output)
+                                pbar.finish()
 
-                    elif media_type == "video" and args.embed_src == True and args.embed_dst == False:
+                            if os.path.isfile(src_dst_tmp_output):
+                                shutil.copy(src_dst_tmp_output, embedded_media_filepath)
+                                print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                                completed_tasks += 1
+                                #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
+                            else:
+                                print("Unknown error!")
+
+                            if os.path.isfile(src_dst_tmp_output):
+                                os.remove(src_dst_tmp_output)
+                            if os.path.isfile(src_tmp_output):
+                                os.remove(src_tmp_output)
 
-                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+                        elif media_type == "video" and args.embed_src == True and args.embed_dst == False:
 
-                        base, ext = os.path.splitext(media_filepath)
+                            ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
-                        if ext[1:] == "ts":
-                            media_format = "mp4"
-                        else:
-                            media_format = ext[1:]
-
-                        src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
-                        embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
-
-                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        src_tmp_output = subtitle_embedder(media_filepath)
-                        pbar.finish()
+                            base, ext = os.path.splitext(media_filepath)
 
-                        if os.path.isfile(src_tmp_output):
-                            shutil.copy(src_tmp_output, embedded_media_filepath)
-                            os.remove(src_tmp_embedded_media_filepath)
-                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
-                            completed_tasks += 1
-                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
-                        else:
-                            print("Unknown error!")
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
 
-                    elif media_type == "video" and args.embed_src == False and args.embed_dst == True:
+                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{media_format}"
+                            embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{media_format}"
 
-                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+                            widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            src_tmp_output = subtitle_embedder(media_filepath)
+                            pbar.finish()
 
-                        base, ext = os.path.splitext(media_filepath)
+                            if os.path.isfile(src_tmp_output):
+                                shutil.copy(src_tmp_output, embedded_media_filepath)
+                                os.remove(src_tmp_embedded_media_filepath)
+                                print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                                completed_tasks += 1
+                                #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == True and args.embed_dst == False : completed_tasks = {completed_tasks}\n")
+                            else:
+                                print("Unknown error!")
 
-                        if ext[1:] == "ts":
-                            media_format = "mp4"
-                        else:
-                            media_format = ext[1:]
-
-                        dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
-                        embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
-
-                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        dst_tmp_output = subtitle_embedder(media_filepath)
-                        pbar.finish()
+                        elif media_type == "video" and args.embed_src == False and args.embed_dst == True:
 
-                        if os.path.isfile(dst_tmp_output):
-                            shutil.copy(dst_tmp_output, embedded_media_filepath)
-                            os.remove(dst_tmp_output)
-                            print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
-                            completed_tasks += 1
-                            #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
-                        else:
-                            print("Unknown error!")
+                            ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
-            print('')
+                            base, ext = os.path.splitext(media_filepath)
 
-            #print(f"len(media_filepaths) = {len(media_filepaths)}")
-            #print(f"completed_tasks = {completed_tasks}\n")
+                            if ext[1:] == "ts":
+                                media_format = "mp4"
+                            else:
+                                media_format = ext[1:]
 
-            if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
-                transcribe_end_time = time.time()
-                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
-                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
-                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
-                hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
-                print(msg)
+                            dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{media_format}"
+                            embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{media_format}"
 
-        except KeyboardInterrupt:
-            pbar.finish()
-            pool.terminate()
-            pool.close()
-            pool.join()
-            print("Cancelling all tasks")
+                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            dst_tmp_output = subtitle_embedder(media_filepath)
+                            pbar.finish()
 
-            if sys.platform == "win32":
-                stop_ffmpeg_windows(error_messages_callback=show_error_messages)
-            else:
-                stop_ffmpeg_linux(error_messages_callback=show_error_messages)
+                            if os.path.isfile(dst_tmp_output):
+                                shutil.copy(dst_tmp_output, embedded_media_filepath)
+                                os.remove(dst_tmp_output)
+                                print(f"Subtitles embedded {media_type} file saved as  : '{embedded_media_filepath}'")
+                                completed_tasks += 1
+                                #print(f"\ndo_translate == True, media_type == 'video', args.embed_src == False and args.embed_dst == True : completed_tasks = {completed_tasks}\n")
+                            else:
+                                print("Unknown error!")
 
-            remove_temp_files("flac")
-            remove_temp_files("wav")
-            return 1
+                print('')
 
-        except Exception as e:
-            if not KeyboardInterrupt in str(e):
+            except KeyboardInterrupt:
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
-                print(e)
+                print("Cancelling all tasks")
 
                 if sys.platform == "win32":
                     stop_ffmpeg_windows(error_messages_callback=show_error_messages)
                 else:
                     stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
                 remove_temp_files("flac")
                 remove_temp_files("wav")
                 return 1
 
+            except Exception as e:
+                if not KeyboardInterrupt in str(e):
+                    pbar.finish()
+                    pool.terminate()
+                    pool.close()
+                    pool.join()
+                    print(e)
+
+                    if sys.platform == "win32":
+                        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
+                    else:
+                        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
+
+                    remove_temp_files("flac")
+                    remove_temp_files("wav")
+                    return 1
+
+    #print(f"len(media_filepaths) = {len(media_filepaths)}")
+    #print(f"completed_tasks = {completed_tasks}\n")
+
+    if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
+        transcribe_end_time = time.time()
+        transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+        transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+        transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+        hour, minute, second = transcribe_elapsed_time_str.split(":")
+        msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
+        print(msg)
+
     if pool:
         pool.close()
         pool.join()
         pool = None
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
```

### Comparing `autosrt-1.4.7/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.8/autosrt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.7
+Version: 1.4.8
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.7/setup.py` & `autosrt-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/test/test1.py` & `autosrt-1.4.8/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/test/test2.py` & `autosrt-1.4.8/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/test/test3.py` & `autosrt-1.4.8/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.7/test/test4.py` & `autosrt-1.4.8/test/test4.py`

 * *Files identical despite different names*

