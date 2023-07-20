# Comparing `tmp/chichitk-0.0.3.tar.gz` & `tmp/chichitk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chichitk-0.0.3.tar", last modified: Sat Apr 29 23:45:06 2023, max compression
+gzip compressed data, was "chichitk-0.0.4.tar", last modified: Thu Jul 20 15:27:11 2023, max compression
```

## Comparing `chichitk-0.0.3.tar` & `chichitk-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.329406 chichitk-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-16 02:22:07.000000 chichitk-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3375 2023-04-29 23:45:06.328408 chichitk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-04-22 16:09:51.000000 chichitk-0.0.3/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.303208 chichitk-0.0.3/chichitk/
--rw-rw-rw-   0        0        0      699 2023-04-29 22:46:55.000000 chichitk-0.0.3/chichitk/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-04-17 00:34:05.000000 chichitk-0.0.3/chichitk/aspect_frame.py
--rw-rw-rw-   0        0        0    26614 2023-04-21 01:55:06.000000 chichitk-0.0.3/chichitk/buttons.py
--rw-rw-rw-   0        0        0    49997 2023-04-16 02:08:01.000000 chichitk-0.0.3/chichitk/canvas_items.py
--rw-rw-rw-   0        0        0     6834 2023-04-29 23:10:26.000000 chichitk-0.0.3/chichitk/collapse_frame.py
--rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.3/chichitk/dropdowns.py
--rw-rw-rw-   0        0        0     8943 2023-04-22 15:48:45.000000 chichitk-0.0.3/chichitk/entry_boxes.py
--rw-rw-rw-   0        0        0     6098 2023-04-18 17:15:53.000000 chichitk-0.0.3/chichitk/file_dialog.py
--rw-rw-rw-   0        0        0     4288 2023-04-16 21:18:55.000000 chichitk-0.0.3/chichitk/function_progress.py
--rw-rw-rw-   0        0        0    34820 2023-04-18 17:09:52.000000 chichitk-0.0.3/chichitk/icons.py
--rw-rw-rw-   0        0        0    23868 2023-04-29 03:36:03.000000 chichitk-0.0.3/chichitk/labels.py
--rw-rw-rw-   0        0        0    10238 2023-04-21 01:24:23.000000 chichitk-0.0.3/chichitk/pdf_display.py
--rw-rw-rw-   0        0        0     7301 2023-04-16 23:35:43.000000 chichitk-0.0.3/chichitk/player.py
--rw-rw-rw-   0        0        0     5152 2023-03-24 16:40:10.000000 chichitk-0.0.3/chichitk/progress_bar.py
--rw-rw-rw-   0        0        0     3990 2023-04-20 02:51:35.000000 chichitk-0.0.3/chichitk/scrollable_frame.py
--rw-rw-rw-   0        0        0    66444 2023-04-17 23:52:20.000000 chichitk-0.0.3/chichitk/sliders.py
--rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.3/chichitk/temp_menu.py
--rw-rw-rw-   0        0        0    11203 2023-04-19 18:24:06.000000 chichitk-0.0.3/chichitk/text_boxes.py
--rw-rw-rw-   0        0        0     9855 2023-04-15 18:26:04.000000 chichitk-0.0.3/chichitk/timer.py
--rw-rw-rw-   0        0        0     6880 2023-03-23 19:14:50.000000 chichitk-0.0.3/chichitk/tool_tip.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.326280 chichitk-0.0.3/chichitk.egg-info/
--rw-rw-rw-   0        0        0     3375 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1161 2023-04-29 23:42:20.000000 chichitk-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 23:45:06.330404 chichitk-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 15:27:11.392752 chichitk-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 02:22:07.000000 chichitk-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3375 2023-07-20 15:27:11.375629 chichitk-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2637 2023-04-22 16:09:51.000000 chichitk-0.0.4/Readme.md
+drwxrwxrwx   0        0        0        0 2023-07-20 15:27:11.328982 chichitk-0.0.4/chichitk/
+-rw-rw-rw-   0        0        0      726 2023-06-16 21:43:43.000000 chichitk-0.0.4/chichitk/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-04-17 00:34:05.000000 chichitk-0.0.4/chichitk/aspect_frame.py
+-rw-rw-rw-   0        0        0    30761 2023-07-01 20:16:30.000000 chichitk-0.0.4/chichitk/buttons.py
+-rw-rw-rw-   0        0        0    49997 2023-04-16 02:08:01.000000 chichitk-0.0.4/chichitk/canvas_items.py
+-rw-rw-rw-   0        0        0     7697 2023-04-30 23:26:46.000000 chichitk-0.0.4/chichitk/collapse_frame.py
+-rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.4/chichitk/dropdowns.py
+-rw-rw-rw-   0        0        0     8943 2023-04-22 15:48:45.000000 chichitk-0.0.4/chichitk/entry_boxes.py
+-rw-rw-rw-   0        0        0     6098 2023-04-18 17:15:53.000000 chichitk-0.0.4/chichitk/file_dialog.py
+-rw-rw-rw-   0        0        0     4445 2023-04-30 03:22:46.000000 chichitk-0.0.4/chichitk/function_progress.py
+-rw-rw-rw-   0        0        0    34820 2023-04-18 17:09:52.000000 chichitk-0.0.4/chichitk/icons.py
+-rw-rw-rw-   0        0        0    28235 2023-07-07 01:34:37.000000 chichitk-0.0.4/chichitk/labels.py
+-rw-rw-rw-   0        0        0    10238 2023-04-21 01:24:23.000000 chichitk-0.0.4/chichitk/pdf_display.py
+-rw-rw-rw-   0        0        0     8639 2023-05-18 02:39:40.000000 chichitk-0.0.4/chichitk/player.py
+-rw-rw-rw-   0        0        0     5534 2023-07-14 19:52:52.000000 chichitk-0.0.4/chichitk/progress_bar.py
+-rw-rw-rw-   0        0        0     3990 2023-04-20 02:51:35.000000 chichitk-0.0.4/chichitk/scrollable_frame.py
+-rw-rw-rw-   0        0        0    64712 2023-07-19 00:17:52.000000 chichitk-0.0.4/chichitk/sliders.py
+-rw-rw-rw-   0        0        0     2188 2023-07-05 19:15:13.000000 chichitk-0.0.4/chichitk/temp_label.py
+-rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.4/chichitk/temp_menu.py
+-rw-rw-rw-   0        0        0    13363 2023-07-16 04:25:50.000000 chichitk-0.0.4/chichitk/text_boxes.py
+-rw-rw-rw-   0        0        0     9915 2023-05-18 02:42:43.000000 chichitk-0.0.4/chichitk/timer.py
+-rw-rw-rw-   0        0        0     6780 2023-05-02 01:00:40.000000 chichitk-0.0.4/chichitk/tool_tip.py
+drwxrwxrwx   0        0        0        0 2023-07-20 15:27:11.375629 chichitk-0.0.4/chichitk.egg-info/
+-rw-rw-rw-   0        0        0     3375 2023-07-20 15:27:11.000000 chichitk-0.0.4/chichitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-07-20 15:27:11.000000 chichitk-0.0.4/chichitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 15:27:11.000000 chichitk-0.0.4/chichitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-20 15:27:11.000000 chichitk-0.0.4/chichitk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 15:27:11.000000 chichitk-0.0.4/chichitk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1161 2023-07-20 15:25:27.000000 chichitk-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 15:27:11.392752 chichitk-0.0.4/setup.cfg
```

### Comparing `chichitk-0.0.3/LICENSE` & `chichitk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/PKG-INFO` & `chichitk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chichitk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python UI library built upon Tkinter
 Author-email: Samuel Gibson <samuelpgibson12@gmail.com>
 Project-URL: Homepage, https://github.com/SamGibson1/ChichiTk
 Project-URL: Documentation, https://github.com/SamGibson1/ChichiTk/wiki
 Project-URL: Bug Tracker, https://github.com/SamGibson1/ChichiTk/issues
 Keywords: python,tkinter,custom,widgets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `chichitk-0.0.3/Readme.md` & `chichitk-0.0.4/Readme.md`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/__init__.py` & `chichitk-0.0.4/chichitk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .function_progress import *
 from .labels import *
 from .pdf_display import PdfDisplay
 from .player import *
 from .progress_bar import *
 from .scrollable_frame import *
 from .sliders import *
+from .temp_label import *
 from .temp_menu import *
 from .text_boxes import *
 from .timer import *
 from .tool_tip import *
 
 # not importing from .canvas_items because these are not intended
 # to be used outside of chichitk
```

### Comparing `chichitk-0.0.3/chichitk/aspect_frame.py` & `chichitk-0.0.4/chichitk/aspect_frame.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/buttons.py` & `chichitk-0.0.4/chichitk/buttons.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,25 +191,26 @@
             :param bar_height: Int - height of bar at the bottom of button
         '''
         BaseButton.__init__(self, master, command, bar_height=bar_height, **kwargs) # bar already packed buttom
         self.icon_frame = Frame(self)
         self.icon_frame.pack(side='top', padx=self.padx, pady=self.pady)
         self.icon = Button(self.icon_frame, borderwidth=0, command=self.click_button)
         self.icon.pack(side='left')
+        self.label_text = label
         self.label = Label(self.icon_frame, text=label, font=(self.font_name, self.font_size), bd=0)
         self.label.pack(side='right', fill='y')
 
         self.icon_frame.bind("<Button-1>", self.click_button)
         self.label.bind("<Button-1>", self.click_button)
         
         # Load icon
         if isinstance(icon_path, str): # path to image
-            assert len(icon_path) > 4, f'Invalid path: {icon_path}'
-            assert icon_path[-4:] == '.png', f'icon_path is not a .png file: {icon_path}'
-            assert os.path.exists(icon_path), f'Path to .png file does not exist: {icon_path}'
+            assert len(icon_path) > 4, f'IconButton Error: Invalid path: {icon_path}'
+            assert icon_path[-4:] == '.png', f'IconButton Error: icon_path is not a .png file: {icon_path}'
+            assert os.path.exists(icon_path), f'IconButton Error: Path to .png file does not exist: {icon_path}'
             self.base_img = cv2.imread(icon_path)
         elif isinstance(icon_path, np.ndarray): # 3d numpy array
             self.base_img = icon_path
         else:
             raise TypeError(f'Invalid icon input to IconButton: {icon_path}')
 
         # Create Icons
@@ -226,14 +227,15 @@
         '''sets colors based on self.selected, self.hovering, and self.active'''
         if self.active:
             bg, fg = self.bg_colors[self.selected][self.hovering], self.fg_colors[self.selected][self.hovering]
             bar_color, image = self.bar_colors[self.selected][self.hovering], self.images[self.selected][self.hovering]
         else:
             bg, fg, bar_color, image = self.bg_colors[0][0], self.off_fg, self.bg_colors[0][0], self.off_icon
         self.config(bg=bg)
+        self.icon_frame.config(bg=bg)
         self.bar.config(bg=bar_color)
         self.label.config(bg=bg, fg=fg)
         self.icon.config(image=image, bg=bg, activebackground=bg)
 
     def set_color(self, color:str, which:str='bg', selected:bool=False, hover:bool=False):
         '''sets a single color
         
@@ -250,14 +252,18 @@
             self.fg_colors[selected][hover] = color
             temp_img = image_replace_colors(self.base_img.copy(), [('#ffffff', color), ('#000000', self.bg_colors[selected][hover])])
             self.images[selected][hover] = ImageTk.PhotoImage(image=Image.fromarray(temp_img), master=self.icon_frame)
         elif which == 'bar':
             self.bar_colors[selected][hover] = color
         self.config_colors()
 
+    def get_label(self) -> str:
+        '''returns button label'''
+        return self.label_text
+
 class ToggleIconButton(IconButton):
     ''' Toggle version of IconButton. The callback command is given a boolean
         parameter which indicates whether the button is being turned on or off.
     '''
     def __init__(self, master, icon_path:str, command=None, label:str='', bar_height:int=3, **kwargs):
         '''Toggle version of IconButton
         
@@ -271,20 +277,25 @@
     def click(self):
         '''called when button is clicked'''
         self.selected = not self.selected
         self.config_colors()
         if self.toggle_command is not None:
             self.toggle_command(self.selected)
 
+    def get(self) -> bool:
+        '''returns selection status'''
+        return self.selected
+
 class DoubleIconButton(Frame):
     ''' DoubleIconButton contains two IconButtons that swap when clicked.
         There are separate commands for the two IconButtons
     '''
-    def __init__(self, master, icon1:str, icon2:str, command1, command2, label1:str='', label2:str='',
-                 popup_label1=None, popup_label2=None, **kwargs):
+    def __init__(self, master, icon1:str, icon2:str, command1, command2,
+                 label1:str='', label2:str='', popup_label1=None, popup_label2=None,
+                 inactive_fg:str='#888888', active_fg:str='#ffffff', **kwargs):
         '''IconButton that changes when clicked
         
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param icon1: str - icon path for first IconButton
             :param icon2: str - icon path for second button
@@ -292,17 +303,17 @@
             :param command2: 0 argument function - called when second button is clicked - changes to first button
         '''
         Frame.__init__(self, master)
         self.__command1, self.__command2 = command1, command2
         self.__double_status = False # False when button 1 is active and True when button 2 is active
 
         self.Button1 = IconButton(self, icon1, self.click1, label=label1, selectable=False,
-                                    popup_label=popup_label1, **kwargs)
+                                    popup_label=popup_label1, inactive_fg=inactive_fg, **kwargs)
         self.Button2 = IconButton(self, icon2, self.click2, label=label2, selectable=False,
-                                    popup_label=popup_label2, **kwargs)
+                                    popup_label=popup_label2, inactive_fg=active_fg, **kwargs)
         self.Button1.pack(fill='both', expand=True)
 
     def switch1(self):
         '''
         Purpose:
             switches to button1 without calling any command
         Pre-conditions:
@@ -357,17 +368,34 @@
             changes active (visible) button
         Returns:
             (none)
         '''
         self.switch1()
         self.__command2()
 
+    def turn_on(self):
+        '''makes button interactable'''
+        self.Button1.turn_on()
+        self.Button2.turn_on()
+
+    def turn_off(self):
+        '''makes button uninteractable'''
+        self.Button1.turn_off()
+        self.Button2.turn_off()
+
     def get(self):
         '''returns False if button1 is active and True if button2 is active'''
         return self.__double_status
+    
+    def get_label(self) -> str:
+        '''returns current button label'''
+        if self.__double_status: # button2 is active
+            return self.Button2.get_label()
+        else:
+            return self.Button1.get_label()
 
 class CheckButton(DoubleIconButton):
     ''' Special version of DoubleIconButton that has a checkbox icon - checked and unchecked
         Takes a single callback command - passes boolean to indicate new checkbox status
     '''
     def __init__(self, master, command, label:str='', active_popup_label=None,
                  inactive_popup_label=None, active=False, **kwargs):
@@ -387,14 +415,22 @@
                                   lambda: command(True), lambda: command(False),
                                   label1=label, label2=label,
                                   popup_label1=inactive_popup_label,
                                   popup_label2=active_popup_label, **kwargs)
         if active:
             self.Button1.click_button()
 
+    def select(self):
+        '''select check button without calling callback command'''
+        self.switch2()
+
+    def deselect(self):
+        '''deselect check button without calling callback command'''
+        self.switch1()
+
 class LabelButton(BaseButton):
     ''' LabelButton includes bar underneath the label. The parameter
         'bar_height' can be set to 0 to remove the bar.
         
         Background and foreground color can change based on select/hover status.
     '''
     def __init__(self, master, command, label:str='', **kwargs):
@@ -437,26 +473,85 @@
     def click(self):
         '''called when button is clicked'''
         self.selected = not self.selected
         self.config_colors()
         if self.toggle_command is not None:
             self.toggle_command(self.selected)
 
+class ToggleIconButtonGroup(Frame):
+    ''' Group of ToggleIconButtons where only one can be active at a time
+    
+        Clicking a button will automatically deselect all other buttons in the
+        group and call their respective off callback functions
+    '''
+    def __init__(self, master:Frame, button_info:list, orientation:str='h',
+                 bg='#ffffff', buttons_padx=0, buttons_pady=0, **kwargs):
+        '''
+        Parameters
+        ----------
+            :master: Frame - parent frame
+            :param button_info: list[dict] - contains keys for each button:
+                icon_path: str - path to .png file
+                on_callback: function() - called when button is clicked
+                off_callback: function() - called when button is deselected
+                label (optional): str - button label
+                popup_label (optional): str - button popup label
+        '''
+        assert orientation in ['h', 'v'], f'ToggleIconButtonGroup Error: Invalid orientation: {orientation}'
+        super().__init__(master, bg=bg)
+        self.__button_info = button_info
+
+        pack_side = 'left' if orientation == 'h' else 'top'
+
+        self.__buttons: list[ToggleIconButton] = []
+        for i, info in enumerate(self.__button_info):
+            label = info['label'] if 'label' in info.keys() else ''
+            popup_label = info['popup_label'] if 'popup_label' in info.keys() else ''
+            button = ToggleIconButton(self, info['icon_path'],
+                                      command=lambda b, x=i: self.__callback(b, x),
+                                      label=label, popup_label=popup_label, **kwargs)
+            button.pack(side=pack_side, padx=buttons_padx, pady=buttons_pady, fill='both')
+            self.__buttons.append(button)
+
+    def __callback(self, active:bool, button_index:int):
+        '''called when the ith button is clicked'''
+        if active: # callback and deactivate all other buttons
+            for i, button in enumerate(self.__buttons):
+                if i == button_index: # callback for clicked button
+                    self.__button_info[i]['on_callback']()
+                else: # deactivate other buttons
+                    button.deselect()
+                    self.__button_info[i]['off_callback']()
+        else: # off callback for clicked button
+            self.__button_info[button_index]['off_callback']()
+
+    def set_color(self, button_index:int, color:str, **kwargs):
+        '''sets color for the button with the specified index'''
+        self.__buttons[button_index].set_color(color, **kwargs)
+
+    def click(self, button_index:int):
+        '''clicks the specified button'''
+        self.__buttons[button_index].click_button()
+
+    def get(self) -> list:
+        '''returns list of booleans indicating selection status of each button'''
+        return [button.get() for button in self.__buttons]
+
 class PlayerButtons(Frame):
     ''' Collection of IconButtons for controlling the playback of music, a
         video, or something like that.
         
         Includes 6 buttons in the following order, with corresponding callbacks:
             previous - go to previous song or beginning of current song
             skip_back - go back by a given increment
             play/pause - toggle button to start/stop playback
             skip_forward - go forward by a given increment
             next - go to next song or end of current song
             loop (toggle) - turn looping on or off
-            '''
+    '''
     def __init__(self, master, bg, play_function, stop_function, step_forward_function,
                  step_back_function, next_function, previous_function,
                  active_icon_color='#ffffff', hover_fg='#aaaaaa',
                  button_padx=6, padx_weight=6, active=True):
         '''
         Parameters
         ----------
```

### Comparing `chichitk-0.0.3/chichitk/canvas_items.py` & `chichitk-0.0.4/chichitk/canvas_items.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/collapse_frame.py` & `chichitk-0.0.4/chichitk/collapse_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,26 @@
         or with an external command.
 
         Contains the attributes 'header' and 'frame' which are both tk.Frame
         objects refering to the header and body frames respectively.
 
         DO NOT put anything directly in the CollapseFrame. Only user the header
         and body frames.
+
+        Warning: if CollapseFrame is initially close, and not collapsable,
+        there will be no way for user to access the content of the body frame.
     '''
     def __init__(self, master:Frame, open_callback=None, close_callback=None,
                  label=None, bg='#ffffff', border_bg=None,
                  inactive_bg=None, active_bg=None, inactive_hover_bg=None,
                  active_hover_bg=None, inactive_fg='#000000', active_fg=None,
                  inactive_hover_fg=None, active_hover_fg=None,
                  label_side='left', font_name='Segoe UI', font_size=10,
                  label_padx=0, label_pady=0, body_padx=0, body_pady=0,
-                 active=True, **kwargs):
+                 active=True, collapsable=True, **kwargs):
         '''active refers to the state when the body frame is visible
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param open_callback: function () - called when body frame is made visible
             :param close_callback: function () - called when body frame is hidden
             :param label: str or None - header text
@@ -41,14 +44,15 @@
             :param font_name: str - label font name
             :param font_size: str - label font size
             :param label_padx: int - x padding of label within header frame
             :param label_pady: int - y padding of label within header frame
             :param body_padx: int - x padding around body frame
             :param body_pady: int - y padding around body frame
             :param active: bool - initial visibility of body frame
+            :param collapsable: bool - if True, CollapseFrame is static
         '''
         super_bg = border_bg if border_bg is not None else bg
         super().__init__(master, bg=super_bg, **kwargs)
         self.__open_callback = open_callback
         self.__close_callback = close_callback
         self.__body_padx, self.__body_pady = body_padx, body_pady
         inactive_bg = inactive_bg if inactive_bg is not None else bg
@@ -57,28 +61,31 @@
         active_hover_bg = active_hover_bg if active_hover_bg is not None else active_bg
         self.__bg_colors = [[inactive_bg, active_bg], [inactive_hover_bg, active_hover_bg]]
         active_fg = active_fg if active_fg is not None else inactive_fg
         inactive_hover_fg = inactive_hover_fg if inactive_hover_fg is not None else inactive_fg
         active_hover_fg = active_hover_fg if active_hover_fg is not None else active_fg
         self.__fg_colors = [[inactive_fg, active_fg], [inactive_hover_fg, active_hover_fg]]
         self.__draw_label = label is not None
+        self.__collapsable = collapsable
         self.__active, self.__hovering = active, False
 
         # Header Frame
         self.header = Frame(self)
         self.header.pack(side='top', fill='x')
-        self.header.bind('<Enter>', self.hover_enter)
-        self.header.bind('<Leave>', self.hover_leave)
-        self.header.bind('<Button-1>', self.header_click)
+        if self.__collapsable:
+            self.header.bind('<Enter>', self.hover_enter)
+            self.header.bind('<Leave>', self.hover_leave)
+            self.header.bind('<Button-1>', self.header_click)
         if self.__draw_label:
             self.label = Label(self.header, text=label, font=(font_name, font_size))
             self.label.pack(side=label_side, padx=label_padx, pady=label_pady)
-            self.label.bind('<Enter>', self.hover_enter)
-            self.label.bind('<Leave>', self.hover_leave)
-            self.label.bind('<Button-1>', self.header_click)
+            if self.__collapsable:
+                self.label.bind('<Enter>', self.hover_enter)
+                self.label.bind('<Leave>', self.hover_leave)
+                self.label.bind('<Button-1>', self.header_click)
 
         # Body Frame
         self.frame = Frame(self, bg=bg)
         if self.__active:
             self.show(callback=False)
 
         self.__color_config()
@@ -97,24 +104,33 @@
 
     def set_fg(self, color:str, hovering=False, active=False):
         '''updates foreground color for given hover/select status'''
         self.__fg_colors[hovering][active] = color
 
     def hover_enter(self, event=None):
         '''called when mouse enters header'''
+        if not self.__collapsable:
+            print('CollapseFrame Error: tried to hover enter when CollapseFrame is not collapsable')
+            return
         self.__hovering = True
         self.__color_config()
 
     def hover_leave(self, event=None):
         '''called when mouse leaves header'''
+        if not self.__collapsable:
+            print('CollapseFrame Error: tried to hover leave when CollapseFrame is not collapsable')
+            return
         self.__hovering = False
         self.__color_config()
 
     def header_click(self, event=None):
         '''called when mouse clicks on header - toggles active status'''
+        if not self.__collapsable:
+            print('CollapseFrame Error: tried to toggle body frame when CollapseFrame is not collapsable')
+            return
         if self.__active:
             self.hide(callback=True)
         else:
             self.show(callback=True)
 
     def show(self, callback=True):
         '''makes body frame visible'''
```

### Comparing `chichitk-0.0.3/chichitk/dropdowns.py` & `chichitk-0.0.4/chichitk/dropdowns.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/entry_boxes.py` & `chichitk-0.0.4/chichitk/entry_boxes.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/file_dialog.py` & `chichitk-0.0.4/chichitk/file_dialog.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/function_progress.py` & `chichitk-0.0.4/chichitk/function_progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from tkinter import Frame, Label
 
 from .progress_bar import ProgressBar
 from .buttons import IconButton
 from .icons import icons
 
 
@@ -14,28 +13,29 @@
         
         Indictes if function has already been executed
 
         When function is being executed, it should call self.Progress.increment()
         with each iteration to increment progress bar
     '''
     def __init__(self, master, command, label, bg, loading_text='Loading...',
-                 height=25, indicator_pady=0, font_name='Segoe UI',
+                 icon_path=None, height=25, indicator_pady=0, font_name='Segoe UI',
                  font_size=10, text_font_size=12, inactive_bg:str='#ffffff',
                  loaded_bg:str='#00ff00', text_side='bottom', active_color='#00ff00',
                  text_color='#cccccc', inactive_color=None):
         '''
         
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param command: function () - called when button is clicked
                                         - function should increment progress bar
             :param label: str - label for IconButton - to call command
             :param bg: str (hex code) - widget background color
             :param loading_text: str - text displayed while command is running
+            :param icon_path: str - optioal path to png file to replace default 'edit' icon
             :param height: int - height of progress bar
             :param indicator_pady: int - pady for indicator square
             :param inactive_bg: str (hex code) - color of indicator when incomplete
             :param loaded_bg: str (hex code) - color of indicator when complete
             :param text_side: Literal['bottom', 'top', 'right', 'left'] - for progress bar
             :param active_color: str (hex code) - color of active part of progress bar
             :param text_color: str (hex code) - color of text in progress bar
@@ -44,15 +44,16 @@
         Frame.__init__(self, master, bg=bg)
         self.inactive_bg, self.loaded_bg = inactive_bg, loaded_bg
         inactive_color = inactive_color if inactive_color else bg
         self.complete = False
 
         self.main_frame = Frame(self, bg=bg)
         self.main_frame.pack(side='top', fill='both', expand=True)
-        button = IconButton(self.main_frame, icons['edit'], command, label=label,
+        icon = icon_path if icon_path is not None else icons['edit']
+        button = IconButton(self.main_frame, icon, command, label=label,
                             selectable=False, inactive_bg=bg, bar_height=2)
         button.pack(side='left', fill='both', expand=True)
         self.indicator = Label(self.main_frame, text=' ' * 3, bg=self.inactive_bg,
                                font=(font_name, font_size))
         self.indicator.pack(side='right', fill='y', pady=indicator_pady)
 
         self.Progress = ProgressBar(self, 100, bg, active_color=active_color,
@@ -80,8 +81,7 @@
         self.Progress.pack_forget()
         self.main_frame.pack(side='top', fill='both', expand=True)
         self.indicator.config(bg=self.inactive_bg)
 
     def is_complete(self) -> bool:
         '''returns True if function is complete, otherwise False'''
         return self.complete
-
```

### Comparing `chichitk-0.0.3/chichitk/icons.py` & `chichitk-0.0.4/chichitk/icons.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/labels.py` & `chichitk-0.0.4/chichitk/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.editable = editable
         self.dragging = False
         self.check_function = check_function
         self.hover_enter_function = hover_enter_function
         self.hover_leave_function = hover_leave_function
         self.entry_on_function = entry_on_function
         self.entry_off_function = entry_off_function
+        self.last_callback = time.time() # to avoid double callbacks
 
         Frame.__init__(self, master, bg=bg)
         
         self.label = Label(self, text=self.text, bg=bg, fg=fg, font=(font_name, font_size))
         self.label.pack(fill='both')
         self.Entry = CheckEntry(self, default=self.text, allowed_chars=allowed_chars,
                                 max_len=max_len, check_function=check_function,
@@ -123,24 +124,29 @@
             self.label.pack_forget()
             self.Entry.activate(text=self.text, select=True)
             self.Entry.pack(fill='both')
             if self.entry_on_function:
                 self.entry_on_function()
 
     def to_label(self, event=None, callback=True):
-        self.Entry.pack_forget()
-        self.label.focus_set() # to take focus away from Entry so that keyboard strokes are no longer read by Entry
-        self.label.pack(fill='both')
-        if self.check_function == None or self.check_function(self.Entry.get()): # only if text in Entry is good
-            self.text = self.Entry.get()
-            self.label.config(text=self.text)
-            if callback and self.callback:
-                self.callback(self.text)
-        if self.entry_off_function:
-            self.entry_off_function()
+        '''switching from entry box to label'''
+        current_time = time.time()
+        if current_time - self.last_callback > 0.05: # avoid double callback
+            self.last_callback = current_time
+            self.Entry.pack_forget()
+            self.label.focus_set() # to take focus away from Entry so that keyboard strokes are no longer read by Entry
+            self.label.pack(fill='both')
+            if self.check_function is None or self.check_function(self.Entry.get()): # only if text in Entry is good
+                if self.Entry.get() != self.text: # only callback if text has changed
+                    self.text = self.Entry.get()
+                    self.label.config(text=self.text)
+                    if callback and self.callback:
+                        self.callback(self.text)
+            if self.entry_off_function:
+                self.entry_off_function()
 
     def get(self) -> str:
         return self.text
 
 class NumberEditLabel(EditLabel):
     ''' Extension of EditLabel that only handles numbers and allows the to
         adjust the number by dragging on top of the label.
@@ -163,14 +169,15 @@
         the 'step' argument. If step evenly divisible by 1 (not necessarily of
         type int), return values from .get() will be integers, otherwise return
         values will be floats.
         
         NumberEditLabel is an excellent compact solution when there is not room
         to display a scrollbar or slider for the user to adjust numeric values.
     '''
+    allowed_chars = '0123456789'
 
     def __init__(self, master, callback=None, min_value=0, max_value=100,
                  step=1, default_value=None, reference_width=2.0, max_len=None,
                  drag_threshold=0.2, draggable=True, **kwargs):
         '''
         Parameters
         ----------
@@ -181,140 +188,238 @@
             :param step: int or float - number increment
             :param default_value: int or float - default value if different from min_value
             :param reference_width: float - fraction of label width
             :param max_len: int - maximum number of characters in entry box
             :param drag_threshold: float (seconds) - click duration to be considered a single click (not drag)
             :param draggable: bool - if True, label value can be changed by dragging (like a slider)
         '''
-        if step % 1 == 0: # integer
-            self.__decimals = 0
+        self._step = step
+        if self._step % 1 == 0: # integer
+            self._decimals = 0
         else:
-            self.__decimals = len(str(self.__step).split(".")[1])
+            self._decimals = len(str(self._step).split(".")[1])
         default_value = default_value if default_value is not None else min_value
-        allowed_chars = '0123456789' + '.' * (self.__decimals > 0)
+        allowed_chars = self.allowed_chars + '.' * (self._decimals > 0)
         
-        super().__init__(master, self.__get_text(default_value),
-                         callback=self.__entry_update, allowed_chars=allowed_chars,
-                         max_len=max_len, check_function=self.__check_function, **kwargs)
-        
-        self.__callback_function = callback
-        self.__min_value, self.__max_value = min_value, max_value
-        self.__step = step
-        self.__values = np.arange(self.__min_value, self.__max_value + self.__step * 0.9, self.__step)
-        self.__drag_threshold = drag_threshold
-        self.__reference_width = reference_width
+        super().__init__(master, self._get_text(default_value),
+                         callback=self._entry_update, allowed_chars=allowed_chars,
+                         max_len=max_len, check_function=self._check_function, **kwargs)
+        
+        self._callback_function = callback
+        self._min_value, self._max_value = min_value, max_value
+        self._values = np.arange(self._min_value, self._max_value + self._step * 0.9, self._step)
+        self._drag_threshold = drag_threshold
+        self._reference_width = reference_width
 
         if draggable:
             self.label.config(cursor='sb_h_double_arrow')
-            self.label.bind("<Button-1>", self.__mouse_click)
-            self.label.bind("<ButtonRelease-1>", self.__mouse_release, add='+')
-            self.label.bind("<B1-Motion>", self.__mouse_drag)
+            self.label.bind("<Button-1>", self._mouse_click)
+            self.label.bind("<ButtonRelease-1>", self._mouse_release, add='+')
+            self.label.bind("<B1-Motion>", self._mouse_drag)
 
-    def __check_function(self, text:str) -> bool:
+    def _check_function(self, text:str) -> bool:
         '''
         called when text is edited in entry box - checks if text is good
         input text is guaranteed to contain only numbers and '.' if return_type
         is float
         '''
         if text == '':
             return False
-        if text[0] == '.' or text.count('.') >= 1: # improperly formatted number
+        if text[0] == '.' or text[-1] == '.' or text.count('.') > 1: # improperly formatted number
             return False
         value = float(text)
-        if value < self.__min_value or value > self.__max_value: # out of range
+        if value < self._min_value or value > self._max_value: # out of range
             return False
         return True
         
-    def __entry_update(self, text:str):
+    def _entry_update(self, text:str):
         '''
         called when number is updated by user exiting entry box
-        text is guaranteed to have passed self.__check_function
+        text is guaranteed to have passed self._check_function
         reformats text if necessary and calls callback function
         '''
         # to reformat if necessary
-        self.label.config(text=self.__get_text(self.get()))
-        if self.__callback_function is not None:
-            self.__callback_function(self.get())
+        self.text = self._get_text(self.get())
+        self.label.config(text=self.text)
+        if self._callback_function is not None:
+            self._callback_function(self.get())
 
-    def __mouse_click(self, event):
+    def _mouse_click(self, event):
         '''
         called when mouse clicks on label
         store current position for dragging
         store time so that release can decide to go to entry box or not
         '''
         self.dragging = True
-        self.__click_value = self.get()
-        self.__click_position = event.x
-        self.__click_time = time.time()
+        self._click_value = self.get()
+        self._click_position = event.x
+        self._click_time = time.time()
 
-    def __mouse_release(self, event=None):
+    def _mouse_release(self, event=None):
         '''
         called when mouse releases click
         if a short enough time has passed since click, goes to entry box
         a short time would indicate that the user simply clicked and didn't drag
         '''
-        if time.time() - self.__click_time < self.__drag_threshold:
+        if time.time() - self._click_time < self._drag_threshold:
             self.to_entry()
 
-    def __mouse_drag(self, event):
+    def _mouse_drag(self, event):
         '''
         called when mouse drags on label
         changes value based on drag distance
         '''
         # compute percentage of reference width that drag has traversed
-        p = (event.x - self.__click_position) / (self.label.winfo_width() * self.__reference_width)
+        p = (event.x - self._click_position) / (self.label.winfo_width() * self._reference_width)
         # compute increment based on traversal percentage
-        increment = (self.__max_value - self.__min_value) * p
+        increment = (self._max_value - self._min_value) * p
         # add increment to click value and round to nearest allowed value
-        value = self.__values[(np.absolute(self.__values - (self.__click_value + increment))).argmin()]
+        value = self._values[(np.absolute(self._values - (self._click_value + increment))).argmin()]
 
-        self.text = self.__get_text(value)
+        self.text = self._get_text(value)
         self.label.config(text=self.text)
-        if self.__callback_function is not None:
-            self.__callback_function(self.get())
+        if self._callback_function is not None:
+            self._callback_function(self.get())
 
     def set_min_value(self, min_value:int):
         '''sets minimum value - must be less than current maximum value'''
-        assert min_value <= self.__max_value, f'Tried to set minimum value, {min_value}, that is greater than current maximum value, {self.__max_value}'
-        self.__min_value = min_value
-        self.__values = np.arange(self.__min_value, self.__max_value + self.__step * 0.9, self.__step)
+        assert min_value <= self._max_value, f'Tried to set minimum value, {min_value}, that is greater than current maximum value, {self._max_value}'
+        self._min_value = min_value
+        self._values = np.arange(self._min_value, self._max_value + self._step * 0.9, self._step)
 
     def set_max_value(self, max_value:int):
         '''sets maximum value - must be greater than current minimum value'''
-        assert max_value >= self.__min_value, f'Tried to set maximum value, {max_value}, that is greater than current minimum value, {self.__min_value}'
-        self.__max_value = max_value
-        self.__values = np.arange(self.__min_value, self.__max_value + self.__step * 0.9, self.__step)
+        assert max_value >= self._min_value, f'Tried to set maximum value, {max_value}, that is greater than current minimum value, {self._min_value}'
+        self._max_value = max_value
+        self._values = np.arange(self._min_value, self._max_value + self._step * 0.9, self._step)
+
+    def get_min_value(self) -> int:
+        '''returns current minimum value'''
+        return self._min_value
+    
+    def get_max_value(self) -> int:
+        '''returns current maximum value'''
+        return self._max_value
 
-    def __get_text(self, value:int) -> str:
+    def _get_text(self, value:int) -> str:
         '''converts value to string based on step and return_type'''
-        if self.__decimals == 0: # integer
+        if self._decimals == 0: # integer
             return str(int(value))
-        text = str(round(value, self.__decimals))
+        text = str(round(value, self._decimals))
         if '.' in text:
             dec = len(text.split(".")[1])
         else:
             text += '.'
             dec = 0
-        return text + '0' * (self.__decimals - dec)
+        return text + '0' * (self._decimals - dec)
 
     def set(self, value:int):
         '''updates value'''
-        super().set_text(self.__get_text(value))
+        super().set_text(self._get_text(value))
 
     def get(self) -> int:
         '''
         returns number current in NumberEditLabel as int or float depending
         on preset return_type
         text currently in label is guaranteed to be formatted correctly
         '''
-        if self.__decimals == 0: # integer
+        if self._decimals == 0: # integer
             return int(super().get())
         else:
             return float(super().get())
 
+    def set_perc(self, perc:float):
+        '''sets value based on percentage - float between 0 and 1'''
+        self.set(self._min_value + (self._max_value - self._min_value) * perc)
+
+    def get_perc(self) -> float:
+        '''returns label value as a percentage - float between 0 and 1'''
+        return (self.get() - self._min_value) / (self._max_value - self._min_value)
+
+class TimeEditLabel(NumberEditLabel):
+    ''' Extension of NumberEditLabel that displays time in the form
+        (h):(m)m:ss.xxx instead of simple number.
+        
+        set() and get() methods deal in seconds.
+        
+        Input/output type can be int or float depending on step
+        
+        See NumberEditLabel for further implementation details.
+    '''
+    allowed_chars = '0123456789:'
+
+    def _check_function(self, text:str) -> bool:
+        '''
+        called when text is edited in entry box - checks if text is good
+        input text is guaranteed to contain only numbers and ':' and '.' if
+        return_type is float
+        '''
+        if text == '':
+            return False
+        if text.count(':') > 2 or text[0] == ':' or text[-1] == ':':
+            return False
+        if text.count('.') > 1 or text[0] == '.' or text[-1] == '.':
+            return False
+        for t in text.split(':')[1:]: # minute, second components
+            if len(t) < 2 or float(t) >= 60:
+                return False
+        for t in text.split(':')[:-1]: # hour, minute components
+            if t == '' or '.' in t or len(t) > 2 or int(t) >= 60:
+                return False
+        value = self.__get_text_value(text)
+        if value < self._min_value or value > self._max_value: # out of range
+            return False
+        return True
+        
+    def _get_text(self, sec:float) -> str:
+        '''converts value to string based on self._decimals'''
+        # compute hours, minutes, and seconds
+        s = int(sec)
+        if sec >= 3600: # at least one hour
+            text = f'{s // 3600}:{(s % 3600) // 60:0>2}:{(s % 60) // 1:0>2}'
+        else: # less than one hour
+            text = f'{s // 60}:{(s % 60) // 1:0>2}'
+
+        # compute partial seconds
+        if self._decimals > 0:
+           if sec % 1 == 0: # whole seconds - still add zeros
+               text += '.' + '0' * self._decimals
+           else:
+               dec = str(round(sec % 1, self._decimals))[1:] # in form .xxx
+               text += f'{dec:0>{self._decimals + 1}}'
+        return text
+
+    def __get_text_value(self, text:str) -> float:
+        '''
+            returns the value of text in form (h):(m)m:ss.xxx in seconds
+            text passed is guaranteed to have passed self._check_function
+        '''
+        if text.count(':') == 2: # includes hours - in form hh:mm:ss.xxx
+            hours, minutes, seconds = text.split(':')
+        elif text.count(':') == 1: # includes minutes - in form mm:ss.xx
+            hours = 0
+            minutes, seconds = text.split(':')
+        else: # only minutes - in form mm:ss.xxx
+            hours, minutes = 0, 0
+            seconds = text
+
+        value = float(hours) * 3600 + float(minutes) * 60 + float(seconds)
+        if self._decimals == 0: # integer
+            return int(round(value, 0))
+        else: # float
+            return round(value, self._decimals)
+        
+    def set(self, seconds:float):
+        '''updates value'''
+        self.set_text(self._get_text(seconds))
+
+    def get(self) -> float:
+        '''returns current value as int or float (seconds) depending on step'''
+        return self.__get_text_value(EditLabel.get(self))
+
 class RangeLabel(Frame):
     ''' Pair of NumberEditLabels that allow user to select a range
     '''
     def __init__(self, master, callback=None, bg='#ffffff', sep_text='to',
                  min_val=0, max_val=100, default_min=None, default_max=None,
                  step=1, min_range=0, label_fg='#888888', label_font_size=10,
                  **kwargs):
@@ -331,89 +436,90 @@
             :param default_max: int - default maximum value if different from max_val
             :param step: int or float - slider increment
             :param min_range: int - minimum allowed distance between min and max
             :param label_fg: str (hex code) - color of sep_text
             :param label_font_size: int - font size of sep text
         '''
         super().__init__(master, bg=bg)
-        self.__min_range = min_range
-        self.__callback_function = callback
+        self._min_range = min_range
+        self._callback_function = callback
         default_min = default_min if default_min is not None else min_val
         default_max = default_max if default_max is not None else max_val
+        max_len = len(str(max_val)) if step % 1 == 0 else None
 
-        self.__MinLabel = NumberEditLabel(self, self.__min_callback, bg=bg,
+        self._MinLabel = NumberEditLabel(self, self._min_callback, bg=bg,
                                           min_value=min_val,
-                                          max_value=default_max - self.__min_range,
+                                          max_value=default_max - self._min_range,
                                           step=step, default_value=default_min,
-                                          max_len=len(str(max_val)), **kwargs)
-        self.__MaxLabel = NumberEditLabel(self, self.__max_callback, bg=bg,
-                                          min_value=default_min + self.__min_range,
+                                          max_len=max_len, **kwargs)
+        self._MaxLabel = NumberEditLabel(self, self._max_callback, bg=bg,
+                                          min_value=default_min + self._min_range,
                                           max_value=max_val, step=step,
                                           default_value=default_max,
-                                          max_len=len(str(max_val)), **kwargs)
-        self.__MinLabel.pack(side='left', fill='x', expand=True)
+                                          max_len=max_len, **kwargs)
+        self._MinLabel.pack(side='left', fill='x', expand=True)
         Label(self, text=f' {sep_text} ', bg=bg, fg=label_fg,
               font=('Segoe UI', label_font_size)).pack(side='left')
-        self.__MaxLabel.pack(side='left', fill='x', expand=True)
+        self._MaxLabel.pack(side='left', fill='x', expand=True)
 
     def set_min(self, new_min:int):
         '''updates current min value - does not change range limits'''
-        self.__MinLabel.set(new_min)
-        self.__MaxLabel.set_min_value(new_min + self.__min_range)
+        self._MinLabel.set(new_min)
+        self._MaxLabel.set_min_value(new_min + self._min_range)
 
     def set_max(self, new_max:int):
         '''updates current max value - does not change range limits'''
-        self.__MaxLabel.set(new_max)
-        self.__MinLabel.set_max_value(new_max - self.__min_range)
+        self._MaxLabel.set(new_max)
+        self._MinLabel.set_max_value(new_max - self._min_range)
 
     def set_min_limit(self, new_min_limit:int):
         '''updates min limit - does not change current values'''
-        self.__MinLabel.set_min_value(new_min_limit)
+        self._MinLabel.set_min_value(new_min_limit)
 
     def set_max_limit(self, new_max_limit:int):
         '''updates max limit - does not change current values'''
-        self.__MaxLabel.set_max_value(new_max_limit)
+        self._MaxLabel.set_max_value(new_max_limit)
 
     def set_min_range(self, min_range:int):
         '''updates the minimum allowed distance between min and max values'''
-        self.__min_range = min_range
-        self.__MaxLabel.set_min_value(self.__MinLabel.get() + self.__min_range)
-        self.__MinLabel.set_max_value(self.__MaxLabel.get() - self.__min_range)
+        self._min_range = min_range
+        self._MaxLabel.set_min_value(self._MinLabel.get() + self._min_range)
+        self._MinLabel.set_max_value(self._MaxLabel.get() - self._min_range)
 
-    def __min_callback(self, min_value:int):
+    def _min_callback(self, min_value:int):
         '''
         called when min label is changed
         updates minimum value of max label and calls callback function
         '''
-        self.__MaxLabel.set_min_value(min_value + self.__min_range)
-        if self.__callback_function is not None:
-            self.__callback_function(*self.get())
+        self._MaxLabel.set_min_value(min_value + self._min_range)
+        if self._callback_function is not None:
+            self._callback_function(*self.get())
 
-    def __max_callback(self, max_value:int):
+    def _max_callback(self, max_value:int):
         '''
         called when max label is changed
         updates maximum value of min label and calls callback function
         '''
-        self.__MinLabel.set_max_value(max_value - self.__min_range)
-        if self.__callback_function is not None:
-            self.__callback_function(*self.get())
+        self._MinLabel.set_max_value(max_value - self._min_range)
+        if self._callback_function is not None:
+            self._callback_function(*self.get())
 
     def get(self):
         '''
         Purpose:
             gets minimum and maximum value from EditLabels
         Pre-conditions:
             (none)
         Post-conditions:
             (none)
         Returns:
             :return int - minimum value
             :return int - maximum value
         '''
-        return self.__MinLabel.get(), self.__MaxLabel.get()
+        return self._MinLabel.get(), self._MaxLabel.get()
 
 class NumberIncrementLabel(Frame):
     ''' Widget that allows user to select a number by typing in CheckEntry
         or by clicking '+' and '-' buttons
         
         EditLabel is used to allow user to enter a number
```

### Comparing `chichitk-0.0.3/chichitk/pdf_display.py` & `chichitk-0.0.4/chichitk/pdf_display.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/player.py` & `chichitk-0.0.4/chichitk/player.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from tkinter import Frame
 
 from .timer import Timer
 from .buttons import PlayerButtons
-from .sliders import SimpleScrollBar, PlotScrollBar, DoubleScrollBar
+from .sliders import TimeSlider, PlotScrollBar, DoubleScrollBar
 
+# TODO: make TimeSlider attribute customizable through Player
 
 class Player(Frame):
     ''' Player executes a callback function with precise timing.
 
         Combines PlayerButtons and a scrollbar to give user control of playback
     
         Includes a scrollbar for user to control playing.
         
         An example use case could be playing frames from a video
     '''
     def __init__(self, master:Frame, callback, delay:float, bg:str='#000000',
                  slider_type:str='single', frame_num=1000, frame_rate=29.97,
                  step_increment:int=150, end_callback=None, start_callback=None,
                  stop_callback=None, skip_callback=None, buttons_on_top=False,
-                 buttons_padx_weight=6, value_display_fact=1):
+                 buttons_padx_weight=6, simple_slider_width=None,
+                 limit_running_callbacks=False):
         ''' Only keeps track of the current frame using Timer
 
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param callback: function (step) - called with each iteration
             :param delay: float - seconds between each iteration
@@ -35,69 +37,85 @@
             :param end_callback: function () - called when final step is reached
                                              - not called if looping is on
             :param start_callback: function (current_step) - called when timer is started
             :param stop_callback: function () - called when timer is stopped
             :param skip_callback: function (current_step) - called when step is incremented
             :param buttons_on_top: bool - True to put buttons on top, or False for bottom
             :param buttons_padx_weight: int - weight of padding for PlayerButtons
-            :param value_display_fact: int - pushed only to SimpleScrollBar
+            :param limit_running_callbacks: bool - if True, does not call callback function immediately when slider is moved while running
+                                                 - to avoid calling the callback function in multiple different threads
         '''
         self.__callback = callback
         self.__end_callback = end_callback
         self.__frame_rate = frame_rate
         self.__step_increment = step_increment
+        self.__slider_type = slider_type
+        self.__limit_running_callbacks = limit_running_callbacks
         super().__init__(master, bg=bg)
 
         # compute sides for widget packing
         sides = ['bottom', 'top']
         slider_side = sides[not buttons_on_top]
         buttons_side = sides[buttons_on_top]
 
         self.__Timer = Timer(delay, self.__timer_update, end_callback=self.__end,
                              start_callback=start_callback, stop_callback=stop_callback,
                              skip_callback=skip_callback, min_step=0, max_step=frame_num)
 
         if slider_type == 'simple':
-            self.__Slider = SimpleScrollBar(self, self.__slider_update, min_value=0,
-                                            max_value=frame_num, start_value=0, bg=bg,
-                                            value_display_fact=value_display_fact,
-                                            limit_labels=True)
+            self.__Slider = TimeSlider(self, self.__slider_update, bg=bg,
+                                       frame_num=frame_num, active_line_color='#ffffff',
+                                       active_line_hover_color='#13ce12', slider_color='#ffffff',
+                                       hide_slider=True, steps_per_sec=1/delay,
+                                       slider_type='circle', width=simple_slider_width)
         elif slider_type == 'single':
             self.__Slider = PlotScrollBar(self, self.__slider_update, None, frame_num,
                                           min_frame=0, start_frame=0, frame_rate=self.__frame_rate,
                                           height=60, bg=bg)
         elif slider_type == 'double':
             self.__Slider = DoubleScrollBar(self, self.__slider_update, None, frame_num,
                                             min_frame=0, start_frame=0, frame_rate=self.__frame_rate,
                                             bg=bg)
         self.__Slider.pack(side=slider_side, fill='x')
 
         self.__Buttons = PlayerButtons(self, bg, self.__Timer.start, self.__Timer.stop,
                                        self.step_forward, self.step_back,
-                                       self.__Timer.to_end, self.__Timer.reset,
+                                       self.to_end, self.to_start,
                                        padx_weight=buttons_padx_weight)
         self.__Buttons.pack(side=buttons_side, fill='x')
 
     def start(self):
         '''starts player - called externally - not from buttons'''
         self.__Timer.start()
         self.__Buttons.to_stop()
 
     def stop(self):
         '''stops player - called externally - not from buttons'''
         self.__Timer.stop()
         self.__Buttons.to_play()
 
+    def __callback_status(self):
+        '''returns True if callback should be called (for slider or command events)'''
+        return not self.__limit_running_callbacks or not self.is_running()
+
     def step_forward(self):
         '''same as clicking 'skip forward' button in PlayerButtons'''
-        self.__Timer.increment(self.__step_increment, callback=True)
+        self.__Timer.increment(self.__step_increment, callback=self.__callback_status())
 
     def step_back(self):
         '''same as clicking 'step back' button in PlayerButtons'''
-        self.__Timer.increment(-self.__step_increment, callback=True)
+        self.__Timer.increment(-self.__step_increment, callback=self.__callback_status())
+
+    def to_start(self):
+        '''same as clicking 'previous' button in PlayerButtons'''
+        self.__Timer.reset(callback=self.__callback_status())
+
+    def to_end(self):
+        '''same as clicking 'next' button in PlayerButtons'''
+        self.__Timer.to_end(callback=self.__callback_status())
 
     def set_frame(self, frame:int):
         '''updates the current frame and calls callback function'''
         self.__Timer.set(frame)
         self.__Slider.set_frame(frame)
         self.__callback(frame)
 
@@ -112,14 +130,16 @@
         self.__Timer.set_delay(1 / self.__frame_rate)
         self.__Slider.set_frame_num(self.__Timer.get_max_step(), self.__frame_rate)
 
     def set_delay(self, delay:float):
         '''updates delay of timer
         intended for when Player is not being used to play video frames'''
         self.__Timer.set_delay(delay)
+        if self.__slider_type == 'simple':
+            self.__Slider.set_steps_per_sec(1 / delay)
 
     def set_increment(self, inc:int):
         '''sets number of steps to skip when 'skip forward' and 'skip back'
         buttons are clicked'''
         self.__step_increment = inc
 
     def get_step(self) -> int:
@@ -134,24 +154,29 @@
         '''returns the maximum number of steps'''
         return self.__Timer.get_max_step()
 
     def get_frame_rate(self) -> float:
         '''returns frame rate'''
         return self.__frame_rate
 
+    def is_running(self) -> bool:
+        '''returns True if Player is running, otherwise False'''
+        return self.__Timer.is_running()
+
     def __timer_update(self, step:int):
         '''called by timer when playing'''
         self.__Slider.set_frame(step)
         self.__callback(step)
 
     def __slider_update(self, step:int):
         '''called when slider is moved by user
         it does not matter whether timer is running or not'''
         self.__Timer.set(step)
-        self.__callback(step)
+        if self.__callback_status():
+            self.__callback(step)
 
     def __end(self):
         '''called when player reaches the end (max step)'''
         if self.__Buttons.is_looped():
             self.__Timer.reset()
             self.__Timer.start()
         else: # no loop - actually stopping
```

### Comparing `chichitk-0.0.3/chichitk/progress_bar.py` & `chichitk-0.0.4/chichitk/progress_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,21 @@
         self.label = Label(self.frame, text=self.get_percentage_text(), bg=bg,
                            fg=text_color, font=(val_font_name, val_font_size))
         self.label.pack(side='left')
         self.bar_id = self.canvas.create_rectangle(*self.get_bar_coords(),
                                                    fill=active_color, width=0,
                                                    state='normal')
 
+    def set(self, perc:float):
+        '''sets progress bar given a completion percentage'''
+        assert perc >= 0 and perc <= 1, f'Progress Bar Error: Invalid completion percentage: {perc}'
+        self.current_value = int(self.iterations * perc)
+        self.canvas.coords(self.bar_id, *self.get_bar_coords())
+        self.label.config(text=self.get_percentage_text())
+
     def set_text(self, text:str):
         '''updates progress bar loading text'''
         self.loading_label.config(text=text)
 
     def get_percentage_text(self) -> str:
         '''return completion percentage'''
         perc = self.current_value * 100 / self.iterations
```

### Comparing `chichitk-0.0.3/chichitk/scrollable_frame.py` & `chichitk-0.0.4/chichitk/scrollable_frame.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/sliders.py` & `chichitk-0.0.4/chichitk/sliders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,716 +1,694 @@
 from tkinter import Canvas, Frame, Label
 
 import numpy as np
 
 from .tool_tip import ToolTip
-from .labels import EditLabel
+from .labels import NumberEditLabel
 from .canvas_items import CanvasEditLine, CanvasEditFill, brighten
 
+__all__ = ['Slider', 'TimeSlider', 'HorizontalSlider', 'VerticalSlider', 'ScrollBar',
+           'HorizontalSliderGroup', 'VerticalSliderGroup', 'PlotScrollBar', 'DoubleScrollBar', 'brighten']
 
 # helper functions
 def seconds_text(sec:float):
     '''converts seconds to text in form (hh):(m)m:ss'''
     sec = int(sec)
     if sec >= 3600: # at least one hour
         return f'{sec // 3600}:{(sec % 3600) // 60:0>2}:{(sec % 60) // 1:0>2}'
     else: # less than one hour
         return f'{sec // 60}:{(sec % 60) // 1:0>2}'
-    
 
-class BasicSlider(Frame):
-    ''' Parent class of HorizontalSlider and VerticalSlider - contains common
-        methods
-        
-        DO NOT use this class directly because it will not work
+
+class Slider(Canvas):
+    ''' Basic slider that takes values between 0 and 1
+
+        Can be configured horizontally or vertically with circle or rectangle
+        slider.
     '''
-    def __init__(self, master:Frame, command, bg:str, min_value:float,
-                 max_value:float, step:float, start_value=0, padx=0, pady=0,
-                 slider_ac='#13ce12', slider_ic='#ffffff', line_ac='#999999',
-                 line_ic='#888888', slider_height=20, slider_width=35, active=True):
+    def __init__(self, master:Frame, callback=None, default_value=0, bg='#000000',
+                 line_color='#555555', active_line_color=None, active_line_hover_color=None,
+                 slider_color='#ffffff', slider_drag_color=None, hide_slider=False,
+                 slider_visible=True, slider_height=20, slider_width=20, slider_type='circle',
+                 orientation='h', line_width=2, height=0, width=0, **kwargs):
         '''
         Parameters
         ----------
             :param master: tk.Frame - parent widget
-            :param command: function (value) - called when slider is moved
+            :param callback: function (float) - called only when slider is moved by user
+            :param default_value: float between 0 and 1 - initial slider value
             :param bg: str (hex code) - background color
-            :param min_value: float - slider minimum value
-            :param max_value: float - slider maximum value
-            :param step: float - slider increment
-            :param start_value: float - default value
-            :param padx: int - internal x pad
-            :param pady: int - internal y pad
-            :param slider_ac: str (hex code) - slider color while being dragged
-            :param slider_ic: str (hex code) - slider color when not dragging
-            :param line_ac: str (hex code) - line color when cursor is hovering
-            :param line_ic: str (hex code) - line color when not hovering
-            :param slider_height: int - height of slider in pixels
+            :param line_color: str (hex code) - color of line
+            :param active_line_color: str (hex code) - color of active portion of line (if different from line_color)
+            :param active_line_hover_color: str (hex code) - color of active portion of line when hovering
+                                                           - if different from active_line_color
+            :param slider_color: str (hex code) - slider color
+            :param slider_drag_color: str (hex code) - slider color when mouse is depressed (if different from slider color)
+            :param hide_slider: bool - if True, slider is hidden when cursor is not hovering
+            :param slider_visible: bool - if False, slider is never visible
+            :param slider_height: int - height of slider in pixels (or diameter for circle slider)
             :param slider_width: int - width of slider in pixels
-            :param active: bool - if True, slider is interactable by user
-        '''
-        self.active = active
-        self.command = command
-        if step % 1 == 0: # integer
-            self.decimals = 0
-        else:
-            self.decimals = len(str(step).split(".")[1])
-        self.slider_colors = [slider_ic, slider_ac]
-        self.line_colors = [line_ic, line_ac]
-        self.hovering, self.slider_hovering, self.dragging = False, False, False
-        self.min, self.max, self.current_value, self.step = min_value, max_value, start_value, step
-        self.values = np.arange(self.min, self.max + self.step * 0.9, self.step)
-        self.slider_height, self.slider_width = slider_height, slider_width
-        Frame.__init__(self, master, bg=bg, padx=padx, pady=pady)
-
-    def color_config(self):
-        '''updates color of line and slider based on hover and drag status'''
-        self.canvas.itemconfig(self.line_id, fill=self.line_colors[self.hovering or self.dragging])
-        self.canvas.itemconfig(self.slider_id, fill=self.slider_colors[self.slider_hovering or self.dragging])
-
-    def get_value_text(self) -> str:
-        '''returns value text formatted as string'''
-        if self.decimals == 0:
-            return str(int(self.current_value))
-        text = str(round(self.current_value, self.decimals))
-        if '.' in text:
-            dec = len(text.split(".")[1])
-        else:
-            text += '.'
-            dec = 0
-        return text + '0' * (self.decimals - dec)
-    
-    def get_value(self):
-        '''returns slider value'''
-        return self.current_value
-
-    def set_value(self, value:float, callback=False):
-        '''
-        Purpose:
-            sets the value of slider
-            called when slider is moved (with drag) or EditLabel is updated
-        Pre-conditions:
-            :param value: float - new value of slider
-            :param callback: bool - if True calls self.command(value)
-        Post-conditions:
-            changes the value of slider
-        Returns:
-            (none)
-        '''
-        self.current_value = value
-        self.canvas.coords(self.slider_id, *self.get_slider_coords())
-        self.label.set_text(text=self.get_value_text(), callback=False)
-        if callback:
-            self.command(self.current_value)
-
-    def round_value(self, value:float):
-        '''
-        Purpose:
-            rounds value to the closest acceptable value based on self.values
-            intended to be called when value is set manually with EditLabel
-        Pre-conditions:
-            :param value: float - new value
-        Post-conditions:
-            (none)
-        Returns:
-            :return: float or int - new rounded value
-        '''
-        return self.values[np.absolute(self.values - value).argmin()]
-
-    def slider_hover_enter(self, event=None):
-        '''called when cursor hovers on the slider'''
-        if self.active:
-            self.slider_hovering = True
-            self.color_config()
-
-    def slider_hover_leave(self, event=None):
-        '''called when cursor leaves the slider'''
-        if self.active:
-            self.slider_hovering = False
-            self.color_config()
+            :param slider_type: Literal['circle', 'rectangle'] - type of slider
+            :param orientation: Literal['h', 'v'] - horizontal or vertical orientation
+            :param line_width: int - width of slider line in pixels
+            :param height: int - canvas height in pixels
+            :param width: int - canvas width in pixels
+        '''
+        assert slider_type in ['circle', 'rectangle'], f'Slider Error: Invalid slider type: {slider_type}'
+        assert orientation in ['h', 'v'], f'Slider Error: Invalid orientation: {orientation}'
+        assert default_value >= 0 and default_value <= 1, f'Default value must be between 0 and 1, not {default_value}'
+        if slider_type == 'circle' and slider_height != slider_width: # not a circle (not fatal)
+            print(f'Slider Warning: Initiated circle slider but slider height ({slider_height}) does not equal slider width ({slider_width})')
+        canvas_height = slider_height if orientation == 'h' else height
+        canvas_width = slider_width if orientation == 'v' else width
+        super().__init__(master, bg=bg, highlightthickness=0,
+                         height=canvas_height, width=canvas_width, **kwargs)
+        self.__value = default_value
+        self.__callback = callback
+        self.__orientation = orientation
+        self.__slider_type = slider_type
+        self.__slider_height, self.__slider_width = slider_height, slider_width
+        self.__active_line_color = active_line_color if active_line_color is not None else line_color
+        self.__hover_line_color = active_line_hover_color if active_line_hover_color is not None else self.__active_line_color
+        self.__slider_color = slider_color if slider_color is not None else self.__active_line_color
+        self.__slider_drag_color = slider_drag_color if slider_drag_color is not None else self.__slider_color
+        self.__slider_state = 'hidden' if hide_slider or not slider_visible else 'disabled' # when not hovering
+        self.__slider_hover_state = 'disabled' if slider_visible else 'hidden' # when hovering
+        self.__dragging = False
+
+        # Draw Lines and Slider
+        self.__line_id = self.create_line(0, 0, 0, 0, fill=line_color,
+                                          width=line_width, state='disabled')
+        self.__active_line_id = self.create_line(0, 0, 0, 0, fill=self.__active_line_color,
+                                                 width=line_width, state='disabled')
+        if self.__slider_type == 'circle':
+            self.__slider_id = self.create_oval(0, 0, 0, 0, fill=self.__slider_color,
+                                                state=self.__slider_state)
+        elif self.__slider_type == 'rectangle':
+            self.__slider_id = self.create_rectangle(0, 0, 0, 0, fill=self.__slider_color,
+                                                     width=0, state=self.__slider_state)
+            
+        # Event Bindings
+        self.bind("<Button-1>", self.__click)
+        self.bind("<ButtonRelease-1>", self.__release)
+        self.bind("<B1-Motion>", self.__motion)
+        self.bind("<Enter>", self.__hover_enter)
+        self.bind("<Leave>", self.__hover_leave)
+        self.bind('<Configure>', self.__set_coords)
+        
+        self.event_generate('<Configure>', when='tail')
 
-    def label_hover_enter(self, event=None):
-        '''called when cursor enters the label'''
-        if self.popup_label:
-            self.tool_tip.fadein(0, self.popup_label, event)
+    def __set_coords(self, event=None):
+        '''updates coordinates of lines and slider based on canvas size and current value'''
+        h, w = self.winfo_height(), self.winfo_width()
+        rx, ry = self.__slider_width / 2, self.__slider_height / 2
+        if self.__orientation == 'h': # horizontal
+            x = (w - self.__slider_width) * self.__value + rx
+            y = h / 2
+            self.coords(self.__line_id, rx, y, w - rx, y)
+            self.coords(self.__active_line_id, rx, y, x, y)
+        elif self.__orientation == 'v': # vertical
+            x = w / 2
+            y = h - ry - (h - self.__slider_height) * self.__value
+            self.coords(self.__line_id, w / 2, ry, w / 2, h - ry)
+            self.coords(self.__active_line_id, x, y, x, h - ry)
+        self.coords(self.__slider_id, x - rx, y - ry, x + rx, y + ry)
+
+    def __get_value(self, x:float, y:float):
+        '''computes value based on (x, y) coordinates'''
+        if self.__orientation == 'h': # horizontal
+            value = (x - self.__slider_width / 2) / (self.winfo_width() - self.__slider_width)
+        elif self.__orientation == 'v': # vertical
+            value = (self.winfo_height() - self.__slider_height / 2 - y) / (self.winfo_height() - self.__slider_height)
+        return max(0, min(1, value))
+    
+    def __hover_enter(self, event=None):
+        '''cursor enters canvas'''
+        self.itemconfig(self.__active_line_id, fill=self.__hover_line_color)
+        self.itemconfig(self.__slider_id, state=self.__slider_hover_state)
+
+    def __hover_leave(self, event=None):
+        '''cursor leaves canvas'''
+        if not self.__dragging:
+            self.itemconfig(self.__active_line_id, fill=self.__active_line_color)
+            self.itemconfig(self.__slider_id, state=self.__slider_state)
+
+    def __click(self, event):
+        '''cursor clicks on canvas - move slider to click position'''
+        self.__dragging = True
+        self.itemconfig(self.__slider_id, fill=self.__slider_drag_color)
+        self.__value = self.__get_value(event.x, event.y)
+        self.__set_coords()
+        if self.__callback is not None:
+            self.__callback(self.__value)
+
+    def __release(self, event):
+        '''cursor releases click - change slider color to normal'''
+        self.__dragging = False
+        self.itemconfig(self.__slider_id, fill=self.__slider_color)
+        w, h = self.winfo_width(), self.winfo_height()
+        if event.x < 0 or event.x > w or event.y < 0 or event.y > h: # not hovering
+            self.__hover_leave()
+
+    def __motion(self, event):
+        '''cursor drags slider'''
+        self.__value = self.__get_value(event.x, event.y)
+        self.__set_coords()
+        if self.__callback is not None:
+            self.__callback(self.__value)
+
+    def set(self, value:float):
+        '''sets slider value - must be between 0 and 1 (does not call callback function)'''
+        assert value >= 0 and value <= 1, f'Slider Error: set slider to invalid value: {value}'
+        self.__value = value
+        self.__set_coords()
+
+    def get(self):
+        '''returns current slider value'''
+        return self.__value
 
-    def label_hover_leave(self, event=None):
-        '''called when cursor enters the label'''
-        if self.popup_label:
-            self.tool_tip.fadeout(1, event) # first argument is initial alpha
+class TimeSlider(Frame):
+    ''' Combines Slider with two labels to display a time slider.
+    
+        There can be multiple steps per second. The callback function is given
+        the current step not the current time
+    '''
+    def __init__(self, master:Frame, callback=None, frame_num=100, start_frame=0,
+                 steps_per_sec=1, bg='#000000', fg='#888888',
+                 val_font_name='Segoe UI', limit_font_name='Segoe UI',
+                 val_font_size=12, limit_font_size=12, **kwargs):
+        '''
+        Parameters
+        ----------
+            :param master: tk.Frame - parent widget
+            :param callback: function (int) - called when slider is moved
+            kwargs are passed to Slider (not Frame)
+        '''
+        super().__init__(master, bg=bg)
+        self.__callback = callback
+        self.__frame_num = frame_num
+        self.__steps_per_sec = steps_per_sec
+
+        # End Time Label - Right
+        self.__end_label = Label(self, text=seconds_text(frame_num / steps_per_sec),
+                                 bg=bg, fg=fg, font=(limit_font_name, limit_font_size))
+        self.__end_label.pack(side='right')
+
+        # Current Time Label - Left
+        self.__label = Label(self, text=seconds_text(start_frame / steps_per_sec),
+                             bg=bg, fg=fg, font=(val_font_name, val_font_size))
+        self.__label.pack(side='left')
+
+        # Slider - Center
+        self.__Slider = Slider(self, self.__slider_callback,
+                               default_value=start_frame / frame_num, bg=bg,
+                               orientation='h', **kwargs)
+        self.__Slider.pack(side='left', fill='x', expand=True)
+
+    def __slider_callback(self, perc:float):
+        '''called when slider is moved by user
+        :param perc: float between 0 and 1 - new slider value
+        '''
+        frame = self.__frame_num * perc
+        self.__label.config(text=seconds_text(frame / self.__steps_per_sec))
+        if self.__callback is not None:
+            self.__callback(int(frame))
+
+    def set_frame(self, frame:int):
+        '''sets current step - does not call callback function'''
+        assert frame <= self.__frame_num, f'TimeSlider Error: Tried to set frame to {frame} which is greater than max frame: {self.__frame_num}'
+        self.__Slider.set(frame / self.__frame_num)
+        self.__label.config(text=seconds_text(frame / self.__steps_per_sec))
+
+    def set_frame_num(self, frame_num:int, frame_rate):
+        '''sets max frame - frame_rate is just there for consistency with Scrollbars'''
+        self.__Slider.set(self.__frame_num * self.__Slider.get() / frame_num)
+        self.__frame_num = frame_num
+        self.__end_label.config(text=seconds_text(self.__frame_num / self.__steps_per_sec))
+
+    def set_steps_per_sec(self, steps_per_sec:float):
+        '''updates steps per sec without changing the number of steps'''
+        self.__steps_per_sec = steps_per_sec
+        self.__label.config(text=seconds_text(self.__Slider.get() * self.__frame_num / self.__steps_per_sec))
+        self.__end_label.config(text=seconds_text(self.__frame_num / self.__steps_per_sec))
+
+    def get(self) -> int:
+        '''returns the current frame'''
+        return int(self.__frame_num * self.__Slider.get())
+    
+    def get_sec(self) -> float:
+        '''returns current slider position in seconds'''
+        return self.__frame_num * self.__Slider.get() / self.__steps_per_sec
+
+class LabelSlider(Frame):
+    ''' Combination of Slider and NumberEditLabel so that slider value can be
+        seen by the user.
 
-    def hover_enter(self, event=None):
-        '''called when cursor enters the widget'''
-        if self.active:
-            self.hovering = True
-            self.color_config()
-
-    def hover_leave(self, event=None):
-        '''called when cursor leaves the widget'''
-        if self.active:
-            self.hovering = False
-            self.color_config()
-
-    def click(self, event):
-        '''cursor clicks on canvas - move slider to click location'''
-        if self.active:
-            self.dragging = True
-            self.color_config()
-            value = self.get_cursor_value(event.x, event.y)
-            if value != self.current_value:
-                self.set_value(value, callback=True)
-
-    def release(self, event=None):
-        '''cursor releases click on the canvas'''
-        if self.active:
-            self.dragging = False
-            self.color_config()
-
-    def motion(self, event):
-        '''called when cursor drags slider'''
-        if self.active:
-            value = self.get_cursor_value(event.x, event.y)
-            if value != self.current_value:
-                self.set_value(value, callback=True)
-
-    def turn_on(self):
-        '''called externally to make slider interactable by user'''
-        self.active = True
-        self.label.set_active()
-
-    def turn_off(self):
-        '''called externally to make slider uninteractable by user'''
-        self.active = False
-        self.label.set_inactive()
+        LabelSlider can handle any range of values, unlike Slider, which only
+        handles values between 0 and 1.
 
-class HorizontalSlider(BasicSlider):
-    ''' Horizontally oriented slider - user slides from left to right
+        LabelSlider has three components: slider, number label, and text label.
+        The number label displays the current value and text label is static.
 
-        User can double slick on the value label to enter an exact value
-    
-        Calls callback command whenever slider is moved by user
+        DO NOT user LabelSlider directly. It is only for inheritance from
+        HorizontalSlider and VerticalSlider.
     '''
-    def __init__(self, master:Frame, label:str, command, bg:str,
-                 min_value:float, max_value:float, step:float, start_value=0,
-                 popup_label=None, padx:int=0, pady:int=0, width:int=250,
-                 slider_ac='#13ce12', slider_ic='#ffffff', line_ac='#999999',
-                 line_ic='#888888', text_color='#888888', popup_bg='#000000',
-                 font_name='Segoe UI', label_font_size=14, val_font_size=11,
-                 slider_height=35, slider_width=20, line_width=10,
-                 justify='right', title_label=False, active=True):
-        '''Horizontal Slider
-        
+    def __init__(self, master:Frame, child_frame=None, callback=None, bg='#ffffff',
+                 label:str='', popup_label=None, font_name='Segoe UI', font_size=10,
+                 text_fg='#000000', popup_bg='#000000', popup_font_name=None,
+                 popup_font_size=None, min_value=0, max_value=100, step=1, default_value=None,
+                 label_editable=True, label_draggable=False, reference_width=2.0,
+                 max_len=None, drag_threshold=0.2, label_justify='left', label_bg=None,
+                 label_fg=None, label_hover_bg:str=None, label_error_color='#ff0000',
+                 line_color='#555555', active_line_color=None, active_line_hover_color=None,
+                 slider_color='#ffffff', slider_drag_color=None, hide_slider=False,
+                 slider_visible=True, slider_height=20, slider_width=20, slider_type='circle',
+                 orientation='h', line_width=2, canvas_height=0, canvas_width=0,
+                 **kwargs):
+        '''
         Parameters
         ----------
             :param master: tk.Frame - parent widget
-            :param label: str - label displayed to the left of slider
-            :param command: function (value) - called when slider is moved
-            :param bg: str (hex code) - background color
-            :param min_value: float - slider minimum value
-            :param max_value: float - slider maximum value
-            :param step: float - slider increment
-            :param start_value: float - default value
-            :param popup_label: str - text displayed in info popup upon mouse hover
-            :param padx: int (pixels) - internal x pad
-            :param pady: int (pixels) - internal y pad
-            :param width: int (pixels) - widget width
-            :param slider_ac: str (hex code) - slider color while being dragged
-            :param slider_ic: str (hex code) - slider color when not dragging
-            :param line_ac: str (hex code) - line color when cursor is hovering
-            :param line_ic: str (hex code) - line color when not hovering
-            :param slider_height: int - height of slider in pixels
+            :param child_frame: tk.Frame - to optionally put widgets in a frame other than self
+            :param callback: function (int|float), called when value is changed
+
+        Slider Parameters
+        -----------------
+            :param line_color: str (hex code) - color of line
+            :param active_line_color: str (hex code) - color of active portion of line (if different from line_color)
+            :param active_line_hover_color: str (hex code) - color of active portion of line when hovering
+                                                           - if different from active_line_color
+            :param slider_color: str (hex code) - slider color
+            :param slider_drag_color: str (hex code) - slider color when mouse is depressed (if different from slider color)
+            :param hide_slider: bool - if True, slider is hidden when cursor is not hovering
+            :param slider_visible: bool - if False, slider is never visible
+            :param slider_height: int - height of slider in pixels (or diameter for circle slider)
             :param slider_width: int - width of slider in pixels
-            :param text_color: String (hex code) - color of text
-            :param popup_bg: str (hex code) - background color of info popup
-            :param justify: str - slider placement in frame - options: ['left', 'right', 'center']
-            :param title_label: bool - if True, display 'fade_in' as 'Fade In' - convert snake_case to Title Case
-            :param active: bool - if True, slider is interactable by user
-        '''
-        self.width = width
-        BasicSlider.__init__(self, master, command, bg, min_value, max_value,
-                             step, start_value=start_value, padx=padx, pady=pady,
-                             slider_ac=slider_ac, slider_ic=slider_ic,
-                             line_ac=line_ac, line_ic=line_ic,
+            :param slider_type: Literal['circle', 'rectangle'] - type of slider
+            :param orientation: Literal['h', 'v'] - horizontal or vertical orientation
+            :param line_width: int - width of slider line in pixels
+            :param canvas_height: int - slider canvas height in pixels
+            :param canvas_width: int - slider canvas width in pixels
+
+        Label Parameters
+        ----------
+            :param min_value: int or float - minimum value
+            :param max_value: int or float - maximum value
+            :param step: int or float - number increment
+            :param default_value: int or float - default value if different from min_value
+            :param label_editable: bool - if True, label can be double clicked to enter exact value
+            :param label_draggable: bool - if True, label can be dragged to adjust value
+            :param reference_width: float - fraction of label width
+            :param max_len: int - maximum number of characters in entry box
+            :param drag_threshold: float (seconds) - click duration to be considered a single click (not drag)
+            :param label_justify: Literal['left', 'right', 'center'] - justification in label entry box
+            :param label_bg: str (hex code) - label background color (if different from bg)
+            :param label_fg: str (hex code) - label text color (if different from text_fg)
+            :param label_hover_bg: str (hex code) - label background color when hovering (if different from label_bg)
+            :param label_error_color: str (hex code) - background color in entry box for bad text
+        '''
+        if child_frame is None: # dont need to init Frame if nothing is being put in it
+            super().__init__(master, bg=bg, **kwargs)
+        self.__callback = callback
+
+        child_frame = child_frame if child_frame is not None else self
+
+        # Slider
+        self.Slider = Slider(child_frame, self.__slider_callback,
+                             bg=bg, line_color=line_color, active_line_color=active_line_color,
+                             active_line_hover_color=active_line_hover_color,
+                             slider_color=slider_color, slider_drag_color=slider_drag_color,
+                             hide_slider=hide_slider, slider_visible=slider_visible,
                              slider_height=slider_height, slider_width=slider_width,
-                             active=active)
+                             slider_type=slider_type, orientation=orientation,
+                             height=canvas_height, width=canvas_width,
+                             line_width=line_width)
+        
+        # Number Label
+        label_bg = label_bg if label_bg is not None else bg
+        label_fg = label_fg if label_fg is not None else text_fg
+        label_hover_bg = label_hover_bg if label_hover_bg is not None else label_bg
+        self.Label = NumberEditLabel(child_frame, self.__label_callback, min_value=min_value,
+                                     max_value=max_value, step=step, default_value=default_value,
+                                     reference_width=reference_width, max_len=max_len,
+                                     drag_threshold=drag_threshold, draggable=label_draggable,
+                                     editable=label_editable, justify=label_justify,
+                                     bg=label_bg, fg=label_fg, hover_bg=label_hover_bg,
+                                     error_color=label_error_color,
+                                     font_name=font_name, font_size=font_size)
+        
+        # Static Text Label
+        self.__popup_label = popup_label
+        self.Text = Label(child_frame, text=label, bg=bg, fg=text_fg, font=(font_name, font_size))
+        if self.__popup_label is not None:
+            popup_font_name = popup_font_name if popup_font_name is not None else font_name
+            popup_font_size = popup_font_size if popup_font_size is not None else font_size
+            self.tool_tip = ToolTip(self.Text, bg=popup_bg, fg='#ffffff',
+                                    font=(popup_font_name, popup_font_size))
+            self.Text.bind('<Enter>', self.__text_hover_enter)
+            self.Text.bind('<Leave>', self.__text_hover_leave)
+        
+        # Set Slider Value
+        self.Slider.set(self.Label.get_perc())
 
-        frame = Frame(self, bg=bg, height=slider_height)
-        if justify == 'center':
-            frame.place(relx=0.5, rely=0.5, anchor='center')
-        else:
-            frame.pack(side=justify)
-        check_function = lambda s: len(s) > 0 and s.count('.') <= 1 and s != '.' and float(s) >= self.min and float(s) <= self.max
-        self.label = EditLabel(frame, self.get_value_text(), fg=text_color, bg=bg, hover_bg=brighten(bg, 0.02),
-                               callback=lambda s: self.set_value(self.round_value(float(s)), callback=True),
-                               check_function=check_function, allowed_chars='0123456789.', editable=self.active,
-                               justify='left', font_name=font_name, font_size=val_font_size)
-        self.label.pack(side='right')
-        self.canvas = Canvas(frame, bg=bg, height=self.slider_height, width=self.width, highlightthickness=0)
-        self.canvas.pack(side='right')
-        label_text = label.replace('_', ' ').title() if title_label else label # convert from snake_case to Title Case
-        self.popup_label = label_text + ': ' + popup_label if popup_label else popup_label
-        slider_label = Label(frame, text=label_text, bg=bg, fg=text_color, font=(font_name, label_font_size))
-        slider_label.pack(side='right')
-        self.tool_tip = ToolTip(self, bg=popup_bg, fg='#ffffff', font=(font_name, val_font_size))
-        slider_label.bind('<Enter>', self.label_hover_enter)
-        slider_label.bind('<Leave>', self.label_hover_leave)
-
-        self.canvas.bind('<Enter>', self.hover_enter)
-        self.canvas.bind('<Leave>', self.hover_leave)
-        self.canvas.bind('<Button-1>', self.click)
-        self.canvas.bind('<B1-Motion>', self.motion)
-        self.canvas.bind('<ButtonRelease-1>', self.release)
-
-        self.line_id = self.canvas.create_line(self.slider_width / 2, self.slider_height / 2, self.width - self.slider_width / 2,
-                                                self.slider_height / 2, fill=self.line_colors[0],
-                                                width=line_width, state='disabled')
-        self.slider_id = self.canvas.create_rectangle(*self.get_slider_coords(), fill=self.slider_colors[0], width=0, state='normal')
-        self.canvas.tag_bind(self.slider_id, '<Enter>', self.slider_hover_enter)
-        self.canvas.tag_bind(self.slider_id, '<Leave>', self.slider_hover_leave)
-
-    def get_value_text(self) -> str:
-        '''returns value text formatted as string - overrides same function in BasicSlider'''
-        if self.decimals == 0:
-            return str(int(self.current_value)) + '  ' * (len(str(int(self.max))) - len(str(int(self.current_value))))
-        text = str(round(self.current_value, self.decimals))
-        if '.' in text:
-            dec = len(text.split(".")[1])
-        else:
-            text += '.'
-            dec = 0
-        return text + '0' * (self.decimals - dec) + '  ' * (len(str(int(self.max))) - len(str(int(self.current_value))))
-
-    def get_slider_coords(self):
-        '''returns x0, y0, x1, and y1 for slider based on self.current_value'''
-        perc = (self.current_value - self.min) / (self.max - self.min)
-        x_center = self.slider_width / 2 + (self.width - self.slider_width) * perc
-        return x_center - self.slider_width / 2, 0, x_center + self.slider_width / 2, self.slider_height
-
-    def get_cursor_value(self, x, y):
-        '''returns current_value based on x, y'''
-        perc = (x - self.slider_width / 2) / (self.width - self.slider_width)
-        value = self.min + (self.max - self.min) * perc
-        return self.values[np.absolute(self.values - value).argmin()]
+    def __text_hover_enter(self, event=None):
+        '''called when cursor enters the label'''
+        if self.__popup_label is not None:
+            self.tool_tip.fadein(0, self.__popup_label, event)
 
-class VerticalSlider(BasicSlider):
-    ''' Vertically oriented slider - user slides from bottom to top
-    
-        User can double click on the value label to enter an exact value
+    def __text_hover_leave(self, event=None):
+        '''called when cursor enters the label'''
+        if self.__popup_label is not None:
+            self.tool_tip.fadeout(1, event) # first argument is initial alpha
         
-        Calls callback command whenever slider is moved by user
+    def __slider_callback(self, perc:float):
+        '''called when slider is moved by user
+        :param perc: float between 0 and 1 - slider value
+        '''
+        self.Label.set_perc(perc)
+        if self.__callback is not None:
+            self.__callback(self.Label.get())
+
+    def __label_callback(self, value:float):
+        '''called when label value is changed by user'''
+        self.Slider.set(self.Label.get_perc())
+        if self.__callback is not None:
+            self.__callback(value)
+
+    def set_text(self, text:str):
+        '''sets static text'''
+        self.Text.config(text=text)
+
+    def set_min_value(self, min_value):
+        '''sets minimum value'''
+        self.Label.set_min_value(min_value)
+        self.Slider.set(self.Label.get_perc())
+
+    def set_max_value(self, max_value):
+        '''sets maximum value'''
+        self.Label.set_max_value(max_value)
+        self.Slider.set(self.Label.get_perc())
+
+    def set(self, value):
+        '''updates current value'''
+        self.Label.set(value)
+        self.Slider.set(self.Label.get_perc())
+
+    def get(self):
+        '''returns current value'''
+        return self.Label.get()
+
+class HorizontalSlider(LabelSlider):
+    ''' Horizontal adaptation of LabelSlider
+    
+        Value label and static text label can be on either side of the slider
+
+        There is the option for LabelSlider to be a single widget, or to grid
+        the children directly in the parent frame. To grid children in the
+        parent frame, specify the 'row' argument.
     '''
-    def __init__(self, master:Frame, label:str, command, bg:str,
-                 min_value:float, max_value:float, step:float, start_value=0,
-                 popup_label=None, padx=0, pady=0, height=250, slider_ac='#13ce12',
-                 slider_ic='#ffffff', line_ac='#999999', line_ic='#888888',
-                 text_color='#888888', popup_bg='#000000', font_name='Segoe UI',
-                 label_font_size=14, val_font_size=11, title_label=False,
-                 slider_height=20, slider_width=35, line_width=10, active=True):
-        '''Vertical Slider - inherits from tk.Frame - does not pack or grid
-        
+    def __init__(self, master:Frame, value_left=False, start_col=0, row=None,
+                 slider_pady=0, **kwargs):
+        '''
         Parameters
         ----------
-            :param master: tk.Frame - parent widget
-            :param label: str - label displayed to the left of slider
-            :param command: function (value) - called when slider is moved
-            :param bg: str (hex code) - background color
-            :param min_value: float - slider minimum value
-            :param max_value: float - slider maximum value
-            :param step: float - slider increment
-            :param start_value: float - default value
-            :param popup_label: str - text displayed in info popup upon mouse hover
-            :param padx: int (pixels) - internal x pad
-            :param pady: int (pixels) - internal y pad
-            :param height: int (pixels) - widget height
-            :param slider_ac: str (hex code) - slider color while being dragged
-            :param slider_ic: str (hex code) - slider color when not dragging
-            :param line_ac: str (hex code) - line color when cursor is hovering
-            :param line_ic: str (hex code) - line color when not hovering
-            :param slider_height: int - height of slider in pixels
-            :param slider_width: int - width of slider in pixels
-            :param text_color: String (hex code) - color of text
-            :param popup_bg: str (hex code) - background color of info popup
-            :param justify: str - slider placement in frame - options: ['left', 'right', 'center']
-            :param title_label: bool - if True, display 'fade_in' as 'Fade In' - convert snake_case to Title Case
-            :param active: bool - if True, slider is interactable by user
-        '''
-        self.height = height
-        BasicSlider.__init__(self, master, command, bg, min_value, max_value, step, start_value=start_value, padx=padx, pady=pady,
-                                slider_ac=slider_ac, slider_ic=slider_ic, line_ac=line_ac, line_ic=line_ic, slider_height=slider_height,
-                                slider_width=slider_width, active=active)
-
-        label_text = label.replace('_', ' ').title() if title_label else label
-        self.popup_label = label_text + ': ' + popup_label if popup_label else popup_label
-        slider_label = Label(self, text=label_text, bg=bg, fg=text_color, font=(font_name, label_font_size))
-        slider_label.pack(side='top', fill='x')
-        self.tool_tip = ToolTip(self, bg=popup_bg, fg='#ffffff', font=(font_name, val_font_size))
-        slider_label.bind('<Enter>', self.label_hover_enter)
-        slider_label.bind('<Leave>', self.label_hover_leave)
-        check_function = lambda s: len(s) > 0 and s.count('.') <= 1 and s != '.' and float(s) >= self.min and float(s) <= self.max
-        self.label = EditLabel(self, self.get_value_text(), fg=text_color, bg=bg, hover_bg=brighten(bg, 0.02),
-                               callback=lambda s: self.set_value(self.round_value(float(s)), callback=True),
-                               check_function=check_function, allowed_chars='0123456789.', editable=self.active,
-                               justify='center', font_name=font_name, font_size=val_font_size)
-        self.label.pack(side='bottom', fill='x')
-        self.canvas = Canvas(self, bg=bg, height=self.height, width=self.slider_width, highlightthickness=0)
-        self.canvas.pack(side='top')
-        self.canvas.bind('<Enter>', self.hover_enter)
-        self.canvas.bind('<Leave>', self.hover_leave)
-        self.canvas.bind('<Button-1>', self.click)
-        self.canvas.bind('<B1-Motion>', self.motion)
-        self.canvas.bind('<ButtonRelease-1>', self.release)
+            :param master: tk.Frame - parent frame
+            :param value_left: bool - True to put value label on left side and text on right side
+            :param start_col: int - start column (only if widgets are directly in master)
+            :param row: int - row in master or None to put widgets in self
+        '''
+        child_frame = master if row is not None else None
+        super().__init__(master, child_frame=child_frame, orientation='h', **kwargs)
+
+        if row is not None: # to grid widgets in master
+            if value_left:
+                value_col, text_col = start_col, 2 + start_col
+            else:
+                value_col, text_col = 2 + start_col, start_col
+            slider_col = 1 + start_col
+            self.Slider.grid(row=row, column=slider_col, pady=slider_pady, sticky='ew')
+            self.Label.grid(row=row, column=value_col, pady=slider_pady, sticky='nsew')
+            self.Text.grid(row=row, column=text_col, pady=slider_pady, sticky='nsew')
+        else: # pack in self
+            if value_left:
+                value_side, text_side = 'left', 'right'
+            else:
+                value_side, text_side = 'right', 'left'
+            self.Label.pack(side=value_side)
+            self.Text.pack(side=text_side)
+            self.Slider.pack(side='left', fill='x', expand=True)
+
+class VerticalSlider(LabelSlider):
+    ''' Vertical adaptation of LabelSlider
+    '''
+    def __init__(self, master:Frame, **kwargs):
+        super().__init__(master, orientation='v', label_justify='center', **kwargs)
+
+        self.Label.pack(side='bottom', fill='x') # not sure if this should fill
+        self.Slider.pack(side='bottom', fill='y', expand=True)
+        if 'label' in kwargs.keys() and kwargs['label'] != '': # only pack Text if there is a label
+            self.Text.pack(side='top')
+
+class ScrollBar(Canvas):
+    ''' ScrollBar for navigating scrollable widgets
     
-        self.line_id = self.canvas.create_line(self.slider_width / 2, self.slider_height / 2, self.slider_width / 2,
-                                                self.height - self.slider_height / 2, fill=self.line_colors[0],
-                                                width=line_width, state='disabled')
-        self.slider_id = self.canvas.create_rectangle(*self.get_slider_coords(), fill=self.slider_colors[0], width=0, state='normal')
-        self.canvas.tag_bind(self.slider_id, '<Enter>', self.slider_hover_enter)
-        self.canvas.tag_bind(self.slider_id, '<Leave>', self.slider_hover_leave)
-
-    def get_slider_coords(self):
-        '''returns x0, y0, x1, and y1 for slider based on self.current_value'''
-        perc = (self.current_value - self.min) / (self.max - self.min)
-        y_center = self.slider_height / 2 + (self.height - self.slider_height) * (1 - perc)
-        return 0, y_center - self.slider_height / 2, self.slider_width, y_center + self.slider_height / 2
-
-    def get_cursor_value(self, x, y):
-        '''returns current_value based on x, y'''
-        perc = (self.height - y - self.slider_height / 2) / (self.height - self.slider_height)
-        value = self.min + (self.max - self.min) * perc
-        return self.values[np.absolute(self.values - value).argmin()]
-
-class SimpleScrollBar(Canvas):
-    ''' Slider that handles integer values between a specified minimum and
-        maximum value
+        Only handles values between 0 and 1
         
-        Callback command is called whenever slider value is changed by user
+        The current position is defined by two values that correspond to the
+        visible start and end point of the linked scrollable widget
     '''
-    def __init__(self, frame, command, min_value=0, max_value=100, start_value=0,
-                 padx=0.04, pady=5, radius=10, error_margin=0.015, font_size=8,
-                 val_label=False, limit_labels=False, bg='#000000', pack_side='top',
-                 active_color='#13ce12', inactive_color='#888888', dot_color='#ffffff',
-                 text_color='#888888', drag_color='#ffffff', time_mode=False, mouse_wheel=False,
-                 val_label_font_name='Segoe UI bold', val_label_font_size=14,
-                 limit_label_font_name='Segoe UI', limit_label_font_size=12,
-                 value_display_fact=1):
-        '''basic scroll bar to play videos, set parameters, etc
-        
+    def __init__(self, master:Frame, callback=None, default0=0, default1=1,
+                 bg:str='#ffffff', slider_color:str='#000000',
+                 slider_hover_color=None, slider_drag_color=None,
+                 width=None, height=None, orientation='h',
+                 disappear_when_filled=True):
+        '''
         Parameters
         ----------
-            :param frame: tk.Frame - parent widget
-            :param command: function (value) - functions called whenever scrollbar value is changed
-            :param min_value: int - minimum value for slider
-            :param max_value: int - maximum value for slider
-            :param padx: float - x pad as a percentage of widget width
-            :param pady: int - y pad in pixels
-            :param radius: int - radius of draggable circle in pixels
-            :param font_size: int - size of min/max value labels, if there are any
+            :param master: Frame - parent widget
+            :param callback: function (float, float) - called when slider is moved
+                                                     - takes two values between 0 and 1
+            :param default0: float (between 0 and 1) - default lower bound
+            :param default1: float (between 0 and 1) - default upper bound
             :param bg: str (hex code) - slider background color
-            :param active_color: str (hex code) - color for active portion of slider on hover
-            :param inactive_color: str (hex code) - color for inactive portion of slider when cursor is not hovering
-            :param dot_color: str (hex code) - color for inactive portion when not hovering and dot when hovering
-            :param text_color: str (hex code) - color of text
-            :param error_margin: float - cursor will be considered on the slider if it is within (error_margin * plot width) of slider position
-            :param mouse_wheel: bool - make scrollbar scrollable using mouse wheel
-            :param value_display_fact: float - values are multiplied by this fact only when being displayed
-                                             - this does not affect the callback function
-        '''
-        self.command = command
-        self.min, self.max = min_value, max_value
-        self.padx, self.pady = padx, pady
-        self.r = radius
-        self.error_margin = error_margin
-        self.font_size = font_size
-        self.val_label, self.limit_labels = val_label, limit_labels
-        self.val_label_font_name, self.val_label_font_size = val_label_font_name, val_label_font_size
-        self.limit_label_font_name, self.limit_label_font_size = limit_label_font_name, limit_label_font_size
-        self.inactive_color = inactive_color
-        self.line_colors = [dot_color, active_color]
-        self.circle_colors = [dot_color, drag_color]
-        self.text_color = text_color
-        self.line_id, self.active_line_id, self.circle_id, self.label_id, self.min_label_id, self.max_label_id, self.width = [None] * 7
-        self.dragging, self.hovering = [False] * 2
-        self.time_mode = time_mode
-        self.active = True
-        self.circle_states = ['hidden', 'normal']
-        self.current_value = start_value
-        self.line_height = self.pady + self.r
-        self.value_display_fact = value_display_fact
-
-        super().__init__(frame, height=(self.pady + self.r) * 2 + 22 * self.val_label,
-                         bg=bg, highlightthickness=0)
-        self.pack(side=pack_side, fill='x')
-        self.bind("<Button-1>", lambda e: self.toggle_circle(e, True))
-        self.bind("<ButtonRelease-1>", lambda e: self.toggle_circle(e, False))
-        self.bind("<B1-Motion>", self.drag_move)
-        self.bind("<Enter>", lambda e: self.update_hover(True))
-        self.bind("<Leave>", lambda e: self.update_hover(False))
-        self.bind('<Configure>', self.frame_width)
-        if mouse_wheel:
-            self.bind('<MouseWheel>', self.mouse_wheel_scroll)
+            :param slider_color: str (hex code) - slider color when not hovering or dragging
+            :param slider_hover_color: str (hex code) - slider color when hovering (if different from slider color)
+            :param slider_drag_color: str (hex code) - slider color when dragging (if different from hover color)
+            :param width: int (pixels) or None - canvas width (for vertical orientation)
+            :param height: int (pixels) or None - canvas height (for horiontal orientation)
+            :param orientation: Literal['h', 'v'] - horizontal or vertical orientation
+            :param disappear_when_filled: bool - if True hides slider when no scrolling is possible
+        '''
+        assert orientation in ['h', 'v'], f'ScrollBar Error: Invalid orientation: {orientation}'
+        assert default0 >= 0 and default0 <= 1, f'ScrollBar Error: Default0 out of range: {default0}'
+        assert default1 >= 0 and default1 <= 1, f'ScrollBar Error: Default1 out of range: {default1}'
+
+        super().__init__(master, bg=bg, width=width, height=height, highlightthickness=0)
+
+        self.__dragging = False
+        self.__callback = callback
+        self.__orientation = orientation
+        self.__p0, self.__p1 = default0, default1
+        self.__disappear_when_filled = disappear_when_filled
+        self.__slider_color = slider_color
+        self.__slider_hover_color = slider_hover_color if slider_hover_color is not None else self.__slider_color
+        self.__slider_drag_color = slider_drag_color if slider_drag_color is not None else self.__slider_hover_color
+
+        self.__slider_id = self.create_rectangle(0, 0, 0, 0, fill=self.__slider_color,
+                                                 width=0, state='normal')
+        
+        # Event Bindings
+        self.tag_bind(self.__slider_id, "<Button-1>", self.__click)
+        self.tag_bind(self.__slider_id, "<ButtonRelease-1>", self.__release)
+        self.tag_bind(self.__slider_id, "<B1-Motion>", self.__motion)
+        self.tag_bind(self.__slider_id, "<Enter>", self.__hover_enter)
+        self.tag_bind(self.__slider_id, "<Leave>", self.__hover_leave)
+        
+        self.bind('<Configure>', self.__set_coords)
+        
         self.event_generate('<Configure>', when='tail')
 
-    def frame_width(self, event):
-        '''called whenever window is resized'''
-        self.width = event.width
-        self.update_width()
-        self.draw()
-
-    def format_text(self, val:int) -> str:
-        '''takes as input either self.max or self.current_value
-        returns str according to self.time_mode'''
-        val = int(round(val * self.value_display_fact, 0))
-        if self.time_mode:
-           return seconds_text(val)
+    def __set_coords(self, event=None, filled_thresh=0.001):
+        '''updates coordinates of lines and slider based on canvas size and current value'''
+        # sets slider coordinates based on self.__p0 and self.__p1
+        h, w = self.winfo_height(), self.winfo_width()
+        if self.__orientation == 'h': # horizontal
+            y0, y1 = 0, h
+            x0, x1 = self.__p0 * w, self.__p1 * w
+        elif self.__orientation == 'v': # vertical
+            x0, x1 = 0, w
+            y0, y1 = self.__p0 * h, self.__p1 * h
+        self.coords(self.__slider_id, x0, y0, x1, y1)
+        if self.__disappear_when_filled and self.__p0 < filled_thresh and self.__p1 > 1 - filled_thresh:
+            self.itemconfig(self.__slider_id, state='hidden')
         else:
-            return str(val)
+            self.itemconfig(self.__slider_id, state='normal')
     
-    def update_width(self):
-        '''called after self.width is updated'''
-        self.xmin = self.width * self.padx + 10 * len(self.format_text(self.max)) * self.limit_labels
-        self.xmax = self.width * (1 - self.padx) - 10 * len(self.format_text(self.max)) * self.limit_labels
-
-    def set_limits(self, min_value:int, max_value:int):
-        if min_value != self.min or max_value != self.max:
-            self.min, self.max = min_value, max_value
-            self.current_value = min(self.max, max(self.min, self.current_value))
-            self.draw()
-
-    def set_value(self, value:int, call_command=False):
-        '''moves circle and calls command if value if different from self.current_value'''
-        if self.current_value != value:
-            self.current_value = value
-            x_pos = self.xmin + (self.xmax - self.xmin) * (self.current_value - self.min) / (self.max - self.min)
-            self.coords(self.active_line_id, self.xmin, self.line_height, x_pos, self.line_height)
-            self.coords(self.circle_id, x_pos - self.r, self.line_height - self.r, x_pos + self.r, self.line_height + self.r)
-            if self.val_label:
-                self.itemconfig(self.label_id, text=self.format_text(self.current_value))
-            if self.limit_labels:
-                self.itemconfig(self.min_label_id, text=self.format_text(self.current_value))
-            if call_command:
-                self.command(self.current_value)
-
-    def set_frame(self, value:int):
-        '''
-        doubles self.set_value - necessary because this was designed stupidly
-        does not call callback command
-        '''
-        self.set_value(value, call_command=False)
-
-    def set_frame_num(self, max_value:int, frame_rate):
-        '''for consistency with PlotScrollbar'''
-        self.set_limits(0, max_value)
-
-    def turn_on(self, override=True):
-        '''
-        makes slider interactable by user
-        if override is True, will turn on even if already on
-        '''
-        if override or not self.active:
-            self.active = True
-            self.itemconfig(self.circle_id, fill=self.inactive_color)
-            if self.val_label:
-                self.itemconfig(self.label_id, fill='#ffffff')
-
-    def turn_off(self, override=True):
-        '''
-        makes slider uninteractable by user
-        if override is True, will turn off even if already off
-        '''
-        if override or self.active:
-            self.active = False
-            self.itemconfig(self.circle_id, fill=brighten(self.inactive_color, -0.4))
-            if self.val_label:
-                self.itemconfig(self.label_id, fill=brighten(self.inactive_color, -0.4))
-
-    def remove(self):
-        '''removes everything from the canvas'''
-        if self.line_id is not None:
-            self.delete(self.line_id)
-            self.line_id = None
-        if self.active_line_id is not None:
-            self.delete(self.active_line_id)
-            self.active_line_id = None
-        if self.circle_id is not None:
-            self.delete(self.circle_id)
-            self.circle_id = None
-        if self.label_id is not None:
-            self.delete(self.label_id)
-            self.label_id = None
-        if self.min_label_id is not None:
-            self.delete(self.min_label_id)
-            self.min_label_id = None
-        if self.max_label_id is not None:
-            self.delete(self.max_label_id)
-            self.max_label_id = None
-
-    def draw(self):
-        '''called when window is resized - redraws canvas according to new size'''
-        if not self.width:
-            return None
-        self.remove()
-        self.line_id = self.create_line(self.xmin, self.line_height, self.xmax, self.line_height,
-                                                fill=brighten(self.inactive_color, -0.4), width=2)
-        x_pos = self.xmin + (self.xmax - self.xmin) * (self.current_value - self.min) / (self.max - self.min)
-        self.active_line_id = self.create_line(self.xmin, self.line_height, x_pos, self.line_height, fill=self.line_colors[0], width=2)
-        self.circle_id = self.create_oval(x_pos - self.r, self.line_height - self.r, x_pos + self.r, self.line_height + self.r,
-                                                    fill=self.circle_colors[0], state='hidden')
-        if self.val_label:
-            self.label_id = self.create_text(self.width / 2, self.pady + self.r * 2 - 1, text=str(self.current_value), fill='#ffffff',
-                                                        font=(self.val_label_font_name, self.val_label_font_size), anchor='n')
-        if self.limit_labels:
-            self.min_label_id = self.create_text(self.xmin - self.r - 2, self.line_height, text=self.format_text(self.current_value),
-                                                        fill=self.inactive_color, font=(self.limit_label_font_name, self.limit_label_font_size),
-                                                        anchor='e')
-            self.max_label_id = self.create_text(self.xmax + self.r + 2, self.line_height, text=self.format_text(self.max),
-                                                        fill=self.inactive_color, font=(self.limit_label_font_name, self.limit_label_font_size),
-                                                        anchor='w')
-        if not self.active:
-            self.turn_off()
-
-    def update_hover(self, hover:bool):
-        '''called when cursor enters or leaves line'''
-        if self.active:
-            self.hovering = hover
-            self.itemconfig(self.active_line_id, fill=self.line_colors[self.hovering or self.dragging])
-            self.itemconfig(self.circle_id, state=self.circle_states[self.hovering or self.dragging])
-
-    def toggle_circle(self, event, onclick:bool):
-        '''mouse clicks or releases click anywhere on canvas'''
-        if self.active:
-            self.dragging = onclick
-            self.itemconfig(self.circle_id, fill=self.circle_colors[self.dragging])
-            self.drag_move(event)
-            if not self.dragging and not self.hovering:
-                self.update_hover(False)
-
-    def drag_move(self, event):
-        '''called when mouse drags slider'''
-        if self.active:
-            x_perc = (event.x - self.xmin) / (self.xmax - self.xmin)
-            value = self.min + (self.max- self.min) * x_perc
-            self.set_value(int(round(min(self.max, max(self.min, value)), 0)), call_command=True)
-
-    def mouse_wheel_scroll(self, event, fact=1):
-        '''called when mouse wheel is scrolled while mouse hovers on slider'''
-        # event.delta / 120 is float - number of scroll steps - positive for up, negative for down
-        if self.active:
-            value = self.current_value + event.delta / 120 * fact
-            self.set_value(int(min(self.max, max(self.min, value))), call_command=True)
+    def __hover_enter(self, event=None):
+        '''cursor enters canvas'''
+        self.itemconfig(self.__slider_id, fill=self.__slider_hover_color)
+
+    def __hover_leave(self, event=None):
+        '''cursor leaves canvas'''
+        if not self.__dragging:
+            self.itemconfig(self.__slider_id, fill=self.__slider_color)
+
+    def __click(self, event):
+        '''cursor clicks on canvas - move slider to click position'''
+        self.__dragging = True
+        self.itemconfig(self.__slider_id, fill=self.__slider_drag_color)
+        x0, y0, _, _ = self.coords(self.__slider_id)
+        self.__click_x = event.x - x0 # pixels from mouse to left edge of slider
+        self.__click_y = event.y - y0 # pixels from mouse to top edge of slider
+
+    def __release(self, event):
+        '''cursor releases click - change slider color to normal'''
+        self.__dragging = False
+        self.itemconfig(self.__slider_id, fill=self.__slider_hover_color)
+        x0, y0, x1, y1 = self.coords(self.__slider_id)
+        if event.x < x0 or event.x > x1 or event.y < y0 or event.y > y1: # not hovering
+            self.__hover_leave()
+
+    def __motion(self, event):
+        '''cursor drags slider'''
+        x0, y0, x1, y1 = self.coords(self.__slider_id)
+        w, h = self.winfo_width(), self.winfo_height()
+        if self.__orientation == 'h':
+            add = max(-x0, min(w - x1, (event.x - x0) - self.__click_x))
+            x0 += add
+            x1 += add
+            self.__p0, self.__p1 = x0 / w, x1 / w
+        elif self.__orientation == 'v':
+            add = max(-y0, min(h - y1, (event.y - y0) - self.__click_y))
+            y0 += add
+            y1 += add
+            self.__p0, self.__p1 = y0 / h, y1 / h
+        self.coords(self.__slider_id, x0, y0, x1, y1)
+        if self.__callback is not None:
+            self.__callback(self.__p0, self.__p1)
+
+    def set(self, p0:float, p1:float):
+        '''sets slider value - must be between 0 and 1 (does not call callback function)'''
+        assert p0 >= 0 and p0 <= 1, f'ScrollBar Error: set lower bound to invalid value: {p0}'
+        assert p1 >= 0 and p1 <= 1, f'ScrollBar Error: set upper bound to invalid value: {p1}'
+        assert p1 >= p0 ,f'ScrollBar Error: lower bound is greater than upper bound! lower: {p0}, upper: {p1}'
+        self.__p0, self.__p1 = p0, p1
+        self.__set_coords()
+
+    def get(self):
+        '''returns current slider value'''
+        return self.__p0, self.__p1
 
-class VerticalSliderGroup(Frame):
-    ''' Group of vertically oriented sliders connected by a single callback
+
+class HorizontalSliderGroup(Frame):
+    ''' Group of horizontally oriented sliders connected by a single callback
         function
         
         The callback function is called whenever any of the slider values is
         changed by the user and is given 2 arguments: (slider_label, new_value)
     '''
-    def __init__(self, master, parameters:list, callback, bg:str, rows:int,
-                 columns:int, height=250, slider_pady=5, slider_padx=5,
-                 slider_ac='#13ce12', slider_ic='#ffffff', line_ac='#999999',
-                 line_ic='#888888', text_color='#888888', font_name='Segoe UI',
-                 label_font_size=14, val_font_size=11, slider_height=20,
-                 slider_width=35, line_width=10, title_label=True):
-        '''Group of vertical sliders aranged in rows and columns
+    def __init__(self, master:Frame, parameters:list, callback, bg='#ffffff',
+                 width=250, slider_pady=5, frame_padx=0, title_label=True,
+                 **kwargs):
+        '''Group of horizontal sliders aranged in a single column
         
         Parameters
         ----------
             :param master: tk.Frame - frame in which to put slider group
             :param parameters: list of dicts - each dict contains the keys:
                         label: str - slider name (given to callback function)
                         value: float - default value
                         min_value: float - minimum value
                         max_value: float - maximum value
                         step: float - slider increment
-                        description: str - info displayed when mouse hovers on slider
+                        description: str - info displayed when mouse hovers on slider (optional)
             :param callback: function (parameter_name, value) - called whenever a slider is adjusted
             :param bg: str (hex code) - background color
-            :param rows: int - rows of sliders - filling begins rowwise at top left
-            :param columns: int - columns of sliders - filling begins rowwise at top left
-            :param height: int - height of each slider in pixels
-            :param pady: int - y pad inside each slider
-            :param slider_ac: str (hex code) - color of slider when mouse button is depressed
-            :param slider_ic: str (hex code) - color of slider when mouse button is not depressed
-            :param line_ac: str (hex code) - color of line when mouse is on Canvas
-            :param line_ic: str (hex code) - color of line when mouse is not on Canvas
-            :param text_color: str (hex code) - color of text
+            :param width: int - width of each slider in pixels
+            :param slider_pady: int - y pad inside sliders
+            :param frame_padx: int - x pad inside frame
             :param title_label: bool - if True display 'fade_in' as 'Fade In'
+            **kwargs passed to each slider
         '''
-        Frame.__init__(self, master, bg=bg)
-        for i in range(rows):
-            self.grid_rowconfigure(i, weight=1)
-        for i in range(columns):
-            self.grid_columnconfigure(i, weight=1)
-        self.sliders = []
+        Frame.__init__(self, master, bg=bg, padx=frame_padx)
+        self.grid_columnconfigure(0, weight=0) # text label
+        self.grid_columnconfigure(1, weight=1) # slider
+        self.grid_columnconfigure(2, weight=0) # value label
+        self.sliders: list[HorizontalSlider] = []
+        self.labels = [d['label'] for d in parameters]
         for i, param in enumerate(parameters):
-            S = VerticalSlider(self, param['label'], lambda x, l=param['label']: callback(l, x),
-                               bg, param['min_value'], param['max_value'],
-                               param['step'], start_value=param['value'],
-                               popup_label=param['description'], padx=slider_padx,
-                               pady=slider_pady, height=height, slider_ac=slider_ac,
-                               slider_ic=slider_ic, line_ac=line_ac, line_ic=line_ic,
-                               text_color=text_color, font_name=font_name,
-                               label_font_size=label_font_size, val_font_size=val_font_size,
-                               slider_height=slider_height, slider_width=slider_width,
-                               line_width=line_width, title_label=title_label)
-            S.grid(row=i // columns, column=i % columns, sticky='nsew')
+            label = param['label'].replace('_', ' ').title() if title_label else param['label']
+            popup_label = param['description'] if 'description' in param.keys() else None
+            S = HorizontalSlider(self, start_col=0, row=i, bg=bg, canvas_width=width,
+                                 callback=lambda x, l=param['label']: callback(l, x),
+                                 min_value=param['min_value'], max_value=param['max_value'],
+                                 step=param['step'], default_value=param['value'],
+                                 label=label, popup_label=popup_label,
+                                 slider_pady=slider_pady, **kwargs)
             self.sliders.append(S)
 
-class HorizontalSliderGroup(Frame):
-    ''' Group of horizontally oriented sliders connected by a single callback
+    def get(self) -> dict:
+        '''returns dictionary with current value of each slider'''
+        return [{label:slider.get()} for label, slider in zip(self.labels, self.sliders)]
+
+class VerticalSliderGroup(Frame):
+    ''' Group of vertically oriented sliders connected by a single callback
         function
         
         The callback function is called whenever any of the slider values is
         changed by the user and is given 2 arguments: (slider_label, new_value)
     '''
-    def __init__(self, master, parameters:list, callback, bg:str,
-                 width=250, slider_pady=5, slider_padx=5,
-                 slider_ac='#13ce12', slider_ic='#ffffff', line_ac='#999999',
-                 line_ic='#888888', text_color='#888888', font_name='Segoe UI',
-                 label_font_size=14, val_font_size=11,
-                 slider_height=35, slider_width=18, line_width=10, title_label=True):
-        '''Group of horizontal sliders aranged in a single column
+    def __init__(self, master, parameters:list, callback, bg:str, rows:int,
+                 columns:int, height=250, slider_pady=5, slider_padx=5,
+                 title_label=True, **kwargs):
+        '''Group of vertical sliders aranged in rows and columns
         
         Parameters
         ----------
             :param master: tk.Frame - frame in which to put slider group
             :param parameters: list of dicts - each dict contains the keys:
                         label: str - slider name (given to callback function)
                         value: float - default value
                         min_value: float - minimum value
                         max_value: float - maximum value
                         step: float - slider increment
                         description: str - info displayed when mouse hovers on slider
             :param callback: function (parameter_name, value) - called whenever a slider is adjusted
             :param bg: str (hex code) - background color
-            :param width: int - width of each slider in pixels
-            :param pady: int - y pad inside each slider
-            :param slider_ac: str (hex code) - color of slider when mouse button is depressed
-            :param slider_ic: str (hex code) - color of slider when mouse button is not depressed
-            :param line_ac: str (hex code) - color of line when mouse is on Canvas
-            :param line_ic: str (hex code) - color of line when mouse is not on Canvas
-            :param text_color: str (hex code) - color of text
+            :param rows: int - rows of sliders - filling begins rowwise at top left
+            :param columns: int - columns of sliders - filling begins rowwise at top left
+            :param height: int - height of each slider in pixels
+            :param slider_pady: int - y pad between sliders
+            :param slider_padx: int - x pad between sliders
             :param title_label: bool - if True display 'fade_in' as 'Fade In'
+            **kwargs passed to each slider
         '''
         Frame.__init__(self, master, bg=bg)
-        self.sliders = []
-        for param in parameters:
-            S = HorizontalSlider(self, param['label'], lambda x, l=param['label']: callback(l, x),
-                                 bg, param['min_value'], param['max_value'],
-                                 param['step'], start_value=param['value'],
-                                 popup_label=param['description'], padx=slider_padx,
-                                 pady=slider_pady, width=width, slider_ac=slider_ac,
-                                 slider_ic=slider_ic, line_ac=line_ac, line_ic=line_ic,
-                                 text_color=text_color, font_name=font_name,
-                                 label_font_size=label_font_size, val_font_size=val_font_size,
-                                 justify='right', slider_height=slider_height,
-                                 slider_width=slider_width, line_width=line_width,
-                                 title_label=title_label)
-            S.pack(side='top')
+        for i in range(rows):
+            self.grid_rowconfigure(i, weight=1)
+        for i in range(columns):
+            self.grid_columnconfigure(i, weight=1)
+        self.sliders: list[VerticalSlider] = []
+        self.labels = [d['label'] for d in parameters]
+        for i, param in enumerate(parameters):
+            label = param['label'].replace('_', ' ').title() if title_label else param['label']
+            popup_label = param['description'] if 'description' in param.keys() else None
+            S = VerticalSlider(self, callback=lambda x, l=param['label']: callback(l, x),
+                               min_value=param['min_value'], max_value=param['max_value'],
+                               step=param['step'], default_value=param['value'],
+                               label=label, popup_label=popup_label, bg=bg,
+                               canvas_height=height, **kwargs)
+            S.grid(row=i // columns, column=i % columns, sticky='nsew',
+                   padx=slider_padx, pady=slider_pady)
             self.sliders.append(S)
-    
+
+    def get(self) -> dict:
+        '''returns dictionary with current value of each slider'''
+        return [{label:slider.get()} for label, slider in zip(self.labels, self.sliders)]
+   
 class PlotScrollBar(Canvas):
     ''' Horizontally oriented plot slider that handles integer values between
         a specified minimum and maximum value
         
         Callback command is called whenever the slider is moved by the user
 
         Values are displayed to the user in seconds (formatted m:ss), but on the
```

### Comparing `chichitk-0.0.3/chichitk/temp_menu.py` & `chichitk-0.0.4/chichitk/temp_menu.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.3/chichitk/text_boxes.py` & `chichitk-0.0.4/chichitk/text_boxes.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         
         TextBox can optionally display an error color when there are blank
         lines or consecutive spaces
     '''
     def __init__(self, master, callback=None, bg:str='#ffffff', fg:str='#000000',
                  cursor_color=None, disabled_bg=None, disabled_fg=None,
                  error_bg:str='#3c2525', error_highlight_bg:str='#ff0000',
-                 error_highlight_fg:str='#000000', track_fg:str='#bbbbbb',
-                 font_name:str='Consolas', font_size:int=15,  wrap='none',
+                 error_highlight_fg:str='#000000', track_fg:str='#a6a6a6',
+                 track_active_fg:str='#ffffff', active_line_indices:list=None,
+                 font_name:str='Consolas', font_size:int=15, wrap='none',
                  focus_in_function=None, focus_out_function=None,
+                 scroll_callback=None, line_num_callback=None,
                  check_blank_lines:bool=True, check_consecutive_spaces:bool=True,
                  line_numbers_labels=True, width=None, height=None,
                  justify='left', inactive_justify='center'):
         '''Text box with number lines and callback when text box is edited
         
         Parameters
         ----------
@@ -69,63 +71,86 @@
             :param cursor_color: str (hex code) - cursor color - if different from fg
             :param disabled_bg: str (hex code) - background color when disabled
             :param disabled_fg: str (hex code) - foreground color when disabled
             :param error_bg: str (hex code) - background color when there is an error
             :param error_highlight_bg: str (hex code) - highlight on text causing error
             :param error_highlight_fg: str (hex code) - color of text cauing error
             :param track_fg: str (hex code) - color of track text - line numbers
+            :param track_active_fg: str (hex code) - color of active lines in track box
+            :param active_line_indices: list[int] - indices of active lines
             :param font_name: str - font for text box and line numbers
             :param font_size: int - font size for text box and line numbers
             :param wrap: str Literal['none', 'char', 'word'] - wrap setting
             :param focus_in_function: function () - called when text box takes focus
             :param focus_out_function: function () - called when text box loses focus
+            :param scroll_callback: function(yview_moveto) - called when text box is scrolled
+            :param line_num_callback: function(line_num) - called when number of lines is changed
             :param check_blank_lines: bool - if True, show error when there are blank lines
             :param check_consecutive_spaces: bool - if True, show error when there are consecutive spaces
             :param line_numbers_labels: bool - if True, show line numbers
         '''
         self.callback_function = callback
+        self.scroll_callback = scroll_callback
+        self.line_num_callback = line_num_callback
+        self.line_num = 0
+        self.active_line_indices = active_line_indices if active_line_indices is not None else []
         self.bg, self.fg = bg, fg
+        self.track_active_fg = track_active_fg
         self.error_bg = error_bg
         self.error_highlight_bg = error_highlight_bg
         self.error_highlight_fg = error_highlight_fg
         self.disabled_bg = disabled_bg if disabled_bg else bg
         self.disabled_fg = disabled_fg if disabled_fg else fg
         self.justify, self.inactive_justify = justify, inactive_justify
         Frame.__init__(self, master, bg=bg)
         self.good_format = True # False if there are errors in the text box
         self.check_blank_lines = check_blank_lines
         self.check_consecutive_spaces = check_consecutive_spaces
         cursor_color = cursor_color if cursor_color else fg
 
         self.track = Text(self, width=4, height=height, font=(font_name, font_size),
-                          bg=bg, fg=track_fg, wrap='none', bd=0,
-                          yscrollcommand=lambda a, b: self.box.yview_moveto(a))
+                          bg=bg, fg=track_fg, wrap='none', bd=0)
         if line_numbers_labels:
             self.track.pack(side='left', fill='y')
         self.track.insert('end', '  1')
         self.track.config(state='disabled')
         # undo must be False because Ctrl+z causes infinite loop (no idea why)
         self.box = Text(self, width=width, height=height, font=(font_name, font_size),
-                        bg=bg, fg=fg, insertbackground=cursor_color, undo=False, wrap=wrap,
-                        yscrollcommand=lambda a, b: self.track.yview_moveto(a), bd=0)
+                        bg=bg, fg=fg, insertbackground=cursor_color, undo=False,
+                        wrap=wrap, yscrollcommand=self.__box_scroll, bd=0)
         self.box.pack(side='right', fill='both', expand=True)
         self.box.tag_add("justify", 1.0, "end")
         self.box.tag_configure('justify', justify=self.justify)
         self.box.bind("<<TextModified>>", self.callback)
+        # must not set yscrollcommand until after self.box is defined
+        # to avoid AttributeError
+        self.track.config(yscrollcommand=self.__track_scroll)
         #self.box.bind("<Key>", self.callback)
-        if focus_in_function:
+        if focus_in_function is not None:
             self.box.bind("<FocusIn>", focus_in_function)
-        if focus_out_function:
+        if focus_out_function is not None:
             self.box.bind("<FocusOut>", focus_out_function)
 
         # create a proxy for the underlying widget
         self.box._orig = self.box._w + "_orig"
         self.box.tk.call("rename", self.box._w, self.box._orig)
         self.box.tk.createcommand(self.box._w, self._proxy)
 
+    def __box_scroll(self, a, b):
+        '''called when text box is scrolled with mousewheel'''
+        self.track.yview_moveto(a)
+        if self.scroll_callback is not None:
+            self.scroll_callback(a)
+
+    def __track_scroll(self, a, b):
+        '''called when track box is scrolled with mousewheel'''
+        self.box.yview_moveto(a)
+        if self.scroll_callback is not None:
+            self.scroll_callback(a)
+
     def _proxy(self, command, *args):
         '''facilitates callback - called whenever Text box is edited by user'''
         cmd = (self.box._orig, command) + args
         try:
             result = self.box.tk.call(cmd)
         except:
             # As far as I can tell, this error only occurs when pasting
@@ -147,14 +172,19 @@
         self.track.config(state='normal')
         self.track.delete(0.0, 'end')
         self.track.insert('end', '\n'.join([f'{x} ' for x in range(1, text.count('\n') + 2)]))
         self.track.config(state='disabled')
         self.track.tag_delete('right')
         self.track.tag_add("right", 1.0, "end")
         self.track.tag_configure("right", justify='right')
+        self.set_active_lines(self.active_line_indices) # reset after updating track box
+        if text.count('\n') + 1 != self.line_num: # number of lines has changed
+            self.line_num = text.count('\n') + 1
+            if self.line_num_callback is not None:
+                self.line_num_callback(self.line_num)
 
         # do basic error checking
         self.good_format = True
         self.box.tag_delete('empty_line')
         self.box.tag_delete('consecutive_space')
         if text != '' and (self.check_blank_lines or self.check_consecutive_spaces):
             for i, line in enumerate(text.split('\n')):
@@ -181,14 +211,24 @@
                 self.track.config(bg=self.error_bg)
 
         self.box.yview_moveto(y_pos)
         self.track.yview_moveto(y_pos)
         if self.callback_function:
             self.callback_function(text)
 
+    def set_active_lines(self, line_indices:list):
+        '''changes the foreground in track box for the given line indices
+        :param line_indices: list of ints - indices of lines to highlight
+        '''
+        self.active_line_indices = line_indices
+        self.track.tag_delete('active_track_line')
+        for i in line_indices:
+            self.track.tag_add('active_track_line', f'{i + 1}.0', f'{i + 2}.0')
+        self.track.tag_config('active_track_line', foreground=self.track_active_fg)
+
     def get(self, strip=True) -> str:
         '''returns entire text in text box
 
         Parameters
         -----------
             :param strip: bool - if True, removes spaces and newline characters for beginning and end
         '''
@@ -196,19 +236,19 @@
             return self.box.get(0.0, 'end').strip()
         return self.box.get(0.0, 'end')
 
     def clear(self):
         '''clears all text from text box'''
         self.box.delete(0.0, 'end')
 
-    def insert(self, text):
+    def insert(self, text:str):
         '''inserts text at the end of text box'''
         self.box.insert('end', text)
 
-    def clear_insert(self, text):
+    def clear_insert(self, text:str):
         '''clears all text from text box and adds text'''
         self.clear()
         self.insert(text)
 
     def set_active(self):
         '''
         Purpose:
```

### Comparing `chichitk-0.0.3/chichitk/timer.py` & `chichitk-0.0.4/chichitk/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,27 +105,28 @@
         if self.__running:
             self.__running = False
             if self.__stop_callback is not None:
                 self.__stop_callback()
             return True
         return False
 
-    def reset(self):
+    def reset(self, callback=True):
         '''resets step to min_step and calls callback function
         does not stop the timer'''
-        self.increment(self.__min_step - self.__current_step, callback=True)
+        self.increment(self.__min_step - self.__current_step, callback=callback)
 
-    def to_end(self):
+    def to_end(self, callback=True):
         '''sets step to max_step, stops timer, and calls callback function'''
         assert self.__max_step is not None, 'Skipped timer to end when max_step is not defined'
         self.stop()
         if self.__end_callback is not None:
             self.__end_callback()
         self.__current_step = self.__max_step
-        self.__callback(self.__current_step)
+        if callback:
+            self.__callback(self.__current_step)
 
     def set(self, step:int):
         '''
         Purpose:
             sets timer to the current step.
             if timer is currently running, it will continue uninterrupted
             the next callback will reflect the updated step
```

### Comparing `chichitk-0.0.3/chichitk/tool_tip.py` & `chichitk-0.0.4/chichitk/tool_tip.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import tkinter as tk
+from tkinter import Toplevel, Label, Widget, Event
 
 
 def add_line_breaks(text:str, max_line_len:int, split_char=' ', replace_char='\n'):
     '''splits text into multiple lines - only splits at split_char
     the only way a line can be longer than max_line_len
     is if a single word is longer than max_line_len
     
@@ -20,15 +20,15 @@
                 line_len = 0
                 continue
         output_text += char
         line_len += 1
     return output_text
 
 
-class ToolTip(tk.Toplevel):
+class ToolTip(Toplevel):
     ''' Popup to display information when the cursor hovers on a widget
     
         Info can be displayed on multiple lines by setting chars_per_line
         
         Popup will be displayed directly above the parent widget by default
         but it will check where the edge of the root frame is and adjust its
         position so that it does not extend beyond the root frame
@@ -41,31 +41,31 @@
             :param master: tk.Frame - parent widget
             :param chars_per_line: int - maximum characters before line break
             :param fade_inc: float - amount to adjust fade on every frame
             :param fade_ms: int (milliseconds) - time to wait before next frame
         '''
         self.__chars_per_line = chars_per_line
         self.__fade_inc, self.__fade_ms = fade_inc, fade_ms
-        tk.Toplevel.__init__(self, master)
+        super().__init__(master)
         #make window invisible, on the top, and strip all window decorations/features
         self.attributes('-alpha', 0, '-topmost', True)
         self.overrideredirect(1)
         #style and create label. you can override style with kwargs
         style = dict(bd=2, relief='raised', font='courier 10 bold', bg='#FFFF99', anchor='w')
-        self.label = tk.Label(self, **{**style, **kwargs})
+        self.label = Label(self, **{**style, **kwargs})
         self.label.grid(row=0, column=0, sticky='w')
         #used to determine if an opposing fade is already in progress
         self.fout:bool = False
         
-    def bind(self, target:tk.Widget, text:str, **kwargs):
+    def bind(self, target:Widget, text:str, **kwargs):
         #bind Enter(mouseOver) and Leave(mouseOut) events to the target of this tooltip
         target.bind('<Enter>', lambda e: self.fadein(0, text, e))
         target.bind('<Leave>', lambda e: self.fadeout(1 - self.__fade_inc, e))
 
-    def fadein(self, alpha:float, text:str=None, event:tk.Event=None):
+    def fadein(self, alpha:float, text:str=None, event:Event=None):
         #if event and text then this call came from target
         #~ we can consider this a "fresh/new" call
         if event is not None and text is not None:
             if self.fout: # if we are in the middle of fading out jump to end of fade
                 self.attributes('-alpha', 0)
                 self.fout = False # indicate that we are fading in
             text = add_line_breaks(text, self.__chars_per_line, replace_char=' \n ') # to pad each line with space
@@ -74,22 +74,19 @@
 
             # check widget position (widget that calls tool_tip popup such as button or label)
             widget_width = event.widget.winfo_width()
             widget_height = event.widget.winfo_height()
             widget_x = event.widget.winfo_rootx()
             widget_y = event.widget.winfo_rooty()
 
-            #x and y offsets
-            offset_x = int((widget_width - self.label.winfo_width()) / 2)
-            offset_y = int((widget_height + self.label.winfo_height()) / 2)
-            #get geometry
+            # compute popup geometry
             w = self.label.winfo_width()
             h = self.label.winfo_height()
-            x = widget_x + offset_x
-            y = widget_y - offset_y
+            x = widget_x + int((widget_width - w) / 2) # to center horizontally
+            y = widget_y - h # directly above widget
 
             # check root coordinates
             root_width = event.widget.winfo_toplevel().winfo_width()
             root_height = event.widget.winfo_toplevel().winfo_height()
             root_x = event.widget.winfo_toplevel().winfo_rootx() # x position of app on computer screen
             root_y = event.widget.winfo_toplevel().winfo_rooty() # y position of app on computer screen
 
@@ -100,27 +97,27 @@
                 y = root_y + root_height - h
             x = max(root_x, x) # enforce left edge
             y = max(root_y, y) # enforce top edge
 
             # ensure tool_tip is not on top of widget - this makes a button unclickable!
             # this can only happen if tool_tip was moved down by top enforcement, so move it to below widget
             if y + h > widget_y:
-                y = widget_y + offset_y # position tool_tip below widget
+                y = widget_y + widget_height # position tool_tip below widget
 
             #apply geometry
             self.geometry(f'{w}x{h}+{x}+{y}')
                
         #if we aren't fading out, fade in
         if not self.fout:
             self.attributes('-alpha', alpha)
         
             if alpha < 1:
                 self.after(self.__fade_ms, lambda: self.fadein(min(alpha + self.__fade_inc, 1)))
 
-    def fadeout(self, alpha:float, event:tk.Event=None):
+    def fadeout(self, alpha:float, event:Event=None):
         #if event then this call came from target 
         #~ we can consider this a "fresh/new" call
         if event is not None:
             #indicate that we are fading out
             self.fout = True
         
         #if we aren't fading in, fade out
```

### Comparing `chichitk-0.0.3/chichitk.egg-info/PKG-INFO` & `chichitk-0.0.4/chichitk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chichitk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python UI library built upon Tkinter
 Author-email: Samuel Gibson <samuelpgibson12@gmail.com>
 Project-URL: Homepage, https://github.com/SamGibson1/ChichiTk
 Project-URL: Documentation, https://github.com/SamGibson1/ChichiTk/wiki
 Project-URL: Bug Tracker, https://github.com/SamGibson1/ChichiTk/issues
 Keywords: python,tkinter,custom,widgets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `chichitk-0.0.3/chichitk.egg-info/SOURCES.txt` & `chichitk-0.0.4/chichitk.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 chichitk/icons.py
 chichitk/labels.py
 chichitk/pdf_display.py
 chichitk/player.py
 chichitk/progress_bar.py
 chichitk/scrollable_frame.py
 chichitk/sliders.py
+chichitk/temp_label.py
 chichitk/temp_menu.py
 chichitk/text_boxes.py
 chichitk/timer.py
 chichitk/tool_tip.py
 chichitk.egg-info/PKG-INFO
 chichitk.egg-info/SOURCES.txt
 chichitk.egg-info/dependency_links.txt
```

### Comparing `chichitk-0.0.3/pyproject.toml` & `chichitk-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chichitk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Samuel Gibson", email="samuelpgibson12@gmail.com" },
 ]
 description = "Python UI library built upon Tkinter"
 readme = "Readme.md"
 requires-python = ">=3.7"
 dependencies = ["opencv-python", "numpy", "Pillow", "PyMuPDF"]
```

