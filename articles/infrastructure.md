---
uid: infrastructure
---

# Infrastructure

A user-oriented POV explanation of how the environment is built. First of all, it should be clear what the different stages are; i.e. do we have regression, staging, and/or pre-production DataMiner Agents, besides the production?


Secondly, a high-overview explanation is done to understand:

* How many agents are in the cluster?
  * Where are they hosted (physical server, VMs on same/different server, SAN or SSD, etc.)
* Do we have failover and if so how many agents?
* What is the type of database in use?
  * External or local Cassandra
  * STaaS
  * Indexing engine (OpenSearch or ElasticSearch)
* Where are backups typically stored (locally or network share)?