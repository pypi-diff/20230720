# Comparing `tmp/infix-postfix-1.1.0.tar.gz` & `tmp/infix-postfix-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infix-postfix-1.1.0.tar", last modified: Mon Feb  6 05:16:09 2023, max compression
+gzip compressed data, was "infix-postfix-1.2.0.tar", last modified: Thu Jul 20 10:24:10 2023, max compression
```

## Comparing `infix-postfix-1.1.0.tar` & `infix-postfix-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-02-06 05:16:09.468392 infix-postfix-1.1.0/
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1075 2023-01-31 07:18:31.000000 infix-postfix-1.1.0/LICENSE
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     2043 2023-02-06 05:16:09.468272 infix-postfix-1.1.0/PKG-INFO
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1088 2023-02-06 05:05:30.000000 infix-postfix-1.1.0/README.md
-drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-02-06 05:16:09.467451 infix-postfix-1.1.0/infix_postfix/
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)        0 2023-01-31 07:57:48.000000 infix-postfix-1.1.0/infix_postfix/__init__.py
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     2435 2023-02-06 05:05:30.000000 infix-postfix-1.1.0/infix_postfix/infix_postfix.py
-drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-02-06 05:16:09.468104 infix-postfix-1.1.0/infix_postfix.egg-info/
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     2043 2023-02-06 05:16:09.000000 infix-postfix-1.1.0/infix_postfix.egg-info/PKG-INFO
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)      271 2023-02-06 05:16:09.000000 infix-postfix-1.1.0/infix_postfix.egg-info/SOURCES.txt
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)        1 2023-02-06 05:16:09.000000 infix-postfix-1.1.0/infix_postfix.egg-info/dependency_links.txt
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       67 2023-02-06 05:16:09.000000 infix-postfix-1.1.0/infix_postfix.egg-info/entry_points.txt
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       14 2023-02-06 05:16:09.000000 infix-postfix-1.1.0/infix_postfix.egg-info/top_level.txt
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       38 2023-02-06 05:16:09.468429 infix-postfix-1.1.0/setup.cfg
--rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1728 2023-02-06 05:06:25.000000 infix-postfix-1.1.0/setup.py
+drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-07-20 10:24:10.780262 infix-postfix-1.2.0/
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1075 2023-01-31 07:18:31.000000 infix-postfix-1.2.0/LICENSE
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     2556 2023-07-20 10:24:10.780067 infix-postfix-1.2.0/PKG-INFO
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1601 2023-07-20 10:18:30.000000 infix-postfix-1.2.0/README.md
+drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-07-20 10:24:10.778475 infix-postfix-1.2.0/infix_postfix/
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)        0 2023-01-31 07:57:48.000000 infix-postfix-1.2.0/infix_postfix/__init__.py
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     3189 2023-07-20 10:19:14.000000 infix-postfix-1.2.0/infix_postfix/infix_postfix.py
+drwxr-xr-x   0 soumadeepchoudhury   (501) staff       (20)        0 2023-07-20 10:24:10.779745 infix-postfix-1.2.0/infix_postfix.egg-info/
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     2556 2023-07-20 10:24:10.000000 infix-postfix-1.2.0/infix_postfix.egg-info/PKG-INFO
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)      271 2023-07-20 10:24:10.000000 infix-postfix-1.2.0/infix_postfix.egg-info/SOURCES.txt
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)        1 2023-07-20 10:24:10.000000 infix-postfix-1.2.0/infix_postfix.egg-info/dependency_links.txt
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       67 2023-07-20 10:24:10.000000 infix-postfix-1.2.0/infix_postfix.egg-info/entry_points.txt
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       14 2023-07-20 10:24:10.000000 infix-postfix-1.2.0/infix_postfix.egg-info/top_level.txt
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)       38 2023-07-20 10:24:10.780339 infix-postfix-1.2.0/setup.cfg
+-rw-r--r--   0 soumadeepchoudhury   (501) staff       (20)     1728 2023-07-20 10:22:13.000000 infix-postfix-1.2.0/setup.py
```

### Comparing `infix-postfix-1.1.0/LICENSE` & `infix-postfix-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infix-postfix-1.1.0/PKG-INFO` & `infix-postfix-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infix-postfix
-Version: 1.1.0
+Version: 1.2.0
 Summary: Converts Infix to Postfix and vice versa...
 Home-page: https://github.com/SoumadeepChoudhury/infixpostfix
 Author: Ahens | An Initiative to Initial (Soumadeep Choudhury)
 Author-email: ahensinitiative@gmail.com
 License: MIT
 Keywords: python,arithmetic,tools,arith-tools,arithmetic operations,Math,python3,pip,pip3,fibonacci,armstrong,boiled-egg,terrace,unique,amicable,infix,postfix,infix2postfix,infixtopostfix,infix-postfix,infix_postfix
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,14 +40,39 @@
 - Run the command `pip install infix-postfix`.
 
 
 # Usage
 - To convert infix to postfix, run `infix-postfix --infix "${infix_expression}"`
 - To convert postfix to infix, run `infix-postfix --postfix "${postfix_expression}"`
 > NOTE : Double quotes ("") is must for writing the expression to get correct output..
+
+```
+How to write expressions? 
+- INFIX expression
+    - Correct Methods
+        - "( A+B)* C/D"
+        - "((A+B)*C/D+E^F)/G"
+        - "20.1 + (5 ^ 2 / 2)"
+        - "20.1 + ( 5 ^ 2 / 2)"
+        - etc...
+
+- POSTFIX ecpression
+    - Correct Methods
+        - "A B + C * D /"
+        - "A B C D + E F + * G / + * H *"
+        - "20.1 5 +"
+    - Wrong Methods
+        - "AB+C*D/"
+        - "ABCD+EF+*G/+*H*"
+        - "20.1 5+"
+        - "20 5+"
+    - In One line, You have to give spaces after every value
+```
+
+
 - To run this application in your own application or python script, run
  
 ```python
 from infix_postfix.infix_postfix import infix,postfix
 $(variable) = $(infix/postfix){expression}
 print($(variable))
 ```
```

### Comparing `infix-postfix-1.1.0/infix_postfix/infix_postfix.py` & `infix-postfix-1.2.0/infix_postfix/infix_postfix.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 
 class Stack:
+    '''Class defining basic stack functions.'''
+
     def __init__(self) -> None:
         self.STACK = list()
 
     def isEmpty(self) -> bool:
+        '''Checks for empty stack'''
         if self.STACK == []:
             return True
         return False
 
     def push(self, item: str) -> None:
+        '''Push element in stack'''
         self.STACK.append(item)
 
     def pop(self) -> str:
+        '''Removes top element from stack'''
         if self.isEmpty():
             return "Underflow"
         item: str = self.STACK.pop()
         return item
 
     def peek(self) -> str:
+        '''Displays the topmost element of the stack'''
         if self.isEmpty():
             return "Underflow"
         else:
             return self.STACK[-1]
 
 
 def isHigherPrecedence(val1: str, val2: str) -> bool:
-    """Returns True if 1st value have higher precedence than 2nd value."""
+    """Checks for precedence. Returns True if 1st value have higher precedence than 2nd value."""
     PRECEDENCE: list = ["^", "*/", "+-"]
     val1_index: int = None
     val2_index: int = None
     for i in range(len(PRECEDENCE)):
         if val1 in PRECEDENCE[i]:
             val1_index = i
         if val2 in PRECEDENCE[i]:
@@ -40,50 +46,63 @@
         else:
             return True
     else:
         return False
 
 
 def postfix(infix: str) -> str:
+    '''Converts infix to postfix expression'''
     STACK: object = Stack()
     if infix[0] != "(" or infix[-1] != ")":
         infix = "("+infix+")"
     postfix: str = ""
     for i in infix:
         if i in "(+-*/^":
+            if postfix != "":
+                postfix += (" " if postfix[-1] != " " else "")
             while isHigherPrecedence(STACK.peek(), i):
                 item: str = STACK.pop()
                 if item not in ("Underflow", "(", ")"):
-                    postfix += item
+                    postfix += item+" "
             STACK.push(i)
         elif i == ")":
+            if postfix != "":
+                postfix += (" " if postfix[-1] != " " else "")
             while STACK.peek() != "(":
                 item: str = STACK.pop()
                 if item not in ("Underflow", "(", ")"):
-                    postfix += item
+                    postfix += item+" "
             item: str = STACK.pop()
             if item not in ("Underflow", "(", ")"):
-                postfix += item
-        else:
+                postfix += item+" "
+        elif (i != ' '):
             postfix += i
-    return postfix
+    return postfix.strip()
 
 
 def infix(postfix: str) -> str:
+    '''Converts postfix to infix expression'''
     STACK: object = Stack()
+    value = ""
     for i in postfix:
         if i not in "+-*/^":
-            STACK.push(i)
+            if (i == " "):
+                if value != "":
+                    STACK.push(value)
+                value = ""
+            else:
+                value += i
         else:
             after: str = STACK.pop()
             before: str = STACK.pop()
             evaluated: str = "("+before+i+after+")"
             STACK.push(evaluated)
     return STACK.pop()[1:-1]
 
 
 def main():
+    '''Startup point of application'''
     import sys
     if sys.argv[1] == "--infix":
         print(postfix(sys.argv[2]))
     elif sys.argv[1] == "--postfix":
         print(infix(sys.argv[2]))
```

### Comparing `infix-postfix-1.1.0/infix_postfix.egg-info/PKG-INFO` & `infix-postfix-1.2.0/infix_postfix.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infix-postfix
-Version: 1.1.0
+Version: 1.2.0
 Summary: Converts Infix to Postfix and vice versa...
 Home-page: https://github.com/SoumadeepChoudhury/infixpostfix
 Author: Ahens | An Initiative to Initial (Soumadeep Choudhury)
 Author-email: ahensinitiative@gmail.com
 License: MIT
 Keywords: python,arithmetic,tools,arith-tools,arithmetic operations,Math,python3,pip,pip3,fibonacci,armstrong,boiled-egg,terrace,unique,amicable,infix,postfix,infix2postfix,infixtopostfix,infix-postfix,infix_postfix
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,14 +40,39 @@
 - Run the command `pip install infix-postfix`.
 
 
 # Usage
 - To convert infix to postfix, run `infix-postfix --infix "${infix_expression}"`
 - To convert postfix to infix, run `infix-postfix --postfix "${postfix_expression}"`
 > NOTE : Double quotes ("") is must for writing the expression to get correct output..
+
+```
+How to write expressions? 
+- INFIX expression
+    - Correct Methods
+        - "( A+B)* C/D"
+        - "((A+B)*C/D+E^F)/G"
+        - "20.1 + (5 ^ 2 / 2)"
+        - "20.1 + ( 5 ^ 2 / 2)"
+        - etc...
+
+- POSTFIX ecpression
+    - Correct Methods
+        - "A B + C * D /"
+        - "A B C D + E F + * G / + * H *"
+        - "20.1 5 +"
+    - Wrong Methods
+        - "AB+C*D/"
+        - "ABCD+EF+*G/+*H*"
+        - "20.1 5+"
+        - "20 5+"
+    - In One line, You have to give spaces after every value
+```
+
+
 - To run this application in your own application or python script, run
  
 ```python
 from infix_postfix.infix_postfix import infix,postfix
 $(variable) = $(infix/postfix){expression}
 print($(variable))
 ```
```

### Comparing `infix-postfix-1.1.0/setup.py` & `infix-postfix-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="infix-postfix",
-    version="1.1.0",
+    version="1.2.0",
     description="Converts Infix to Postfix and vice versa...",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/SoumadeepChoudhury/infixpostfix",
     author="Ahens | An Initiative to Initial (Soumadeep Choudhury)",
     author_email="ahensinitiative@gmail.com",
     license="MIT",
```

