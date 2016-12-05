### AIS to DIS Gateway

A simple gateway that translates from AIS to Distributed Interactive Simulation (DIS).

The basic functionality is there, but one could make it much fancier. The broadcast  
address is hardwired in Network.java and should be changed to fit your network. 
The EntityType is set in the Ship constructor. There's a thread to periodically 
send DIS heartbeat messages.

The program connects to an AIS server on a TCP port. The IP and port are
currently hardwired in AISGW.
