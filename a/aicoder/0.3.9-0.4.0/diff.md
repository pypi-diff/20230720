# Comparing `tmp/aicoder-0.3.9-py3-none-any.whl.zip` & `tmp/aicoder-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21651 bytes, number of entries: 12
--rw-r--r--  2.0 unx    12662 b- defN 23-Jul-02 16:18 aicoder/AICoder.py
--rw-r--r--  2.0 unx     8087 b- defN 23-Jul-02 16:18 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     7160 b- defN 23-Jul-02 16:18 aicoder/AICoderPartial.py
--rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
+Zip file size: 22216 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    10950 b- defN 23-Jul-20 09:01 aicoder/AICoder.py
+-rw-r--r--  2.0 unx     9432 b- defN 23-Jul-20 09:01 aicoder/AICoderFull.py
+-rw-r--r--  2.0 unx     7157 b- defN 23-Jul-20 09:32 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     3777 b- defN 23-Jul-19 22:48 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14810 b- defN 23-Jul-02 16:54 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/RECORD
-12 files, 66663 bytes uncompressed, 20071 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx    16651 b- defN 23-Jul-20 09:31 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-20 09:45 aicoder-0.4.0.dist-info/RECORD
+12 files, 68340 bytes uncompressed, 20636 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/LICENSE
+Filename: aicoder-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/METADATA
+Filename: aicoder-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/WHEEL
+Filename: aicoder-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/entry_points.txt
+Filename: aicoder-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/top_level.txt
+Filename: aicoder-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.3.9.dist-info/RECORD
+Filename: aicoder-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoder.py

```diff
@@ -2,16 +2,15 @@
 import colorlog
 import openai
 import json
 import os
 import re
 import subprocess
 from threading import Lock
-from aicoder.AICoderPrompts import PERSONALITY, PROGRAM_TO_GENERATE, FINAL_CLARIFICATIONS, GET_FILE_CONTENTS, ERROR_FIX, GET_ERRORS_JSON, COMPILATION_COMMAND
-
+from AICoderPrompts import PERSONALITY, PROGRAM_TO_GENERATE, FINAL_CLARIFICATIONS, ERROR_FIX, GET_ERRORS_JSON, COMPILATION_COMMAND
 
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
     logger.addHandler(handler)
@@ -54,19 +53,25 @@
 
         return all_text
     
 
     def remove_fences(self, text: str) -> str:
         """Function that removes code fences from the response"""
 
+        text = text.strip()
         if len(text.split("```")) == 3:
             text = "\n".join(text.split("```")[1].split("\n")[1:])
         
         elif len(text.split("```")) > 3:
-            logger.info(f"The response has more than 3 code fences: " + text)
+            if text.startswith("```"):
+                text = "\n".join(text.split("\n")[1:])
+            if text.endswith("```"):
+                text = "\n".join(text.split("\n")[:-1])
+            
+            logger.info(f"The response had more than 3 code fences: " + text)
         
         return text
 
     def fix_json(self, orig_text: str, orig_response: str, json_error: str) -> str:
         """Function that asks to fix a given json"""
 
         all_msg = f"{orig_text}\n\n You already gave this reponse:\n{orig_response}\n\nWhich resulted in this error:\n{json_error}\n\nPlease fix it and respond with a valid json."
@@ -98,71 +103,22 @@
 
         imports = []
         for line in file_content.split("\n"):
             if re.match(r'^[^\s]*(import|include|require|require_once|include_once|use |from [\w\.]+ import)', line):
                 imports.append(line)
             elif re.match(r'=\s+require', line): # const asd, asd2 = require("asd")
                 imports.append(line)
-            
-            #TODO: In golang it's multiline: import (\n"fmt"\n"math"
-        
-        return imports
-
-    
-    def generate_file(self, file: dict, files_to_generate: list, extra_content:str = ""):
-        """Function that generates the files given a list of files to generate"""
-
-        global ALL_IMPORTS, IMPORTS_LOCK
-        
-        file_path = file["path"]
-        is_main = "/main." in file["path"]
-
-        # Create the folders
-        self.create_folder(file_path)
-
-        # Get the dependencies if not main. Wait until all the dependencies are generated.
-        dependencies_content = ""
-        if not is_main:
-            dependencies_content = self.wait_on_dependencies(file)
         
-        # Generate the code
-        msg = GET_FILE_CONTENTS.replace("__FILE_PATH__", file_path).replace("__FILES_JSON__", json.dumps(files_to_generate, indent=4)) + dependencies_content + extra_content
-        file_content = self.contact(msg, p_info_msg=False)
-
-        # Even if we asked to not return this marks it might return them
-        file_content = self.remove_fences(file_content)
-
-        # Check for todos
-        if self.check_for_todos(file_content):
-            logger.warning(f"Found TODOs in {file_path}")
-            return self.generate_file(file=file, files_to_generate=files_to_generate)
-
-        # Ask if main is as expected
-        if is_main:
-            print("This is the main file content:\n", file_content)
-            print("")
-            print("Is this ok or where you expecting something different? (Y/n)")
-            user_input = input()
-            if user_input.lower() in ["no", "n"]:
-                print("I'll try to generate the files again... Tell me the problem in one line:")
-                extra_content = "\n\nLast time I asked your response was: " + file_content
-                extra_content += "\n\n" + input()
-                return self.generate_file(file=file, files_to_generate=files_to_generate, extra_content=extra_content)
+        # In golang imports are multiline so this function should also be able to find those imports. Example: import (\n"fmt"\n"math"
+        pattern = r'import\s*\((.*?)\)'
+        multiline_imports = re.findall(pattern, file_content, re.DOTALL)
+        for multiline_import in multiline_imports:
+            imports.append(multiline_import)
         
-        # Save the file
-        self.write_file(file_path, file_content)
-
-        # Get imports
-        file_imports = self.extract_imports(file_content)
-        if file_imports:
-            with IMPORTS_LOCK:
-                ALL_IMPORTS[file_path] = file_imports
-
-        return file_content
-
+        return imports
 
     def try_to_compile(self):
         """Function that tries to compile the program"""
 
         global ALL_IMPORTS
 
         msg_imports = f"These are all the imports files are using: {json.dumps(ALL_IMPORTS, indent=4)}\n\n"
@@ -327,8 +283,7 @@
         else:
             # Ask for the command to run
             print("Indicate the command to run in 1 line:")
             command_to_run = input()
 
             # Execute getting the stdout and stderr
             self.fix_errors_per_file_auto(command_to_run)
-
```

## aicoder/AICoderFull.py

```diff
@@ -2,21 +2,22 @@
 import colorlog
 import json
 import os
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
 from time import sleep
-from aicoder.AICoderPrompts import GET_ALL_FILES
-from aicoder.AICoder import AICoder, ALL_IMPORTS, IMPORTS_LOCK
-
+from AICoderPrompts import GET_ALL_FILES, GET_FILE_CONTENTS
+from AICoder import AICoder, ALL_IMPORTS, IMPORTS_LOCK
 
+# Set up logging with colorlog
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
+# Create a logger for this module
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
 
 class AICoderFull(AICoder):
     """Class that generates code using OpenAI's API"""
@@ -28,122 +29,152 @@
     def get_files_to_generate(self, extra_content=""):
         """Function that asks the model to return the file names to generate the program"""
 
         logger.info("Generating list of files...")
         msg = GET_ALL_FILES + extra_content
         files_to_generate = self.contact(msg)
         try:
-            try:
-                all_files = json.loads(self.remove_fences(files_to_generate))
-            except Exception as e:
-                all_files = self.fix_json(msg, files_to_generate, str(e))
-            
-            # If more than 50% of files have .h extension, retry
-            if len([file for file in all_files if file["path"].endswith(".h")]) > len(all_files) * 0.75 and len(all_files) > 3:
-                logger.warning("Found more than 75% of .h files, retrying asking for the implementations...")
-                extra_content = "\nLast time I asked your response was:\n" + files_to_generate
-                extra_content += "\n\nDon't forget to include the implementation files."
-                return self.get_files_to_generate(extra_content=extra_content)
-
-            # If more than 50% of files have .m extension, retry
-            if len([file for file in all_files if file["path"].endswith(".m")]) > len(all_files) * 0.75 and len(all_files) > 3:
-                logger.warning("Found more than 75% of .m files, retrying asking for the headers...")
-                extra_content = "\nLast time I asked your response was:\n" + files_to_generate
-                extra_content += "\n\nDon't forget to include the header files"
-                return self.get_files_to_generate(extra_content=extra_content)
-            
-            # If more than 50% of files have .c extension, retry
-            if len([file for file in all_files if file["path"].endswith(".c")]) > len(all_files) * 0.75 and len(all_files) > 3:
-                logger.warning("Found more than 75% of .c files, retrying asking for the headers...")
-                extra_content = "\nLast time I asked your response was:\n" + files_to_generate
-                extra_content += "\n\nDon't forget to include the header files."
-                return self.get_files_to_generate(extra_content=extra_content)
-
-            # If more than 50% of files have .cpp extension, retry
-            if len([file for file in all_files if file["path"].endswith(".cpp")]) > len(all_files) * 0.75 and len(all_files) > 3:
-                logger.warning("Found more than 75% of .cpp files, retrying asking for the headers...")
-                extra_content = "\nLast time I asked your response was:\n" + files_to_generate
-                extra_content += "\n\nDon't forget to include the header files."
-                return self.get_files_to_generate(extra_content=extra_content)
-            
-            # Check if files are going to be generated in "./generated/"
-            for f in all_files:
-                if not "/generated/" in f["path"]:
-                    logger.warning(f"Found a file not in './generated/' ({f['path']}). Asking to re-generate...")
-                    extra_content = "\nLast time I asked your response was:\n" + files_to_generate
-                    extra_content += "\n\nDon't forget to generate the files in the foler './generated/'"
-                    return self.get_files_to_generate(extra_content=extra_content)
-            
-            print("Files to generate: ", json.dumps(all_files, indent=4))
-
-            # Ask user if thats ok
-            print("Is this ok? (Y/n)")
-            user_input = input()
-            if user_input.lower() in ["no", "n"]:
-                print("I'll try to generate the files again... Tell me the problem:")
-                extra_content = "\n" + input()
-                return self.get_files_to_generate(extra_content=extra_content)
-            
-            return all_files
+            # Try to parse the response as JSON
+            all_files = json.loads(self.remove_fences(files_to_generate))
         except Exception as e:
-            raise e
-
+            # If parsing fails, try to fix the JSON
+            all_files = self.fix_json(msg, files_to_generate, str(e))
+        
+        # Check for file extension imbalance and file location
+        file_extensions = [".h", ".m", ".c", ".cpp"]
+        for ext in file_extensions:
+            if self.check_file_extension(all_files, ext):
+                extra_content = self.generate_extra_content(files_to_generate, ext)
+                return self.get_files_to_generate(extra_content=extra_content)
+        
+        if self.check_file_location(all_files):
+            extra_content = self.generate_extra_content(files_to_generate, "/generated/")
+            return self.get_files_to_generate(extra_content=extra_content)
+        
+        return self.confirm_files(all_files)
+        
+    def check_file_extension(self, all_files, extension):
+        # Check if more than 75% of the files have the same extension
+        return len([file for file in all_files if file["path"].endswith(extension)]) > len(all_files) * 0.75 and len(all_files) > 3
+
+    def check_file_location(self, all_files):
+        # Check if any file is not in the /generated/ directory
+        return any("/generated/" not in f["path"] for f in all_files)
+
+    def generate_extra_content(self, files_to_generate, extension):
+        # Generate extra content for the next request based on the previous response
+        extra_content = "\nLast time I asked your response was:\n" + files_to_generate
+        extra_content += "\n\nDon't forget to include the " + ("header" if extension == ".h" else "implementation") + " files."
+        return extra_content
+
+    def confirm_files(self, all_files):
+        # Confirm the list of files with the user
+        print("Files to generate: ", json.dumps(all_files, indent=4))
+        print("Is this ok? (Y/n)")
+        user_input = input()
+        if user_input.lower() in ["no", "n"]:
+            print("I'll try to generate the files again... Tell me the problem:")
+            extra_content = "\n" + input()
+            return self.get_files_to_generate(extra_content=extra_content)
+        return all_files
 
     def wait_on_dependencies(self, file: dict) -> str:
         """Function that waits until all the dependencies are generated"""
 
-        dependencies_content = ""
         cont = 0
         all_exists = True
         while cont < 50:
-            for dep in file["dependencies"]:
-                if not os.path.exists(dep):
-                    all_exists = False
-                    logger.info(f"Sleeping from {file['path']} the dependency: {dep}")
-                    sleep(10)
-                    if cont > 48:
-                        logger.warning(f"The dependency {dep} of {file['path']} doesn't exist.")
-                    cont += 1
-                    continue
+            all_exists = self.check_dependencies(file, cont, all_exists)
             if all_exists:
                 break
+        return self.get_dependencies_content(file)
+
+    def generate_file(self, file: dict, files_to_generate: list, extra_content:str = ""):
+        """Function that generates the files given a list of files to generate"""
+
+        global ALL_IMPORTS, IMPORTS_LOCK
+        
+        file_path = file["path"]
+        is_main = "/main." in file["path"]
+
+        # Create the folders
+        self.create_folder(file_path)
+
+        # Get the dependencies if not main. Wait until all the dependencies are generated.
+        dependencies_content = ""
+        if not is_main:
+            dependencies_content = self.wait_on_dependencies(file)
         
+        # Generate the code
+        msg = GET_FILE_CONTENTS.replace("__FILE_PATH__", file_path).replace("__FILES_JSON__", json.dumps(files_to_generate, indent=4)) + dependencies_content + extra_content
+        file_content = self.contact(msg, p_info_msg=False)
+
+        # Even if we asked to not return this marks it might return them
+        file_content = self.remove_fences(file_content)
+
+        # Check for todos
+        if self.check_for_todos(file_content):
+            logger.warning(f"Found TODOs in {file_path}")
+            return self.generate_file(file=file, files_to_generate=files_to_generate)
+
+        # Ask if main is as expected
+        if is_main:
+            print("This is the main file content:\n", file_content)
+            print("")
+            print("Is this ok or where you expecting something different? (Y/n)")
+            user_input = input()
+            if user_input.lower() in ["no", "n"]:
+                print("I'll try to generate the files again... Tell me the problem in one line:")
+                extra_content = "\n\nLast time I asked your response was: " + file_content
+                extra_content += "\n\n" + input()
+                return self.generate_file(file=file, files_to_generate=files_to_generate, extra_content=extra_content)
+        
+        # Save the file
+        self.write_file(file_path, file_content)
+
+        # Get imports
+        file_imports = self.extract_imports(file_content)
+        if file_imports:
+            with IMPORTS_LOCK:
+                ALL_IMPORTS[file_path] = file_imports
+
+        return file_content
+
+    def check_dependencies(self, file, cont, all_exists):
+        # Check if all dependencies exist
+        for dep in file["dependencies"]:
+            if not os.path.exists(dep):
+                all_exists = False
+                logger.info(f"Sleeping from {file['path']} the dependency: {dep}")
+                sleep(10)
+                if cont > 48:
+                    logger.warning(f"The dependency {dep} of {file['path']} doesn't exist.")
+                cont += 1
+        return all_exists
+
+    def get_dependencies_content(self, file):
+        # Get the content of all dependencies
+        dependencies_content = ""
         for dep in file["dependencies"]:
             if os.path.exists(dep):
                 with open(dep, "r") as f:
                     dependencies_content += "\n\nThis is the content of the dependency file '" + file["path"] + "':\n" + f.read()
-        
         return dependencies_content
 
-
     def generate_program(self):
         """Function that generates a full program from 0"""
 
-        global ALL_IMPORTS
-
         # Get files to generate
         files_to_generate = self.get_files_to_generate()
 
         # Order files to generated from less amount of dependencies to more
         files_to_generate = sorted(files_to_generate, key=lambda x: len(x["dependencies"]))
         
-        # Put the main file the first one and generate it now
-        main_file_found = False
-        for file in files_to_generate:
-            if "/main." in file["path"].lower():
-                logger.info("Generating main file...")
-                main_file_content = self.generate_file(file, files_to_generate)
-                files_to_generate.remove(file)
-                file["description"] = file["description"] + "\nMain file content:\n" + main_file_content
-                files_to_generate.insert(0, file)
-                main_file_found = True
-                break
-        
-        if not main_file_found:
-            raise Exception("No main file found")
+        # Generate main file
+        files_to_generate = self.generate_main_file(files_to_generate)
         
         # Initialize a ThreadPoolExecutor and a progress bar
         with tqdm(total=len(files_to_generate[1:]), desc="Generating files", unit="file") as pbar:
             sleep(0.1) #Allow the progress bar to be displayed
             with ThreadPoolExecutor(max_workers=3) as executor: # 3 is ok, don't oversaturate the server
                 # Submit tasks to the executor
                 futures = {executor.submit(self.generate_file, file, files_to_generate): file for file in files_to_generate[1:]}
@@ -163,7 +194,24 @@
                         pbar.update(1)  # update progress bar
 
         # Try to compile the program
         self.try_to_compile()
 
         # Try to run the program
         self.try_to_run()
+
+    def generate_main_file(self, files_to_generate):
+        # Generate the main file first
+        main_file_found = False
+        for file in files_to_generate:
+            if "/main." in file["path"].lower():
+                logger.info("Generating main file...")
+                main_file_content = self.generate_file(file, files_to_generate)
+                files_to_generate.remove(file)
+                file["description"] = file["description"] + "\nMain file content:\n" + main_file_content
+                files_to_generate.insert(0, file)
+                main_file_found = True
+                break
+        
+        if not main_file_found:
+            raise Exception("No main file found")
+        return files_to_generate
```

## aicoder/AICoderPartial.py

```diff
@@ -1,16 +1,16 @@
 import logging
 from typing import List
 import colorlog
 import subprocess
 import os
 from time import sleep
 from github import Github
-from aicoder.AICoderPrompts import MODIFY_FILE, FILE_FROM_TEMPALTES
-from aicoder.AICoder import AICoder
+from AICoderPrompts import MODIFY_FILE, FILE_FROM_TEMPALTES, ASK_FOR_FILE
+from AICoder import AICoder
 
 # Setting up logger
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
@@ -47,15 +47,14 @@
         
         # If branch, create PR
         if orig_branch and repo_name:
             commit_msg = f"File {os.path.basename(file_path)} modified by AICoder"
             commit_body = f"AICoder modified the file {file_path} according to this input:\n{prompt}"
             self.create_pull_request(commit_msg, commit_body, orig_branch, to_branch, repo_name)
 
-
     def gen_file_from_templates(self, template_file_paths: List[str], final_file_path: str, prompt: str, orig_branch: str, to_branch: str, repo_name:str):
         """Function that generates a file from a template"""
 
         if orig_branch:
             self.change_branch(orig_branch)
 
         # Create needed folders
```

## aicoder/AICoderPrompts.py

```diff
@@ -1,13 +1,13 @@
 
 
 
-PERSONALITY = "You are a developer. The code you generate is beautiful, all commented, and very modular. You never leave TODOs or incomplete code and only respond with code."
+PERSONALITY = "You are a developer. The code you generate is beautiful, all commented, very modular, and secure. You never leave TODOs or incomplete code and only respond with code."
 
-PROGRAM_TO_GENERATE = """These are the specifications of the code you need to generate:\n\n"""
+PROGRAM_TO_GENERATE = """These are the specifications of the code you need to generate or check:\n\n"""
 
 GET_ALL_FILES = """Return a valid json with all the file paths from the directory './generated/' that need to be created to generate the program.
 
 The main file should be called 'main' with the extension (e.g. 'main.py'), it must contain the flow of the program so it should be the one importing from the rest.
 
 The JSON must have this structure:
 [
@@ -84,12 +84,19 @@
 Respond only with final code of the file, don't add apologies or explanations, just respond the full code.
 
 The file __FILE_PATH__ has the following content:
 
 __FILE_CONTENT__
 """
 
+ASK_FOR_FILE = """Based on the following content from the file __FILE_PATH__ follows this indications: __PROMPT__.
+
+The file __FILE_PATH__ has the following content:
+
+__FILE_CONTENT__
+"""
+
 FILE_FROM_TEMPALTES = """Develop the file __FINAL_FILE_PATH__ following this indications: __PROMPT__.
 Respond only with final code of the file, don't add apologies or explanations, just respond the full code.
 
 Please, use as templates the following files:
 """
```

## aicoder/main.py

```diff
@@ -35,52 +35,54 @@
     aicoderfull = AICoderFull(prompt, api_key, "", model)
     aicoderfull.generate_program()
 
 def file_generator(prompt: str, api_key: str, github_token: str, model: str, template_files: list, final_file_path: str, orig_branch: str, to_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
     aicoderpartial.gen_file_from_templates(template_files, final_file_path, prompt, orig_branch, to_branch, repo_name)
 
-def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
+def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, prompt, orig_branch, to_branch, repo_name)
+    aicoderpartial.modify_file(file_path, prompt, orig_branch, to_branch, repo_name)
 
-def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
+def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, add useful comments to it inside the code to easily understand what it does."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def check_security(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
+def check_security(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, search for security vulnerabilities and potential backdoors on it and if any, create a new code fixing it (if possible). Return only the fixed code with the comments. If you changed anything, add at the end of the code comments explaining the changes."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
+def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean and beautiful, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
     final_prompt += "Don't remove comments, just improve them if possible. If you cannot improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes. "
     final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if part of the code can be improved the different functionalities must be keeped."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
+def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code and keeping the same functionality fix all the bugs in it. Also, don't remove comments, just improve them if possible."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
+
+def todoer(prompt: str, api_key: str, github_token: str, model: str, file_path: list, orig_branch: str, to_branch: str, repo_name: str):
+    final_prompt = "Given some code, check all the TODOs and remove them adding the code that performs the functionality mentioned inside the TODO comment. If you need more information about any TODO, ask for more information inside the TODO comment and leave the comment in the code."
+    if prompt:
+        final_prompt = "\n" + prompt
+    aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
 def add_common_arguments(parser):
     parser.add_argument('--api-key', default=None, type=str, help='Input API key')
     parser.add_argument('--model', default="gpt-4", type=str, help='Model to use')
     parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
 
 def get_git_org_repo_name():
@@ -94,16 +96,17 @@
     full_generator_parser = subparsers.add_parser('full-generator', help='Generate a full program from the prompt.')
     file_generator_parser = subparsers.add_parser('file-generator', help='Generate a file based on others as templates.')
     file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on the given prompt.')
     file_commentor_parser = subparsers.add_parser('file-comments', help='Ask to add comments to a file.')
     file_security_parser = subparsers.add_parser('file-security', help='Ask to search security vulnerabilities and backdoors in a file.')
     file_optimizer_parser = subparsers.add_parser('file-optimizer', help='Ask to optimize a file in terms of clean code and efficiency.')
     file_bug_fixer_parser = subparsers.add_parser('file-bugfixer', help='Ask to fix bugs in a file.')
+    file_todoer_parser = subparsers.add_parser('file-todoer', help='Ask to complete the TODOs inside the code.')
 
-    for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser, file_bug_fixer_parser]:
+    for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser, file_bug_fixer_parser, file_todoer_parser]:
         add_common_arguments(subparser)
 
     file_generator_parser.add_argument('--template-files', type=str, help='Comma separated list of template files')
     file_generator_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_generator_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_generator_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_generator_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
@@ -122,56 +125,66 @@
     file_commentor_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
     file_security_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to search vulnerabilities')
     file_security_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_security_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_security_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_security_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
+    file_security_parser.add_argument('--only-ask', default=None, type=str, help='Indicate that you only want to ask for security problems, not to change the code.')
     
     file_optimizer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to optimize')
     file_optimizer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_optimizer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_optimizer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_optimizer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
+    file_optimizer_parser.add_argument('--only-ask', default=None, type=str, help='Indicate that you only want to ask for optimizations, not to change the code.')
 
     file_bug_fixer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to fix bugs')
     file_bug_fixer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_bug_fixer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_bug_fixer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_bug_fixer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
+    file_bug_fixer_parser.add_argument('--only-ask', default=None, type=str, help='Indicate that you only want to ask for the bugs, not fix them.')
+
+    file_todoer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to complete TODOs')
+    file_todoer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
+    file_todoer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
+    file_todoer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
+    file_todoer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
     api_key = os.environ.get("INPUT_OPENAI_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
+    github_token = os.environ.get("GITHUB_TOKEN")
 
-    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
+    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer", "file-todoer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
         repo_name = os.environ.get("GITHUB_REPOSITORY") or args.repo_name or get_git_org_repo_name()
 
         if args.mode == "file-generator":
             template_files = os.environ.get("TEMPLATE_FILES") or args.template_files
             template_files = list(template_files.strip().split(","))
             final_file_path = os.environ.get("FINAL_FILE_PATH") or args.file_path
             if not template_files or not final_file_path:
                 logger.error("Error: Missing template_files or final_file_path.")
                 parser.print_help()
                 sys.exit(1)
                 
-        elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
+        elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer", "file-todoer"]:
             check_paths = os.environ.get("CHECK_PATHS") or args.paths
             check_paths = list(check_paths.split(","))
             if not check_paths:
                 logger.error("Error: Missing check_paths.")
                 parser.print_help()
                 sys.exit(1)
-    
-    if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
+            
+    if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer", "file-bugfixer", "file-todoer"]:
         logger.error("Error: Missing prompt.")
         parser.print_help()
         sys.exit(1)
     
     if not api_key:
         logger.error("Error: Missing API key.")
         parser.print_help()
@@ -209,25 +222,27 @@
         logger.error("Error: No repo name. PRs cannot be created automatically. Stopping.")
         exit(1)
     
     elif args.mode == 'file-generator':
         file_generator(prompt, api_key, github_token, model, template_files, final_file_path, orig_branch, to_branch, repo_name)
         exit(0)
     
-    elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bugfixer']:
+    elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bugfixer', 'file-todoer']:
         if args.mode == 'file-enhancer':
             f = enhancer
         elif args.mode == 'file-comments':
             f = add_comments
         elif args.mode == 'file-security':
             f = check_security
         elif args.mode == 'file-optimizer':
             f = optimize_file
         elif args.mode == 'file-bugfixer':
             f = fix_bugs
+        elif args.mode == 'file-todoer':
+            f = todoer
         
         for file_path in check_paths:
             if os.path.isfile(file_path):
                 logger.info(f"Given path {file_path} is a file.")
                 f(prompt, api_key, github_token, model, file_path, orig_branch, to_branch, repo_name)
         
             elif os.path.isdir(file_path):
```

## Comparing `aicoder-0.3.9.dist-info/LICENSE` & `aicoder-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

