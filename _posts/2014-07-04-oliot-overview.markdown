---
permalink: overview_oliot.html
layout: default

title: Oliot LLRP Documentation
---
<!--
[English](http://www.google.com) [한국어](http://www.google.com)
-->
GS1/Oliot Project Overview
==========================

<!--
Table of Contents
-----------------
  * [About Oliot](#about-oliot)
  * [GS1 and Auto-ID Labs](#gs1-and-auto-id-labs)
  * [List of Subprojects](#list-of-subprojects)
  * [Mailing Lists](#mailing-lists)
  * [Credits](#credits)
  * [License](#license)
  * [Supplementary Materials](#supplementary-materials)
 -->
!TOC

About Oliot
-----------
![Rome Map](http://gs1oliot.github.io/oliot/images/rome_map.jpg)

**Oliot** is aiming an international standard based **Internet of Things (IoT) Infrastructure Platform**, by extending the code system of GS1 and their standard architecture to support various IoT connectivity and protocols such as bar code, RFID, ZigBee, 6LoWPAN, etc. Oliot  also aims a complete implementation of GS1/EPCglobal standard.

Oliot is a spin-off project of **Fosstrak** (http://fosstrak.org), an open source RFID software platform that implements the GS1 EPC Network specifications. So significant portion of Oliot implementation was derived from that of Fosstrak project.

The name of this project, *Oliot* is the abbreviation of *Open Language for Internet of Things*. Also, *oliot* is the plural form of *olio*, which means *thing* or *object* in Finnish, and means stew of various meats and vegetables in Spanish.


GS1 and Auto-ID Labs
--------------------
![AutoIDLab](images/Auto-IDLabsLogo.png)  ![GS1](images/gs1-epcglobal.png)  
The term **Internet of Things** was firstly introduced in 1999 by Kevin Ashton at the Auto-ID Labs, MIT (http://www.autoidlabs.org), which is the primary research partner of GS1.

GS1 provides various types of codes such as bar code, RFID code, QR code for thing identification, and standardizing system infrastructure for global business and applications (supply chain, food safety, medication, etc.).

GS1 is making an effort to hold the position of a standard technology for IoT era as well as B2C from B2B via GS1 code extension, GS1 digital, and IoT standard technology development.

Among seven Auto-ID Labs (MIT, Cambridge, ETH Zurich, Keio, Fudan, Adelaide, KAIST) over the world, Auto-ID Lab, KAIST started research and development in IoT field since 2002, starting from the RFID and wireless sensor network technology. And since 2005, we started to develop various IoT technologies that are specialized to GS1 standard.

We are currently working on following projects:

 * Oliot (GS1 based IoT Infrastructure Platform)
 * SNAIL (6LoWPAN based IoT Connectivity Platform)
 * SeaHaven (Visual Sensor Network Cloud Platform)
 * IoTMaaS (IoT Mashup Cloud Service Platform)
 * Lilliput (IoT SNS Platform)

History of Oliot Project
------------------------
 * Smart Thing Information Service (STIS), since 2005 to 2011
   * Expand GS1 EPCglobal Network to integrate various sensor network protocols
   * Successor of EPC Sensor Network
   * ZigBee, 6LoWPAN/CoAP/Obix integration
   * Complex Event Processing, etc.

 * GS1 EPCglobal Network on the Cloud for Groceries Trace Framework, since 2013
   * **Complete Implementation of latest GS1 EPCglobal framework**
   * EPCIS Enhanced with NOSQL DB
   * Cloud Support
   * ELFIN: Enhanced LLRP-enabling Framework for the INternet of Things
   * Geo-discovery Service
   * ONS 2.0.1 implemented

 * Oliot 1.0 (Current version)
   * **Complete implementation of latest GS1 EPCglobal framework**
   * Run on any clouds that supports mysql and cassandra.
   * Extended parts of Oliot project compared to Fosstrak is as follows,

![fosstrak-diff](images/fosstrak-diff-table.png)

Oliot Next
---------- 

![current-sit](images/current-sit.png)

We will integrate Oliot with EPCSN and STIS project in the next release. Specifically, for Oliot-fc, we will generalize Oliot-fc middleware role to process stream-based raw data from various devices to generate refined high-level events following GS1 standard. We are planning to integrate various sensor network protocols (e.g. Zigbee, 6LoWPAN, RESTful device) and other IoT platforms (e.g. MQTT, and AllJoyN). The data from these various devices is abstracted to a concept of stream, for which we will develop stream processing feature. For Oliot-epcis, we will implement EPCIS 1.1 standard which was newly released, and we will define master data of various domains such as mobile health care to promote sharing of EPCIS data in IoT context.

Release plan is as follows,

 * **4Q 2014** – Oliot 1.1 (provide EPCIS 1.1, strengthened to support GS1 keys, food industry)
 * **2015** – Oliot 2.0 (support internet of things, merging auto-id lab, KAIST’s Epc sensor network, STIS , MQTT, lwM2M, Alljoyn, and more)

List of Subprojects
-------------------
 * Oliot LLRP Reader ([Link](https://github.com/gs1oliot/oliot-llrp))
 * Oliot F&C (ALE) ([Link](https://github.com/gs1oliot/oliot-fc))
 * Oliot EPCIS ([Link](https://github.com/gs1oliot/oliot-epcis))
 * Oliot ONS ([Link](https://github.com/gs1oliot/oliot-ons))
 * Oliot Cloudstack ([Link](https://github.com/gs1oliot/oliot-cloudstack))


Mailing Lists
-------------
 * Oliot general mailing list
   * oliot@resl.kaist.ac.kr
   * https://groups.google.com/a/resl.kaist.ac.kr/forum/#!forum/oliot
 * LLRP mailing list
   * oliot-llrp@resl.kaist.ac.kr
   * https://groups.google.com/a/resl.kaist.ac.kr/forum/#!forum/oliot-llrp
 * F&C mailing list
   * oliot-fc@resl.kaist.ac.kr
   * https://groups.google.com/a/resl.kaist.ac.kr/forum/#!forum/oliot-fc
 * EPCIS mailing list
   * oliot-epcis@resl.kaist.ac.kr
   * https://groups.google.com/a/resl.kaist.ac.kr/forum/#!forum/oliot-epcis
 * ONS mailing list
   * oliot-ons@resl.kaist.ac.kr
   * https://groups.google.com/a/resl.kaist.ac.kr/forum/#!forum/oliot-ons

Credits
-------
Oliot is developed at Auto-ID Lab, KAIST, in Daejeon, Korea.  
This project is a spin-off project of Fosstrak (http://fosstrak.org).  
Related works of this project were funded by following organizations.

 * EPC Sensor Network (EPCSN)
   * National Research Foundation of Korea (http://nrf.re.kr) National Research Lab, 2005-2011
   * National IT Industry Promotion Agency (http://nipa.kr) Information Technology Research Center (ITRC), 2008-2009
 * Smart Thing Information Service (STIS)
   * EU FP7 IoT6 (http://www.iot6.eu/), 2011-2014
   * National Research Foundation of Korea (http://nrf.re.kr) National Research Lab, 2001-2014
 * GS1 EPCglobal Network on the Cloud for Groceries Trace Framework
   * Samsung (http://samsung.com), 2013-2014
   * Samsung donated part of the project (whole impl. of EPCglobal standard) as open source.


License
-------
Oliot is distributed under [LGPL-2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) license.  
You may copy, distribute and modify the software provided that modifications are described inside the modified files and licensed for free under LGPL-2.1.  Derivatives or non-separate (statically-linked) works of the software must be licensed under LGPL, but separate, parent projects don't have to be.  
(Summary is referenced from [here](https://tldrlegal.com/license/gnu-lesser-general-public-license-v2.1-&#40;lgpl-2.1&#41;))


Supplementary Materials and Slides
----------------------------------
 * The Road to Internet of Things ([Link][roadtoiot_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_the_road_to_internet_of_things.jpg)][roadtoiot_url]
[roadtoiot_url]: http://www.slideshare.net/gatordkim/the-road-to-internet-of-things

 * GS1 EPCglobal framework and Oliot Project Overview ([Link][overview_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_epcglobal_framework_and_oliot_project_overview.jpg)][overview_url]
[overview_url]: http://www.slideshare.net/gatordkim/gs1-epcglobal-framework-and-oliot-project-overview-oliot-workshop-2014

 * GS1 Source ([Link][gs1_source_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_source.jpg)][gs1_source_url]
[gs1_source_url]: http://www.slideshare.net/gatordkim/gs1-source
 * GS1 Digital ([Link][gs1_digital_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_digital.jpg)][gs1_digital_url]
[gs1_digital_url]: http://www.slideshare.net/gatordkim/gs1-digital
 * GS1/Oliot LLRP ([Link][gs1_oliot_llrp_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_llrp.jpg)][gs1_oliot_llrp_url]
[gs1_oliot_llrp_url]: http://www.slideshare.net/gatordkim/gs1oliot-llrp
 * GS1/Oliot ALE and Next ([Link][gs1_oliot_ale_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_ale.jpg)][gs1_oliot_ale_url]
[gs1_oliot_ale_url]: http://www.slideshare.net/gatordkim/gs1oliot-ale-and-next
 * GS1/Oliot EPCIS and Next ([Link][gs1_epcis_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_epcis.jpg)][gs1_epcis_url]
[gs1_epcis_url]: http://www.slideshare.net/gatordkim/gs1oliot-epcis-and-next
 * GS1/Oliot ONS/DS and Next ([Link][onsds_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_ons_ds.jpg)][onsds_url]
[onsds_url]: http://www.slideshare.net/gatordkim/gs1oliot-onsds-and-next
 * Oliot Open Source Project ([Link][oliot_open_source_url])  
[![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_oliot_open_source_project.jpg)][oliot_open_source_url]
[oliot_open_source_url]: http://www.slideshare.net/gatordkim/oliot-open-source-project
 * Oliot Facebook Group ([Link](https://www.facebook.com/groups/oliot/))



