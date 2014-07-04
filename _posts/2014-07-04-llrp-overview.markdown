---
permalink: overview_llrp.html
layout: default

title: Oliot LLRP Documentation
---

[repo_url]: https://github.com/gs1oliot/oliot-llrp
Oliot LLRP 
==========
Oliot-fc is an implementation of EPCglobal application level events (ALE) interface. It provides APIs for filtering and grouping radio frequency identification (RFID) based data. Clients of Oliot-fc can define filtering and grouping pattern according to EPCglobal ALE interface, and the result is returned back to them.

LLRPReader--+---cxxtest-4.3 (cxxtest framework)  
                                +---libs (pre-built libraries for LLRPReader)  
                                +---LLRP_Reader (Reader impl)  
                                +---LTK (XML2, LTKCPP Library)  
                                +---PR9200_rfid (PR9200 Library)  
                                +---target (build output folder of LLRP Reader and Stubappexample)  
                                +---Tests (cxxtest testsuites)  


[![thumbnail](images/viewon.png)][repo_url]  