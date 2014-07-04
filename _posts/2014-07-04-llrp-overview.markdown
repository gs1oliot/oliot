---
permalink: overview_llrp.html
layout: default

title: Oliot LLRP Documentation
---

Oliot LLRP
==========
<!--
CONTENTS
--------
 * [Introduction](#toc_2)
 * [Download & Compilation](#toc_3)
 * [Project Summaries](#toc_4)
 -->
 !TOC
 

INTRODUCTION
------------
Oliot-fc is an implementation of EPCglobal application level events (ALE) interface. It provides APIs for filtering and grouping radio frequency identification (RFID) based data. Clients of Oliot-fc can define filtering and grouping pattern according to EPCglobal ALE interface, and the result is returned back to them.

LLRPReader--+---cxxtest-4.3 (cxxtest framework)  
                                +---libs (pre-built libraries for LLRPReader)  
                                +---LLRP_Reader (Reader impl)  
                                +---LTK (XML2, LTKCPP Library)  
                                +---PR9200_rfid (PR9200 Library)  
                                +---target (build output folder of LLRP Reader and Stubappexample)  
                                +---Tests (cxxtest testsuites)  
 
You can refer Doxygen document in following URL
http://~~URL
DEVELOPER GUIDE
This section is for the developers.
 
DOWNLOAD & COMPILATION
----------------------

1. Install Boost Library
http://www.boost.org/
version: 1.54 or above
 
2. Install build tools as follows.
sudo apt-get install libstdc++6
sudo ldconfig
 
sudo apt-get install build-essential
sudo apt-get install automake
sudo apt-get install autoconf
sudo apt-get install libtool
sudo apt-get install xsltproc
 
3. Use make command according to the arch type you want to build for.
x86_64: make ARCH=x86_64 all
arm-generic-linux-gnueabi: make ARCH=arm all
arm-fsl-linux-gnueabi: make ARCH=armfs all
i386: make ARCH=i386 all
* Because -m32 option was not used for x86_64, x86_64/i386 cannot be built in 32bit/64bit computer.
 
Each build options cannot coexist, so you should ‘make ARCH=(arch_type) clean’ before you run one of above.
 
4. Executables would be generated in the ‘target’ folder. You can run them as follows.
 i) Using LD_LIBRARY_PATH
Set the LD_LIBRARY_PATH environment variable to the path of boost, LTK, xml2, and other generated library files. You can refer to the run.sh in the project root folder.
 
The examples of required library paths for fridge app are follows. If you built it in the machine you would use, then use former one. If you cross-compiled it for arm, then use latter one.
XML2: libxml2.so (ex. ./LTK/opensource/.libs or ./lib/arm)
Boost Library: libboost_***.so (ex. /usr/local/lib or ./lib/arm)
LLRP Wrapper: libllrpreader.so (ex. ./target)
PR9200 API: librfid_pr9200.so (ex. ./target)
 
 ii) Copying library files
Set LD_LIBARY_PATH=./:$LD_LIBRARY_PATH, and copy all required library files and configuration files into ‘target’ directory and run in that directory. All libraries should be exist in the current working directory.
 
5. When you run the executables, you should set the options as follows. You can see options
./stubappexample -c<path-to-reader.cfg> -l<path-to-config.llrp>
 
6. You can change configuration of reader by modifying reader.cfg file in the root folder.
 
PROJECT SUMMARIES
-----------------

 
 
