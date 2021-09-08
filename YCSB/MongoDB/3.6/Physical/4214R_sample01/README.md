## Operating System ##
CentOS 7.9 kernel 3.10.0-1160.41.1.el7.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) Silver 4214R 2.40GHz * 2, Cascade Lake Q1'20, disable Hyper-threading 
- 128G DDR4 2400 MHz Memory
- 480GB 6Gbps SATA MU TLC 2.5 SSD * 8 RAID10
- Gigabit Ethernet

## Redis Version ##
Percona Server for MongoDB 3.6.23-13.0, WiredTiger Storage Engine with Journal

## Measurement ##
- 10 Million documents operation, each with 1 KB (10 fields, 100 bytes each, plus key) data size
- Requests no acknowledgment of the write operation
- Synchronous driver
- 64 threads

## Benchmark Results ##
    ┌──────────────┬─────────────────────┐
    │   Workload   │ Throughput(ops/sec) │
    ├──────────────┼─────────────────────┤
    │     load     │          200,100.05 │
    ├──────────────┼─────────────────────┤
    │       A      │          127,469.73 │
    ├──────────────┼─────────────────────┤
    │       B      │           93,139.35 │
    ├──────────────┼─────────────────────┤
    │       C      │           90,490.37 │
    ├──────────────┼─────────────────────┤
    │       D      │           99,186.67 │
    ├──────────────┼─────────────────────┤
    │       E      │            2,105.02 │
    ├──────────────┼─────────────────────┤
    │       F      │           75,309.71 │
    └──────────────┴─────────────────────┘
