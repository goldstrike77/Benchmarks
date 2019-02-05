## Operating System ##
CentOS 6.10 kernel 2.6.32-754.10.1.el6.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) CPU E5-2650 v4 @ 2.20GHz * 2 disable Hyper-threading
- 64G DIMM DDR4 2133 MHz Memory
- ST9500620SS 500GB 7200RPM 2.5-inch NL-SAS 6Gb * 4 RAID10
- Gigabit Ethernet

## MongoDB Version ##
Percona Server for MongoDB 3.6.8-2.0

## Measurement ##
- 10 Million documents operation, each with 1 KB (10 fields, 100 bytes each, plus key) data size
- 32 threads

## Benchmark Results ##
    ┌──────────────┬─────────────────────┐
    │   Workload   │ Throughput(ops/sec) │
    ├──────────────┼─────────────────────┤
    │       A      │           90,391.39 │
    ├──────────────┼─────────────────────┤
    │       B      │          138,400.64 │
    ├──────────────┼─────────────────────┤
    │       C      │          154,038.11 │
    ├──────────────┼─────────────────────┤
    │       D      │          149,004.64 │
    ├──────────────┼─────────────────────┤
    │       E      │           13,718.21 │
    ├──────────────┼─────────────────────┤
    │       F      │           57,260.97 │
    └──────────────┴─────────────────────┘