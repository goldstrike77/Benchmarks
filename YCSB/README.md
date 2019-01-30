## **Yahoo! Cloud System Benchmark** ##
YCSB is a framework for benchmarking systems.The goal of the YCSB project is to develop a framework and common set of workloads for evaluating the performance of different “key-value” and “cloud” serving stores. The project comprises two things:

- The YCSB Client, an extensible workload generator
- The Core workloads, a set of workload scenarios to be executed by the generator

Because there are many new serving databases available, including:

- HBase
- Hypertable
- Cassandra
- Couchbase
- Voldemort
- MongoDB
- OrientDB
- Infinispan
- Redis
- GemFire
- DynamoDB
- Tarantool
- Memcached…and many others

It is difficult to decide which system is right for your application, partially because the features differ between systems, and partially because there is not an easy way to compare the performance of one system versus another.

A common use of the tool is to benchmark multiple systems and compare them. For example, you can install multiple systems on the same hardware configuration, and run the same workloads against each system. Then you can plot the performance of each system (for example, as latency versus throughput curves) to see when one system does better than another.