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

YCSB was contrasted with the TPC-H benchmark from the Transaction Processing Performance Council, with YCSB being called a big data benchmark while TPC-H is a decision support system benchmark.

YCSB includes a set of core workloads that define a basic benchmark for cloud systems. Of course, you can define your own workloads, as described in Implementing New Workloads. However, the core workloads are a useful first step, and obtaining these benchmark numbers for a variety of different systems would allow you to understand the performance
tradeoffs of different systems.

The core workloads consist of six different workloads:

1. Workload A: Update heavy workload, Read/update ratio: 50/50
This workload has a mix of 50/50 reads and writes. An application example is a session store recording recent actions.

2. Workload B: Read mostly workload, Read/update ratio: 95/5
This workload has a 95/5 reads/write mix. Application example: photo tagging; add a tag is an update, but most operations are to read tags.

3. Workload C: Read only, Read/update ratio: 100/0
This workload is 100% read. Application example: user profile cache, where profiles are constructed elsewhere (e.g., Hadoop).

4. Workload D: Read latest workload,Read/update/insert ratio: 95/0/5
 In this workload, new records are inserted, and the most recently inserted records are the most popular. Application example: user status updates; people want to read the latest.

5. Workload E: Short ranges, Scan/insert ratio: 95/5
In this workload, short ranges of records are queried, instead of individual records. Application example: threaded conversations, where each scan is for the posts in a given thread (assumed to be clustered by thread id).

6. Workload F: Read-modify-write, Read/read-modify-write ratio: 50/50
In this workload, the client will read a record, modify it, and write back the changes. Application example: user database, where user records are read and modified by the user or to record user activity.