# Comparing `tmp/cmsis_stream-1.5.1-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 81278 bytes, number of entries: 67
+Zip file size: 83299 bytes, number of entries: 69
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -27,43 +27,45 @@
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3762 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/ccode.py
 -rw-rw-rw-  2.0 fat     7077 b- defN 23-Jul-11 06:04 cmsis_stream/cg/scheduler/config.py
 -rw-rw-rw-  2.0 fat    41853 b- defN 23-Jun-09 07:44 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat    10849 b- defN 23-Jun-09 12:50 cmsis_stream/cg/scheduler/graphviz.py
 -rw-rw-rw-  2.0 fat    38334 b- defN 23-Jul-11 12:02 cmsis_stream/cg/scheduler/node.py
--rw-rw-rw-  2.0 fat     1864 b- defN 23-Jul-11 05:59 cmsis_stream/cg/scheduler/pythoncode.py
+-rw-rw-rw-  2.0 fat     1868 b- defN 23-Jul-18 10:59 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     7540 b- defN 23-Jul-11 06:29 cmsis_stream/cg/scheduler/standard.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
 -rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
 -rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/example/main_board.c
 -rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/example/run.bat
--rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple.cproject.yml
+-rw-rw-rw-  2.0 fat      598 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/simple.cproject.yml
 -rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 -rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
 -rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
 -rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
--rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/vht.clayer.yml
--rw-rw-rw-  2.0 fat    16762 b- defN 23-Jul-11 12:57 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jul-11 12:57 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat      878 b- defN 23-Jul-20 11:15 cmsis_stream/cg/scheduler/example/vht.clayer.yml
+-rw-rw-rw-  2.0 fat    17428 b- defN 23-Jul-20 12:22 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jul-20 12:22 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      434 b- defN 23-Jun-12 07:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
--rw-rw-rw-  2.0 fat     1584 b- defN 23-Jul-11 06:54 cmsis_stream/cg/scheduler/templates/code.h
--rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
+-rw-rw-rw-  2.0 fat     1587 b- defN 23-Jul-19 09:23 cmsis_stream/cg/scheduler/templates/code.h
+-rw-rw-rw-  2.0 fat     2202 b- defN 23-Jul-19 09:25 cmsis_stream/cg/scheduler/templates/code.py
 -rw-rw-rw-  2.0 fat     3316 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
--rw-rw-rw-  2.0 fat     5659 b- defN 23-Jul-11 06:54 cmsis_stream/cg/scheduler/templates/commonc.cpp
+-rw-rw-rw-  2.0 fat     5662 b- defN 23-Jul-19 09:25 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1427 b- defN 23-Jun-12 05:39 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     7826 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/dot_template.dot
 -rw-rw-rw-  2.0 fat     7555 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4416 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6473 b- defN 23-Jul-11 12:57 cmsis_stream-1.5.1.dist-info/RECORD
-67 files, 246863 bytes uncompressed, 70696 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-17 05:58 cmsis_stream/cg/sds/__init__.py
+-rw-rw-rw-  2.0 fat     3923 b- defN 23-Jul-18 08:03 cmsis_stream/cg/sds/sds_nodes.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4779 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6648 b- defN 23-Jul-20 12:22 cmsis_stream-1.6.0.dist-info/RECORD
+69 files, 252056 bytes uncompressed, 72439 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -177,26 +177,32 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/LICENSE.txt
+Filename: cmsis_stream/cg/sds/__init__.py
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/METADATA
+Filename: cmsis_stream/cg/sds/sds_nodes.py
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/WHEEL
+Filename: cmsis_stream-1.6.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/entry_points.txt
+Filename: cmsis_stream-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/top_level.txt
+Filename: cmsis_stream-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.5.1.dist-info/RECORD
+Filename: cmsis_stream-1.6.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: cmsis_stream-1.6.0.dist-info/top_level.txt
+Comment: 
+
+Filename: cmsis_stream-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/pythoncode.py

```diff
@@ -36,15 +36,15 @@
        trim_blocks=True
     )
     
     template = env.get_template("code.py")
 
     cfile=os.path.join(directory,"%s.py" % config.schedulerPythonFileName)
 
-    if config.identification:
+    if config.nodeIdentification:
        config.heapAllocation = True
 
     with open(cfile,"w") as f:
          nbFifos = len(sched._graph._allFIFOs)
          print(template.render(fifos=sched._graph._allFIFOs,
             nbFifos=nbFifos,
             nodes=sched.nodes,
```

## cmsis_stream/cg/scheduler/example/simple.cproject.yml

```diff
@@ -7,19 +7,19 @@
 
   add-path:
     - .
        
   components:
     - component: ARM::CMSIS:RTOS2:Keil RTX5&Source@5.5.4 
     - component: Keil::Compiler&ARM Compiler:Event Recorder&Semihosting@1.5.1
-      for-type: 
+      for-context: 
           - .CommandLine
     - component: Keil::Compiler&ARM Compiler:Event Recorder&DAP@1.5.1
-      for-type: 
+      for-context: 
           - .IDE
     - component: Keil::Compiler&ARM Compiler:I/O:STDOUT&EVR
-      for-type: 
+      for-context: 
           - .IDE
   
   layers:
     - layer: vht.clayer.yml
```

## cmsis_stream/cg/scheduler/example/vht.clayer.yml

```diff
@@ -1,30 +1,30 @@
 layer:  
   # name: VHT
   description: Boot code for Virtual Hardware
 
   components:
     - component: ARM::CMSIS:CORE
     - component: Device:Startup&C Startup
-      not-for-type: 
+      not-for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
     - component: ARM::Device:Definition
-      for-type: 
+      for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
     - component: ARM::Device:Startup&Baremetal
-      for-type: 
+      for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
     - component: ARM::Native Driver:Timeout
-      for-type: 
+      for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
     - component: ARM::Native Driver:SysCounter
-      for-type: 
+      for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
     - component: ARM::Native Driver:SysTimer
-      for-type: 
+      for-context: 
         - +VHT-Corstone-300 
         - +VHT-Corstone-310
```

## cmsis_stream/cg/scheduler/templates/GenericNodes.h

```diff
@@ -65,17 +65,25 @@
 #endif
 
 template<typename T>
 class FIFOBase{
 public:
     virtual T* getWriteBuffer(int nb)=0;
     virtual T* getReadBuffer(int nb)=0;
+    /*
+
+    Below functions are only useful in asynchronous mode.
+    Synchronous implementation can provide an empty
+    implementation.
+
+    */
     virtual bool willUnderflowWith(int nb) const = 0;
     virtual bool willOverflowWith(int nb) const = 0;
     virtual int nbSamplesInFIFO() const = 0;
+    virtual int nbOfFreeSamplesInFIFO() const = 0;
 
 };
 
 template<typename T, int length, int isArray=0, int isAsync = 0>
 class FIFO;
 
 /* Real FIFO, Synchronous */
@@ -85,18 +93,25 @@
     public:
         FIFO(T *buffer,int delay=0):mBuffer(buffer),readPos(0),writePos(delay) {};
         
         /* Constructor used for memory sharing optimization.
            The buffer is a shared memory wrapper */
         FIFO(void *buffer,int delay=0):mBuffer((T*)buffer),readPos(0),writePos(delay) {};
 
-        /* Not used in synchronous mode */
-        bool willUnderflowWith(int nb) const final {(void)nb;return false;};
-        bool willOverflowWith(int nb) const final {(void)nb;return false;};
-        int nbSamplesInFIFO() const final {return 0;};
+        bool willUnderflowWith(int nb) const final
+        {
+            return((writePos - readPos - nb)<0);
+        }
+
+        bool willOverflowWith(int nb) const final
+        {
+            return((writePos - readPos + nb)>length);
+        }
+        int nbSamplesInFIFO() const final {return (writePos - readPos);};
+        int nbOfFreeSamplesInFIFO() const final {return (length - writePos + readPos);};
 
         T * getWriteBuffer(int nb) final
         {
             
             T *ret;
             if (readPos > 0)
             {
@@ -142,32 +157,42 @@
             }
             std::cout << std::endl;
             std::cout << std::endl;
         }
         #endif
 
     protected:
-        T *mBuffer;
+        T * const mBuffer;
         int readPos,writePos;
 };
 
 /* Buffer, Synchronous */
 template<typename T, int length>
 class FIFO<T,length,1,0>: public FIFOBase<T> 
 {
     public:
-        FIFO(T *buffer,int delay=0):mBuffer(buffer),readPos(0),writePos(delay) {};
-        FIFO(void *buffer,int delay=0):mBuffer((T*)buffer),readPos(0),writePos(delay) {};
+        /* No delay argument for this version of the FIFO.
+           This version will not be generated when there is a delay
+        */
+        FIFO(T *buffer):mBuffer(buffer) {};
+        FIFO(void *buffer):mBuffer((T*)buffer) {};
 
-        /* Not used in synchronous mode */
+        /* 
+           Not used in synchronous mode 
+           and this version of the FIFO is
+           never used in asynchronous mode 
+           so empty functions are provided.
+        */
         bool willUnderflowWith(int nb) const final {(void)nb;return false;};
         bool willOverflowWith(int nb) const final {(void)nb;return false;};
-        int nbSamplesInFIFO() const final {return 0;};
+        int nbSamplesInFIFO() const final {return(0);};
+        int nbOfFreeSamplesInFIFO() const final {return( 0);};
 
-        T * getWriteBuffer(int nb) final
+
+        T* getWriteBuffer(int nb) final
         {
             (void)nb;
             return(mBuffer);
         };
 
         T* getReadBuffer(int nb) final
         {
@@ -192,25 +217,24 @@
             }
             std::cout << std::endl;
             std::cout << std::endl;
         }
         #endif
 
     protected:
-        T *mBuffer;
-        int readPos,writePos;
+        T * const mBuffer;
 };
 
 /* Real FIFO, Asynchronous */
 template<typename T, int length>
 class FIFO<T,length,0,1>: public FIFOBase<T> 
 {
     public:
-        FIFO(T *buffer,int delay=0):mBuffer(buffer),readPos(0),writePos(delay),nbSamples(delay) {};
-        FIFO(void *buffer,int delay=0):mBuffer((T*)buffer),readPos(0),writePos(delay),nbSamples(delay) {};
+        FIFO(T *buffer,int delay=0):mBuffer(buffer),readPos(0),writePos(delay) {};
+        FIFO(void *buffer,int delay=0):mBuffer((T*)buffer),readPos(0),writePos(delay) {};
 
         /* 
 
         Check for overflow must have been done
         before using this function 
         
         */
@@ -223,51 +247,51 @@
                 memcpy((void*)mBuffer,(void*)(mBuffer+readPos),(writePos-readPos)*sizeof(T));
                 writePos -= readPos;
                 readPos = 0;
             }
             
             ret = mBuffer + writePos;
             writePos += nb; 
-            nbSamples += nb;
             return(ret);
         };
 
         /* 
         
         Check for undeflow must have been done
         before using this function 
         
         */
         T* getReadBuffer(int nb) final
         {
            
             T *ret = mBuffer + readPos;
             readPos += nb;
-            nbSamples -= nb;
             return(ret);
         }
 
         bool willUnderflowWith(int nb) const final
         {
-            return((nbSamples - nb)<0);
+            return((writePos - readPos - nb)<0);
         }
 
         bool willOverflowWith(int nb) const final
         {
-            return((nbSamples + nb)>length);
+            return((writePos - readPos + nb)>length);
         }
 
-        int nbSamplesInFIFO() const final {return nbSamples;};
+        int nbSamplesInFIFO() const final {return (writePos - readPos);};
+        int nbOfFreeSamplesInFIFO() const final {return (length - writePos + readPos);};
+
 
         #ifdef DEBUGSCHED
         void dump()
         {
             int nb=0;
             std::cout << std::endl;
-            std::cout << "FIFO nb samples = " << nbSamples << std::endl;
+            std::cout << "FIFO nb samples = " << (writePos - readPos) << std::endl;
             for(int i=0; i < length ; i++)
             {
                 std::cout << (typename Debug<T>::type)mBuffer[i] << " ";
                 nb++;
                 if (nb == 10)
                 {
                     nb=0;
@@ -276,28 +300,27 @@
             }
             std::cout << std::endl;
             std::cout << std::endl;
         }
         #endif
 
     protected:
-        T *mBuffer;
+        T * const mBuffer;
         int readPos,writePos;
-        int nbSamples;
 };
 
 // GENERIC NODES 
 
 class NodeBase
 {
 public:
     virtual int run()=0;
     virtual int prepareForRunning()=0;
     void setID(int id){mNodeID = id;};
-    int nodeID(){return(mNodeID);};
+    int nodeID() const {return(mNodeID);};
 protected:
     int mNodeID = UNIDENTIFIED_NODE;
 };
 
 template<typename IN, int inputSize,typename OUT, int outputSize>
 class GenericNode:public NodeBase
 {
```

## cmsis_stream/cg/scheduler/templates/code.h

```diff
@@ -1,13 +1,13 @@
 /*
 
-Generated with CMSIS-DSP Compute Graph Scripts.
-The generated code is not covered by CMSIS-DSP license.
+Generated with CMSIS-Stream python scripts.
+The generated code is not covered by CMSIS-Stream license.
 
-The support classes and code is covered by CMSIS-DSP license.
+The support classes and code are covered by CMSIS-Stream license.
 
 */
 
 #ifndef _{{config.schedulerCFileName |replace(".h","")|upper()}}_H_ 
 #define _{{config.schedulerCFileName |replace(".h","")|upper()}}_H_
 
 {% macro optionalargs(first) -%}
```

## cmsis_stream/cg/scheduler/templates/code.py

```diff
@@ -1,12 +1,12 @@
 #
-# Generated with CMSIS-DSP Compute Graph Scripts.
-# The generated code is not covered by CMSIS-DSP license.
+# Generated with CMSIS-Stream python scripts.
+# The generated code is not covered by CMSIS-Stream license.
 # 
-# The support classes and code is covered by CMSIS-DSP license.
+# The support classes and code are covered by CMSIS-Stream license.
 #
 
 import sys
 
 
 import numpy as np
 import cmsisdsp as dsp
```

## cmsis_stream/cg/scheduler/templates/commonc.cpp

```diff
@@ -1,13 +1,13 @@
 /*
 
-Generated with CMSIS-DSP Compute Graph Scripts.
-The generated code is not covered by CMSIS-DSP license.
+Generated with CMSIS-Stream python scripts.
+The generated code is not covered by CMSIS-Stream license.
 
-The support classes and code is covered by CMSIS-DSP license.
+The support classes and code are covered by CMSIS-Stream license.
 
 */
 
 {% if config.dumpFIFO %}
 #define DEBUGSCHED 1
 {% endif %}
```

## Comparing `cmsis_stream-1.5.1.dist-info/LICENSE.txt` & `cmsis_stream-1.6.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.5.1.dist-info/METADATA` & `cmsis_stream-1.6.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.5.1
+Version: 1.6.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -24,31 +24,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: networkx (>=3.0)
 Requires-Dist: jinja2 (<4.0,>=3.1.2)
 Requires-Dist: sympy (>=1.7.1)
 Requires-Dist: MarkupSafe (<3.0,>=2.1.2)
 Requires-Dist: numpy
+Requires-Dist: PyYAML (>=6.0)
 
 # README
 
 This is a Python package for the Arm open source [CMSIS-Stream library](https://github.com/ARM-software/CMSIS-Stream).
 
 You can install it with:
 
 `pip install cmsis-stream`
 
 Then you can follow the [documentation](https://github.com/ARM-software/CMSIS-Stream) to learn how to:
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
-* Generate a C scheduler to run the graph on your target
+* Generate at build time a static C scheduler to run the graph on your target (no need of an RTOS)
 
 # Change history
 
+## Version 1.6.0:
+
+* SDS sensor and recorder nodes to interact with the [Arm SDS Framework](https://github.com/ARM-software/SDS-Framework/tree/main) to record stream of samples and replay them in Arm Virtual Hardware
+* YAML import / export of a graph and its code generation settings
+
 ## Version 1.5.1:
 
 * Wrong `GenericNodes.h` was included in version 1.5.0
 * 1.5.0 is no more available for download and has been replaced by 1.5.1 correction
 
 ## Version 1.5.0:
```

## Comparing `cmsis_stream-1.5.1.dist-info/RECORD` & `cmsis_stream-1.6.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -26,42 +26,44 @@
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=NBv9eqec1TdyhRcn2-ZwBb7sVeIc4SwmS5rOStt0HoY,3762
 cmsis_stream/cg/scheduler/config.py,sha256=SOSgp7rDFccmVEjikyodwUczN9hfdeJAKFQnTmu6E_w,7077
 cmsis_stream/cg/scheduler/description.py,sha256=FPLRFTxk3mGduq2_hLPxNiL5MNzpFDzl-Nk1ivyyBVk,41853
 cmsis_stream/cg/scheduler/graphviz.py,sha256=TwiDslHOJlek2otwA_5sspTWaf_trLV4QMthpv6fzM4,10849
 cmsis_stream/cg/scheduler/node.py,sha256=b_tO27sp1gphHM710mwRrHsOW8aezwxzJHDY_cSsR3s,38334
-cmsis_stream/cg/scheduler/pythoncode.py,sha256=48KAT64uzM5z8S2QoqkZPZLCUnk3TpOIPjhUGEbnyA4,1864
+cmsis_stream/cg/scheduler/pythoncode.py,sha256=A5iuUMvzgDJCe7uNyeuhtZA0wZfc4PeSeDXDymeCaKc,1868
 cmsis_stream/cg/scheduler/standard.py,sha256=LFenG7Da-TBzzp_Pl2BKAzJj3li9WFLNOJF4xwnkoY4,7540
 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
 cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
 cmsis_stream/cg/scheduler/example/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
 cmsis_stream/cg/scheduler/example/README.md,sha256=_o0nMzYUELDms9o9Gh__4fuOTYqUAwabijVBSHkqsiA,566
 cmsis_stream/cg/scheduler/example/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
 cmsis_stream/cg/scheduler/example/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
-cmsis_stream/cg/scheduler/example/simple.cproject.yml,sha256=1Zpzt5Ebl30KDJ-5nh_9Ypg-igqrPiA_ek_2kGAJGzc,589
+cmsis_stream/cg/scheduler/example/simple.cproject.yml,sha256=fFDUn3xWbqpvstxwcIXLAP7UFc7QrSK7-a383ZsJyZM,598
 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
 cmsis_stream/cg/scheduler/example/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
 cmsis_stream/cg/scheduler/example/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
 cmsis_stream/cg/scheduler/example/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
 cmsis_stream/cg/scheduler/example/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
-cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
-cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=pkPmC15O_GVKo3ALdra6txsRmfEOG6KG99bBDrzEe4Y,16762
+cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=BOZ44mIcb3P2r43vAyff5QkI8r75I5HIzwLOBqcyu2g,878
+cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=sgw6-HeFS0l6G5IVLBhbCmpHHWPWL3HjbrYEKj0oxuI,17428
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=Fw5MHQqCZt2srXAuJjvXSHS1m-78DGdT4sGHDEQgG28,434
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=iC5sSkuZ01iGT0dBfqNPUbMKE86y10-0Gj8fLOfbgi8,287
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=JMn_nIJiPYSnu7qVKHS8jKEtAjktGpWSyzxg-r2olgw,682
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
-cmsis_stream/cg/scheduler/templates/code.h,sha256=EL-F5iS31gGrFK7WMi5bxWThZyALgmovpqVbOkLMNVw,1584
-cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
+cmsis_stream/cg/scheduler/templates/code.h,sha256=aYlk0BrpUYIRaMkhP7Whujfvijza_Z-H1dYrzcmsYFk,1587
+cmsis_stream/cg/scheduler/templates/code.py,sha256=K77zYiYQdqMGynPVABcWNmxqdGFx9cMfV1yOvuc4u8M,2202
 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=QoQiLGGb_AUbeTE2LyaOneAkkfccxl4Ah-K-AbVoh-M,3316
-cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=r0lKbtH4QL_fhdX43iLeU5nqHA8FkuoCnq7vywtTsR4,5659
+cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=AwlzR5yhV4geF5FjDYmXHWLmiqMI7aWZ2sLBbH3_Gzo,5662
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=KoW0i45XF2-Ghcs-snyqlyysT0SfcKVJcStrBotO1gE,1427
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=_4a8oe0kvSDx-Hl1P0aIZMFAOYMpknhGkeOUI8Nqy6g,7826
 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot,sha256=wLfhZpZS0VHm43dpaQYZBSd8ftd0KdUS_hSo2cSHwLU,7555
-cmsis_stream-1.5.1.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.5.1.dist-info/METADATA,sha256=UFDXQ5w1MhWA0feBeFAM-xG_Fh5uNDCXFU3qEqtdg8M,4416
-cmsis_stream-1.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.5.1.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.5.1.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.5.1.dist-info/RECORD,,
+cmsis_stream/cg/sds/__init__.py,sha256=TCh0rypl6S4qKWie66n0ZGYaUGznTLIWOFl_1-2XvLE,26
+cmsis_stream/cg/sds/sds_nodes.py,sha256=NiOBo0gIGYdb9Am0RyFvivrQbDJKpnvMHl4iOZ7zDbc,3923
+cmsis_stream-1.6.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.6.0.dist-info/METADATA,sha256=SbjYldA1UR6r3bu3p6vutu6ROTacUm3MQ3fk3TXogu0,4779
+cmsis_stream-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.6.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.6.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.6.0.dist-info/RECORD,,
```

