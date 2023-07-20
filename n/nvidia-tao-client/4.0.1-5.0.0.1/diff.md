# Comparing `tmp/nvidia_tao_client-4.0.1-py3-none-any.whl.zip` & `tmp/nvidia_tao_client-5.0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,52 @@
-Zip file size: 26017 bytes, number of entries: 30
--rw-rw-r--  2.0 unx        0 b- defN 23-Jan-11 18:46 tao_cli/__init__.py
--rw-rw-r--  2.0 unx     1674 b- defN 23-Jan-11 18:46 tao_cli/constants.py
--rw-rw-r--  2.0 unx      932 b- defN 23-Jan-11 18:46 tao_cli/login.py
--rw-rw-r--  2.0 unx     1966 b- defN 23-Jan-11 18:46 tao_cli/tao.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jan-11 18:46 tao_cli/cli_actions/__init__.py
--rw-rw-r--  2.0 unx     2213 b- defN 23-Jan-11 18:46 tao_cli/cli_actions/actions.py
--rw-rw-r--  2.0 unx     1016 b- defN 23-Jan-11 18:46 tao_cli/cli_actions/dataset.py
--rw-rw-r--  2.0 unx     1026 b- defN 23-Jan-11 18:46 tao_cli/cli_actions/model.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jan-11 18:46 tao_cli/networks/__init__.py
--rw-rw-r--  2.0 unx     7014 b- defN 23-Jan-11 18:46 tao_cli/networks/detectnet_v2.py
--rw-rw-r--  2.0 unx     7014 b- defN 23-Jan-11 18:46 tao_cli/networks/efficientdet.py
--rw-rw-r--  2.0 unx     6990 b- defN 23-Jan-11 18:46 tao_cli/networks/faster_rcnn.py
--rw-rw-r--  2.0 unx     6229 b- defN 23-Jan-11 18:46 tao_cli/networks/lprnet.py
--rw-rw-r--  2.0 unx     6941 b- defN 23-Jan-11 18:46 tao_cli/networks/mask_rcnn.py
--rw-rw-r--  2.0 unx     6417 b- defN 23-Jan-11 18:46 tao_cli/networks/multi_class_classification.py
--rw-rw-r--  2.0 unx     6626 b- defN 23-Jan-11 18:46 tao_cli/networks/multi_task_classification.py
--rw-rw-r--  2.0 unx     6942 b- defN 23-Jan-11 18:46 tao_cli/networks/retinanet.py
--rw-rw-r--  2.0 unx     5170 b- defN 23-Jan-11 18:46 tao_cli/networks/spectro_gen.py
--rw-rw-r--  2.0 unx     6798 b- defN 23-Jan-11 18:46 tao_cli/networks/ssd.py
--rw-rw-r--  2.0 unx     6185 b- defN 23-Jan-11 18:46 tao_cli/networks/unet.py
--rw-rw-r--  2.0 unx     3186 b- defN 23-Jan-11 18:46 tao_cli/networks/vocoder.py
--rw-rw-r--  2.0 unx     6894 b- defN 23-Jan-11 18:46 tao_cli/networks/yolo_v3.py
--rw-rw-r--  2.0 unx     6894 b- defN 23-Jan-11 18:46 tao_cli/networks/yolo_v4.py
--rw-rw-r--  2.0 unx     7009 b- defN 23-Jan-11 18:46 tao_cli/networks/yolo_v4_tiny.py
--rw-rw-r--  2.0 unx      552 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      744 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2577 b- defN 23-Jan-11 18:46 nvidia_tao_client-4.0.1.dist-info/RECORD
-30 files, 109157 bytes uncompressed, 21835 bytes compressed:  80.0%
+Zip file size: 73968 bytes, number of entries: 50
+-rw-rw-r--  2.0 unx      639 b- defN 23-Jul-18 18:54 tao_cli/__init__.py
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Jul-18 18:54 tao_cli/constants.py
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jul-18 19:29 tao_cli/login.py
+-rw-rw-r--  2.0 unx     4025 b- defN 23-Jul-18 18:54 tao_cli/tao.py
+-rw-rw-r--  2.0 unx      647 b- defN 23-Jul-18 18:54 tao_cli/cli_actions/__init__.py
+-rw-rw-r--  2.0 unx     2648 b- defN 23-Jul-18 19:29 tao_cli/cli_actions/actions.py
+-rw-rw-r--  2.0 unx     1289 b- defN 23-Jul-18 19:29 tao_cli/cli_actions/dataset.py
+-rw-rw-r--  2.0 unx     1291 b- defN 23-Jul-18 19:29 tao_cli/cli_actions/model.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jul-18 18:54 tao_cli/networks/__init__.py
+-rw-rw-r--  2.0 unx     5234 b- defN 23-Jul-18 18:54 tao_cli/networks/action_recognition.py
+-rw-rw-r--  2.0 unx     2383 b- defN 23-Jul-18 18:54 tao_cli/networks/analytics.py
+-rw-rw-r--  2.0 unx     2209 b- defN 23-Jul-18 18:54 tao_cli/networks/annotations.py
+-rw-rw-r--  2.0 unx     2211 b- defN 23-Jul-18 18:54 tao_cli/networks/augmentation.py
+-rw-rw-r--  2.0 unx     2197 b- defN 23-Jul-18 18:54 tao_cli/networks/auto_label.py
+-rw-rw-r--  2.0 unx     7775 b- defN 23-Jul-18 18:54 tao_cli/networks/bpnet.py
+-rw-rw-r--  2.0 unx     5835 b- defN 23-Jul-18 18:54 tao_cli/networks/deformable_detr.py
+-rw-rw-r--  2.0 unx     7999 b- defN 23-Jul-18 18:54 tao_cli/networks/detectnet_v2.py
+-rw-rw-r--  2.0 unx     5637 b- defN 23-Jul-18 18:54 tao_cli/networks/dino.py
+-rw-rw-r--  2.0 unx     7799 b- defN 23-Jul-18 18:54 tao_cli/networks/dssd.py
+-rw-rw-r--  2.0 unx     8099 b- defN 23-Jul-18 18:54 tao_cli/networks/efficientdet_tf1.py
+-rw-rw-r--  2.0 unx     8099 b- defN 23-Jul-18 18:54 tao_cli/networks/efficientdet_tf2.py
+-rw-rw-r--  2.0 unx     7972 b- defN 23-Jul-18 18:54 tao_cli/networks/faster_rcnn.py
+-rw-rw-r--  2.0 unx     6104 b- defN 23-Jul-18 18:54 tao_cli/networks/fpenet.py
+-rw-rw-r--  2.0 unx     7116 b- defN 23-Jul-18 18:54 tao_cli/networks/lprnet.py
+-rw-rw-r--  2.0 unx     4438 b- defN 23-Jul-18 18:54 tao_cli/networks/mal.py
+-rw-rw-r--  2.0 unx     7922 b- defN 23-Jul-18 18:54 tao_cli/networks/mask_rcnn.py
+-rw-rw-r--  2.0 unx     5718 b- defN 23-Jul-18 18:54 tao_cli/networks/ml_recog.py
+-rw-rw-r--  2.0 unx     5828 b- defN 23-Jul-18 18:54 tao_cli/networks/multi_class_classification_pyt.py
+-rw-rw-r--  2.0 unx     7423 b- defN 23-Jul-18 18:54 tao_cli/networks/multi_class_classification_tf1.py
+-rw-rw-r--  2.0 unx     7423 b- defN 23-Jul-18 18:54 tao_cli/networks/multi_class_classification_tf2.py
+-rw-rw-r--  2.0 unx     7539 b- defN 23-Jul-18 18:54 tao_cli/networks/multi_task_classification.py
+-rw-rw-r--  2.0 unx     6812 b- defN 23-Jul-18 18:54 tao_cli/networks/ocdnet.py
+-rw-rw-r--  2.0 unx     7855 b- defN 23-Jul-18 18:54 tao_cli/networks/ocrnet.py
+-rw-rw-r--  2.0 unx     6207 b- defN 23-Jul-18 18:54 tao_cli/networks/optical_inspection.py
+-rw-rw-r--  2.0 unx     7368 b- defN 23-Jul-18 18:54 tao_cli/networks/pointpillars.py
+-rw-rw-r--  2.0 unx     5269 b- defN 23-Jul-18 18:54 tao_cli/networks/pose_classification.py
+-rw-rw-r--  2.0 unx     5237 b- defN 23-Jul-18 18:54 tao_cli/networks/re_identification.py
+-rw-rw-r--  2.0 unx     7924 b- defN 23-Jul-18 18:54 tao_cli/networks/retinanet.py
+-rw-rw-r--  2.0 unx     5727 b- defN 23-Jul-18 18:54 tao_cli/networks/segformer.py
+-rw-rw-r--  2.0 unx     7774 b- defN 23-Jul-18 18:54 tao_cli/networks/ssd.py
+-rw-rw-r--  2.0 unx     7077 b- defN 23-Jul-18 18:54 tao_cli/networks/unet.py
+-rw-rw-r--  2.0 unx     7874 b- defN 23-Jul-18 18:54 tao_cli/networks/yolo_v3.py
+-rw-rw-r--  2.0 unx     7874 b- defN 23-Jul-18 18:54 tao_cli/networks/yolo_v4.py
+-rw-rw-r--  2.0 unx     7999 b- defN 23-Jul-18 18:54 tao_cli/networks/yolo_v4_tiny.py
+-rw-rw-r--  2.0 unx    44474 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      706 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4392 b- defN 23-Jul-20 16:25 nvidia_tao_client-5.0.0.1.dist-info/RECORD
+50 files, 288967 bytes uncompressed, 66934 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -21,71 +21,131 @@
 
 Filename: tao_cli/cli_actions/model.py
 Comment: 
 
 Filename: tao_cli/networks/__init__.py
 Comment: 
 
+Filename: tao_cli/networks/action_recognition.py
+Comment: 
+
+Filename: tao_cli/networks/analytics.py
+Comment: 
+
+Filename: tao_cli/networks/annotations.py
+Comment: 
+
+Filename: tao_cli/networks/augmentation.py
+Comment: 
+
+Filename: tao_cli/networks/auto_label.py
+Comment: 
+
+Filename: tao_cli/networks/bpnet.py
+Comment: 
+
+Filename: tao_cli/networks/deformable_detr.py
+Comment: 
+
 Filename: tao_cli/networks/detectnet_v2.py
 Comment: 
 
-Filename: tao_cli/networks/efficientdet.py
+Filename: tao_cli/networks/dino.py
+Comment: 
+
+Filename: tao_cli/networks/dssd.py
+Comment: 
+
+Filename: tao_cli/networks/efficientdet_tf1.py
+Comment: 
+
+Filename: tao_cli/networks/efficientdet_tf2.py
 Comment: 
 
 Filename: tao_cli/networks/faster_rcnn.py
 Comment: 
 
+Filename: tao_cli/networks/fpenet.py
+Comment: 
+
 Filename: tao_cli/networks/lprnet.py
 Comment: 
 
+Filename: tao_cli/networks/mal.py
+Comment: 
+
 Filename: tao_cli/networks/mask_rcnn.py
 Comment: 
 
-Filename: tao_cli/networks/multi_class_classification.py
+Filename: tao_cli/networks/ml_recog.py
+Comment: 
+
+Filename: tao_cli/networks/multi_class_classification_pyt.py
+Comment: 
+
+Filename: tao_cli/networks/multi_class_classification_tf1.py
+Comment: 
+
+Filename: tao_cli/networks/multi_class_classification_tf2.py
 Comment: 
 
 Filename: tao_cli/networks/multi_task_classification.py
 Comment: 
 
+Filename: tao_cli/networks/ocdnet.py
+Comment: 
+
+Filename: tao_cli/networks/ocrnet.py
+Comment: 
+
+Filename: tao_cli/networks/optical_inspection.py
+Comment: 
+
+Filename: tao_cli/networks/pointpillars.py
+Comment: 
+
+Filename: tao_cli/networks/pose_classification.py
+Comment: 
+
+Filename: tao_cli/networks/re_identification.py
+Comment: 
+
 Filename: tao_cli/networks/retinanet.py
 Comment: 
 
-Filename: tao_cli/networks/spectro_gen.py
+Filename: tao_cli/networks/segformer.py
 Comment: 
 
 Filename: tao_cli/networks/ssd.py
 Comment: 
 
 Filename: tao_cli/networks/unet.py
 Comment: 
 
-Filename: tao_cli/networks/vocoder.py
-Comment: 
-
 Filename: tao_cli/networks/yolo_v3.py
 Comment: 
 
 Filename: tao_cli/networks/yolo_v4.py
 Comment: 
 
 Filename: tao_cli/networks/yolo_v4_tiny.py
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/LICENSE.txt
+Filename: nvidia_tao_client-5.0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/METADATA
+Filename: nvidia_tao_client-5.0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/WHEEL
+Filename: nvidia_tao_client-5.0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/entry_points.txt
+Filename: nvidia_tao_client-5.0.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/top_level.txt
+Filename: nvidia_tao_client-5.0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_tao_client-4.0.1.dist-info/RECORD
+Filename: nvidia_tao_client-5.0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tao_cli/__init__.py

```diff
@@ -0,0 +1,40 @@
+00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
+00000010: 3230 3233 2c20 4e56 4944 4941 2043 4f52  2023, NVIDIA COR
+00000020: 504f 5241 5449 4f4e 2e20 2041 6c6c 2072  PORATION.  All r
+00000030: 6967 6874 7320 7265 7365 7276 6564 2e0a  ights reserved..
+00000040: 230a 2320 4c69 6365 6e73 6564 2075 6e64  #.# Licensed und
+00000050: 6572 2074 6865 2041 7061 6368 6520 4c69  er the Apache Li
+00000060: 6365 6e73 652c 2056 6572 7369 6f6e 2032  cense, Version 2
+00000070: 2e30 2028 7468 6520 224c 6963 656e 7365  .0 (the "License
+00000080: 2229 3b0a 2320 796f 7520 6d61 7920 6e6f  ");.# you may no
+00000090: 7420 7573 6520 7468 6973 2066 696c 6520  t use this file 
+000000a0: 6578 6365 7074 2069 6e20 636f 6d70 6c69  except in compli
+000000b0: 616e 6365 2077 6974 6820 7468 6520 4c69  ance with the Li
+000000c0: 6365 6e73 652e 0a23 2059 6f75 206d 6179  cense..# You may
+000000d0: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+000000e0: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+000000f0: 0a23 0a23 2020 2020 2068 7474 703a 2f2f  .#.#     http://
+00000100: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+00000110: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00000120: 322e 300a 230a 2320 556e 6c65 7373 2072  2.0.#.# Unless r
+00000130: 6571 7569 7265 6420 6279 2061 7070 6c69  equired by appli
+00000140: 6361 626c 6520 6c61 7720 6f72 2061 6772  cable law or agr
+00000150: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
+00000160: 672c 2073 6f66 7477 6172 650a 2320 6469  g, software.# di
+00000170: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00000180: 7468 6520 4c69 6365 6e73 6520 6973 2064  the License is d
+00000190: 6973 7472 6962 7574 6564 206f 6e20 616e  istributed on an
+000001a0: 2022 4153 2049 5322 2042 4153 4953 2c0a   "AS IS" BASIS,.
+000001b0: 2320 5749 5448 4f55 5420 5741 5252 414e  # WITHOUT WARRAN
+000001c0: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
+000001d0: 4e53 204f 4620 414e 5920 4b49 4e44 2c20  NS OF ANY KIND, 
+000001e0: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
+000001f0: 7220 696d 706c 6965 642e 0a23 2053 6565  r implied..# See
+00000200: 2074 6865 204c 6963 656e 7365 2066 6f72   the License for
+00000210: 2074 6865 2073 7065 6369 6669 6320 6c61   the specific la
+00000220: 6e67 7561 6765 2067 6f76 6572 6e69 6e67  nguage governing
+00000230: 2070 6572 6d69 7373 696f 6e73 2061 6e64   permissions and
+00000240: 0a23 206c 696d 6974 6174 696f 6e73 2075  .# limitations u
+00000250: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00000260: 2e0a 0a22 2222 5441 4f20 436c 6965 6e74  ..."""TAO Client
+00000270: 2043 4c49 206d 6f64 756c 6522 2222 0a     CLI module""".
```

## tao_cli/constants.py

```diff
@@ -1,50 +1,98 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""Defining enums for dataset and model formats and types"""
 import enum
 
+
 class dataset_format(str, enum.Enum):
+    """Class defining dataset formats in enum"""
+
     default = "default"
     kitti = "kitti"
     lprnet = "lprnet"
     coco = "coco"
     raw = "raw"
     coco_raw = "coco_raw"
-    ljspeech = "ljspeech"
-    hifigan = "hifigan"
     custom = "custom"
-    auxillary = "auxillary"
     unet = "unet"
+    classification_pyt = "classification_pyt"
+
 
 class dataset_type(str, enum.Enum):
+    """Class defining dataset types in enum"""
+
     semantic_segmentation = "semantic_segmentation"
     image_classification = "image_classification"
     object_detection = "object_detection"
     character_recognition = "character_recognition"
     instance_segmentation = "instance_segmentation"
-    speech = "speech"
-    mel_spectrogram = "mel_spectrogram"
+    bpnet = "bpnet"
+    fpenet = "fpenet"
+    action_recognition = "action_recognition"
+    ml_recog = "ml_recog"
+    ocdnet = "ocdnet"
+    ocrnet = "ocrnet"
+    optical_inspection = "optical_inspection"
+    pointpillars = "pointpillars"
+    pose_classification = "pose_classification"
+    re_identification = "re_identification"
+
 
 class network_type(str, enum.Enum):
+    """Class defining network types in enum"""
+
+    # TF1 CV networks
     detectnet_v2 = "detectnet_v2"
-    efficientdet = "efficientdet"
+    dssd = "dssd"
+    efficientdet_tf1 = "efficientdet_tf1"
     lprnet = "lprnet"
     unet = "unet"
     multitask_classification = "multitask_classification"
-    classification = "classification"
+    classification_tf1 = "classification_tf1"
     mask_rcnn = "mask_rcnn"
     ssd = "ssd"
     retinanet = "retinanet"
     faster_rcnn = "faster_rcnn"
     yolo_v3 = "yolo_v3"
     yolo_v4 = "yolo_v4"
     yolo_v4_tiny = "yolo_v4_tiny"
+    # TF1 DRIVEIX networks
+    bpnet = "bpnet"
+    fpenet = "fpenet"
+    # TF2 CV networks
+    classification_tf2 = "classification_tf2"
+    efficientdet_tf2 = "efficientdet_tf2"
+    # PYTORCH CV networks
+    action_recognition = "action_recognition"
+    classification_pyt = "classification_pyt"
+    deformable_detr = "deformable_detr"
+    dino = "dino"
+    mal = "mal"
+    ml_recog = "ml_recog"
+    ocdnet = "ocdnet"
+    ocrnet = "ocrnet"
+    optical_inspection = "optical_inspection"
+    pointpillars = "pointpillars"
+    pose_classification = "pose_classification"
+    segformer = "segformer"
+    re_identification = "re_identification"
+    # PYTORCH TTS
     spectro_gen = "spectro_gen"
     vocoder = "vocoder"
+    # Data Services
+    annotations = "annotations"
+    analytics = "analytics"
+    auto_label = "auto_label"
+    augmentation = "augmentation"
```

## tao_cli/login.py

```diff
@@ -1,22 +1,29 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""Login modules"""
 import requests
 import click
 import json
 import os
 
+
 @click.command()
 @click.option('--ngc-api-key', prompt='ngc_api_key', help='Your NGC API KEY.', required=True)
 def login(ngc_api_key):
+    """User login method"""
     base_url = os.getenv('BASE_URL', 'http://localhost/api/v1')
     endpoint = base_url + "/login/" + ngc_api_key
-    response = requests.get(endpoint)
+    response = requests.get(endpoint, timeout=600)
     click.echo(json.dumps(response.json()))
```

## tao_cli/tao.py

```diff
@@ -1,56 +1,113 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""Add click network groups to the cli command"""
 import click
 
 from tao_cli.login import login
 
+# TF1 CV networks
 from tao_cli.networks.detectnet_v2 import detectnet_v2
-from tao_cli.networks.efficientdet import efficientdet
+from tao_cli.networks.dssd import dssd
+from tao_cli.networks.efficientdet_tf1 import efficientdet_tf1
 from tao_cli.networks.lprnet import lprnet
 from tao_cli.networks.unet import unet
 from tao_cli.networks.multi_task_classification import multitask_classification
-from tao_cli.networks.multi_class_classification import classification
+from tao_cli.networks.multi_class_classification_tf1 import classification_tf1
 from tao_cli.networks.mask_rcnn import mask_rcnn
 from tao_cli.networks.ssd import ssd
 from tao_cli.networks.retinanet import retinanet
 from tao_cli.networks.faster_rcnn import faster_rcnn
 from tao_cli.networks.yolo_v3 import yolo_v3
 from tao_cli.networks.yolo_v4 import yolo_v4
 from tao_cli.networks.yolo_v4_tiny import yolo_v4_tiny
-from tao_cli.networks.spectro_gen import spectro_gen
-from tao_cli.networks.vocoder import vocoder
+# TF1 DRIVEIX networks
+from tao_cli.networks.bpnet import bpnet
+from tao_cli.networks.fpenet import fpenet
+# TF2 CV networks
+from tao_cli.networks.multi_class_classification_tf2 import classification_tf2
+from tao_cli.networks.efficientdet_tf2 import efficientdet_tf2
+# PYTORCH CV networks
+from tao_cli.networks.action_recognition import action_recognition
+from tao_cli.networks.multi_class_classification_pyt import classification_pyt
+from tao_cli.networks.mal import mal
+from tao_cli.networks.ml_recog import ml_recog
+from tao_cli.networks.ocdnet import ocdnet
+from tao_cli.networks.ocrnet import ocrnet
+from tao_cli.networks.optical_inspection import optical_inspection
+from tao_cli.networks.pointpillars import pointpillars
+from tao_cli.networks.pose_classification import pose_classification
+from tao_cli.networks.re_identification import re_identification
+from tao_cli.networks.segformer import segformer
+from tao_cli.networks.deformable_detr import deformable_detr
+from tao_cli.networks.dino import dino
+# Data Services
+from tao_cli.networks.annotations import annotations
+from tao_cli.networks.analytics import analytics
+from tao_cli.networks.auto_label import auto_label
+from tao_cli.networks.augmentation import augmentation
+
 
 @click.group()
 @click.version_option(package_name='nvidia-tao-client')
 @click.pass_context
 def cli(ctx):
+    """Create base nvidia-tao-client group"""
     pass
 
+
 cli.add_command(login)
+# TF1 CV networks
 cli.add_command(detectnet_v2)
-cli.add_command(efficientdet)
+cli.add_command(dssd)
+cli.add_command(efficientdet_tf2)
 cli.add_command(lprnet)
 cli.add_command(unet)
 cli.add_command(multitask_classification)
-cli.add_command(classification)
+cli.add_command(classification_tf1)
 cli.add_command(mask_rcnn)
 cli.add_command(ssd)
 cli.add_command(retinanet)
 cli.add_command(faster_rcnn)
 cli.add_command(yolo_v3)
 cli.add_command(yolo_v4)
 cli.add_command(yolo_v4_tiny)
-cli.add_command(spectro_gen)
-cli.add_command(vocoder)
+# TF1 DRIVEIX networks
+cli.add_command(bpnet)
+cli.add_command(fpenet)
+# TF2 CV networks
+cli.add_command(classification_tf2)
+cli.add_command(efficientdet_tf1)
+# PYTORCH CV networks
+cli.add_command(action_recognition)
+cli.add_command(classification_pyt)
+cli.add_command(mal)
+cli.add_command(ml_recog)
+cli.add_command(ocdnet)
+cli.add_command(ocrnet)
+cli.add_command(optical_inspection)
+cli.add_command(pointpillars)
+cli.add_command(pose_classification)
+cli.add_command(re_identification)
+cli.add_command(segformer)
+cli.add_command(deformable_detr)
+cli.add_command(dino)
+# Data Services
+cli.add_command(annotations)
+cli.add_command(analytics)
+cli.add_command(auto_label)
+cli.add_command(augmentation)
 
 if __name__ == '__main__':
     cli()
-
```

## tao_cli/cli_actions/__init__.py

```diff
@@ -0,0 +1,41 @@
+00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
+00000010: 3230 3233 2c20 4e56 4944 4941 2043 4f52  2023, NVIDIA COR
+00000020: 504f 5241 5449 4f4e 2e20 2041 6c6c 2072  PORATION.  All r
+00000030: 6967 6874 7320 7265 7365 7276 6564 2e0a  ights reserved..
+00000040: 230a 2320 4c69 6365 6e73 6564 2075 6e64  #.# Licensed und
+00000050: 6572 2074 6865 2041 7061 6368 6520 4c69  er the Apache Li
+00000060: 6365 6e73 652c 2056 6572 7369 6f6e 2032  cense, Version 2
+00000070: 2e30 2028 7468 6520 224c 6963 656e 7365  .0 (the "License
+00000080: 2229 3b0a 2320 796f 7520 6d61 7920 6e6f  ");.# you may no
+00000090: 7420 7573 6520 7468 6973 2066 696c 6520  t use this file 
+000000a0: 6578 6365 7074 2069 6e20 636f 6d70 6c69  except in compli
+000000b0: 616e 6365 2077 6974 6820 7468 6520 4c69  ance with the Li
+000000c0: 6365 6e73 652e 0a23 2059 6f75 206d 6179  cense..# You may
+000000d0: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+000000e0: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+000000f0: 0a23 0a23 2020 2020 2068 7474 703a 2f2f  .#.#     http://
+00000100: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+00000110: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00000120: 322e 300a 230a 2320 556e 6c65 7373 2072  2.0.#.# Unless r
+00000130: 6571 7569 7265 6420 6279 2061 7070 6c69  equired by appli
+00000140: 6361 626c 6520 6c61 7720 6f72 2061 6772  cable law or agr
+00000150: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
+00000160: 672c 2073 6f66 7477 6172 650a 2320 6469  g, software.# di
+00000170: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00000180: 7468 6520 4c69 6365 6e73 6520 6973 2064  the License is d
+00000190: 6973 7472 6962 7574 6564 206f 6e20 616e  istributed on an
+000001a0: 2022 4153 2049 5322 2042 4153 4953 2c0a   "AS IS" BASIS,.
+000001b0: 2320 5749 5448 4f55 5420 5741 5252 414e  # WITHOUT WARRAN
+000001c0: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
+000001d0: 4e53 204f 4620 414e 5920 4b49 4e44 2c20  NS OF ANY KIND, 
+000001e0: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
+000001f0: 7220 696d 706c 6965 642e 0a23 2053 6565  r implied..# See
+00000200: 2074 6865 204c 6963 656e 7365 2066 6f72   the License for
+00000210: 2074 6865 2073 7065 6369 6669 6320 6c61   the specific la
+00000220: 6e67 7561 6765 2067 6f76 6572 6e69 6e67  nguage governing
+00000230: 2070 6572 6d69 7373 696f 6e73 2061 6e64   permissions and
+00000240: 0a23 206c 696d 6974 6174 696f 6e73 2075  .# limitations u
+00000250: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00000260: 2e0a 0a22 2222 5441 4f20 636c 6965 6e74  ..."""TAO client
+00000270: 2063 6c69 2061 6374 696f 6e73 206d 6f64   cli actions mod
+00000280: 756c 6522 2222 0a                        ule""".
```

## tao_cli/cli_actions/actions.py

```diff
@@ -1,48 +1,62 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""TAO-Client base actions module"""
 import json
 import requests
 import os
 
+
 class Actions:
+    """Base class which defines API functions for general actions"""
+
     def __init__(self):
+        """Initialize the actions base class"""
         self.user = os.getenv('USER', 'nobody')
         self.base_url = os.getenv('BASE_URL', 'http://localhost/api/v1/') + f"/user/{self.user}"
         self.token = os.getenv('TOKEN', 'invalid')
         self.headers = {"Authorization": f"Bearer {self.token}"}
         self.sub_action = self.__class__.__name__.lower()
 
     def get_action_spec(self, id, action):
-        endpoint = self.base_url + "/{}/{}/specs/{}/schema".format(self.sub_action, id, action)
-        response = requests.get(endpoint, headers=self.headers)
+        """Return spec dictionary for the action passed"""
+        endpoint = self.base_url + f"/{self.sub_action}/{id}/specs/{action}/schema"
+        response = requests.get(endpoint, headers=self.headers, timeout=600)
         data = response.json()["default"]
         return data
 
     def get_automl_defaults(self, id, action):
-        endpoint = self.base_url + "/{}/{}/specs/{}/schema".format(self.sub_action, id, action)
-        response = requests.get(endpoint, headers=self.headers)
+        """Return automl parameters enabled for a network"""
+        endpoint = self.base_url + f"/{self.sub_action}/{id}/specs/{action}/schema"
+        response = requests.get(endpoint, headers=self.headers, timeout=600)
         data = response.json()["automl_default_parameters"]
         return data
 
     def run_action(self, id, job, action):
-        data = json.dumps( { "job": job, "actions": action } )
-        endpoint = self.base_url + "/{}/{}/job".format(self.sub_action, id)
-        response = requests.post(endpoint, data=data, headers=self.headers)
+        """Submit post request for an action"""
+        data = json.dumps({"job": job, "actions": action})
+        endpoint = self.base_url + f"/{self.sub_action}/{id}/job"
+        response = requests.post(endpoint, data=data, headers=self.headers, timeout=600)
         job_id = response.json()[0]
         return job_id
 
     def model_job_cancel(self, id, job):
-        endpoint = self.base_url + "/{}/{}/job/{}/cancel".format(self.sub_action, id, job)
-        response = requests.post(endpoint, headers=self.headers)
+        """Pause a running job"""
+        endpoint = self.base_url + f"/{self.sub_action}/{id}/job/{job}/cancel"
+        requests.post(endpoint, headers=self.headers, timeout=600)
 
     def model_job_resume(self, id, job):
-        endpoint = self.base_url + "/{}/{}/job/{}/resume".format(self.sub_action, id, job)
-        response = requests.post(endpoint, headers=self.headers)
+        """Resume a paused job"""
+        endpoint = self.base_url + f"/{self.sub_action}/{id}/job/{job}/resume"
+        requests.post(endpoint, headers=self.headers, timeout=600)
```

## tao_cli/cli_actions/dataset.py

```diff
@@ -1,25 +1,35 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""TAO-Client dataset module"""
 import json
 import requests
 
 from tao_cli.cli_actions.actions import Actions
 
+
 class Dataset(Actions):
-    def __init__(self):
-        super().__init__()
+    """Class which defines API functions for dataset specific actions"""
+
+    # def __init__(self):
+    #     """Intialize Dataset class"""
+    #     super().__init__()
 
     def dataset_create(self, dataset_type, dataset_format):
-        data = json.dumps( {"type": dataset_type, "format": dataset_format} )
+        """Create a dataset and return the id"""
+        data = json.dumps({"type": dataset_type, "format": dataset_format})
         endpoint = self.base_url + "/dataset"
-        response = requests.post(endpoint, data=data, headers=self.headers)
+        response = requests.post(endpoint, data=data, headers=self.headers, timeout=600)
         id = response.json()["id"]
         return id
```

## tao_cli/cli_actions/model.py

```diff
@@ -1,25 +1,35 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+"""TAO-Client model module"""
 import json
 import requests
 
 from tao_cli.cli_actions.actions import Actions
 
+
 class Model(Actions):
-    def __init__(self):
-        super().__init__()
+    """Class which defines API functions for model specific actions"""
+
+    # def __init__(self):
+    #     """Intialize Model class"""
+    #     super().__init__()
 
     def model_create(self, network_arch, encryption_key):
-        data = json.dumps( {"network_arch": network_arch, "encryption_key": encryption_key} )
+        """Create a model and return the id"""
+        data = json.dumps({"network_arch": network_arch, "encryption_key": encryption_key})
         endpoint = self.base_url + "/model"
-        response = requests.post(endpoint, data=data, headers=self.headers)
+        response = requests.post(endpoint, data=data, headers=self.headers, timeout=600)
         id = response.json()["id"]
         return id
```

## tao_cli/networks/__init__.py

```diff
@@ -0,0 +1,41 @@
+00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
+00000010: 3230 3233 2c20 4e56 4944 4941 2043 4f52  2023, NVIDIA COR
+00000020: 504f 5241 5449 4f4e 2e20 2041 6c6c 2072  PORATION.  All r
+00000030: 6967 6874 7320 7265 7365 7276 6564 2e0a  ights reserved..
+00000040: 230a 2320 4c69 6365 6e73 6564 2075 6e64  #.# Licensed und
+00000050: 6572 2074 6865 2041 7061 6368 6520 4c69  er the Apache Li
+00000060: 6365 6e73 652c 2056 6572 7369 6f6e 2032  cense, Version 2
+00000070: 2e30 2028 7468 6520 224c 6963 656e 7365  .0 (the "License
+00000080: 2229 3b0a 2320 796f 7520 6d61 7920 6e6f  ");.# you may no
+00000090: 7420 7573 6520 7468 6973 2066 696c 6520  t use this file 
+000000a0: 6578 6365 7074 2069 6e20 636f 6d70 6c69  except in compli
+000000b0: 616e 6365 2077 6974 6820 7468 6520 4c69  ance with the Li
+000000c0: 6365 6e73 652e 0a23 2059 6f75 206d 6179  cense..# You may
+000000d0: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+000000e0: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+000000f0: 0a23 0a23 2020 2020 2068 7474 703a 2f2f  .#.#     http://
+00000100: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+00000110: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00000120: 322e 300a 230a 2320 556e 6c65 7373 2072  2.0.#.# Unless r
+00000130: 6571 7569 7265 6420 6279 2061 7070 6c69  equired by appli
+00000140: 6361 626c 6520 6c61 7720 6f72 2061 6772  cable law or agr
+00000150: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
+00000160: 672c 2073 6f66 7477 6172 650a 2320 6469  g, software.# di
+00000170: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00000180: 7468 6520 4c69 6365 6e73 6520 6973 2064  the License is d
+00000190: 6973 7472 6962 7574 6564 206f 6e20 616e  istributed on an
+000001a0: 2022 4153 2049 5322 2042 4153 4953 2c0a   "AS IS" BASIS,.
+000001b0: 2320 5749 5448 4f55 5420 5741 5252 414e  # WITHOUT WARRAN
+000001c0: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
+000001d0: 4e53 204f 4620 414e 5920 4b49 4e44 2c20  NS OF ANY KIND, 
+000001e0: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
+000001f0: 7220 696d 706c 6965 642e 0a23 2053 6565  r implied..# See
+00000200: 2074 6865 204c 6963 656e 7365 2066 6f72   the License for
+00000210: 2074 6865 2073 7065 6369 6669 6320 6c61   the specific la
+00000220: 6e67 7561 6765 2067 6f76 6572 6e69 6e67  nguage governing
+00000230: 2070 6572 6d69 7373 696f 6e73 2061 6e64   permissions and
+00000240: 0a23 206c 696d 6974 6174 696f 6e73 2075  .# limitations u
+00000250: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00000260: 2e0a 0a22 2222 5441 4f2d 436c 6965 6e74  ..."""TAO-Client
+00000270: 2069 6e64 6976 6964 7561 6c20 6e65 7477   individual netw
+00000280: 6f72 6b20 6d6f 6475 6c65 7322 2222 0a    ork modules""".
```

## tao_cli/networks/detectnet_v2.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# DETECTNET_V2
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""DetectNet V2 tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def detectnet_v2():
+    """Create DetectNet V2 model click group"""
     pass
 
+
 @detectnet_v2.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @detectnet_v2.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @detectnet_v2.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/faster_rcnn.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# Faster-RCNN
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""FasterRCNN tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def faster_rcnn():
+    """Create FasterRCNN model click group"""
     pass
 
+
 @faster_rcnn.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @faster_rcnn.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @faster_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/lprnet.py

```diff
@@ -1,159 +1,203 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# LPRNET
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""LPRNET tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def lprnet():
+    """Create LPRNET model click group"""
     pass
 
+
 @lprnet.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @lprnet.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @lprnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/mask_rcnn.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# MaskRCNN
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""MaskRCNN tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def mask_rcnn():
+    """Create MaskRCNN model click group"""
     pass
 
+
 @mask_rcnn.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @mask_rcnn.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @mask_rcnn.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/multi_task_classification.py

```diff
@@ -1,159 +1,203 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# Multi-task Classification
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Multi-task classification tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def multitask_classification():
+    """Create Multi-task classification model click group"""
     pass
 
+
 @multitask_classification.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @multitask_classification.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @multitask_classification.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/retinanet.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# RetinaNet
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""RetinaNet tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def retinanet():
+    """Create RetinaNet model click group"""
     pass
 
+
 @retinanet.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @retinanet.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @retinanet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/ssd.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# SSD
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""SSD tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def ssd():
+    """Create SSD model click group"""
     pass
 
+
 @ssd.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @ssd.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @ssd.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/unet.py

```diff
@@ -1,159 +1,203 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# Unet
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Unet tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def unet():
+    """Create Unet model click group"""
     pass
 
+
 @unet.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @unet.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @unet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/yolo_v3.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# YOLO V3
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""YOLO v3 tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def yolo_v3():
+    """Create YOLO v3 model click group"""
     pass
 
+
 @yolo_v3.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v3.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v3.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/yolo_v4.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# YOLO V3
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""YOLO v4 tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def yolo_v4():
+    """Create YOLO v4 model click group"""
     pass
 
+
 @yolo_v4.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v4.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v4.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## tao_cli/networks/yolo_v4_tiny.py

```diff
@@ -1,173 +1,221 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# YOLO V3
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""YOLO v4 tiny tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
 def yolo_v4_tiny():
+    """Create YOLO v4 tiny model click group"""
     pass
 
+
 @yolo_v4_tiny.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert_defaults(id, action):
+    """Return default dataset convert spec"""
     data = dataset_obj.get_action_spec(id, action)
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The dataset ID.', required=True)
 @click.option('--action', prompt='action', help='The dataset convert action.', required=True)
 def dataset_convert(id, action):
+    """Run dataset_convert action"""
     job_id = dataset_obj.run_action(id=id, job=None, action=[action])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
+
 @yolo_v4_tiny.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## Comparing `tao_cli/networks/efficientdet.py` & `tao_cli/networks/optical_inspection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,173 +1,169 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# EfficientDet
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""OCRNET tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
-def efficientdet():
+def optical_inspection():
+    """Create DetectNet V2 model click group"""
     pass
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The dataset ID.', required=True)
-@click.option('--action', prompt='action', help='The dataset convert action.', required=True)
-def dataset_convert_defaults(id, action):
-    data = dataset_obj.get_action_spec(id, action)
-    click.echo(json.dumps(data, indent=2))
-
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The dataset ID.', required=True)
-@click.option('--action', prompt='action', help='The dataset convert action.', required=True)
-def dataset_convert(id, action):
-    job_id = dataset_obj.run_action(id=id, job=None, action=[action])
-    click.echo(f"{job_id}")
 
-@efficientdet.command()
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def dataset_job_cancel(id, job):
+    """Pause/Cancel a running dataset job"""
     job = dataset_obj.dataset_job_cancel(id, job)
     click.echo(f"{job}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_prune_defaults(id):
-    data = model_obj.get_action_spec(id, "prune")
-    click.echo(json.dumps(data, indent=2))
-
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train job ID.', required=False, default=None)
-def model_prune(id, job):
-    job_id = model_obj.run_action(id, job, ["prune"])
-    click.echo(f"{job_id}")
 
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_retrain_defaults(id):
-    data = model_obj.get_action_spec(id, "retrain")
-    click.echo(json.dumps(data, indent=2))
-
-@efficientdet.command()
-@click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The prune job ID.', required=False, default=None)
-def model_retrain(id, job):
-    job_id = model_obj.run_action(id, job, ["retrain"])
-    click.echo(f"{job_id}")
-
-@efficientdet.command()
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
-@efficientdet.command()
+
+@optical_inspection.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## Comparing `tao_cli/networks/multi_class_classification.py` & `tao_cli/networks/ocdnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,194 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: LicenseRef-NvidiaProprietary
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
 #
-# NVIDIA CORPORATION, its affiliates and licensors retain all intellectual
-# property and proprietary rights in and to this material, related
-# documentation and any modifications thereto. Any use, reproduction,
-# disclosure or distribution of this material and related documentation
-# without an express license agreement from NVIDIA CORPORATION or
-# its affiliates is strictly prohibited.
-
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# Multi-Class Classification
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""OCRNET tao-client modules"""
 import click
 import json
 
 from tao_cli.cli_actions.dataset import Dataset
 from tao_cli.cli_actions.model import Model
 
 from tao_cli.constants import dataset_format, dataset_type, network_type
 
 dataset_obj = Dataset()
 model_obj = Model()
 
+
 @click.group()
-def classification():
+def ocdnet():
+    """Create DetectNet V2 model click group"""
     pass
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--dataset_type', prompt='dataset_type', type=click.Choice(dataset_type), help='The dataset type.', required=True)
 @click.option('--dataset_format', prompt='dataset_format', type=click.Choice(dataset_format), help='The dataset format.', required=True)
 def dataset_create(dataset_type, dataset_format):
+    """Create a dataset and return the id"""
     id = dataset_obj.dataset_create(dataset_type, dataset_format)
     click.echo(f"{id}")
 
-@classification.command()
-@click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', prompt='job', help='The job ID.', required=True)
-def dataset_job_cancel(id, job):
-    job = dataset_obj.dataset_job_cancel(id, job)
-    click.echo(f"{job}")
 
-@classification.command()
+@ocdnet.command()
 @click.option('--network_arch', prompt='network_arch', type=click.Choice(network_type), help='Network architecture.', required=True)
 @click.option('--encryption_key', prompt='encryption_key', help='Encryption_key.', required=True)
 def model_create(network_arch, encryption_key):
+    """Create a model and return the id"""
     id = model_obj.model_create(network_arch, encryption_key)
     click.echo(f"{id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_train_defaults(id):
+    """Return default train spec"""
     data = model_obj.get_action_spec(id, "train")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_automl_defaults(id):
+    """Return default automl parameters"""
     data = model_obj.get_automl_defaults(id, "train")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The dataset convert job ID.', required=False, default=None)
 def model_train(id, job):
+    """Run train action"""
     job_id = model_obj.run_action(id, job, ["train"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_evaluate_defaults(id):
+    """Return default evaluate spec"""
     data = model_obj.get_action_spec(id, "evaluate")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_evaluate(id, job):
+    """Run evaluate action"""
     job_id = model_obj.run_action(id, job, ["evaluate"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_export_defaults(id):
+    """Return default export spec"""
     data = model_obj.get_action_spec(id, "export")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train, prune or retrain job ID.', required=False, default=None)
 def model_export(id, job):
+    """Run export action"""
     job_id = model_obj.run_action(id, job, ["export"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-def model_convert_defaults(id):
-    data = model_obj.get_action_spec(id, "convert")
+def model_gen_trt_engine_defaults(id):
+    """Return default gen_trt_engine spec"""
+    data = model_obj.get_action_spec(id, "gen_trt_engine")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The export job ID.', required=False, default=None)
-def model_convert(id, job):
-    job_id = model_obj.run_action(id, job, ["convert"])
+def model_gen_trt_engine(id, job):
+    """Run gen_trt_engine action"""
+    job_id = model_obj.run_action(id, job, ["gen_trt_engine"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_inference_defaults(id):
+    """Return default inference spec"""
     data = model_obj.get_action_spec(id, "inference")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
-@click.option('--job', help='The train, prune, retrain, export or convert job ID.', required=False, default=None)
+@click.option('--job', help='The train, prune, retrain, export or gen_trt_engine job ID.', required=False, default=None)
 def model_inference(id, job):
+    """Run inference action"""
     job_id = model_obj.run_action(id, job, ["inference"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_prune_defaults(id):
+    """Return default prune spec"""
     data = model_obj.get_action_spec(id, "prune")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The train job ID.', required=False, default=None)
 def model_prune(id, job):
+    """Run prune action"""
     job_id = model_obj.run_action(id, job, ["prune"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 def model_retrain_defaults(id):
+    """Return default retrain spec"""
     data = model_obj.get_action_spec(id, "retrain")
     click.echo(json.dumps(data, indent=2))
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', help='The prune job ID.', required=False, default=None)
 def model_retrain(id, job):
+    """Run retrain action"""
     job_id = model_obj.run_action(id, job, ["retrain"])
     click.echo(f"{job_id}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_cancel(id, job):
+    """Pause a running job"""
     model_obj.model_job_cancel(id, job)
     click.echo(f"{job}")
 
-@classification.command()
+
+@ocdnet.command()
 @click.option('--id', prompt='id', help='The model ID.', required=True)
 @click.option('--job', prompt='job', help='The job ID.', required=True)
 def model_job_resume(id, job):
+    """Resume a paused job"""
     model_obj.model_job_resume(id, job)
     click.echo(f"{job}")
```

## Comparing `nvidia_tao_client-4.0.1.dist-info/METADATA` & `nvidia_tao_client-5.0.0.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: nvidia-tao-client
-Version: 4.0.1
-Summary: NVIDIA's TAO Client for TAO Toolkit.
-Home-page: UNKNOWN
-Author: Steve Masson
-Author-email: smasson@nvidia.com
+Version: 5.0.0.1
+Summary: NVIDIA's package for using REST-API via TAO-Client.
+Author: Varun Praveen
+Author-email: vpraveen@nvidia.com
 License: NVIDIA Proprietary Software
-Keywords: nvidia,tao,client,cli
-Platform: UNKNOWN
+Keywords: nvidia,tao,api
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: requests (>=2.27.1)
 
-UNKNOWN
-
```

