## Operating System ##
CentOS 7.9 kernel 3.10.0-1160.41.1.el7.x86_64

## Hardware Specifications ##
- Intel(R) Xeon(R) Silver 4214R 2.40GHz * 2, Cascade Lake Q1'20, disable Hyper-threading 
- 128G DDR4 2400 MHz Memory
- 480GB 6Gbps SATA MU TLC 2.5 SSD * 8 RAID10
- Gigabit Ethernet

## Redis Version ##
Redis 5.0.13 with AOF persistence

## Measurement ##
- 10 Million documents operation, each with 1 KB (10 fields, 100 bytes each, plus key) data size
- 32 threads

## Benchmark Results ##
    ┌──────────────┬─────────────────────┐
    │   Workload   │ Throughput(ops/sec) │
    ├──────────────┼─────────────────────┤
    │       A      │           77,788.93 │
    ├──────────────┼─────────────────────┤
    │       B      │           73,397.73 │
    ├──────────────┼─────────────────────┤
    │       C      │           74,205.45 │
    ├──────────────┼─────────────────────┤
    │       D      │           69,753.00 │
    ├──────────────┼─────────────────────┤
    │       E      │            1,383.20 │
    ├──────────────┼─────────────────────┤
    │       F      │           52,926.57 │
    └──────────────┴─────────────────────┘
