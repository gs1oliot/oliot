---
permalink: overview_geods.html
layout: default

title: Oliot Discovery Service Documentation
---

Oliot DS (Discovery Service)
==================================

Oliot DS is an implementation of EPCglobal Discovery Service. It provides the service to find the physical locations of desired GS1 ID embedded products inner distance radius from current location. If the user gives GS1 ID, time period, and size of distance radius to Oliot DS, it shows the markers corresponding the physical locations of the products on the google maps satisfying the given conditions.  The architecture of Oliot DS is as follows.

![img6](images/ds-pics/oliot-ds-img1.png)

Firstly, events captured from things are registered to Oliot DS through EPCISs. Then, the client gets the address of Oliot DS from ONS. By using the address receiving from ONS, it queries the physical locations of products embedding the given GS1 ID to Oliot DS. Finally, Oliot DS gives the desired information to the client and the browser shows the physical locations on the google maps.

## Contributors
 * Kiwoong Kwon, Ph.D student of KAIST

[![thumbnail](images/viewon.png)](https://github.com/gs1oliot/oliot-ds-1.1)
