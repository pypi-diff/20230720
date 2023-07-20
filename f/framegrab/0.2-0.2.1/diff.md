# Comparing `tmp/framegrab-0.2.tar.gz` & `tmp/framegrab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.2.tar", max compression
+gzip compressed data, was "framegrab-0.2.1.tar", max compression
```

## Comparing `framegrab-0.2.tar` & `framegrab-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.2/LICENSE.txt
--rw-r--r--   0        0        0     5638 2023-07-07 20:44:56.340056 framegrab-0.2/README.md
--rw-r--r--   0        0        0      485 2023-07-07 20:44:56.340418 framegrab-0.2/pyproject.toml
--rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.2/src/framegrab/__init__.py
--rw-r--r--   0        0        0    30230 2023-07-07 20:44:56.340879 framegrab-0.2/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2456 2023-07-07 20:44:37.695695 framegrab-0.2/src/framegrab/motion.py
--rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 framegrab-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     5638 2023-07-07 20:44:56.340056 framegrab-0.2.1/README.md
+-rw-r--r--   0        0        0      487 2023-07-20 16:25:40.616168 framegrab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.2.1/src/framegrab/__init__.py
+-rw-r--r--   0        0        0    30853 2023-07-20 16:13:43.312030 framegrab-0.2.1/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2533 2023-07-20 16:25:40.616496 framegrab-0.2.1/src/framegrab/motion.py
+-rw-r--r--   0        0        0     6410 1970-01-01 00:00:00.000000 framegrab-0.2.1/PKG-INFO
```

### Comparing `framegrab-0.2/LICENSE.txt` & `framegrab-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.2/README.md` & `framegrab-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `framegrab-0.2/src/framegrab/grabber.py` & `framegrab-0.2.1/src/framegrab/grabber.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,17 @@
         """Check the config to ensure it conforms to the required format and data types
         Returns a corrected version of the config.
         """
         output_config = config.copy()
 
         # Ensure that serial numbers are strings
         try:
-            output_config["id"]["serial_number"] = str(output_config["id"]["serial_number"])
+            output_config["id"]["serial_number"] = str(
+                output_config["id"]["serial_number"]
+            )
         except KeyError:
             pass
 
         # Ensure that there are some options, even if they are empty
         if not output_config.get("options"):
             output_config["options"] = {}
 
@@ -100,15 +102,17 @@
 
         # Ensure the config is properly constructed and typed
         config = FrameGrabber._validate_config(config)
 
         # At a minimum, input_type must be provided
         input_type = config.get("input_type", None)
         if input_type is None:
-            raise ValueError(f"No input_type provided. Valid types are {InputTypes.get_options()}")
+            raise ValueError(
+                f"No input_type provided. Valid types are {InputTypes.get_options()}"
+            )
 
         # Based on input_type, create correct type of FrameGrabber
         if input_type == InputTypes.WEBCAM:
             grabber = WebcamFrameGrabber(config)
         elif input_type == InputTypes.RTSP:
             grabber = RTSPFrameGrabber(config)
         elif input_type == InputTypes.BASLER_USB:
@@ -166,37 +170,45 @@
 
     def _crop(self, frame: np.ndarray) -> np.ndarray:
         """Looks at FrameGrabber's options and decides to either crop in an absolute manner (by pixels) or
         in a relative manner (normalized).
 
         Returns a cropped frame.
         """
-        absolute_crop_params = self.config.get("options", {}).get("crop", {}).get("absolute")
+        absolute_crop_params = (
+            self.config.get("options", {}).get("crop", {}).get("absolute")
+        )
         if absolute_crop_params:
             return self._crop_absolute(frame, absolute_crop_params)
 
-        relative_crop_params = self.config.get("options", {}).get("crop", {}).get("relative")
+        relative_crop_params = (
+            self.config.get("options", {}).get("crop", {}).get("relative")
+        )
         if relative_crop_params:
             return self._crop_relative(frame, relative_crop_params)
 
         return frame
 
-    def _crop_absolute(self, frame: np.ndarray, crop_params: Dict[str, int]) -> np.ndarray:
+    def _crop_absolute(
+        self, frame: np.ndarray, crop_params: Dict[str, int]
+    ) -> np.ndarray:
         """Crops the provided frame according to the FrameGrabbers cropping configuration.
         Crops according to pixels positions.
         """
         top = crop_params.get("top", 0)
         bottom = crop_params.get("bottom", frame.shape[0])
         left = crop_params.get("left", 0)
         right = crop_params.get("right", frame.shape[1])
         frame = frame[top:bottom, left:right]
 
         return frame
 
-    def _crop_relative(self, frame: np.ndarray, crop_params: Dict[str, float]) -> np.ndarray:
+    def _crop_relative(
+        self, frame: np.ndarray, crop_params: Dict[str, float]
+    ) -> np.ndarray:
         """Crops the provided frame according to the FrameGrabbers cropping configuration.
         Crops according to relative positions (0-1).
         """
         top = crop_params.get("top", 0) * frame.shape[0]
         bottom = crop_params.get("bottom", 1) * frame.shape[0]
         left = crop_params.get("left", 0) * frame.shape[1]
         right = crop_params.get("right", 1) * frame.shape[1]
@@ -297,15 +309,17 @@
                 if idx in WebcamFrameGrabber.indices_in_use:
                     continue  # Webcam is already in use, moving on
 
                 capture = cv2.VideoCapture(idx)
                 if capture.isOpened():
                     break  # Found a valid capture, no need to look any further
             else:
-                raise ValueError(f"Unable to connect to webcam by index. Is your webcam plugged in?")
+                raise ValueError(
+                    f"Unable to connect to webcam by index. Is your webcam plugged in?"
+                )
 
         # A valid capture has been found, saving it for later
         self.capture = capture
 
         # Log the current webcam index as 'in use' to prevent other WebcamFrameGrabbers from stepping on it
         self.idx = idx
         WebcamFrameGrabber.indices_in_use.add(idx)
@@ -334,34 +348,40 @@
         and actual plugged in devices.
 
         This function only works on Linux, and was specifically tested on an Nvidia Jetson.
         """
 
         # ls /dev/video* returns device paths for all plugged in webcams
         command = "ls /dev/video*"
-        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        process = subprocess.Popen(
+            command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+        )
         stdout, _ = process.communicate()
         output = stdout.decode("utf-8")
         devices = output.strip().split("\n")
 
         plugged_in_devices = {}
         for devpath in devices:
             # ls -l /sys/class/video4linux/video0/device returns a path that points back into the /sys/bus/usb/devices/
             # directory where can determine the serial number.
             # e.g. /sys/bus/usb/devices/2-3.2:1.0 -> /sys/bus/usb/devices/<bus>-<port>.<subport>:<config>.<interface>
             devname = devpath.split("/")[-1]
             command = f"ls -l /sys/class/video4linux/{devname}/device"
-            process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            process = subprocess.Popen(
+                command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+            )
             stdout, _ = process.communicate()
             output = stdout.decode("utf-8")
             bus_port_subport = output.split("/")[-1].split(":")[0]
 
             # find the serial number
             command = f"cat /sys/bus/usb/devices/{bus_port_subport}/serial"
-            process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            process = subprocess.Popen(
+                command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+            )
             stdout, _ = process.communicate()
             serial_number = stdout.decode("utf-8").strip()
 
             if serial_number:
                 plugged_in_devices[devpath] = serial_number
 
         return plugged_in_devices
@@ -377,24 +397,29 @@
     """
 
     def __init__(self, config: dict):
         self.config = config
 
         stream = self.config.get("address", {}).get("rtsp_url")
         if not stream:
-            raise ValueError(f"No RTSP URL provided. " "Please add an address attribute to the configuration.")
+            raise ValueError(
+                f"No RTSP URL provided. "
+                "Please add an address attribute to the configuration."
+            )
         self.capture = cv2.VideoCapture(stream)
 
         if not self.capture.isOpened():
             raise ValueError(
                 f"Could not open RTSP stream: {stream}. "
                 "Is the RSTP URL correct? Is the camera connected to the network?"
             )
 
-        logger.debug(f"Initialized video capture with backend={self.capture.getBackendName()}")
+        logger.debug(
+            f"Initialized video capture with backend={self.capture.getBackendName()}"
+        )
 
         self.run = True
         self.lock = Lock()
         Thread(target=self._drain).start()
 
     def grab(self) -> np.ndarray:
         with self.lock:
@@ -441,27 +466,33 @@
 
         self.config = config
 
         tlf = pylon.TlFactory.GetInstance()
         devices = tlf.EnumerateDevices()
 
         if not devices:
-            raise ValueError("No Basler USB cameras were found. Is your camera plugged in?")
+            raise ValueError(
+                "No Basler USB cameras were found. Is your camera plugged in?"
+            )
 
         # Attempt to match the provided serial number with a plugged in device. If no serial number was provided, just
         # pick the first found device that is not currently in use.
         serial_number = config.get("id", {}).get("serial_number")
         for device in devices:
             curr_serial_number = device.GetSerialNumber()
             if curr_serial_number in BaslerUSBFrameGrabber.serial_numbers_in_use:
                 continue
             if serial_number is None or serial_number == curr_serial_number:
-                camera = pylon.InstantCamera(pylon.TlFactory.GetInstance().CreateDevice(device))
+                camera = pylon.InstantCamera(
+                    pylon.TlFactory.GetInstance().CreateDevice(device)
+                )
                 camera.Open()
-                logger.info(f"Connected to Basler USB camera with serial number {curr_serial_number}.")
+                logger.info(
+                    f"Connected to Basler USB camera with serial number {curr_serial_number}."
+                )
                 break
         else:
             raise ValueError(
                 f"Unable to connect to Basler USB camera with serial number: {serial_number}. "
                 "Please verify that the camera is plugged in and that the serial number is correct."
             )
 
@@ -517,26 +548,31 @@
                 "Please install pyrealsense2 and try again."
             )
 
         self.config = config
 
         ctx = rs.context()
         if len(ctx.devices) == 0:
-            raise ValueError(f"No Intel RealSense cameras detected. Is your camera plugged in?")
+            raise ValueError(
+                f"No Intel RealSense cameras detected. Is your camera plugged in?"
+            )
 
         provided_serial_number = self.config.get("id", {}).get("serial_number")
 
         # Iterate through each detected camera and attempt to match it with the provided camera config
         for device in ctx.devices:
             pipeline = rs.pipeline()
             rs_config = rs.config()
 
             curr_serial_number = device.get_info(rs.camera_info.serial_number)
 
-            if provided_serial_number is None or curr_serial_number == provided_serial_number:
+            if (
+                provided_serial_number is None
+                or curr_serial_number == provided_serial_number
+            ):
                 rs_config.enable_device(curr_serial_number)
 
                 # Try to connect to the camera
                 try:
                     pipeline_profile = pipeline.start(rs_config)
                     break  # succesfully connected, breaking out of loop
                 except RuntimeError as e:
@@ -555,41 +591,51 @@
     def grab(self) -> np.ndarray:
         frames = self.pipeline.wait_for_frames()
         depth_frame = frames.get_depth_frame()
         color_frame = frames.get_color_frame()
 
         # Convert images to numpy arrays and convet from RGB to BGR
         depth_image = np.asanyarray(depth_frame.get_data())
-        color_image = cv2.cvtColor(np.asanyarray(color_frame.get_data()), cv2.COLOR_BGR2RGB)
+        color_image = cv2.cvtColor(
+            np.asanyarray(color_frame.get_data()), cv2.COLOR_BGR2RGB
+        )
 
         depth_image = self._crop(depth_image)
         depth_image = self._digital_zoom(depth_image)
 
         color_image = self._crop(color_image)
         color_image = self._digital_zoom(color_image)
 
         # side by side
-        display_side_by_side = self.config.get("options", {}).get("depth", {}).get("side_by_side")
+        display_side_by_side = (
+            self.config.get("options", {}).get("depth", {}).get("side_by_side")
+        )
         if display_side_by_side:
             return self._side_by_side(depth_image, color_image)
         else:
             return color_image
 
-    def _side_by_side(self, depth_image: np.ndarray, color_image: np.ndarray) -> np.ndarray:
+    def _side_by_side(
+        self, depth_image: np.ndarray, color_image: np.ndarray
+    ) -> np.ndarray:
         """Merges color image and depth image into a wider image, all in RGB"""
 
         # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
-        depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_BONE)
+        depth_colormap = cv2.applyColorMap(
+            cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_BONE
+        )
         depth_colormap_dim = depth_colormap.shape
         color_colormap_dim = color_image.shape
 
         # If depth and color resolutions are different, resize color image to match depth image for display
         if depth_colormap_dim != color_colormap_dim:
             resized_color_image = cv2.resize(
-                color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA
+                color_image,
+                dsize=(depth_colormap_dim[1], depth_colormap_dim[0]),
+                interpolation=cv2.INTER_AREA,
             )
             sidebyside = np.hstack((resized_color_image, depth_colormap))
         else:
             sidebyside = np.hstack((color_image, depth_colormap))
         return sidebyside
 
     def release(self) -> None:
```

### Comparing `framegrab-0.2/src/framegrab/motion.py` & `framegrab-0.2.1/src/framegrab/motion.py`

 * *Files 21% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         if self.unused:
             self.base_img = new_img
             self.base2 = self.base_img
             self.unused = False
             return True
 
         new_img16 = new_img.astype(np.int16)
+
+        if new_img16.shape != self.base_img.shape:
+            return True
+
         diff1 = np.abs(new_img16 - self.base_img) > self.threshold
         diff2 = np.abs(new_img16 - self.base2) > self.threshold
 
         self.base2 = self.base_img
         self.base_img = new_img
         binarized = (
             diff1 & diff2
```

### Comparing `framegrab-0.2/PKG-INFO` & `framegrab-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.2
+Version: 0.2.1
 Summary: Easily grab frames from cameras or streams
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

