# Messaging Service

Messaging Service is responsible for managing the internode socket communication in a ring. 
It runs at each node in a ring acting as a gateway messaging server. 
The Messaging Service is represented by the singleton class *org.apache.cassandra.net.MessagingService*.

The Message Service processes the following communications

* read
* write
* gossip
* read digest

**Sockets**

Each node creates two socket connections per node that it communicates with. 

Example

In a Cassandra cluster with 11 nodes, there would be 20 sockets on each node to handle communication with other nodes.

**Messages**

A message contains a *verb* that contains information for the receiving node on

* **Deserialization**: How the payload of the message has to be deserialized
* **Message/Verb Handler**: What handler should be executed for the message



