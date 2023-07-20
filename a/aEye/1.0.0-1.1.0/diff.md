# Comparing `tmp/aEye-1.0.0.tar.gz` & `tmp/aEye-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.0.0.tar", last modified: Mon Jul 17 21:44:24 2023, max compression
+gzip compressed data, was "aEye-1.1.0.tar", last modified: Thu Jul 20 16:17:52 2023, max compression
```

## Comparing `aEye-1.0.0.tar` & `aEye-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:44:24.706971 aEye-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 21:44:12.000000 aEye-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-17 21:44:24.706971 aEye-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-07-17 21:44:12.000000 aEye-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:44:24.702971 aEye-1.0.0/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 21:44:12.000000 aEye-1.0.0/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-17 21:44:12.000000 aEye-1.0.0/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-17 21:44:12.000000 aEye-1.0.0/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-07-17 21:44:12.000000 aEye-1.0.0/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-17 21:44:12.000000 aEye-1.0.0/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:44:24.706971 aEye-1.0.0/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-17 21:44:24.000000 aEye-1.0.0/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 21:44:24.000000 aEye-1.0.0/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:44:24.000000 aEye-1.0.0/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 21:44:24.000000 aEye-1.0.0/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 21:44:24.000000 aEye-1.0.0/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:44:24.706971 aEye-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-17 21:44:13.000000 aEye-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:44:24.706971 aEye-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-17 21:44:12.000000 aEye-1.0.0/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:17:38.000000 aEye-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-20 16:17:52.090942 aEye-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-20 16:17:38.000000 aEye-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:17:52.090942 aEye-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 16:17:38.000000 aEye-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-20 16:17:38.000000 aEye-1.1.0/tests/test_extract_metadata.py
```

### Comparing `aEye-1.0.0/LICENSE` & `aEye-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.0.0/PKG-INFO` & `aEye-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -17,25 +17,19 @@
 ```
 ├──  aEye				contains video class and processor class that manage from loading, processing and uploading
 │   ├── video.py
 |   ├── auxiliary.py
 |   ├── extractor.py
 |   ├── labeler.py
 │   ├── auxiliary.py
-│   ├── mediapipe
-│      ├── object_detection.py
-│      ├── visualize.py
-├──  runner_notebooks
-│   ├── leto-demo.ipynb
 ├──  tests				contains unit tests
 │   ├── test_get_meta_data.py
 │   ├── conftest.py
 │   ├── test_data
 │      ├── test_video.mp4
-├── lambda_function.py
 ├── setup.py
 ```
 
 ### **Inital project setup**
 
 1. clone/pull this repo to local machine
 
@@ -68,28 +62,32 @@
 from aEye.extractor import Extractor
 ```
 
 5. Initalize the auxiliary class. This creates a temporary directory for output files 
 
 ```console
 aux = Aux()
+# This class can download and upload videos, as well as executing pending labels
 ```
 
 6. Load the video from the desired bucket and folder.
 
 ```console
 video_list_s3 = aux.load_s3(bucket = 'aeye-data-bucket', prefix = 'input_video/')
 ```
 
 
 7. Initalize the labeler and extractor
 
 ```console
 label = Labeler()
+# This is used to apply labels like 'crop', 'trim', etc to a video object
+
 extract = Extractor()
+# This is used to extract frames as PNG's 
 ```
 
 
 How to process videos using Labeler and Extractor:
 
 The labeler provides multiple actions that can be applied to a video or a list of videos. Each action takes a video or list of videos as its first parameter and returns a modified video or list of videos. 
 To chain multiple labels together, you can pass the output of one process as the input for the next process.
@@ -154,23 +152,30 @@
 
 change_resolution(video_list, desired_res) -> Changes the resolution to a 'standard' resolution.
 
 trim_video_start_end(video_list, start, end) -> Given start and end times in seconds, modified a trimmed down version of the video to the modified file.
 
 trim_into_clips(video_list, interval) -> Splits the video into X second clips, sends all these clips to output folder.
 
-split_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
+trim_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
 
-split_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
+trim_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
 to copy, splits the video to all of the frames within that frame range.
 
 crop_video_section(video_list, start_x, start_y, width, height) -> Create a width x height crop of the input video starting at pixel values"\
 start_x, start_y and sends the smaller video to the modified file.
 
-blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video
+blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video.
+
+set_bitrate(video_list, desired_bitrate) -> Sets the bitrate at which the video will re-encode to.
+
+change_fps(video_list, new_framerate) -> Sets the framerate at which the video will re-encode. Note, reducing the 
+bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
+
+grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
 frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
 specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
@@ -185,15 +190,17 @@
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
 The TRIM_INTO_CLIPS operation must be executed last. It creates multiple output videos from a single input, and these outputs cannot be processed further.
 Here's an example of using the labeler utility to downsize, crop, and trim a video:
 
 
 ```console
 to_process = label.trim_video_start_end(video_list_s3, 1, 9)              #Trims from 1s to 9s
+
 to_process = label.change_resolution(to_process, "720p")                  #Converts to 720p
+
 final_video_list = label.crop_video_section(to_process, 0, 0, 150, 100)   #Creates a 150x100 crop at (0,0)
 ```
 
 
 8. Use auxiliary class to execute and write the videos with labels.
 
 ```console
@@ -235,22 +242,7 @@
 ```
 
 14. Execute all labels and write the output to data/ folder.
 
 ```console
 aux.execute_label_and_write_local(trimmed_local,'data/')
 ```
-
-### **Docker Image Setup**
-
-The docker image is built automatically via github workflow action on every tag push.
-The rough sequence is below:
-
-    1) The workflow action will build a wheel file based on setup.py,
-    2) Then it will create a docker image based on the dockerfile.
-    3) Finally it will push the image to ECR (currently, this will be loaded in ECR: Leto).
-
-Please refer to mp-to-ecr.yml to get the exact sequences of the github workflow action, the dockerfile for the exact content in the docker image and setup.py for the exact built version.
-
-### **Lambda Function**
-
-Please refer to lambda_function.py for the logic of the lambda function.
```

### Comparing `aEye-1.0.0/README.md` & `aEye-1.1.0/aEye.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+Metadata-Version: 2.1
+Name: aEye
+Version: 1.1.0
+Summary: Extensible Video Processing Framework
+Home-page: https://github.com/DISHDevEx/aEye
+Author-email: devex@dish.com
+License: Dish Wireless
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # aEye
 
 Extensible Video Processing Framework with Additional Features Continuously Deployed
 
 ### **Project Structure**
 
 ```
 ├──  aEye				contains video class and processor class that manage from loading, processing and uploading
 │   ├── video.py
 |   ├── auxiliary.py
 |   ├── extractor.py
 |   ├── labeler.py
 │   ├── auxiliary.py
-│   ├── mediapipe
-│      ├── object_detection.py
-│      ├── visualize.py
-├──  runner_notebooks
-│   ├── leto-demo.ipynb
 ├──  tests				contains unit tests
 │   ├── test_get_meta_data.py
 │   ├── conftest.py
 │   ├── test_data
 │      ├── test_video.mp4
-├── lambda_function.py
 ├── setup.py
 ```
 
 ### **Inital project setup**
 
 1. clone/pull this repo to local machine
 
@@ -58,28 +62,32 @@
 from aEye.extractor import Extractor
 ```
 
 5. Initalize the auxiliary class. This creates a temporary directory for output files 
 
 ```console
 aux = Aux()
+# This class can download and upload videos, as well as executing pending labels
 ```
 
 6. Load the video from the desired bucket and folder.
 
 ```console
 video_list_s3 = aux.load_s3(bucket = 'aeye-data-bucket', prefix = 'input_video/')
 ```
 
 
 7. Initalize the labeler and extractor
 
 ```console
 label = Labeler()
+# This is used to apply labels like 'crop', 'trim', etc to a video object
+
 extract = Extractor()
+# This is used to extract frames as PNG's 
 ```
 
 
 How to process videos using Labeler and Extractor:
 
 The labeler provides multiple actions that can be applied to a video or a list of videos. Each action takes a video or list of videos as its first parameter and returns a modified video or list of videos. 
 To chain multiple labels together, you can pass the output of one process as the input for the next process.
@@ -144,23 +152,30 @@
 
 change_resolution(video_list, desired_res) -> Changes the resolution to a 'standard' resolution.
 
 trim_video_start_end(video_list, start, end) -> Given start and end times in seconds, modified a trimmed down version of the video to the modified file.
 
 trim_into_clips(video_list, interval) -> Splits the video into X second clips, sends all these clips to output folder.
 
-split_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
+trim_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
 
-split_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
+trim_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
 to copy, splits the video to all of the frames within that frame range.
 
 crop_video_section(video_list, start_x, start_y, width, height) -> Create a width x height crop of the input video starting at pixel values"\
 start_x, start_y and sends the smaller video to the modified file.
 
-blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video
+blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video.
+
+set_bitrate(video_list, desired_bitrate) -> Sets the bitrate at which the video will re-encode to.
+
+change_fps(video_list, new_framerate) -> Sets the framerate at which the video will re-encode. Note, reducing the 
+bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
+
+grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
 frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
 specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
@@ -175,15 +190,17 @@
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
 The TRIM_INTO_CLIPS operation must be executed last. It creates multiple output videos from a single input, and these outputs cannot be processed further.
 Here's an example of using the labeler utility to downsize, crop, and trim a video:
 
 
 ```console
 to_process = label.trim_video_start_end(video_list_s3, 1, 9)              #Trims from 1s to 9s
+
 to_process = label.change_resolution(to_process, "720p")                  #Converts to 720p
+
 final_video_list = label.crop_video_section(to_process, 0, 0, 150, 100)   #Creates a 150x100 crop at (0,0)
 ```
 
 
 8. Use auxiliary class to execute and write the videos with labels.
 
 ```console
@@ -225,22 +242,7 @@
 ```
 
 14. Execute all labels and write the output to data/ folder.
 
 ```console
 aux.execute_label_and_write_local(trimmed_local,'data/')
 ```
-
-### **Docker Image Setup**
-
-The docker image is built automatically via github workflow action on every tag push.
-The rough sequence is below:
-
-    1) The workflow action will build a wheel file based on setup.py,
-    2) Then it will create a docker image based on the dockerfile.
-    3) Finally it will push the image to ECR (currently, this will be loaded in ECR: Leto).
-
-Please refer to mp-to-ecr.yml to get the exact sequences of the github workflow action, the dockerfile for the exact content in the docker image and setup.py for the exact built version.
-
-### **Lambda Function**
-
-Please refer to lambda_function.py for the logic of the lambda function.
```

### Comparing `aEye-1.0.0/aEye/auxiliary.py` & `aEye-1.1.0/aEye/auxiliary.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 
 from aEye.video import Video
 import boto3
 import tempfile
 import os
 import subprocess
 import logging
-from static_ffmpeg import run
+import static_ffmpeg
 
-#Please comment this out when setting up a docker image.
-#This will fail when we use the docker image in the lambda function on AWS.
-ffmpeg, ffprobe = run.get_or_fetch_platform_executables_else_raise()
 
 class Aux:
     """
     Aux is the class that works as a pipeline to load, write, and upload all video from S3 bucket.
 
     Attributes
     ----------
@@ -28,35 +25,56 @@
             An internal variable for temp folder path.
 
         _local_path: string
             An internal variable for local folder path.
 
 
     Methods
-    -------
+    ---------
         load_s3(bucket, prefix) -> list[Video]:
             Loads in video files as Video classes into a list from S3.
 
         load_local(path) -> list[Video]:
             Loads in video files as Video classes into a list from local machine.
 
-        write() -> None:
-            Execute and run the video's labels and write the video to temp folder.
+        upload_s3(video_list, bucket, prefix) -> None:
+            Uploads the contents of the temp folder to S3. Bucket can be specifed, and the prefix is the path
+            to the folder within that bucket where the output videos should end up.
 
-        execute_label_and_write_local(video_list) -> List[Video]
+        execute_label_and_write_local(video_list) -> List[Video]:
             Super important function to execute any pending labels on video list. This is how the FFmpeg
             command is run, and if further processing is needed, it returns a processed video list.
 
+        clean() -> None:
+            Removes the temp directory and anything within it. Really useful for a debug, and everything
+            should be cleaned up after uploading to S3. (Unless you want to keep the files locally)
+
+        set_local_path(path) -> None:
+            If the local path is not set by the time the video is ready to be uploaded, set the path to the
+            output folder.
+    Examples
+    ---------
+        load_s3(bucket='aeye-data-bucket', prefix='input_video/') -> Loads everything from the aEye data bucket in the input_video
+        directory.
+
+        load_local('/documents/testVid.mp4') -> Loads video directly from the local file location
+
+        upload_s3(modified_video_list, 'aeye-data-bucket', 'output_videos/')
+
+        execute_label_and_write_local(list_of_videos) -> Executes the pending labels for all video objects in the list
+
+        clean() -> Cleans the temp folder
+
+        set_local_path(cur_path) -> sets the local path to whatever you pass it. Unlikely a user will need this
 
     """
 
     def __init__(self):
-
         self._s3 = boto3.client('s3')
-        self._temp_folder = tempfile.mkdtemp(dir="")
+        self._temp_folder = None
         self._local_path = None
 
     def load_s3(self, bucket, prefix):
         """
         This method will load the video files from S3 and return them
         into a list of video classes.
 
@@ -65,15 +83,15 @@
 
         bucket: string
             The bucket name to path into S3 to get the video files.
         prefix: string
             The folder name where the video files belong in the S3 bucket.
 
         Returns
-        -------
+        ----------
 
         video_list: list
             The list of all video files loaded from S3 bucket.
         """
 
         video_list = []
         result = self._s3.list_objects(Bucket=bucket, Prefix=prefix)
@@ -109,16 +127,14 @@
         -------
 
         video_list: list
             The list of all video files loaded from local bucket.
         """
         video_list = []
 
-        # video_list = [Video(file=  path + i, title=i) for i in os.listdir(path) if Video(file=  path + i, title=i)]
-
         if os.path.isdir(path):
             for i in os.listdir(path):
                 new_vid = Video(file=path + i, title=i)
                 new_vid.path = self._temp_folder
                 video_list.append(new_vid)
 
         else:
@@ -147,15 +163,14 @@
             prefix: string
                 The subfolder name that the video list will be uploaded to.
 
         """
 
         s3 = boto3.client('s3')
         for video in video_list:
-            # if video.get_label() != "":
             if not self._local_path:
                 path = self._temp_folder + '/' + video.get_output_title()
             else:
                 path = self._local_path + '/' + video.get_output_title()
             s3.upload_file(path, bucket, prefix + video.get_output_title())
 
         logging.info(f"successfully upload the output files S3 bucket: s3://{bucket}/{prefix}/")
@@ -166,40 +181,40 @@
         This will default write the output video into a temp folder unless the user provide a local path.
 
         Parameters
         ----------
             video_list: list
                 The list of video that needs to be executed and wrote as output files.
 
-            local: string
+            path: string
                 The path to write the output videos to.
 
         """
 
         # If the user prompts this method with a specific path, then this will save it into the internal variable.
         # This will check if there exists an local path internal. If there exists, then we will write video files there.
         if path is None:
-            path = self._local_path if self._local_path else self._temp_folder
-
+            if self._local_path:
+                path = self._local_path
+            else:
+                self._temp_folder = tempfile.mkdtemp(dir="")
+                path = self._temp_folder
         else:
             self.set_local_path(path)
 
         list_video = []
 
         for video in video_list:
-            # This if statement will skip over any untouched videos.
-            # if video.get_label() != "":
-
             if video.out == '':
                 source = video.get_presigned_url()
             else:
                 source = video.out
             if len(video.complex_filter) > 0:
                 video.create_complex_filter(video)
-            command = f"{ffmpeg} -y -i {source} {video.get_label()} {path}/{video.get_output_title()}"
+            command = f"static_ffmpeg -y -i {source} {video.get_label()} {path}/{video.get_output_title()}"
             subprocess.run(command, shell=True)
             logging.info(command)
             # print(command)  # REALLY useful for debug
             new_path = video.get_output_title()
             video.reset_label()
             new_video = Video(f'{path}/{video.get_output_title()}', title=f'{video.get_output_title()}')
             new_video.set_output(f"'{path}/{new_path}'")
@@ -241,8 +256,8 @@
         path : str
             The path to set
 
         Returns
         ----------
 
         """
-        self._local_path = path
+        self._local_path = path
```

### Comparing `aEye-1.0.0/aEye/extractor.py` & `aEye-1.1.0/aEye/extractor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import cv2
 import logging
 import os
 
+
 class Extractor:
     """
     The Extractor class is used for frame extractions using openCV. Any time the methods
     within the Extractor are run, they will instantly execute. To get frames from processed
     videos, use Aux.execute_label_and_write_local and pass the resulting list to the extractor.
 
     Methods
@@ -16,15 +17,25 @@
 
     specific_frame_extractor(video_list, frame) -> List[Video]
         Will extract the frame # that is passed in and store it as a PNG in the temp folder
 
     multiple_frame_extractor(video_list, start_frame, num_frames) -> List[Video]
         Extract the next num_frames after start_frame and send ALL the images to the output folder. This has the
         capacity to create a HUGE amount of images per video, use with caution!
+
+    Examples
+    --------
+
+    frame_at_time_extractor(s3_videos, 10) -> Output images come from timestamp 10s
+
+    specific_frame_extractor(s3_videos, 320) -> Output image comes from frame 320
+
+    multiple_frame_extractor(s3_videos, 634, 10) -> Extract 10 contiguous frames starting from 634
     """
+
     def frame_at_time_extractor(self, video_list, time):
         """
         Given a time in seconds, this will extract the closest frame.
         Img extraction that takes less than half as long as the FFMpeg version.
 
         Parameters
         -------
@@ -37,36 +48,38 @@
 
         Returns
         -------
 
         Returns a list of videos, but creates an image in the output folder
         """
         for video in video_list:
-            if video.label != '':
-                print(f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
-            if video.out != '':
-                file_path = video.out.strip("'")
-            else:
-                file_path = video.get_presigned_url().strip("'")
-            ## Currently, if you try to run the same cv method with an input upstream, it wont work bc it changes the FP
-            ## I would rather have you able to extract processed imgs instead tho. 98% of the time this wont be an issue.
-            print(file_path)
-            cv_video = cv2.VideoCapture(file_path)
-            fps = cv_video.get(cv2.CAP_PROP_FPS)
-            frame_id = int(fps * time)
-            cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame_id)
-            ret, frame = cv_video.read()
-            actual_title = os.path.splitext(video.title)[0]
-            if video.path is None:
-                path = file_path.split('/')[0]
-            else:
-                path = video.path
-            cv2.imwrite(f"{path}/output_cv_extract_frame_at_time_{time}_{actual_title}.png", frame)
-            cv_video.release()
-            logging.info(f"Extracted frame at time {time}")
+            try:
+                assert float(video.get_duration()) >= time >= 0
+                if video.label != '':
+                    logging.error(
+                        f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
+                if video.out != '':
+                    file_path = video.out.strip("'")
+                else:
+                    file_path = video.get_presigned_url().strip("'")
+                cv_video = cv2.VideoCapture(file_path)
+                fps = cv_video.get(cv2.CAP_PROP_FPS)
+                frame_id = int(fps * time)
+                cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame_id)
+                ret, frame = cv_video.read()
+                actual_title = os.path.splitext(video.title)[0]
+                if video.path is None:
+                    path = file_path.split('/')[0]
+                else:
+                    path = video.path
+                cv2.imwrite(f"{path}/output_cv_extract_frame_at_time_{time}_{actual_title}.png", frame)
+                cv_video.release()
+                logging.info(f"Extracted frame at time {time}")
+            except:
+                logging.error(f" Cannot extract frame at time {time} for video {video}")
         return video_list
 
     def specific_frame_extractor(self, video_list, frame):
         """
         OpenCv method to grab a single frame as a PNG. Passed argument frame is the frame that
         will be extracted. (No decimals please)
 
@@ -81,31 +94,36 @@
 
         Returns
         -------
 
         Returns a list of video objects and outputs an image.
         """
         for video in video_list:
-            if video.label != '':
-                print(f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
-            if video.out == '':
-                file_path = video.get_presigned_url().strip("'")
-            else:
-                file_path = video.out.strip("'")
-            cv_video = cv2.VideoCapture(file_path)
-            cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame)
-            ret, output = cv_video.read()
-            actual_title = os.path.splitext(video.title)[0]
-            if video.path is None:
-                path = file_path.split('/')[0]
-            else:
-                path = video.path
-            cv2.imwrite(f"{path}/output_cv_extract_specific_frame_{frame}_{actual_title}.png", output)
-            logging.info(f"Frame #{frame} extracted ")
-            cv_video.release()
+            try:
+                assert int(video.get_num_frames()) >= frame >= 0
+                if video.label != '':
+                    logging.error(
+                        f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
+                if video.out == '':
+                    file_path = video.get_presigned_url().strip("'")
+                else:
+                    file_path = video.out.strip("'")
+                cv_video = cv2.VideoCapture(file_path)
+                cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame)
+                ret, output = cv_video.read()
+                actual_title = os.path.splitext(video.title)[0]
+                if video.path is None:
+                    path = file_path.split('/')[0]
+                else:
+                    path = video.path
+                cv2.imwrite(f"{path}/output_cv_extract_specific_frame_{frame}_{actual_title}.png", output)
+                logging.info(f"Frame #{frame} extracted ")
+                cv_video.release()
+            except:
+                logging.error(f" Cannot extract frame {frame} for video {video}")
         return video_list
 
     def multiple_frame_extractor(self, video_list, start_frame, num_frames):
         """
         Given a start_frame, extract the next num_frames from the video, and store the resulting
         collection of frames in the output folder. num_Frames is the number of frames to be returned
         Has the potential to create like a million images, only use this when you REALLY need a lot
@@ -117,35 +135,43 @@
         video_list  : List[Video]
             List of all video objects loaded for processing.
 
         start_frame : Integer
             Number of the frame at which to start all the frame grabs.
 
         num_frames  : Integer
-            Number of frames to extract. THIS IS THE AMOUNT OF IMAGES PER VIDEO YOU WANT
+            Number of frames to extract. THIS IS THE AMOUNT OF IMAGES PER VIDEO YOU WANT.
             UNLESS YOU NEED A TON OF CONTIGUOUS FRAMES, DO NOT SET THIS TO A HIGH NUMBER.
 
         Returns
         -------
 
         Returns a list of Videos, and many frames are output as PNG's
         """
         for video in video_list:
-            if video.label != '':
-                print(f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
-            if video.out == '':
-                file_path = video.get_presigned_url().strip("'")
-            else:
-                file_path = video.out.strip("'")
-            vid_obj = cv2.VideoCapture(file_path)
-            actual_title = os.path.splitext(video.title)[0]
-            if video.path is None:
-                path = file_path.split('/')[0]
-            else:
-                path = video.path
-            for x in range(num_frames):
-                ret, frame = vid_obj.read()
-                fn = f"{path}/output_extract_many_frames_{start_frame}_{num_frames}_{actual_title}_{x}.png"
-                cv2.imwrite(fn, frame)
-            vid_obj.release()
-            logging.info(f"Extracted {num_frames} from video, saved as PNG's")
-        return video_list
+            try:
+                assert 0 <= start_frame < int(video.get_num_frames()) and int(
+                    start_frame + num_frames) <= int(video.get_num_frames())
+                if video.label != '':
+                    logging.error(
+                        f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
+                if video.out == '':
+                    file_path = video.get_presigned_url().strip("'")
+                else:
+                    file_path = video.out.strip("'")
+                vid_obj = cv2.VideoCapture(file_path)
+                actual_title = os.path.splitext(video.title)[0]
+                if video.path is None:
+                    path = file_path.split('/')[0]
+                else:
+                    path = video.path
+                #  Sets the relative file location
+                for x in range(num_frames):
+                    vid_obj.set(cv2.CAP_PROP_POS_FRAMES, start_frame + x)
+                    ret, frame = vid_obj.read()
+                    fn = f"{path}/output_extract_many_frames_{start_frame}_{num_frames}_{actual_title}_{x}.png"
+                    cv2.imwrite(fn, frame)
+                vid_obj.release()
+                logging.info(f"Extracted {num_frames} from video, saved as PNG's")
+            except:
+                logging.error(f" Cannot extract {num_frames} starting from frame {start_frame}!")
+        return video_list
```

### Comparing `aEye-1.0.0/aEye/labeler.py` & `aEye-1.1.0/aEye/labeler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
-from static_ffmpeg import run
 import math
 
-ffmpeg, ffprobe = run.get_or_fetch_platform_executables_else_raise()
 
 
 class Labeler:
     """
     The Labler class works by applying "labels" to a Video object. These labels are
     FFmpeg commands that will be executed upon the Aux.execute_label_and_write_local command.
     If two simple labels of the same type (trim for example) are applied, only the most recent
-    label will be run. This does not apply for multiple video_filter applications, as those are
+    label will be run. This does not apply for multiple video_filter labels, as those are
     turned into a complex filter and applied sequentially.
 
     Methods
     -------
 
     resize_by_ratio(video_list, x_ratio, y_ratio) -> List[Video]:
         Given a ratio from 0 to 1, the video will be resized by that ratio. This uses
@@ -29,34 +27,67 @@
         the video to the modified file.
 
     trim_into_clips(video_list, interval) -> List[Video]:
         Splits the video into X second clips, sends all these clips to output
         folder.
         *will re-encode
 
-    split_on_frame(video_list, frame) -> List[Video]:
+    trim_on_frame(video_list, frame) -> List[Video]:
         Given a specific frame, start the video there, removes any preceding frames.
         *will re-encode
 
-    split_num_frames(video_list, start_frame, num_frames) -> List[Video]:
+    trim_num_frames(video_list, start_frame, num_frames) -> List[Video]:
         Given a start frame and the amount of frames that a user wants to copy, splits the video to all of the frames
         within that frame range.
         *will re-encode
 
     crop_video_section(video_list, width, height, start_x, start_y) -> List[Video]:
         Create a width x height crop of the input video starting at pixel values start_x, start_y and sends the
         smaller video to the modified file.
 
     blur_video(video_list, blur_level, blur_steps) -> List[Video]:
         Adds the blur_level amount of blur blur_steps amount of times to a video.
         *will re-encode
+
+    set_bitrate(video_list, new_bitrate) -> List[Video]
+        Adjust the bitrate of the VIDEO stream (stream[0]) to the desired output. New_bitrate should be an
+        integer in KB/s, but setting it to 0 will set the bitrate to 1/10th the original encoded bitrate.
+
+    change_fps(video_list, new_framerate) -> List[Video]
+        Change the video frames per second. Lowering the FPS from the original video will not reencode all
+        original frames at the new framerate, but rather will drop i/b frames to achieve the original duration.
+
+    Examples
+    --------
+
+    resize_by_ratio(s3_videos, 0.75, 0.75) -> Creates an output video at 75% scale
+
+    change_resolution(s3_videos, '480p') -> Creates an output video thats 640x480
+
+    trim_video_start_end(s3_videos, 12, 53) -> Creates a video trimmed from 12s to 53s
+
+    trim_into_clips(s3_videos, 10) -> Splits the whole video into 10s clips (duration % interval # of clips)
+
+    trim_on_frame(s3_videos, 1550) -> Create a trim starting from frame 1550 to the end
+
+    trim_num_frames(s3_videos, 300, 600) -> Starting from frame 300, create a clip of the next 600 frames
+
+    crop_video_section(s3_videos, 0, 0, 250, 500) -> Create a 250x500 crop originating from (0,0)
+
+    blur_video(s3_videos, 15, 2) -> Applies a level 15 Gaussian blur 2 times
+
+    set_bitrate(s3_video, 0) -> Reencodes videos at 1/10th the native bitrate
+
+    set_bitrate(s3_video, 1500) -> Reencodes videos at 1500 KB/s (1.5MB/s) bitrate
+
+    change_fps(s3_video, 24) -> Reencodes video at 24 frames per second
     """
 
     def __init__(self) -> None:
-        print("---aEye Video Label Maker v0---")
+        logging.info("---aEye Video Label Maker v0---")
         pass
 
     def resize_by_ratio(self, video_list, x_ratio=.8, y_ratio=.8):
         """
         This method will add resizing label to all target the video that will be multiplying the
         width by x_ratio and height by y_ratio.
         Both values have to be non negative and non zero value.
@@ -78,19 +109,24 @@
             video_list: list
                 The list of video that contains the resize label.
 
         """
 
         # Go to each video and add the resizing ffmpeg label.
         for video in video_list:
-            video.extract_metadata()
-            new_width = int(video.get_width() * x_ratio)
-            new_height = int(video.get_height() * y_ratio)
-
-            video.add_label(f"-vf scale={math.ceil(new_width / 2) * 2}:{math.ceil(new_height / 2) * 2},setsar=1:1 ")
+            try:
+                video.extract_metadata()
+                new_width = int(video.get_width() * x_ratio)
+                new_height = int(video.get_height() * y_ratio)
+
+                video.complex_filter.append(
+                    f"scale={math.ceil(new_width / 2) * 2}:{math.ceil(new_height / 2) * 2},setsar=1:1")
+                video.add_output_title(f"resized_ratio_{x_ratio}_{y_ratio}_")
+            except:
+                logging.error(f" Cannot crop with ratio {x_ratio},{y_ratio} on video {video}")
 
         logging.info(f"successfully added resizing mod to all video by ratio of {x_ratio} and {y_ratio}")
 
         return video_list
 
     def trim_video_start_end(self, video_list, start, end):
         """
@@ -111,18 +147,22 @@
 
         Returns
         -------
 
         List of videos with labels applied to it
         """
         for video in video_list:
-            duration = end - start
-            video.add_label(f"-ss {start} -t {duration} ")
-            video.add_output_title(f"trimmed_{start}_to_{end}_")
-            logging.info(f"Created a sub-video from {start} to {end}")
+            try:
+                assert start < float(video.get_duration()) and start >= 0
+                duration = end - start
+                video.add_label(f"-ss {start} -t {duration} ")
+                video.add_output_title(f"trimmed_{start}_to_{end}_")
+                logging.info(f"Created a sub-video from {start} to {end}")
+            except:
+                logging.error(f" Video {video} cannot be cut with constaints {start},{end}")
         return video_list
 
     def change_resolution(self, video_list, desired_resolution):
         """
         Add the label for resizing a video according to desired resolution.
         Height is what determines: 420p, 720p, etc.
         Function will automatically select the correct width based off popular sizing.
@@ -154,15 +194,15 @@
 
         try:
             width_height = popular_resolutions[desired_resolution]
 
             # Generate the desired target list of videos to add label.
             # Add the scale ffmpeg label to all desired videos.
             for video in video_list:
-                video.add_label("-c:v libx264 -preset slow -crf 21 ")
+                video.add_label("-c:v libx264 -preset slow -crf 28 ")
                 video.complex_filter.append(f"scale={width_height[0]}x{width_height[1]}:flags=lanczos")
                 video.add_output_title(f"resized_{width_height[0]}x{width_height[1]}_")
 
             logging.info(f"successfully added resize label for desired_resolution")
 
         except:
             logging.error(
@@ -190,18 +230,22 @@
 
         Returns
         -------
 
         List of Video objects with labels applied.
         """
         for video in video_list:
-            video.add_label(
-                f" -map 0 -c:a aac -vsync vfr -reset_timestamps 1 -segment_time {interval} -g {interval} -sc_threshold 0 -force_key_frames 'expr:gte(t,n_forced*{interval})' -f segment ")
-            video.add_output_title(f"trimmed_{interval}_clips_")
-            logging.info(f"Video has been trimmed into {interval} second long clips!")
+            try:
+                assert interval > 0
+                video.add_label(
+                    f" -c:a aac -vsync vfr -reset_timestamps 1 -segment_time {interval} -g {interval} -sc_threshold 0 -force_key_frames 'expr:gte(t,n_forced*{interval})' -f segment ")
+                video.add_output_title(f"trimmed_{interval}_clips_")
+                logging.info(f"Video has been trimmed into {interval} second long clips!")
+            except:
+                logging.error(f" Video {video} cannot have trim applied with {interval} as a constraint!")
         return video_list
 
     def trim_on_frame(self, video_list, frame):
         """
         Given a frame, this method will create a video starting at that specific
         frame and running all the way until the end. Note: Depending on encoding, it can be
         difficult to get the exact frame if it isn't an I/P/B frame.
@@ -217,19 +261,23 @@
 
         Returns
         -------
 
         List of Video Objects with trim labels applied
         """
         for video in video_list:
-            fps = float(video.get_num_frames()) / float(video.get_duration())
-            time_stamp = frame / fps
-            video.add_label(f"-ss {time_stamp} ")
-            video.add_output_title(f"trimmed_on_frame_{frame}_")
-            logging.info(f"Split video at frame {frame}")
+            try:
+                assert 0 <= frame <= int(video.get_num_frames())
+                fps = float(video.get_num_frames()) / float(video.get_duration())
+                time_stamp = frame / fps
+                video.add_label(f"-ss {time_stamp} ")
+                video.add_output_title(f"trimmed_on_frame_{frame}_")
+                logging.info(f"Split video at frame {frame}")
+            except:
+                logging.error(f" Cannot trim video {video} on frame {frame}!")
         return video_list
 
     def trim_num_frames(self, video_list, start_frame, num_frames):
         """
         Given a passed frame (start_Frame), and a duration (num_frames), which in this instance is the number of
         frames to crop to, it will send a cropped video to the output folder.
 
@@ -249,19 +297,23 @@
 
         Returns
         -------
 
         List of Video Objects with trim labels
         """
         for video in video_list:
-            fps = float(video.get_num_frames()) / float(video.get_duration())
-            time_stamp = start_frame / fps
-            logging.info(f"Encoding {num_frames} from {start_frame}")
-            video.add_output_title(f"trim_frames_{start_frame}_to_{start_frame + num_frames}_")
-            video.add_label(f"-ss {str(time_stamp)} -frames:v {num_frames} ")
+            try:
+                assert start_frame > 0 and int(start_frame + num_frames) < int(video.get_num_frames())
+                fps = float(video.get_num_frames()) / float(video.get_duration())
+                time_stamp = start_frame / fps
+                logging.info(f"Encoding {num_frames} from {start_frame}")
+                video.add_output_title(f"trim_frames_{start_frame}_to_{start_frame + num_frames}_")
+                video.add_label(f"-ss {str(time_stamp)} -frames:v {num_frames} ")
+            except:
+                logging.error(f" Cannot create a {num_frames} trim starting on frame {start_frame} for video {video}")
         return video_list
 
     def crop_video_section(self, video_list, start_x, start_y, section_width, section_height):
         """
         Crops a section_width x section_height grab of the video starting at pixel coordinates start_x, start_y
         and just uses the active video object to do so. Note, re-encoding is a necessary
         step for ANY filter application, so there will be noticeable processing time.
@@ -286,17 +338,25 @@
 
         Returns
         -------
 
         A list of Video objects with labels applied
         """
         for video in video_list:
-            video.complex_filter.append(f"crop={section_width}:{section_height}:{start_x}:{start_y} ")
-            video.add_output_title(f"cropped_{section_width}x{section_height}_")
-            logging.info(f"Created a {section_width}x{section_height} crop at ({start_x},{start_y})")
+            try:
+                assert start_x ^ start_y >= 0 and start_x <= int(video.get_width()) and start_y <= int(
+                    video.get_height())  # Crop within bounds
+                assert int(section_width + start_x) <= int(video.get_width()) and int(section_height + start_y) <= int(
+                    video.get_height())  # Crop doesn't exceed bounds
+                video.complex_filter.append(f"crop={section_width}:{section_height}:{start_x}:{start_y} ")
+                video.add_output_title(f"cropped_{section_width}x{section_height}_")
+                logging.info(f"Created a {section_width}x{section_height} crop at ({start_x},{start_y})")
+            except:
+                logging.error(
+                    f" Video {video} cannot be cropped to {section_width}x{section_height} at ({start_x},{start_y})")
         return video_list
 
     def blur_video(self, video_list, blur_level, blur_steps=1):
         """
         Create a Gaussian blur, with the blur_level being the sigma level for the blur, with the
         blur_steps being the amount of times that sigma level is applied to the video. Ex. 6, 2 applies a level 6 blur
         to the video twice. More steps = more blending. Upper limit to steps is 6, default is 1; unsure
@@ -318,11 +378,110 @@
 
         Returns
         -------
 
         List of videos with the blur label applied
         """
         for video in video_list:
-            video.complex_filter.append(f"gblur=sigma={blur_level}:steps={blur_steps} ")
-            video.add_output_title(f"blurred_{blur_level}x{blur_steps}_")
-            logging.info(f"Created a blur of strength {blur_level} and applied it {blur_steps} times")
+            try:
+                assert blur_level in range(0, 52) and blur_steps in range(1, 6)
+                video.complex_filter.append(f"gblur=sigma={blur_level}:steps={blur_steps} ")
+                video.add_output_title(f"blurred_{blur_level}x{blur_steps}_")
+                logging.info(f"Created a blur of strength {blur_level} and applied it {blur_steps} times")
+            except:
+                logging.error(
+                    f" Cannot create a blur with level {blur_level} (max 51) and {blur_steps} steps (max 5) for video {video}")
+        return video_list
+
+    def set_bitrate(self, video_list, bitrate):
+        """
+        Sets the bitrate of the video in KB/s. If bitrate is set as 0, then
+        the framework will do a 10x bitrate reduction for the reencode. This usually leaves
+        the quality watchable.
+
+        Parameters
+        ----------
+
+        video_list : List[Video]
+            List of all the videos loaded currently.
+
+        bitrate    : Integer
+            Desired bitrate for the videos. This is given in Kb, so setting it to 1.5 Mb for exmaple should be
+            1500, not 1.5! Setting to 0 will do a 10x reduction
+
+        Returns
+        ----------
+
+        List of videos with the bitrate adjustment label applied.
+        """
+        if bitrate == 0:
+            tenx = True
+        else:
+            tenx = False
+        for video in video_list:
+            try:
+                if tenx:
+                    video.extract_metadata()
+                    cur_br = int(video.meta_data["streams"][0]["bit_rate"])
+                    bitrate = math.ceil(cur_br / 10000)
+                insert_str = f" -x264-params 'nal-hdr=cbr' -b:v {bitrate}K -minrate {bitrate}K -maxrate {bitrate}K -bufsize {(int(bitrate) * 2)}K "
+                video.add_label(insert_str)
+                video.add_output_title(f"bitrate_{bitrate}K_")
+                logging.info(f"Bitrate adjusted. Not perfectly accurately, but thats ok")
+            except:
+                logging.error(f" Cannot set bitrate to {bitrate}k for video {video}")
         return video_list
+
+    def change_fps(self, video_list, new_framerate):
+        """
+        Super simple video FPS adjustment. Adjusting FPS up can do some funky things
+        to the video as Mac thinks high framerate videos are slow-mo videos,
+        but it still works just fine.
+
+        Parameters
+        ----------
+
+        video_list: List[Video]
+            List of all loaded videos
+
+        new_framerate: Integer
+            The desired frame rate for the video to be re-encoded to. Lowering framerate
+            will reduce the size of the file drastically, but frames will be lost and it can result in
+            a less than ideal viewing experience for humans.
+
+        Returns
+        ----------
+
+        List of all videos with the complex filter to change FPS applied
+        """
+        for video in video_list:
+            try:
+                video.complex_filter.append(f"fps={new_framerate}")
+                video.add_output_title(f"framerate_{new_framerate}_")
+            except:
+                logging.error(f" Cannot adjust video {video} framerate to {new_framerate}!")
+        return video_list
+
+    def grayscale(self, video_list):
+        """
+        Applies grayscale to all videos in the queue
+
+        Parameters
+        ----------
+
+        video_list : List[Video]
+            List of all videos to apply grayscale to
+
+        Returns
+        ----------
+
+        List of all videos with complex filter applied
+        """
+        for video in video_list:
+            try:
+                video.complex_filter.append(f"format=gray")
+                video.add_output_title(f"grayscale_")
+            except:
+                logging.error(f"Cannot apply grayscale to video {video}")
+        return video_list
+
+
```

### Comparing `aEye-1.0.0/aEye/video.py` & `aEye-1.1.0/aEye/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,85 @@
 """
 Module contains the Video class that stores and represents video files as objects.
 
 """
 import cv2
-import os
 import subprocess
 import json
-from static_ffmpeg import run
-
-# Please comment this out when setting up a docker image.
-# This will fail when we use the docker image in the lambda function on AWS.
-ffmpeg, ffprobe = run.get_or_fetch_platform_executables_else_raise()
 import boto3
+from static_ffmpeg import run
 
 s3 = boto3.client("s3")
 
 
 class Video:
     """
     Video class that encapsulates all necessary video information.
     Also contains some useful utility like the ability to grab frames, process
     video clips, trim them down, crop, etc.
     Attributes
     ----------
-    file: str
+    file    : str
         path of the video file associated with the object
-    meta_data: str
+
+    bucket  : str
         JSON dictionary of video metadata, typically streams[0] is the video metadata
-    cv_video: cv2.VideoCapture
-        OpenCV video object, used for any openCV processing
+
+    key     : str
+        Essentially this is the s3 absolute location of the file
+
+    title   : str
+        Title for the output video to build upon
+
     ----------
     Methods
     ----------
     extract_metadata -> str:
         Collects the metadata from all video sources and separates the streams
         Necessary for basically any processing, but still has to be set (none by default)
+
     get_codec -> str:
         Returns the video codec
+
     get_duration -> str:
         Returns video duration in seconds, but does so as a string
+
     get_frames -> str:
         Returns the amount of frames in the video as a string (via OpenCV)
-    getfile -> str:
+
+    get_file -> str:
         Returns video file path
 
+    get_title -> str:
+        Returns video title
+
+    get_width -> str:
+        Returns video width as a string
+
+    get_height -> str:
+        Returns video height as a string
+
+    get_presigned_url -> str:
+        Returns the presigned AWS bucket URL, which acts as the file location for
+        videos uploaded via S3
+
+    add_label -> None:
+        Adds a passed label to the current video object
+
+    reset_label -> None:
+        Sets the video label to an empty string
+
+    add_output_title -> None:
+        Adds the passed string to the output title so it can be informative
+
+    create_complex_filter -> None:
+        Creates a sequential exection label for modifications that use -vf tag. This
+        way multiple -vf filters can be applied to the same video
+
+
     """
 
     def __init__(self, file=None, bucket=None, key=None, title=None) -> None:
         self.file = file
         self.bucket = bucket
         self.key = key
         self.title = title
@@ -104,23 +136,24 @@
         json['streams'][0] because it is the first channel and the dictionary splits streams from error
         Returns
         ---------
             meta_data: dictionary
                 The dictionary of metadata for all streams.
 
         """
+        ffmpeg, probe_path = run.get_or_fetch_platform_executables_else_raise()
         if self.meta_data is None:
             fp = None
             if self.file is None:
                 fp = self.get_presigned_url()
             elif self.out is not '':
                 fp = self.out
             else:
                 fp = self.file
-            command = f"{ffprobe} -hide_banner -show_streams -v error -print_format json -show_format -i {fp}"
+            command = f"{probe_path} -hide_banner -show_streams -v error -print_format json -show_format -i {fp}"
             out = subprocess.check_output(command, shell=True).decode("utf-8")
             json_data = json.loads(out)
             self.meta_data = json_data
             return json_data
 
     def get_codec(self):
         """
@@ -133,15 +166,15 @@
         ----------
 
         Video codec as a string
         """
         if self.meta_data is not None:
             return self.meta_data["streams"][0]["codec_name"]
         else:
-            self.meta_data = self.get_metadata()
+            self.meta_data = self.extract_metadata()
             return self.meta_data["streams"][0]["codec_name"]
 
     def get_duration(self):
         """
         Gets the current video duration
 
         Parameters
@@ -151,15 +184,15 @@
         ----------
 
         The video duration as a STRING. Convert to float before processing if needed
         """
         if self.meta_data is not None:
             return self.meta_data["streams"][0]["duration"]
         else:
-            self.meta_data = self.get_metadata()
+            self.meta_data = self.extract_metadata()
             return self.meta_data["streams"][0]["duration"]
 
     def get_num_frames(self):
         """
         Gets teh number of B-frames in the video
 
         Parameters
@@ -238,15 +271,15 @@
 
         Returns
         ----------
 
         """
         self.capture.release()
 
-    def get_presigned_url(self, time=60):
+    def get_presigned_url(self, time=600):
         """
         This method will return the presigned url of video file from S3.
         If the video file is from local machine then it will return the local path of the video file.
 
         Returns
         ---------
             url: string
@@ -353,15 +386,15 @@
         video: video with VF process(es) like crop or blur
 
         Returns
         ----------
         Nothing, but the video label is appended with the completed complex filter
         """
         filter_steps = video.complex_filter
-        filter_str = "-filter_complex '"
+        filter_str = " -filter_complex '"
         end = len(filter_steps)
         for i in range(len(filter_steps)):
             filter_str += f"[{i}]{filter_steps[i]}[{i + 1}];"
         filter_str = filter_str.strip(";")
         filter_str += f"' -map [{end}] "
         video.add_label(filter_str)
 
@@ -373,23 +406,29 @@
         Returns
         ---------
             result: string
                 The output title of video.
         """
 
         result = ''
-        if 'scale' in self.label:
-            result += "resized_"
-        if '-ss' in self.label:
-            result += "trimmed_"
-        if 'crop' in self.label:
-            result += "cropped_"
-        if 'blur' in self.label:
-            result += "blurred_"
         if '-f segment' in self.label:
             out = self.title.split('.')
             out[0] += "_%02d."
             out = "".join(out)
-            self.title = out  # IMPORTANT FOR SOMETHING LMAO FIGURE OUT WHY
+            self.title = out
         self.out = result + self.title
-        return  self.out_title + self.title
+        return self.out_title + self.title
 
+    def get_title(self):
+        """
+        This method will return the video's title.
+        This will also create the video title based on its key from s3
+
+        Returns
+        ----------
+            title: string
+                The video's title.
+        """
+
+        if not self.title and self.key:
+            self.title = self.key.split('/')[-1]
+        return self.title
```

### Comparing `aEye-1.0.0/aEye.egg-info/PKG-INFO` & `aEye-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,25 @@
-Metadata-Version: 2.1
-Name: aEye
-Version: 1.0.0
-Summary: Extensible Video Processing Framework
-Home-page: https://github.com/DISHDevEx/aEye
-Author-email: devex@dish.com
-License: Dish Wireless
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # aEye
 
 Extensible Video Processing Framework with Additional Features Continuously Deployed
 
 ### **Project Structure**
 
 ```
 ├──  aEye				contains video class and processor class that manage from loading, processing and uploading
 │   ├── video.py
 |   ├── auxiliary.py
 |   ├── extractor.py
 |   ├── labeler.py
 │   ├── auxiliary.py
-│   ├── mediapipe
-│      ├── object_detection.py
-│      ├── visualize.py
-├──  runner_notebooks
-│   ├── leto-demo.ipynb
 ├──  tests				contains unit tests
 │   ├── test_get_meta_data.py
 │   ├── conftest.py
 │   ├── test_data
 │      ├── test_video.mp4
-├── lambda_function.py
 ├── setup.py
 ```
 
 ### **Inital project setup**
 
 1. clone/pull this repo to local machine
 
@@ -68,28 +52,32 @@
 from aEye.extractor import Extractor
 ```
 
 5. Initalize the auxiliary class. This creates a temporary directory for output files 
 
 ```console
 aux = Aux()
+# This class can download and upload videos, as well as executing pending labels
 ```
 
 6. Load the video from the desired bucket and folder.
 
 ```console
 video_list_s3 = aux.load_s3(bucket = 'aeye-data-bucket', prefix = 'input_video/')
 ```
 
 
 7. Initalize the labeler and extractor
 
 ```console
 label = Labeler()
+# This is used to apply labels like 'crop', 'trim', etc to a video object
+
 extract = Extractor()
+# This is used to extract frames as PNG's 
 ```
 
 
 How to process videos using Labeler and Extractor:
 
 The labeler provides multiple actions that can be applied to a video or a list of videos. Each action takes a video or list of videos as its first parameter and returns a modified video or list of videos. 
 To chain multiple labels together, you can pass the output of one process as the input for the next process.
@@ -154,23 +142,30 @@
 
 change_resolution(video_list, desired_res) -> Changes the resolution to a 'standard' resolution.
 
 trim_video_start_end(video_list, start, end) -> Given start and end times in seconds, modified a trimmed down version of the video to the modified file.
 
 trim_into_clips(video_list, interval) -> Splits the video into X second clips, sends all these clips to output folder.
 
-split_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
+trim_on_frame(video_list, frame) -> Given a specific frame, start the video there, removes any preceding frames.
 
-split_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
+trim_num_frames(video_list, start_frame, num_frames) -> Given a start frame and the amount of frames that a user wants "
 to copy, splits the video to all of the frames within that frame range.
 
 crop_video_section(video_list, start_x, start_y, width, height) -> Create a width x height crop of the input video starting at pixel values"\
 start_x, start_y and sends the smaller video to the modified file.
 
-blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video
+blur_video(video_list, blur_level, blur_steps) -> Adds the blur_level amount of blur blur_steps amount of times to a video.
+
+set_bitrate(video_list, desired_bitrate) -> Sets the bitrate at which the video will re-encode to.
+
+change_fps(video_list, new_framerate) -> Sets the framerate at which the video will re-encode. Note, reducing the 
+bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
+
+grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
 frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
 specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
@@ -185,15 +180,17 @@
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
 The TRIM_INTO_CLIPS operation must be executed last. It creates multiple output videos from a single input, and these outputs cannot be processed further.
 Here's an example of using the labeler utility to downsize, crop, and trim a video:
 
 
 ```console
 to_process = label.trim_video_start_end(video_list_s3, 1, 9)              #Trims from 1s to 9s
+
 to_process = label.change_resolution(to_process, "720p")                  #Converts to 720p
+
 final_video_list = label.crop_video_section(to_process, 0, 0, 150, 100)   #Creates a 150x100 crop at (0,0)
 ```
 
 
 8. Use auxiliary class to execute and write the videos with labels.
 
 ```console
@@ -235,22 +232,7 @@
 ```
 
 14. Execute all labels and write the output to data/ folder.
 
 ```console
 aux.execute_label_and_write_local(trimmed_local,'data/')
 ```
-
-### **Docker Image Setup**
-
-The docker image is built automatically via github workflow action on every tag push.
-The rough sequence is below:
-
-    1) The workflow action will build a wheel file based on setup.py,
-    2) Then it will create a docker image based on the dockerfile.
-    3) Finally it will push the image to ECR (currently, this will be loaded in ECR: Leto).
-
-Please refer to mp-to-ecr.yml to get the exact sequences of the github workflow action, the dockerfile for the exact content in the docker image and setup.py for the exact built version.
-
-### **Lambda Function**
-
-Please refer to lambda_function.py for the logic of the lambda function.
```

### Comparing `aEye-1.0.0/setup.py` & `aEye-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.0.0, which will later be replaced with a git tag when performing
+    v1.1.0, which will later be replaced with a git tag when performing
     version releases.
 
     Returns
     -------
     when the bdist_wheel command is given a version flag and version number, such as:
 
     --version 1.x.x
@@ -36,15 +36,15 @@
     If the --version flag is given, but no version number is supplied, such as:
 
     --version
 
     then an IndexError will be thrown and the build will exit with exit status 1.
 
     """
-    version = 'v1.0.0'
+    version = 'v1.1.0'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

