## Operating System ##
CentOS 6.10 kernel 2.6.32-754.10.1.el6.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) Processor E7520 1.87GHz * 4, Nehalem-EX Q1'10, disable Hyper-threading 
- 32G DDR3 1333 MHz Memory
- 300G 10000RPM 2.5-inch SAS 6Gb * 4 RAID10
- Gigabit Ethernet

## MongoDB Version ##
Percona Server for MongoDB 3.6.10-3.0, WiredTiger Storage Engine with Journal

## Measurement ##
- 10 Million documents operation, each with 1 KB (10 fields, 100 bytes each, plus key) data size
- Requests no acknowledgment of the write operation
- Synchronous driver
- 64 threads

## Benchmark Results ##
    ┌──────────────┬─────────────────────┐
    │   Workload   │ Throughput(ops/sec) │
    ├──────────────┼─────────────────────┤
    │     load     │           64,105.85 │
    ├──────────────┼─────────────────────┤
    │       A      │          137,147.87 │
    ├──────────────┼─────────────────────┤
    │       B      │          122,129.95 │
    ├──────────────┼─────────────────────┤
    │       C      │          120,727.75 │
    ├──────────────┼─────────────────────┤
    │       D      │           87,163.44 │
    ├──────────────┼─────────────────────┤
    │       E      │            1,987.12 │
    ├──────────────┼─────────────────────┤
    │       F      │           67,419.51 │
    └──────────────┴─────────────────────┘
