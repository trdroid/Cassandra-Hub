### Representation

*Token*

In Cassandra, each row is identified by a row key known as a token which is a number.

*Unique name*

Each cell/column within a row can have its own unique name. The columns in the rows are sorted by the unique cell name. 

*Keyspace*

The number of rows allowed is very large, so the rows are distributed uniformly across all the available machines in a cluster in equal token groups. 
Each token group contains a set of tokens referred to as a *Keyspace*.

**Cluster Representation**

A Cassandra cluster is represented using a ring structure to show token distribution. 





