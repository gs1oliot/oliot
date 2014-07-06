---
permalink: overview_cs.html
layout: default

title: Oliot Cloud Development Documentation
---

Oliot Cloud Development
=======================

Oliot-cloudstack is an implementation for running Oliot components on Cloud. Currently, the implementation supports a load predictor and TCP connection migration through SSH commands parsing from client to server. This is currently intended for developers only, as the client has to depend on the management & hypervisor servers’ configurations. Later version may provide an interface for easier client deployment.

The current infrastructure consists of the following components:

![cs-img-3](images/cs-pics/oliot-cloudstack-img3.png)  

 * Load Collector
   * Collects load information from CloudStack hypervisor host.
 * Load Predictor
   * Based on the load information collected, predict the future load values.
 * Migration Manager
   * Handling migration process in case of hotspots predicted by the load predictor.

[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-cloudstack
