---
permalink: overview_geods.html
layout: default

title: Oliot Discovery Service Documentation
---

Oliot Discovery Service (Oliot-DS)
==================================

Oliot-ds is an implementation of EPCglobal Discovery Service. It provides the service to find the physical locations of desired GS1 ID embedded products inner distance radius from current location. If the user gives GS1 ID, time period, and size of distance radius to Oliot-ds, it shows the markers corresponding the physical locations of the products on the google maps satisfying the given conditions.  The architecture of Oliot-ds is as follows.

![img6](images/ds-pics/oliot-ds-img1.png)

Firstly, events captured from things are registered to Oliot-ds through EPCISs. Then, the client gets the address of Oliot-ds from ONS. By using the address receiving from ONS, it queries the physical locations of products embedding the given GS1 ID to Oliot-ds. Finally, Oliot-ds gives the desired information to the client and the browser shows the physical locations on the google maps.


[![thumbnail](images/viewon.png)][repo_url]  
[repo_url]: https://github.com/gs1oliot/oliot-geods