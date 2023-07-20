# Comparing `tmp/idkwhttph-0.2.1.tar.gz` & `tmp/idkwhttph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.1.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.2.tar", max compression
```

## Comparing `idkwhttph-0.2.1.tar` & `idkwhttph-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    37487 2023-07-20 10:26:45.009285 idkwhttph-0.2.1/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-20 10:26:39.857294 idkwhttph-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-20 10:26:58.417015 idkwhttph-0.2.1/setup.py
--rw-r--r--   0        0        0      239 2023-07-20 10:26:58.417343 idkwhttph-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    41992 2023-07-20 10:35:13.808375 idkwhttph-0.2.2/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-20 10:35:16.360370 idkwhttph-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-20 10:35:19.723092 idkwhttph-0.2.2/setup.py
+-rw-r--r--   0        0        0      239 2023-07-20 10:35:19.723553 idkwhttph-0.2.2/PKG-INFO
```

### Comparing `idkwhttph-0.2.1/idkwhttph/__init__.py` & `idkwhttph-0.2.2/idkwhttph/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-__version__ = '0.2.1'
-#Imports
-import keyboard
+__version__ = "0.2.2"
+# Imports
 
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
 import json
-import shutil;
+import shutil
 import os
 import unittest
 import requests
 import sys
-#end
+
+# end
 
 """Async and dict-like interfaces for interacting with Repl.it Database."""
 
 from collections import abc
 import json
 from typing import (
     AbstractSet,
@@ -606,301 +606,241 @@
         return f"<{self.__class__.__name__}(db_url={self.db_url!r})>"
 
     def close(self) -> None:
         """Closes the database client connection."""
         self.sess.close()
 
 
-
-
 def printInMiddle(text, columns=shutil.get_terminal_size().columns):
-  # Get the current width of the console
-  console_width = columns
-
-  # Calculate the padding for the left side
-  padding = (console_width - len(text)) // 2 + 5
-
-  # Print the padded text
-  print(' ' * padding + text)
-
-def write(string: str, speed: int=.05) -> None:
-  for char in string:
-    sys.stdout.write(char)
-    sys.stdout.flush()
-    sleep(speed)
-
-
-
-
+    # Get the current width of the console
+    console_width = columns
 
+    # Calculate the padding for the left side
+    padding = (console_width - len(text)) // 2 + 5
 
+    # Print the padded text
+    print(" " * padding + text)
 
 
+def write(string: str, speed: int = 0.05) -> None:
+    for char in string:
+        sys.stdout.write(char)
+        sys.stdout.flush()
+        sleep(speed)
 
 
-
-
-
-backup_file_path = 'backup.json'
+backup_file_path = "backup.json"
 
 
 def create_backup():
-  backup_data = dict(db)
+    backup_data = dict(db)
 
-  with open(backup_file_path, 'w') as file:
-    json.dump(backup_data, file, indent=2)
+    with open(backup_file_path, "w") as file:
+        json.dump(backup_data, file, indent=2)
 
 
 def load_backup():
-  if os.path.exists(backup_file_path):
-    with open(backup_file_path, 'r') as file:
-      backup_data = json.load(file)
-      db.update(backup_data)
+    if os.path.exists(backup_file_path):
+        with open(backup_file_path, "r") as file:
+            backup_data = json.load(file)
+            db.update(backup_data)
 
 
 def save_backup():
-  backup_data = dict(db)
+    backup_data = dict(db)
 
-  with open(backup_file_path, 'w') as file:
-    json.dump(backup_data, file)
+    with open(backup_file_path, "w") as file:
+        json.dump(backup_data, file)
 
 
 def sync_backup():
-  with open(backup_file_path, 'r') as file:
-    backup_data = json.load(file)
-
-  db.update(backup_data)
-
-  create_backup()
-
-
+    with open(backup_file_path, "r") as file:
+        backup_data = json.load(file)
 
+    db.update(backup_data)
 
+    create_backup()
 
 
+CSI = "\033["
+OSC = "\033]"
+BEL = "\a"
 
 
-CSI = '\033['
-OSC = '\033]'
-BEL = '\a'
 def code_to_chars(code):
-  return CSI + str(code) + 'm'
+    return CSI + str(code) + "m"
 
 
 def set_title(title):
-  return OSC + '2;' + title + BEL
+    return OSC + "2;" + title + BEL
 
 
 def clear_screen(mode=2):
-  return CSI + str(mode) + 'J'
+    return CSI + str(mode) + "J"
 
 
 def clear_line(mode=2):
-  return CSI + str(mode) + 'K'
+    return CSI + str(mode) + "K"
 
 
 class AnsiCodes(object):
-
-  def __init__(self):
-    # the subclasses declare class attributes which are numbers.
-    # Upon instantiation we define instance attributes, which are the same
-    # as the class attributes but wrapped with the ANSI escape sequence
-    for name in dir(self):
-      if not name.startswith('_'):
-        value = getattr(self, name)
-        setattr(self, name, code_to_chars(value))
+    def __init__(self):
+        # the subclasses declare class attributes which are numbers.
+        # Upon instantiation we define instance attributes, which are the same
+        # as the class attributes but wrapped with the ANSI escape sequence
+        for name in dir(self):
+            if not name.startswith("_"):
+                value = getattr(self, name)
+                setattr(self, name, code_to_chars(value))
 
 
 class AnsiCursor(object):
+    def UP(self, n=1):
+        return CSI + str(n) + "A"
 
-  def UP(self, n=1):
-    return CSI + str(n) + 'A'
-
-  def DOWN(self, n=1):
-    return CSI + str(n) + 'B'
+    def DOWN(self, n=1):
+        return CSI + str(n) + "B"
 
-  def FORWARD(self, n=1):
-    return CSI + str(n) + 'C'
+    def FORWARD(self, n=1):
+        return CSI + str(n) + "C"
 
-  def BACK(self, n=1):
-    return CSI + str(n) + 'D'
+    def BACK(self, n=1):
+        return CSI + str(n) + "D"
 
-  def POS(self, x=1, y=1):
-    return CSI + str(y) + ';' + str(x) + 'H'
+    def POS(self, x=1, y=1):
+        return CSI + str(y) + ";" + str(x) + "H"
 
 
 class AnsiFore(AnsiCodes):
-  BLACK = 30
-  RED = 31
-  GREEN = 32
-  YELLOW = 33
-  BLUE = 34
-  MAGENTA = 35
-  CYAN = 36
-  WHITE = 37
-  RESET = 39
-
-  # These are fairly well supported, but not part of the standard.
-  LIGHTBLACK_EX = 90
-  LIGHTRED_EX = 91
-  LIGHTGREEN_EX = 92
-  LIGHTYELLOW_EX = 93
-  LIGHTBLUE_EX = 94
-  LIGHTMAGENTA_EX = 95
-  LIGHTCYAN_EX = 96
-  LIGHTWHITE_EX = 97
+    BLACK = 30
+    RED = 31
+    GREEN = 32
+    YELLOW = 33
+    BLUE = 34
+    MAGENTA = 35
+    CYAN = 36
+    WHITE = 37
+    RESET = 39
+
+    # These are fairly well supported, but not part of the standard.
+    LIGHTBLACK_EX = 90
+    LIGHTRED_EX = 91
+    LIGHTGREEN_EX = 92
+    LIGHTYELLOW_EX = 93
+    LIGHTBLUE_EX = 94
+    LIGHTMAGENTA_EX = 95
+    LIGHTCYAN_EX = 96
+    LIGHTWHITE_EX = 97
 
 
 class AnsiBack(AnsiCodes):
-  BLACK = 40
-  RED = 41
-  GREEN = 42
-  YELLOW = 43
-  BLUE = 44
-  MAGENTA = 45
-  CYAN = 46
-  WHITE = 47
-  RESET = 49
-
-  # These are fairly well supported, but not part of the standard.
-  LIGHTBLACK_EX = 100
-  LIGHTRED_EX = 101
-  LIGHTGREEN_EX = 102
-  LIGHTYELLOW_EX = 103
-  LIGHTBLUE_EX = 104
-  LIGHTMAGENTA_EX = 105
-  LIGHTCYAN_EX = 106
-  LIGHTWHITE_EX = 107
+    BLACK = 40
+    RED = 41
+    GREEN = 42
+    YELLOW = 43
+    BLUE = 44
+    MAGENTA = 45
+    CYAN = 46
+    WHITE = 47
+    RESET = 49
+
+    # These are fairly well supported, but not part of the standard.
+    LIGHTBLACK_EX = 100
+    LIGHTRED_EX = 101
+    LIGHTGREEN_EX = 102
+    LIGHTYELLOW_EX = 103
+    LIGHTBLUE_EX = 104
+    LIGHTMAGENTA_EX = 105
+    LIGHTCYAN_EX = 106
+    LIGHTWHITE_EX = 107
 
 
 class AnsiStyle(AnsiCodes):
-  BRIGHT = 1
-  DIM = 2
-  NORMAL = 22
-  RESET_ALL = 0
+    BRIGHT = 1
+    DIM = 2
+    NORMAL = 22
+    RESET_ALL = 0
 
 
 Fore = AnsiFore()
 Back = AnsiBack()
 Style = AnsiStyle()
 Cursor = AnsiCursor()
 
 
-
-
 def print_layer():
-  console_width = shutil.get_terminal_size().columns;
-  for i in range(console_width):
-    print("-", end="");
-  print(); # Print a newline at the end
-
-
-
-
+    console_width = shutil.get_terminal_size().columns
+    for i in range(console_width):
+        print("-", end="")
+    print()
+    # Print a newline at the end
 
 
 def options(prompt, menu, title, bold, PIM: bool) -> int:
-  global bold_yes;
-  if bold:
-    bold_yes = S.BRIGHT;
-  elif bold == False:
-    bold_yes = S.NORMAL;
-  else:
-    return;
-  selection = 0;
-  key = None;
-
-  while True:
-    try:
-      while key != keys.ENTER:
-        clear();
-        if title == False:
-          pass;
-        else:
-          if PIM == True:
-
-            printInMiddle(f'{bold_yes}{title}');
-            print_layer();
-          elif PIM == False:
-            print(f'{bold_yes}{title}');
-            print_layer();
-          else:
-            return;
-        if prompt == False:
-          pass;
-        else:
-          print(f'{bold_yes}{prompt}');
-        for i in range(len(menu)):
-          opt = menu[i];
-          if i == selection:
-            print(f'{bold_yes}> {opt}');
-
-          else:
-            print(f'{bold_yes}  {opt}');
-
-        key = getkey();
-        if key == keys.W or keyboard.is_pressed('up'):
-          clear();
-          selection = (selection - 1) % len(menu);
-          if selection == -1:
-            selection = (selection + len(menu) + 1) % len(menu);
-        elif key == keys.S or keybord.is_pressed('down'):
-          clear();
-          selection = (selection + 1) % len(menu);
-          if selection > len(menu):
-            selection = (selection - len(menu) - 1) % len(menu);
-      return selection;
-
-    except:
-      clear();
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    global bold_yes
+    if bold:
+        bold_yes = S.BRIGHT
+    elif bold == False:
+        bold_yes = S.NORMAL
+    else:
+        return
+    selection = 0
+    key = None
 
+    while True:
+        try:
+            while key != keys.ENTER:
+                clear()
+                if title == False:
+                    pass
+                else:
+                    if PIM == True:
+                        printInMiddle(f"{bold_yes}{title}")
+                        print_layer()
+                    elif PIM == False:
+                        print(f"{bold_yes}{title}")
+                        print_layer()
+                    else:
+                        return
+                if prompt == False:
+                    pass
+                else:
+                    print(f"{bold_yes}{prompt}")
+                for i in range(len(menu)):
+                    opt = menu[i]
+                    if i == selection:
+                        print(f"{bold_yes}> {opt}")
 
+                    else:
+                        print(f"{bold_yes}  {opt}")
 
+                key = getkey()
+                if key == keys.W or key == keys.UP:
+                    clear()
+                    selection = (selection - 1) % len(menu)
+                    if selection == -1:
+                        selection = (selection + len(menu) + 1) % len(menu)
+                elif key == keys.S or key == keys.DOWN:
+                    clear()
+                    selection = (selection + 1) % len(menu)
+                    if selection > len(menu):
+                        selection = (selection - len(menu) - 1) % len(menu)
+            return selection
 
+        except:
+            clear()
 
 
 def crash():
-  
-
-  exec(
-    type((lambda: 0).__code__)(0, 0, 0, 0, 0, 0, b'\x053', (), (), (), '', '',
-                               0, b''))
-  clear()
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    exec(
+        type((lambda: 0).__code__)(
+            0, 0, 0, 0, 0, 0, b"\x053", (), (), (), "", "", 0, b""
+        )
+    )
+    clear()
 
 
 class SyncDatabase(dict):
     """Subclass of dict that syncs with a JSON backup file."""
 
     def __setitem__(self, key, value):
         """Set a key-value pair and sync with the backup file."""
@@ -913,22 +853,33 @@
         sync_backup()
 
     def all(self):
         """Print the keys and values in formatted columns."""
         keys = list(self.keys())
         values = list(self.values())
         num_entries = len(keys)
-        
+
         column_width = 10  # Adjust the column width according to your preference
         num_columns = 6
-        
+
         for i in range(0, num_entries, num_columns):
-            print("key:".ljust(column_width) + "|" + "|".join(keys[i:i+num_columns]).center(column_width, ' '))
+            print(
+                "key:".ljust(column_width)
+                + "|"
+                + "|".join(keys[i : i + num_columns]).center(column_width, " ")
+            )
             print("-" * (column_width * (num_columns + 1)))
-            print("value:".ljust(column_width) + "|" + "|".join(str(values[j]).center(column_width, ' ') for j in range(i, i+num_columns)).center(column_width * (num_columns + 1), ' '))
+            print(
+                "value:".ljust(column_width)
+                + "|"
+                + "|".join(
+                    str(values[j]).center(column_width, " ")
+                    for j in range(i, i + num_columns)
+                ).center(column_width * (num_columns + 1), " ")
+            )
             print()
         print()
 
 
 class TestSyncDatabase(unittest.TestCase):
     """Integration tests for syncing a backup file with the Replit database."""
 
@@ -953,461 +904,565 @@
         for k in self.db.keys():
             del self.db[k]
 
     def test_sync_backup(self) -> None:
         """Test syncing the backup file with the Replit database."""
         # Create a backup
         backup_data = dict(self.db)
-        with open(backup_file_path, 'w') as file:
+        with open(backup_file_path, "w") as file:
             json.dump(backup_data, file, indent=2)
 
         # Sync the backup with the Replit database
-        with open(backup_file_path, 'r') as file:
+        with open(backup_file_path, "r") as file:
             backup_data = json.load(file)
         self.db.update(backup_data)
 
         # Perform necessary tests
         self.assertEqual(self.db["test-key"], "value")
 
         # Update the Replit database and save the changes to the backup file
         self.db["test-key"] = "new-value"
         backup_data = dict(self.db)
-        with open(backup_file_path, 'w') as file:
+        with open(backup_file_path, "w") as file:
             json.dump(backup_data, file)
 
         # Sync the backup with the Replit database again
-        with open(backup_file_path, 'r') as file:
+        with open(backup_file_path, "r") as file:
             backup_data = json.load(file)
         self.db.update(backup_data)
 
         # Perform necessary tests again
         self.assertEqual(self.db["test-key"], "new-value")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     db = SyncDatabase(db)
     create_backup()
     unittest.main()
 
 
+backup_file_path = "backup.json"
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-backup_file_path = 'backup.json'
 def save_backup():
-  backup_data = dict(db)
+    backup_data = dict(db)
+
+    with open(backup_file_path, "w") as file:
+        json.dump(backup_data, file)
 
-  with open(backup_file_path, 'w') as file:
-    json.dump(backup_data, file)
 
 def load_json_data():
-    with open('backup.json', 'r') as file:
+    with open("backup.json", "r") as file:
         data = json.load(file)
     return data
 
-JLI = False
-#Fake password
-username = ['']
-list_1 = ['']
-default = ['a','b','c','d','e','f','g','h','i','j','k','l','n','m','o','p','q','r','s','t','u','v','w','x','y','z','_','-','1','2','3','4','5','6','7','8','9','0','B','B','C','D','E','F','G','H','I','J','K','L','N','M','O','P','Q','R','S','T','U','V','W','X','Y','Z']
-Restrictions = ['a','b','c','d','e','f','g','h','i','j','k','l','n','m','o','p','q','r','s','t','u','v','w','x','y','z','_','-','1','2','3','4','5','6','7','8','9','0','B','B','C','D','E','F','G','H','I','J','K','L','N','M','O','P','Q','R','S','T','U','V','W','X','Y','Z']
 
-options = [
-  'Username: ', 'PassWord: ', 'Show Password', 'Hide password', 'Submit!'
+JLI = False
+# Fake password
+username = [""]
+list_1 = [""]
+default = [
+    "a",
+    "b",
+    "c",
+    "d",
+    "e",
+    "f",
+    "g",
+    "h",
+    "i",
+    "j",
+    "k",
+    "l",
+    "n",
+    "m",
+    "o",
+    "p",
+    "q",
+    "r",
+    "s",
+    "t",
+    "u",
+    "v",
+    "w",
+    "x",
+    "y",
+    "z",
+    "_",
+    "-",
+    "1",
+    "2",
+    "3",
+    "4",
+    "5",
+    "6",
+    "7",
+    "8",
+    "9",
+    "0",
+    "B",
+    "B",
+    "C",
+    "D",
+    "E",
+    "F",
+    "G",
+    "H",
+    "I",
+    "J",
+    "K",
+    "L",
+    "N",
+    "M",
+    "O",
+    "P",
+    "Q",
+    "R",
+    "S",
+    "T",
+    "U",
+    "V",
+    "W",
+    "X",
+    "Y",
+    "Z",
 ]
-def enter_to_continue():
-  print(f'{S.BRIGHT}|{F.BLUE}Enter{F.WHITE}|To Continue')
-  input()
-  
-# Real password
-list_2 = ['']
-list_3 = list_1
-
-
-def Sign_In() -> None:
-  global list_1, list_2, list_3, username,menu,show_hide,alert,JLI,matches
-  username = ['']
-  list_1 = ['']
-  list_2 = ['']
-  list_3 = list_1
-  alert = False
-  show_hide = False
-  if show_hide:
-  
-    menu = [
-    'Username: ', 'PassWord: ', 'Hide Password', 'Submit!'
-  ]
-  if show_hide == False:
-    menu = [
-  'Username: ', 'PassWord: ', 'Show Password', 'Submit!'
+Restrictions = [
+    "a",
+    "b",
+    "c",
+    "d",
+    "e",
+    "f",
+    "g",
+    "h",
+    "i",
+    "j",
+    "k",
+    "l",
+    "n",
+    "m",
+    "o",
+    "p",
+    "q",
+    "r",
+    "s",
+    "t",
+    "u",
+    "v",
+    "w",
+    "x",
+    "y",
+    "z",
+    "_",
+    "-",
+    "1",
+    "2",
+    "3",
+    "4",
+    "5",
+    "6",
+    "7",
+    "8",
+    "9",
+    "0",
+    "B",
+    "B",
+    "C",
+    "D",
+    "E",
+    "F",
+    "G",
+    "H",
+    "I",
+    "J",
+    "K",
+    "L",
+    "N",
+    "M",
+    "O",
+    "P",
+    "Q",
+    "R",
+    "S",
+    "T",
+    "U",
+    "V",
+    "W",
+    "X",
+    "Y",
+    "Z",
 ]
-  opt_2 = ''
-  Hello = False
-  opt = ''
-  
-  if JLI == True:
-    selection = 4
-    JLI = False
-  else:
-    selection = 0
-  key = ''
-  while True:
-    try:
-      if show_hide:
-
-        menu = [
-        'Username: ', 'PassWord: ', 'Hide Password', 'Submit!','Already Have an Account?'
-      ]
-      if show_hide == False:
-        menu = [
-      'Username: ', 'PassWord: ', 'Show Password', 'Submit!','Already Have an Account?'
-    ]
-
 
+options = ["Username: ", "PassWord: ", "Show Password", "Hide password", "Submit!"]
 
 
+def enter_to_continue():
+    print(f"{S.BRIGHT}|{F.BLUE}Enter{F.WHITE}|To Continue")
+    input()
 
 
-      
-      if keyboard.is_pressed('enter'):
-        if opt == 'PassWord: ':
-          break
-      clear()
-      print(f'{S.RESET_ALL}------------------------------------')
-      print('             Sign In!')
-      print('')
-      print('Please use the arrow keys to move Up or Down')
-      print('')
-      for i in range(len(menu)):
-        opt = menu[i]
-        if i == selection:
-          if opt == 'PassWord: ':
-            opt_2 = "".join(list_2)
-            if Hello:
-              print(f'> {opt}{opt_2}')
-            else:
-              opt_2 = ''.join(list_1)
-              print(f'> {opt}{opt_2}')
-
-          elif opt == 'Username: ':
-            if Hello:
-              print(f'> {opt}{"".join(username)}')
-            else:
-              print(f'> {opt}{"".join(username)}')
-          else:
-                
-              print(f'> {opt}')
-    
-        else:
-          if opt == 'PassWord: ':
-            if Hello:
-              print(f'  {opt}{"".join(list_2)}')
-            else:
-              print(f'  {opt}{"".join(list_1)}')
-
-          elif opt == 'Username: ':
-            if Hello:
-              print(f'  {opt}{"".join(username)}')
-            else:
-              print(f'  {opt}{"".join(username)}')
-          else:
-            print(f'  {opt}')
-
-      key = getkey()
-      
-      string = key
-
-      if keyboard.is_pressed('up'):
-
-        selection = (selection - 1) % len(menu)
-        if selection == -1:
-          selection = (selection + len(menu) + 1) % len(menu)
-      elif keyboard.is_pressed('down'):
-
-        selection = (selection + 1) % len(menu)
-        if selection > len(menu):
-          selection = (selection - len(menu) - 1) % len(menu)
-      if keyboard.is_pressed('up') or key == keyboard.is_pressed('down'):
-        pass
-      else:
-        if selection == 0 or selection == 1:
-          if keyboard.is_pressed('enter'):
-            alert = True
-          else:
-            pass
-
-        if alert == True:
-          alert = False
-        
-        elif alert == False:
-
-      
-          
+# Real password
+list_2 = [""]
+list_3 = list_1
 
 
+def Sign_In() -> None:
+    global list_1, list_2, list_3, username, menu, show_hide, alert, JLI, matches
+    username = [""]
+    list_1 = [""]
+    list_2 = [""]
+    list_3 = list_1
+    alert = False
+    show_hide = False
+    if show_hide:
+        menu = ["Username: ", "PassWord: ", "Hide Password", "Submit!"]
+    if show_hide == False:
+        menu = ["Username: ", "PassWord: ", "Show Password", "Submit!"]
+    opt_2 = ""
+    Hello = False
+    opt = ""
+
+    if JLI == True:
+        selection = 4
+        JLI = False
+    else:
+        selection = 0
+    key = ""
+    while True:
+        try:
+            if show_hide:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Hide Password",
+                    "Submit!",
+                    "Already Have an Account?",
+                ]
+            if show_hide == False:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Show Password",
+                    "Submit!",
+                    "Already Have an Account?",
+                ]
+
+            if key == keys.ENTER:
+                if opt == "PassWord: ":
+                    break
             clear()
-            if keyboard.is_pressed('enter') and selection == 4:
-              clear()
-              print('Redirecting you to login!')
-              sleep(3)
-              clear()
-              sleep(0.5)
-              Log_In()
-            else:
-              if keyboard.is_pressed('enter') and selection == 3:
-                if ''.join(username) == '' or ''.join(list_2) == '':
-                  print('You have not entered a username or password')
-                  enter_to_continue()
-                  clear()
-                elif len(list_2) <= 8:
-                  print('Your password must be atleast 8 characters')
-                  enter_to_continue()
-                  clear()
-      
-  
-                    
-                    
-      
-                else:
-                  clear()
-                  print('Signed in!')
-                  enter_to_continue()
-                  clear()
-                  cursor.show()
-                  
-                  matches = db.prefix('Name')
-                  matches = list(matches)
-                  matches = len(matches)
-                  
-                  
-                  db['Name'+str(matches)] = ''.join(username)
-                  db['password'+str(matches)] = ''.join(list_2)
-                  break
-              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Show Password':
-                list_3 = list_2
-                Hello = True
-                show_hide = True
-              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Hide Password':
-                list_3 = list_1
-                Hello = False
-                show_hide = False
-              if selection == 1:
-                if keyboard.is_pressed('backspace'):
-                  temp_var = list_1.pop(-1)
-                  temp_var = list_2.pop(-1)
-                else:
-                  list_1 += '*'
-                  list_2 += string
-              if selection == 0:
-                if keyboard.is_pressed('backspace'):
-                  try:
-                    username.pop(-1)
-                  except:
-                    clear()
+            print(f"{S.RESET_ALL}------------------------------------")
+            print("             Sign In!")
+            print("")
+            print("Please use the arrow keys to move Up or Down")
+            print("")
+            for i in range(len(menu)):
+                opt = menu[i]
+                if i == selection:
+                    if opt == "PassWord: ":
+                        opt_2 = "".join(list_2)
+                        if Hello:
+                            print(f"> {opt}{opt_2}")
+                        else:
+                            opt_2 = "".join(list_1)
+                            print(f"> {opt}{opt_2}")
+
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'> {opt}{"".join(username)}')
+                        else:
+                            print(f'> {opt}{"".join(username)}')
+                    else:
+                        print(f"> {opt}")
+
                 else:
-                  if string not in Restrictions:
-                    pass
-                  else:
-                    if keyboard.is_pressed('enter'):
-                      pass
+                    if opt == "PassWord: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(list_2)}')
+                        else:
+                            print(f'  {opt}{"".join(list_1)}')
+
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(username)}')
+                        else:
+                            print(f'  {opt}{"".join(username)}')
                     else:
-                      username += string
-              clear()
-    except:
-      clear()
+                        print(f"  {opt}")
 
+            key = getkey()
 
-def Log_In():
-  cursor.hide()
-  global list_1, list_2, list_3, username,menu,show_hide,alert,JLI
-  alert = False
-  show_hide = False
-  username = ['']
-  list_1 = ['']
-  list_2 = ['']
-  list_3 = list_1
-  if show_hide:
-  
-    menu = [
-    'Username: ', 'PassWord: ', 'Hide Password', 'Submit!'
-  ]
-  if show_hide == False:
-    menu = [
-  'Username: ', 'PassWord: ', 'Show Password', 'Submit!'
-]
-  opt_2 = ''
-  Hello = False
-  opt = ''
-  selection = 4
-  key = ''
-  while True:
-    try:
-      if show_hide:
-
-        menu = [
-        'Username: ', 'PassWord: ', 'Hide Password', 'Log In!',"Don't have an account?"
-      ]
-      if show_hide == False:
-        menu = [
-      'Username: ', 'PassWord: ', 'Show Password', 'Log In!',"Don't have an account?"
-    ]
+            string = key
 
+            if key == keys.UP:
+                selection = (selection - 1) % len(menu)
+                if selection == -1:
+                    selection = (selection + len(menu) + 1) % len(menu)
+            elif key == keys.DOWN:
+                selection = (selection + 1) % len(menu)
+                if selection > len(menu):
+                    selection = (selection - len(menu) - 1) % len(menu)
+            if key == keys.UP or key == keys.DOWN:
+                pass
+            else:
+                if selection == 0 or selection == 1:
+                    if key == keys.ENTER:
+                        alert = True
+                    else:
+                        pass
 
+                if alert == True:
+                    alert = False
 
+                elif alert == False:
+                    clear()
+                    if key == keys.ENTER and selection == 4:
+                        clear()
+                        print("Redirecting you to login!")
+                        sleep(3)
+                        clear()
+                        sleep(0.5)
+                        Log_In()
+                    else:
+                        if key == keys.ENTER and selection == 3:
+                            if "".join(username) == "" or "".join(list_2) == "":
+                                print("You have not entered a username or password")
+                                enter_to_continue()
+                                clear()
+                            elif len(list_2) <= 8:
+                                print("Your password must be atleast 8 characters")
+                                enter_to_continue()
+                                clear()
+
+                            else:
+                                clear()
+                                print("Signed in!")
+                                enter_to_continue()
+                                clear()
+                                cursor.show()
+
+                                matches = db.prefix("Name")
+                                matches = list(matches)
+                                matches = len(matches)
+
+                                db["Name" + str(matches)] = "".join(username)
+                                db["password" + str(matches)] = "".join(list_2)
+                                break
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Show Password"
+                        ):
+                            list_3 = list_2
+                            Hello = True
+                            show_hide = True
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Hide Password"
+                        ):
+                            list_3 = list_1
+                            Hello = False
+                            show_hide = False
+                        if selection == 1:
+                            if key == keys.BACKSPACE:
+                                temp_var = list_1.pop(-1)
+                                temp_var = list_2.pop(-1)
+                            else:
+                                list_1 += "*"
+                                list_2 += string
+                        if selection == 0:
+                            if key == keys.BACKSPACE:
+                                try:
+                                    username.pop(-1)
+                                except:
+                                    clear()
+                            else:
+                                if string not in Restrictions:
+                                    pass
+                                else:
+                                    if string == keys.ENTER:
+                                        pass
+                                    else:
+                                        username += string
+                        clear()
+        except:
+            clear()
 
 
+def Log_In():
+    cursor.hide()
+    global list_1, list_2, list_3, username, menu, show_hide, alert, JLI
+    alert = False
+    show_hide = False
+    username = [""]
+    list_1 = [""]
+    list_2 = [""]
+    list_3 = list_1
+    if show_hide:
+        menu = ["Username: ", "PassWord: ", "Hide Password", "Submit!"]
+    if show_hide == False:
+        menu = ["Username: ", "PassWord: ", "Show Password", "Submit!"]
+    opt_2 = ""
+    Hello = False
+    opt = ""
+    selection = 4
+    key = ""
+    while True:
+        try:
+            if show_hide:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Hide Password",
+                    "Log In!",
+                    "Don't have an account?",
+                ]
+            if show_hide == False:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Show Password",
+                    "Log In!",
+                    "Don't have an account?",
+                ]
+
+            if key == keys.ENTER:
+                if opt == "PassWord: ":
+                    break
+            clear()
+            print(f"{S.RESET_ALL}------------------------------------")
+            print("             Log In!")
+            print("")
+            print("Please use the arrow keys to move Up or Down")
+            print("")
+            for i in range(len(menu)):
+                opt = menu[i]
+                if i == selection:
+                    if opt == "PassWord: ":
+                        opt_2 = "".join(list_2)
+                        if Hello:
+                            print(f"> {opt}{opt_2}")
+                        else:
+                            opt_2 = "".join(list_1)
+                            print(f"> {opt}{opt_2}")
+
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'> {opt}{"".join(username)}')
+                        else:
+                            print(f'> {opt}{"".join(username)}')
+                    else:
+                        print(f"> {opt}")
 
-      
-      if keyboard.is_pressed('enter'):
-        if opt == 'PassWord: ':
-          break
-      clear()
-      print(f'{S.RESET_ALL}------------------------------------')
-      print('             Log In!')
-      print('')
-      print('Please use the arrow keys to move Up or Down')
-      print('')
-      for i in range(len(menu)):
-        opt = menu[i]
-        if i == selection:
-          if opt == 'PassWord: ':
-            opt_2 = "".join(list_2)
-            if Hello:
-              print(f'> {opt}{opt_2}')
-            else:
-              opt_2 = ''.join(list_1)
-              print(f'> {opt}{opt_2}')
+                else:
+                    if opt == "PassWord: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(list_2)}')
+                        else:
+                            print(f'  {opt}{"".join(list_1)}')
+
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(username)}')
+                        else:
+                            print(f'  {opt}{"".join(username)}')
+                    else:
+                        print(f"  {opt}")
 
-          elif opt == 'Username: ':
-            if Hello:
-              print(f'> {opt}{"".join(username)}')
-            else:
-              print(f'> {opt}{"".join(username)}')
-          else:
-                
-              print(f'> {opt}')
-    
-        else:
-          if opt == 'PassWord: ':
-            if Hello:
-              print(f'  {opt}{"".join(list_2)}')
-            else:
-              print(f'  {opt}{"".join(list_1)}')
+            key = getkey()
+            string = key
 
-          elif opt == 'Username: ':
-            if Hello:
-              print(f'  {opt}{"".join(username)}')
+            if key == keys.UP:
+                selection = (selection - 1) % len(menu)
+                if selection == -1:
+                    selection = (selection + len(menu) + 1) % len(menu)
+            elif key == keys.DOWN:
+                selection = (selection + 1) % len(menu)
+                if selection > len(menu):
+                    selection = (selection - len(menu) - 1) % len(menu)
+            if key == keys.UP or key == keys.DOWN:
+                pass
             else:
-              print(f'  {opt}{"".join(username)}')
-          else:
-            print(f'  {opt}')
-
-      key = getkey()
-      string = key
-
-      if keyboard.is_pressed('up'):
-
-        selection = (selection - 1) % len(menu)
-        if selection == -1:
-          selection = (selection + len(menu) + 1) % len(menu)
-      elif keyboard.is_pressed('down'):
-
-        selection = (selection + 1) % len(menu)
-        if selection > len(menu):
-          selection = (selection - len(menu) - 1) % len(menu)
-      if keyboard.is_pressed('up') or keybord.is_pressed('down'):
-        pass
-      else:
-        if selection == 0 or selection == 1:
-          if keyboard.is_pressed('enter'):
-            alert = True
-          else:
-            pass
-
-        if alert == True:
-          alert = False
-        
-        elif alert == False:
-
-      
-          
+                if selection == 0 or selection == 1:
+                    if key == keys.ENTER:
+                        alert = True
+                    else:
+                        pass
 
+                if alert == True:
+                    alert = False
 
-            clear()
-            if keyboard.is_pressed('enter') and selection == 4:
-              JLI = True
-              Sign_In()
-            else:
-              
-              if keyboard.is_pressed('enter') and selection == 3:
-                if ''.join(username) == '' or ''.join(list_2) == '':
-                  print('You have not entered a username or password')
-                  enter_to_continue()
-                  clear()
-                  break
-      
-  
-                    
-                    
-      
-                else:
-                  data = load_json_data()
-                  matches = len(data)
-              
-                  for i in range(matches):
-                    if ''.join(username) == data['Name'+str(i)] and ''.join(list_2) == data['password'+str(i)]:
-                      clear()
-                      print('Logged in!')
-                      enter_to_continue()
-                      clear()
-                      cursor.show()
-                      
-                      return True
-                  else:
-                      print('Invalid username or password!')
-                      enter_to_continue()
-                      clear()
-              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Show Password':
-                list_3 = list_2
-                Hello = True
-                show_hide = True
-              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Hide Password':
-                list_3 = list_1
-                Hello = False
-                show_hide = False
-              if selection == 1:
-                if keyboard.is_pressed('backspace'):
-                  temp_var = list_1.pop(-1)
-                  temp_var = list_2.pop(-1)
-                else:
-                  list_1 += '*'
-                  list_2 += string
-              if selection == 0:
-                if keyboard.is_pressed('backspace'):
-                  try:
-                    username.pop(-1)
-                  except:
+                elif alert == False:
                     clear()
-                else:
-                  if string not in Restrictions:
-                    pass
-                  else:
-                    if keyboard.is_pressed('enter'):
-                      pass
+                    if key == keys.ENTER and selection == 4:
+                        JLI = True
+                        Sign_In()
                     else:
-                      username += string
-              clear()
-    except:
-      clear()
+                        if key == keys.ENTER and selection == 3:
+                            if "".join(username) == "" or "".join(list_2) == "":
+                                print("You have not entered a username or password")
+                                enter_to_continue()
+                                clear()
+                                break
+
+                            else:
+                                data = load_json_data()
+                                matches = len(data)
+
+                                for i in range(matches):
+                                    if (
+                                        "".join(username) == data["Name" + str(i)]
+                                        and "".join(list_2) == data["password" + str(i)]
+                                    ):
+                                        clear()
+                                        print("Logged in!")
+                                        enter_to_continue()
+                                        clear()
+                                        cursor.show()
+
+                                        return True
+                                else:
+                                    print("Invalid username or password!")
+                                    enter_to_continue()
+                                    clear()
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Show Password"
+                        ):
+                            list_3 = list_2
+                            Hello = True
+                            show_hide = True
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Hide Password"
+                        ):
+                            list_3 = list_1
+                            Hello = False
+                            show_hide = False
+                        if selection == 1:
+                            if key == keys.BACKSPACE:
+                                temp_var = list_1.pop(-1)
+                                temp_var = list_2.pop(-1)
+                            else:
+                                list_1 += "*"
+                                list_2 += string
+                        if selection == 0:
+                            if key == keys.BACKSPACE:
+                                try:
+                                    username.pop(-1)
+                                except:
+                                    clear()
+                            else:
+                                if string not in Restrictions:
+                                    pass
+                                else:
+                                    if string == keys.ENTER:
+                                        pass
+                                    else:
+                                        username += string
+                        clear()
+        except:
+            clear()
```

