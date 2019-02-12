## Operating System ##
CentOS 6.10 kernel 2.6.32-754.10.1.el6.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) Processor E5-2650 v4 2.20GHz * 2, Broadwell Q1'16, disable Hyper-threading 
- 64G DDR4 2133 MHz Memory
- 500GB 7200RPM 2.5-inch NL-SAS 6Gb * 4 RAID10
- Gigabit Ethernet

## Redis Version ##
Redis 5.0.3

## Measurement ##
- 10 Million documents operation, each with 1 KB (10 fields, 100 bytes each, plus key) data size
- 32 threads

## Benchmark Results ##
    ┌──────────────┬─────────────────────┐
    │   Workload   │ Throughput(ops/sec) │
    ├──────────────┼─────────────────────┤
    │       A      │           84,437.35 │
    ├──────────────┼─────────────────────┤
    │       B      │           83,803.33 │
    ├──────────────┼─────────────────────┤
    │       C      │           85,184.68 │
    ├──────────────┼─────────────────────┤
    │       D      │           80,822.45 │
    ├──────────────┼─────────────────────┤
    │       E      │            1,579.47 │
    ├──────────────┼─────────────────────┤
    │       F      │           59,295.10 │
    └──────────────┴─────────────────────┘
