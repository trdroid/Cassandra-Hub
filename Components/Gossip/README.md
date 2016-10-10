# Gossip

Cassandra uses the *gossip* protocol for internode communication to determine the

* state &
* location

of other nodes in the ring.

**The requirement**

The requirement is for the nodes in a ring/cluster to determine the overall map of the cluster (i.e. the location of other nodes) with 
as less number of local interactions as possible.

**Class**

The *gossip* task is handled by the class *org.apache.cassandra.gms.Gossiper*. 
