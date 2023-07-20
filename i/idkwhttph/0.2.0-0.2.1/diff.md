# Comparing `tmp/idkwhttph-0.2.0.tar.gz` & `tmp/idkwhttph-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.0.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.1.tar", max compression
```

## Comparing `idkwhttph-0.2.0.tar` & `idkwhttph-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    37164 2023-07-19 13:18:37.721847 idkwhttph-0.2.0/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-19 13:14:08.898209 idkwhttph-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-19 13:38:48.477754 idkwhttph-0.2.0/setup.py
--rw-r--r--   0        0        0      239 2023-07-19 13:38:48.478515 idkwhttph-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    37487 2023-07-20 10:26:45.009285 idkwhttph-0.2.1/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-20 10:26:39.857294 idkwhttph-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-20 10:26:58.417015 idkwhttph-0.2.1/setup.py
+-rw-r--r--   0        0        0      239 2023-07-20 10:26:58.417343 idkwhttph-0.2.1/PKG-INFO
```

### Comparing `idkwhttph-0.2.0/idkwhttph/__init__.py` & `idkwhttph-0.2.1/idkwhttph/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 #Imports
+import keyboard
 
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
 import json
@@ -833,20 +834,20 @@
           if i == selection:
             print(f'{bold_yes}> {opt}');
 
           else:
             print(f'{bold_yes}  {opt}');
 
         key = getkey();
-        if key == keys.W or key == keys.UP:
+        if key == keys.W or keyboard.is_pressed('up'):
           clear();
           selection = (selection - 1) % len(menu);
           if selection == -1:
             selection = (selection + len(menu) + 1) % len(menu);
-        elif key == keys.S or key == keys.DOWN:
+        elif key == keys.S or keybord.is_pressed('down'):
           clear();
           selection = (selection + 1) % len(menu);
           if selection > len(menu):
             selection = (selection - len(menu) - 1) % len(menu);
       return selection;
 
     except:
@@ -1076,15 +1077,15 @@
 
 
 
 
 
 
       
-      if key == keys.ENTER:
+      if keyboard.is_pressed('enter'):
         if opt == 'PassWord: ':
           break
       clear()
       print(f'{S.RESET_ALL}------------------------------------')
       print('             Sign In!')
       print('')
       print('Please use the arrow keys to move Up or Down')
@@ -1124,52 +1125,52 @@
           else:
             print(f'  {opt}')
 
       key = getkey()
       
       string = key
 
-      if key == keys.UP:
+      if keyboard.is_pressed('up'):
 
         selection = (selection - 1) % len(menu)
         if selection == -1:
           selection = (selection + len(menu) + 1) % len(menu)
-      elif key == keys.DOWN:
+      elif keyboard.is_pressed('down'):
 
         selection = (selection + 1) % len(menu)
         if selection > len(menu):
           selection = (selection - len(menu) - 1) % len(menu)
-      if key == keys.UP or key == keys.DOWN:
+      if keyboard.is_pressed('up') or key == keyboard.is_pressed('down'):
         pass
       else:
         if selection == 0 or selection == 1:
-          if key == keys.ENTER:
+          if keyboard.is_pressed('enter'):
             alert = True
           else:
             pass
 
         if alert == True:
           alert = False
         
         elif alert == False:
 
       
           
 
 
             clear()
-            if key == keys.ENTER and selection == 4:
+            if keyboard.is_pressed('enter') and selection == 4:
               clear()
               print('Redirecting you to login!')
               sleep(3)
               clear()
               sleep(0.5)
               Log_In()
             else:
-              if key == keys.ENTER and selection == 3:
+              if keyboard.is_pressed('enter') and selection == 3:
                 if ''.join(username) == '' or ''.join(list_2) == '':
                   print('You have not entered a username or password')
                   enter_to_continue()
                   clear()
                 elif len(list_2) <= 8:
                   print('Your password must be atleast 8 characters')
                   enter_to_continue()
@@ -1190,40 +1191,40 @@
                   matches = list(matches)
                   matches = len(matches)
                   
                   
                   db['Name'+str(matches)] = ''.join(username)
                   db['password'+str(matches)] = ''.join(list_2)
                   break
-              elif key == keys.ENTER and selection == 2 and menu[2] == 'Show Password':
+              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Show Password':
                 list_3 = list_2
                 Hello = True
                 show_hide = True
-              elif key == keys.ENTER and selection == 2 and menu[2] == 'Hide Password':
+              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Hide Password':
                 list_3 = list_1
                 Hello = False
                 show_hide = False
               if selection == 1:
-                if key == keys.BACKSPACE:
+                if keyboard.is_pressed('backspace'):
                   temp_var = list_1.pop(-1)
                   temp_var = list_2.pop(-1)
                 else:
                   list_1 += '*'
                   list_2 += string
               if selection == 0:
-                if key == keys.BACKSPACE:
+                if keyboard.is_pressed('backspace'):
                   try:
                     username.pop(-1)
                   except:
                     clear()
                 else:
                   if string not in Restrictions:
                     pass
                   else:
-                    if string == keys.ENTER:
+                    if keyboard.is_pressed('enter'):
                       pass
                     else:
                       username += string
               clear()
     except:
       clear()
 
@@ -1265,15 +1266,15 @@
 
 
 
 
 
 
       
-      if key == keys.ENTER:
+      if keyboard.is_pressed('enter'):
         if opt == 'PassWord: ':
           break
       clear()
       print(f'{S.RESET_ALL}------------------------------------')
       print('             Log In!')
       print('')
       print('Please use the arrow keys to move Up or Down')
@@ -1312,49 +1313,49 @@
               print(f'  {opt}{"".join(username)}')
           else:
             print(f'  {opt}')
 
       key = getkey()
       string = key
 
-      if key == keys.UP:
+      if keyboard.is_pressed('up'):
 
         selection = (selection - 1) % len(menu)
         if selection == -1:
           selection = (selection + len(menu) + 1) % len(menu)
-      elif key == keys.DOWN:
+      elif keyboard.is_pressed('down'):
 
         selection = (selection + 1) % len(menu)
         if selection > len(menu):
           selection = (selection - len(menu) - 1) % len(menu)
-      if key == keys.UP or key == keys.DOWN:
+      if keyboard.is_pressed('up') or keybord.is_pressed('down'):
         pass
       else:
         if selection == 0 or selection == 1:
-          if key == keys.ENTER:
+          if keyboard.is_pressed('enter'):
             alert = True
           else:
             pass
 
         if alert == True:
           alert = False
         
         elif alert == False:
 
       
           
 
 
             clear()
-            if key == keys.ENTER and selection == 4:
+            if keyboard.is_pressed('enter') and selection == 4:
               JLI = True
               Sign_In()
             else:
               
-              if key == keys.ENTER and selection == 3:
+              if keyboard.is_pressed('enter') and selection == 3:
                 if ''.join(username) == '' or ''.join(list_2) == '':
                   print('You have not entered a username or password')
                   enter_to_continue()
                   clear()
                   break
       
   
@@ -1374,39 +1375,39 @@
                       cursor.show()
                       
                       return True
                   else:
                       print('Invalid username or password!')
                       enter_to_continue()
                       clear()
-              elif key == keys.ENTER and selection == 2 and menu[2] == 'Show Password':
+              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Show Password':
                 list_3 = list_2
                 Hello = True
                 show_hide = True
-              elif key == keys.ENTER and selection == 2 and menu[2] == 'Hide Password':
+              elif keyboard.is_pressed('enter') and selection == 2 and menu[2] == 'Hide Password':
                 list_3 = list_1
                 Hello = False
                 show_hide = False
               if selection == 1:
-                if key == keys.BACKSPACE:
+                if keyboard.is_pressed('backspace'):
                   temp_var = list_1.pop(-1)
                   temp_var = list_2.pop(-1)
                 else:
                   list_1 += '*'
                   list_2 += string
               if selection == 0:
-                if key == keys.BACKSPACE:
+                if keyboard.is_pressed('backspace'):
                   try:
                     username.pop(-1)
                   except:
                     clear()
                 else:
                   if string not in Restrictions:
                     pass
                   else:
-                    if string == keys.ENTER:
+                    if keyboard.is_pressed('enter'):
                       pass
                     else:
                       username += string
               clear()
     except:
       clear()
```

