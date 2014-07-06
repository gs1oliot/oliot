---
permalink: overview_llrp.html
layout: default

title: Oliot LLRP Documentation
---


Oliot LLRP (ELFIN) Overview
===========================

Oliot-LLRP is an implementation of EPCglobal Low Level Reader Protocol (LLRP).  

![llrp-img-5](images/llrp-pics/llrp-pic5.png) 

LLRP is a protocol between ALE Server and RFID Reader which,

 * defines control of RFID readers up to low level details of RFID  
 * defines inventory, read, write, and other access commands for tags  
 * defines capabilities of reader device  
 * defines status reporting and error handling  

![llrp-img-1](images/llrp-pics/llrp-pic1.png)  

ELFIN is abbreviation of Enhanced LLRP-enabling Framework for the INternet of things, and is implementation of LLRP standard with some extentions. ELFIN is composed of following components

![llrp-img-3](images/llrp-pics/llrp-pic3.png)  

 * Core Operational Component
   * Core operations of LLRP and other supplementary operations
 * Structural Abstraction Component
   * Abstracts the structure of the real-world reader
   * Useful for extension of current LLRP standard
 * Communicational Abstraction Component
   * Abstracts the communication with the real-world reader
   * Useful for supporting various kinds of Tag Readers
 * Messaging Component
   * Abstracts LLRP messaging between reader and ALE server

ELFIN is able to support adaptation of various kinds of connectivity and protocols. So if a thing has its own unique GS1 code, it can be collected by ELFIN reader with some adaptation and utilized within EPCglobal framework.

![llrp-img-4](images/llrp-pics/llrp-pic4.png)  


[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-llrp