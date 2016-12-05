### AIS to DIS Gateway

A simple gateway that translates from AIS to Distributed Interactive Simulation (DIS).
AIS is a live ship tracking system: https://en.wikipedia.org/wiki/Automatic_identification_system .
This reads the AIS messages from an AIS TCP/IP server and translates them into 
DIS. 

The basic functionality is there, but one could make it much fancier. The broadcast  
address is hardwired in Network.java and should be changed to fit your network. 
The EntityType is set in the Ship constructor. There's a thread to periodically 
send DIS heartbeat messages. It's sometimes used as a class example to teach
students about what's involved in gatewaying between protocols.

The program connects to an AIS server on a TCP port. The IP and port are
currently hardwired in AISGW.
