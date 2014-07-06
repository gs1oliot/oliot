---
permalink: overview_cs.html
layout: default

title: Oliot Cloud Development Documentation
---

Oliot Cloud Development
=======================

Oliot-cloudstack is an implementation for running Oliot components on Cloud. Currently, the implementation supports a load predictor and TCP connection migration through SSH commands parsing from client to server. This is currently intended for developers only, as the client has to depend on the management & hypervisor servers’ configurations. Later version may provide an interface for easier client deployment.

The current infrastructure consists of the following components:
* Load Collector
  * Collects load information
* Load Predictor
* Migration Handler

[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-cloudstack
