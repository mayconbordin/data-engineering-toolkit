# data-engineering-toolkit

This is a list of **open source** tools and reference architectures for data engineering professionals.

<!--- add comparison table for each category --->

# Reference Architectures


# Ingestion

 - Airbyte
 - Singer
 - [rtdl](https://rtdl.io/) - rtdl is a universal real-time ingestion and pre-processing layer for every data lake that is compatible with AWS, GCP, and Azure. It ingests JSON data, stores in Parquet, and automatically gives you access to your data via Dremio (included). ([Source Code](https://github.com/realtimedatalake/rtdl)) `MIT` `Go/Docker` `Self-Hosted`


# Data Processing

## Batch Processing

## Stream Processing

# Storage

## Databases
### Relational

* [RQLite](https://github.com/rqlite/rqlite) Replicated SQLite using the Raft consensus protocol
* [MySQL](https://www.mysql.com/) The world's most popular open source database.
	* [TiDB](https://github.com/pingcap/tidb) TiDB is a distributed NewSQL database compatible with MySQL protocol
	* [Percona XtraBackup](https://www.percona.com/software/mysql-database/percona-xtrabackup) Percona XtraBackup is a free, open source, complete online backup solution for all versions of Percona Server, MySQL® and MariaDB®
	* [mysql_utils](https://github.com/pinterest/mysql_utils) Pinterest MySQL Management Tools
* [MariaDB](https://mariadb.org/) An enhanced, drop-in replacement for MySQL.
* [PostgreSQL](https://www.postgresql.org/) The world's most advanced open source database.
* [Amazon RDS](https://aws.amazon.com/rds/) Amazon RDS makes it easy to set up, operate, and scale a relational database in the cloud. 
* [Crate.IO](https://crate.io/) Scalable SQL database with the NOSQL goodies.

### Key-Value
* [Redis](https://redis.io/) An open source, BSD licensed, advanced key-value cache and store.
* [Riak](http://docs.basho.com/riak/kv/) A distributed database designed to deliver maximum data availability by distributing data across multiple servers.
* [AWS DynamoDB](https://aws.amazon.com/dynamodb/) A fast and flexible NoSQL database service for all applications that need consistent, single-digit millisecond latency at any scale.
* [HyperDex](https://github.com/rescrv/HyperDex) HyperDex is a scalable, searchable key-value store. Deprecated.
* [SSDB](http://ssdb.io) A high performance NoSQL database supporting many data structures, an alternative to Redis
* [Kyoto Tycoon](https://github.com/alticelabs/kyoto) Kyoto Tycoon is a lightweight network server on top of the Kyoto Cabinet key-value database, built for high-performance and concurrency
* [IonDB](https://github.com/iondbproject/iondb) A key-value store for microcontroller and IoT applications
* [Dragonfly](https://github.com/dragonflydb/dragonfly)

### Column
	* [Cassandra](https://cassandra.apache.org/) The right choice when you need scalability and high availability without compromising performance.
		* [Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/) This simple form allows you to try out different values for your Apache Cassandra cluster and see what the impact is for your application.
		* [CCM](https://github.com/pcmanus/ccm) A script to easily create and destroy an Apache Cassandra cluster on localhost
		* [ScyllaDB](https://github.com/scylladb/scylla) NoSQL data store using the seastar framework, compatible with Apache Cassandra https://www.scylladb.com/
	* [HBase](https://hbase.apache.org/) The Hadoop database, a distributed, scalable, big data store.
	* [AWS Redshift](https://aws.amazon.com/redshift/) A fast, fully managed, petabyte-scale data warehouse that makes it simple and cost-effective to analyze all your data using your existing business intelligence tools.
	* [FiloDB](https://github.com/filodb/FiloDB) Distributed. Columnar. Versioned. Streaming. SQL.
	* [Vertica](https://www.vertica.com) Distributed, MPP columnar database with extensive analytics SQL.

### Document
	* [MongoDB](https://www.mongodb.com) An open-source, document database designed for ease of development and scaling. 
		* [Percona Server for MongoDB](https://www.percona.com/software/mongo-database/percona-server-for-mongodb) Percona Server for MongoDB® is a free, enhanced, fully compatible, open source, drop-in replacement for the MongoDB® Community Edition that includes enterprise-grade features and functionality.
		* [MemDB](https://github.com/rain1017/memdb) Distributed Transactional In-Memory Database (based on MongoDB)
	* [Elasticsearch](https://www.elastic.co/) Search & Analyze Data in Real Time.
	* [Couchbase](https://www.couchbase.com/) The highest performing NoSQL distributed database.
	* [RethinkDB](https://rethinkdb.com/) The open-source database for the realtime web.
	* [RavenDB](https://ravendb.net/) Fully Transactional NoSQL Document Database.
	* [Deta Base](https://deta.sh) Deta Base is a super easy to use production-grade NoSQL database that supports complex queries and search.

### Graph
	* [Neo4j](https://neo4j.com/) The world’s leading graph database.
	* [OrientDB](https://orientdb.com) 2nd Generation Distributed Graph Database with the flexibility of Documents in one product with an Open Source commercial friendly license.
	* [ArangoDB](https://www.arangodb.com/) A distributed free and open-source database with a flexible data model for documents, graphs, and key-values. 
	* [Titan](https://titan.thinkaurelius.com) A scalable graph database optimized for storing and querying graphs containing hundreds of billions of vertices and edges distributed across a multi-machine cluster.
	* [FlockDB](https://github.com/twitter-archive/flockdb) A distributed, fault-tolerant graph database by Twitter. Deprecated.

### Distributed
	* [DAtomic](https://www.datomic.com) The fully transactional, cloud-ready, distributed database.
	* [Apache Geode](https://geode.apache.org/) An open source, distributed, in-memory database for scale-out applications.
	* [Gaffer ](https://github.com/gchq/Gaffer) A large-scale graph database

### Timeseries
	* [InfluxDB](https://github.com/influxdata/influxdb) Scalable datastore for metrics, events, and real-time analytics.
	* [OpenTSDB](https://github.com/OpenTSDB/opentsdb) A scalable, distributed Time Series Database.
	* [kairosdb](https://github.com/kairosdb/kairosdb) Fast scalable time series database.
	* [Heroic](https://github.com/spotify/heroic) A scalable time series database based on Cassandra and Elasticsearch, by Spotify
	* [Druid](https://github.com/apache/incubator-druid) Column oriented distributed data store ideal for powering interactive applications
	* [Riak-TS](http://basho.com/products/riak-ts/) Riak TS is the only enterprise-grade NoSQL time series database optimized specifically for IoT and Time 

### Series data
	* [Akumuli](https://github.com/akumuli/Akumuli) Akumuli is a numeric time-series database. It can be used to capture, store and process time-series data in real-time. The word "akumuli" can be translated from esperanto as "accumulate".
	* [Rhombus](https://github.com/Pardot/Rhombus) A time-series object store for Cassandra that handles all the complexity of building wide row indexes.
	* [Dalmatiner DB](https://github.com/dalmatinerdb/dalmatinerdb) Fast distributed metrics database
	* [Blueflood](https://github.com/rackerlabs/blueflood) A distributed system designed to ingest and process time series data
	* [Timely](https://github.com/NationalSecurityAgency/timely) Timely is a time series database application that provides secure access to time series data based on Accumulo and Grafana.

### Other
	* [Tarantool](https://github.com/tarantool/tarantool/) Tarantool is an in-memory database and application server.
	* [GreenPlum](https://github.com/greenplum-db/gpdb) The Greenplum Database (GPDB) is an advanced, fully featured, open source data warehouse. It provides powerful and rapid analytics on petabyte scale data volumes.
	* [cayley](https://github.com/cayleygraph/cayley) An open-source graph database. Google.
	* [Snappydata](https://github.com/SnappyDataInc/snappydata) SnappyData: OLTP + OLAP Database built on Apache Spark
	* [TimescaleDB](https://www.timescale.com/): Built as an extension on top of PostgreSQL, TimescaleDB is a time-series SQL database providing fast analytics, scalability, with automated data management on a proven storage engine.

## Serialization format

* [Apache Avro](https://avro.apache.org) Apache Avro™ is a data serialization system
* [Apache Parquet](https://parquet.apache.org) Apache Parquet is a columnar storage format available to any project in the Hadoop ecosystem, regardless of the choice of data processing framework, data model or programming language.
multi-processor, multi-core machines
* [Apache ORC](https://orc.apache.org/) The smallest, fastest columnar storage for Hadoop workloads 
* [Apache Thrift](https://thrift.apache.org) The Apache Thrift software framework, for scalable cross-language services development
* [ProtoBuf](https://github.com/protocolbuffers/protobuf) Protocol Buffers - Google's data interchange format
* [SequenceFile](https://wiki.apache.org/hadoop/SequenceFile) SequenceFile is a flat file consisting of binary key/value pairs. It is extensively used in MapReduce as input/output formats
* [Kryo](https://github.com/EsotericSoftware/kryo) Kryo is a fast and efficient object graph serialization framework for Java
* [Apache Iceberg](https://iceberg.apache.org/) Apache Iceberg is an open table format for huge analytic datasets. Iceberg adds tables to Presto and Spark that use a high-performance format that works just like a SQL table.
* [Apache Hudi](https://hudi.apache.org/)
* [Delta Lake](https://delta.io/)

# Workflow

 - Apache Airflow
 - Dagster
 - Prefect
 - [Flyte](https://flyte.org/)
 - [Kedro](https://kedro.readthedocs.io/en/latest/) Kedro is a framework that makes it easy to build robust and scalable data pipelines by providing uniform project templates, data abstraction, configuration and pipeline assembly.
 - [Kestra](https://github.com/kestra-io/kestra) Open source data orchestration and scheduling platform with declarative syntax.
 - [cheek](https://github.com/datarootsio/cheek) is a simple crontab like scheduler and aims to offer a KISS approach to job scheduling.
 - [Apache NiFi](https://nifi.apache.org) Apache NiFi supports powerful and scalable directed graphs of data routing, transformation, and system mediation logic.




# Data Governance
## Data Catalog

 - [Open Metadata](https://open-metadata.org/)

## Data Quality

 -  Great Expectations
 -  [re_data](https://www.getre.io/)
 -  [Soda](https://github.com/sodadata/soda-core)

# Control Plane
 - [Kuwala](https://github.com/kuwala-io/kuwala) is the data workspace for BI analysts and engineers enabling you to build powerful analytics workflows together. We are set out to bring state-of-the-art data engineering tools you love, such as Airbyte, dbt and Prefect together in one intuitive interface built with React Flow.



## About

Inspired by [awesome-data-engineering](https://github.com/igorbarinov/awesome-data-engineering), [awesome-bigdata](https://github.com/0xnr/awesome-bigdata), [awesome-hadoop](https://github.com/youngwookim/awesome-hadoop#readme), [awesome-streaming](https://github.com/manuzhang/awesome-streaming#readme), [awesome-spark](https://github.com/awesome-spark/awesome-spark#readme).
