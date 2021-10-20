---
permalink: overview_epcis.html
layout: default

title: Oliot EPCIS Documentation
---

Oliot EPCIS (EPC Information Service)
===========================================
Electronic Product Code Information Service (EPCIS) enables to capture and share visibility event and masterdata depicting lifecycle of everyday-objects. With EPCIS, event producer generates and sends events complying with EPCIS Document XML schema into EPCIS Repository Then, these events can be globally shared with given queries.

Oliot EPCIS is a Java Web Service implementing the EPCIS standard in terms of its data type and interface standards and additionally supports additional features to broaden its scope from RFID to the Internet of Things.


![thumbnail](images/epcis-pics/architecture2.png)

## Specification
 * Java, Dynamic Web Service
 * EPCIS v1.2 compliance
 * Maven and Spring framework
 * Supported backends: MongoDB, Relational DBMSs (MySQL, MariaDB, Oracle, and PostgreSQL)
 * Supported web service interface: SOAP, REST
 * Supported message format: XML, JSON

## Contributors
 * Jaewook Byun, Maintainer  : bjw0829@kaist.ac.kr, bjw0829@gmail.com
 * Yalew Kidane Tolcha, MySQL Backend Extension : yalewkidane@kaist.ac.kr, yalewkidane@gmail.com
 * Sungpil Woo, Capture Interface Extension : woosungpil@kaist.ac.kr, woosungpil7@gmail.com


[![thumbnail](images/viewon.png)](https://github.com/JaewookByun/epcis)
