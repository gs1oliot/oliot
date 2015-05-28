---
permalink: overview_epcis.html
layout: default

title: Oliot EPCIS Documentation
---

Oliot EPC Information Service (Oliot EPCIS)
===========================================
Electronic Product Code Information Service (EPCIS) enables to capture and share EPC-based event ( Basically RFID Tag event ). With EPCIS, event producer (e.g. RFID middleware) generates and sends events complying with EPCIS Document XML schema into EPCIS Repository Then, these events can be globally shared with given queries.

* Specification
 * Java, Dynamic Web Service
 * EPCIS v1.1 compliance
 * Maven and Spring framework
 * Multi-backend: MongoDB (Open), MySQL & MariaDB (Developed) and Cassandra (TDB)
 * Multi-service interface: SOAP, REST and Message Queue


![thumbnail](images/epcis-pics/EPCIS_Architecture.png)

[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-epcis-1.1
