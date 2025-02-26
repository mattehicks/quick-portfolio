## Infrastructure: applications and services.

**Project description:** I have worked as a software engineer on numerous projects requiring overall system design, architecting cloud services for a myriad of industries, also writing big-data applications which have tons of variation in how the data is delivered, presented, and memory constraints.  Here is a few projects that were worth delving into:


### 1. Events based services and data flow.
Working with a leader in the SATCOM and communication networks sector, I was tasked with designing and building a platform for a bevy of high-priority clients.
The end goal to create a CMS and network mangagement platform, that could:
Interface with various components from multiple vendors, 
Having a custom built set of drivers that can interface via udp and control 'Systems of Systems' and be a 'Manager of Managers'
Has a collection of backend routines that can handle realtime telemmetry feeds, 
Has an interface with "command and control" capabilities for JAD2C elements and battlefield planning. 
Able to detect network outages and health, and respond in an automated way, to migrate networks between nodes and use the appropriate hardware.

As a matter of security, we utilized COTS libraries and Java/JS packages.  The stack also consisting of frameworks and components related to: 
GRPC, Subscribers, Sockets, realtime maps, live video feed components, CMS and Entity management, RF analysis tools, reporting tools, health and monitoring, hardware drivers, etc.
Thus, allowing us to innovate and design custom components across a number of areas.
The result was; a successful demos and field tests, and mulitiple contract extensions.
 
 ```
Wildfly
Java
Python
Kafka Messaging
Event hub / message queue
3rd party integration
```

<img class='feature' src="images/candc.png?raw=true"/>
<br>
---


### 2. Consumer facing, high volume microservices on AWS.

As a fullstack engineer on a project with incoming messages on order of 10k+ per min.  All components needed to be auto-scaling to handle traffic during peak hours, and be fault-tolerant.  
Java handles the heavy lifting; after the kinesis event stream is split into a database of event logs and a NoSQL store for current device state.  
The modular cloud components are easy to deploy, and services are trivial to stop/start, and CloudWatch was an essential component to catch any failures, and create audits of daily activity. 
A local kinesis build was included in the CI/CD paradigm for faster development.  
The infrastructure rollout looks like this:

```
API Gateway
Kinesis streams
Redshift
Internal API
PostgreSQL Warehouse
```

<img class='feature'  src="images/jacloud.jpg?raw=true"/>

<br>
---

### 3. Big-data and stream processing architectures and workflows.
A bulk-analytics system, as contracted by a government/healthcare association.  Its purpose is to run analytics agents against the claims data-warehouse, in order to detect fraud, descrepancies, and a myriad of other causes of invalid accounting.  This architecture is built with open-source in-mind, using Hive, Spark, SOLR in-memory store, and Java to create large sets of data that could be read from memory, and processed in the period of only a few hours.
Using the knowledge gained from this project, we would eventually expand the functionality into a more comprehensive solution for enterprise analytics.  These modules were enhanced to handle a greater number of data schemas, were modularized for independant deployment, ie; dockerized, and would communicate via a Kinesis central event/message hub.  A widely accredited product and achievement. 
Overview:
 
 ```
Spark
Hive
SOLR
Java
Kinesis Streams
Confluent/Open-source
```

<img class='feature' src="images/humid.jpg?raw=true"/>
<br>

 <img class='feature' src="images/frontend2.jpg?raw=true"/>
 
 
 <style>
.feature{
    border: 1px solid silver !important;
}
</style>
