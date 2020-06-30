# Raft-Implementation
### CS3700 - Network - Final Project 
### Distributed, Replicated Key-Value Store
In his project, you will build a (relatively) simple, distributed, replicated key-value datastore. A key-value datastore is a very simple type of database that supports two API calls from clients: put(key, value) and get(key). The former API allows a client application to store a key-value pair in the database, while the latter API allows a client to retrieve a previously stored value by supplying its key. Real-world examples of distributed key-value datastores include memcached, Redis, DynamoDB, etc.

Of course, it would be simple to build a key-value store if it was a single process. However, your system must be replicated and support strong consistency guarantees. Thus, you will be implementing a simplified version of the Raft consensus protocol. Your datastore will be run multiple times, in parallel, and it will use the Raft protocol to maintain consensus among the replicas
