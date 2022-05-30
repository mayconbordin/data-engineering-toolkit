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

# Serialization format
* [Apache Avro](https://avro.apache.org) Apache Avro™ is a data serialization system
* [Apache Parquet](https://parquet.apache.org) Apache Parquet is a columnar storage format available to any project in the Hadoop ecosystem, regardless of the choice of data processing framework, data model or programming language.
	* [Snappy](https://github.com/google/snappy) A fast compressor/decompressor. Used with Parquet
	* [PigZ](https://zlib.net/pigz/) A parallel implementation of gzip for modern
multi-processor, multi-core machines
* [Apache ORC](https://orc.apache.org/) The smallest, fastest columnar storage for Hadoop workloads 
* [Apache Thrift](https://thrift.apache.org) The Apache Thrift software framework, for scalable cross-language services development
* [ProtoBuf](https://github.com/protocolbuffers/protobuf) Protocol Buffers - Google's data interchange format
* [SequenceFile](https://wiki.apache.org/hadoop/SequenceFile) SequenceFile is a flat file consisting of binary key/value pairs. It is extensively used in MapReduce as input/output formats
* [Kryo](https://github.com/EsotericSoftware/kryo) Kryo is a fast and efficient object graph serialization framework for Java

* [Apache Iceberg](https://iceberg.apache.org/) Apache Iceberg is an open table format for huge analytic datasets. Iceberg adds tables to Presto and Spark that use a high-performance format that works just like a SQL table.

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
