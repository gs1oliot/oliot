---
permalink: overview_fnc.html
layout: default

title: Oliot F&C Documentation
---

Oliot Application Level Event (Oliot-fc)
========================================

Oliot-fc is an implementation of EPCglobal application level events (ALE) interface which provides APIs for filtering and grouping radio frequency identification (RFID) based data.  
Oliot-fc is forked from the Fosstrak Filtering and Collection project. The objective of this fork is to develop EPCglobal-architecture-based IoT platform under the vision of Auto-ID Lab Korea, KAIST.

![thumbnail](images/ale.png)

In Oliot, oliot-fc is located in the middleware position as shown above. Extending the idea of ALE middleware, we will generalize Oliot-fc middleware role to process stream-based raw data from various devices to generate refined high-level events following GS1 standard. In order to achieve this goal, we are planning to integrate various sensor network protocols (e.g. Zigbee, 6LoWPAN, RESTful device) and other IoT platforms (e.g. MQTT, and AllJoyN). The data from these various devices is abstracted to a concept of stream, for which we will develop stream processing feature. 

In the current stage, we developed Oliot filtering and collection to implement ALE interface fully based on Fosstrak fc project. We compared ours with Fosstrak in the following table. We developed newly 3 APIs: Writing API, Tag Memory API, Access Control API, and developed reader initiated connection feature for IoT use case.

![thumbnail](images/fc-comparison.png)

There are 4 projects in Oliot-fc.  

 * fc-client
   * ALE client program for Oliot-fc. It includes Java Swing based user interface. We added API example class to use Writing, Tag Memory, and Access Control API. Swing-based user interface to use newly implemented features is our future work on this project.
 * fc-commons
   * Oliot-fc common components such as web service components, and serializer/deserializer utilities. We added serializer and deserializer utils for TMSpec API, Writing API. 
 * fc-server
   * A main server project of Oliot-fc. Its role includes processing requests from ALE clients, accepting reader connections, generating reports and so on. We implemented newly supported features in this project. 
 * fc-webclient
   * ALE web based client program for Oliot-fc. The compiled binaries can be embedded to the servlet container Tomcat, and they can be access by web browser. There is no modification on this project, but we will implement web based client for Writing, Tag Memory, and Access Control API as our future work.


[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-fc