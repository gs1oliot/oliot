---
permalink: overview_oliot.html
layout: default

title: Oliot Documentation
---
<head>
  <link rel="stylesheet" href="stylesheets/styles.css">
  <link rel="stylesheet" href="stylesheets/pygment_trac.css">
</head> 
  
# Oliot Project
{:.no_toc}
 
* TOC HERE
{:toc}

## About Oliot

![current-sit](images/oliot.png)

**Oliot** is aiming an international standard based **Internet of Things (IoT) Infrastructure Platform**, by extending the code system of GS1 and their standard architecture to support various IoT connectivity and protocols such as bar code, 2D DataMatrix, QR Code, RFID, ZigBee, 6Lo, Bluetooth Low Energy, OneM2M, OCF, etc. Oliot also aims a complete implementation of GS1/EPCglobal standard.

The name of this project, *Oliot* is the abbreviation of *Open Language for Internet of Things*. Also, *oliot* is the plural form of *olio*, which means *thing* or *object* in Finnish, and means stew of various meats and vegetables in Spanish.


## GS1 and Auto-ID Labs
![AutoIDLab](images/Auto-IDLabsLogo.png)  ![GS1](images/gs1-epcglobal.png)  
The term **Internet of Things** was firstly introduced in 1999 by Kevin Ashton at the Auto-ID Labs, MIT (http://www.autoidlabs.org), which is the primary research partner of GS1.

GS1 provides various types of codes such as bar code, RFID, 2D DataMatrix code for thing identification, and standardizing system infrastructure for global business and applications (Transport & Logistics, Retail, Healthcare, Fresh Food, Technical Industry, Financial Service, etc.).

GS1 is making an effort to hold the position of a standard technology for IoT era as well as B2C from B2B via GS1 code extension, GS1 digital, and IoT standard technology development.

Among seven Auto-ID Labs (MIT, Cambridge, ETH Zurich, Keio, Fudan, Adelaide, KAIST) over the world, Auto-ID Labs, KAIST started research and development in IoT field since 2003, starting from the RFID and wireless sensor network technology. And since 2005, we started to develop various IoT technologies that are specialized to GS1 standard.

## History of Oliot Project
 * Oliot 1.2
   * Oliot EPCIS v1.2: the web-service complying with EPCIS v1.2
   * ONS management WebApp

 * Oliot 1.1
   * **Oliot EPCIS v1.1: the web-service complying with EPCIS v1.1 (Clean-slate implementation)**
   * Multi-backend: MongoDB (open), MySQL & MariaDB backend (Developed) and Cassandra (TBD)
   * Multi-service interface: SOAP, REST and Message Queue

 * Oliot 1.0
   * **Complete implementation of latest GS1 EPCglobal framework**
   * Run on any clouds that supports mysql and cassandra.

 * Pre-Oliot Projects
   * GS1 EPCglobal Network on the Cloud for Groceries Trace Framework, since 2013
     * **Complete Implementation of latest GS1 EPCglobal framework**
     * EPCIS Enhanced with NOSQL DB
     * Cloud Support
     * Oliot LLRP Server implemented
     * Geo-discovery Service
     * ONS 2.0.1 implemented

   * Smart Thing Information Service (STIS), since 2011 to 2014
     * Integrate 6Lo/CoAP/Obix protocol to middleware (without LLRP adaptation)

   * EPC Sensor Network (EPCSN), since 2005 to 2011
     * Expand GS1 EPCglobal Network to integrate various sensor network protocols
     * Adaptation of Zigbee and 6Lo to LLRP protocol
     * Complex Event Processing, etc.



## List of Subprojects
 * Oliot EPCIS v1.2 ([Link](https://github.com/JaewookByun/epcis))
 * Oliot ONS ([Link](https://github.com/gs1oliot/oliot-ons-1.1))
 * Oliot GS1 Source ([Link](https://github.com/gs1oliot/gs1source))
 * Oliot DS ([Link](https://github.com/gs1oliot/oliot-ds-1.1))
 * Oliot ALE ([Link](https://github.com/gs1oliot/oliot-fc))
 * Oliot LLRP Reader ([Link](https://github.com/gs1oliot/oliot-llrp))

## Credits
![AutoIDLab](images/Auto-IDLabsLogo.png)  ![KAIST](images/kaist.png)  
Oliot is maintained by Auto-ID Labs, KAIST, in Daejeon, Korea.
Related works of this project were funded or aided by following organizations.

 * GS1 Food Safety Project
   * Institute for Information & communications Technology Promotion(IITP) funded by the Korea government(MSIP), 2015-2017
   * Implementing Food Safety System based on the Oliot Project
 * C-ITRC Project
   * MSIT(Ministry of Science and ICT), Korea, under the ITRC(Information Technology Research Center) support program, 2013-
 * Wise-IoT
   * Institute for Information & communications Technology Promotion(IITP) grant funded by the Korea government(MSIP), 2016-
   * [http://wise-iot.eu/](http://wise-iot.eu/)
 * IoF2020 (Internet of Food and Farm 2020)
   * National Research Foundation of Korea (http://nrf.re.kr) National Research Lab, 2016-
   * [https://www.iof2020.eu/](https://www.iof2020.eu/)
 * KMIT
   * Korean company working together for Oliot enterprise service
   * [http://www.kmit.or.kr](http://www.kmit.or.kr)

## License
Oliot is distributed under [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
For ONS, we open it with Apache license so that users can use it without any restriction. That is because Oliot-ONS consists of the DNS configuration files to implement ONS.


## Supplementary Materials and Slides
 * The Road to Internet of Things

>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_the_road_to_internet_of_things.jpg)](http://www.slideshare.net/gatordkim/the-road-to-internet-of-things)

 * GS1 EPCglobal framework and Oliot Project Overview
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_epcglobal_framework_and_oliot_project_overview.jpg)](http://www.slideshare.net/gatordkim/gs1-epcglobal-framework-and-oliot-project-overview-oliot-workshop-2014)

 * GS1 Source
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_source.jpg)](http://www.slideshare.net/gatordkim/gs1-source)

 * GS1 Digital
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_gs1_digital.jpg)](http://www.slideshare.net/gatordkim/gs1-digital)

 * Oliot LLRP
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_llrp.jpg)](http://www.slideshare.net/gatordkim/gs1oliot-llrp)

 * Oliot ALE and Next
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_ale.jpg)](http://www.slideshare.net/gatordkim/gs1oliot-ale-and-next)

 * Oliot EPCIS and Next
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_epcis.jpg)](http://www.slideshare.net/gatordkim/gs1oliot-epcis-and-next)

 * Oliot ONS/DS and Next
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_ons_ds.jpg)](http://www.slideshare.net/gatordkim/gs1oliot-onsds-and-next)

 * Oliot Open Source Project
 
>>> [![thumbnail](http://gs1oliot.github.io/oliot/images/slide_summary/sum_oliot_open_source_project.jpg)](http://www.slideshare.net/gatordkim/oliot-open-source-project)

 * Oliot Facebook Group ([Link](https://www.facebook.com/groups/oliot/))



