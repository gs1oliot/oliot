---
permalink: overview_ons.html
layout: default

title: Oliot Object Name Service Documentation
---

Oliot Object Name Service (ONS)
===============================

Object Name Service (ONS) is service look-up system on top of Directory Naming Service (DNS). It is located in higher layer of EPC global architecture [http://www.gs1.org/epcglobal]. Briefly, this service have a responsibility of looking up services related to given Electronic Product Code (EPC) [http://www.gs1.org/docs/epcglobal/an_overview_of_EPC.pdf].  

It should be noted that ONS fully leverages DNS. As a service publisher, you need to add/delete/update service lists related to give EPC as a NAPTR Record form [http://www.ietf.org/rfc/rfc2915.txt], leading clients to obtain them by ordinary DNS query (e.g. Java JNDI [http://tomcat.apache.org/tomcat-7.0-doc/jndi-resources-howto.html]. 

For more information, please refer to ONS 2.0.1 specification [http://www.gs1.org/gsmp/kc/epcglobal/ons/ons_2_0_1-standard-20130131.pdf] 


[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-ons-1.1
