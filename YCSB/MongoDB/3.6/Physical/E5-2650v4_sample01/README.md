## Operating System ##
CentOS 6.10 kernel 2.6.32-754.10.1.el6.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) Processor E5-2650 v4 2.20GHz * 2, Broadwell Q1'16, disable Hyper-threading 
- 64G DDR4 2133 MHz Memory
- 500GB 7200RPM 2.5-inch NL-SAS 6Gb * 4 RAID10
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
    │     load     │           67,135.27 │
    ├──────────────┼─────────────────────┤
    │       A      │           97,643.85 │
    ├──────────────┼─────────────────────┤
    │       B      │           76,936.09 │
    ├──────────────┼─────────────────────┤
    │       C      │           85,319.86 │
    ├──────────────┼─────────────────────┤
    │       D      │           85,758.88 │
    ├──────────────┼─────────────────────┤
    │       E      │            2,051.56 │
    ├──────────────┼─────────────────────┤
    │       F      │           60,652.74 │
    └──────────────┴─────────────────────┘
