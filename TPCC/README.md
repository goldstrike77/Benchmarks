## **TPC-C** ##
TPC-C simulates a complete computing environment where a population of users executes transactions against a database. The benchmark is centered around the principal activities (transactions) of an order-entry environment. These transactions include entering and delivering orders, recording payments, checking the status of orders, and monitoring the level of stock at the warehouses. While the benchmark portrays the activity of a wholesale supplier, TPC-C is not limited to the activity of any particular business segment, but, rather represents any industry that must manage, sell, or distribute a product or service.

TPC-C involves a mix of five concurrent transactions of different types and complexity either executed on-line or queued for deferred execution. It does so by exercising a breadth of system components associated with such environments, which are characterized by:

- The simultaneous execution of multiple transaction types that span a breadth of complexity
- On-line and deferred transaction execution modes
- Multiple on-line terminal sessions
- Moderate system and application execution time
- Significant disk input/output
- Transaction integrity (ACID properties)
- Non-uniform distribution of data access through primary and secondary keys
- Databases consisting of many tables with a wide variety of sizes, attributes, and relationships
- Contention on data access and update

TPC-C performance is measured transactions per minute.  The primary metrics are the transaction rate (tpmC), and associated price per transaction ($/tpmC).

## **Transaction & percentage** ##
- 45% New-order: enter a new order from a customer
- 43% Payment: update customer balance to reflect a payment
- 4% Delivery: deliver orders (done as a batch transaction)
- 4% Order-status: retrieve status of customer’s most recent order
- 4% Stock-level: monitor warehouse inventory

## **Warehouse volumes of data** ##
    ┌────────────┬─────────┐
    │    Table   │   Rows  │
    ├────────────┼─────────┤
    │ customer   │  30,000 │
    ├────────────┼─────────┤
    │ district   │      10 │
    ├────────────┼─────────┤
    │ history    │  30,000 │
    ├────────────┼─────────┤
    │ item       │ 100,000 │
    ├────────────┼─────────┤
    │ new_orders │   9,000 │
    ├────────────┼─────────┤
    │ order_line │ 300,008 │
    ├────────────┼─────────┤
    │ orders     │  30,000 │
    ├────────────┼─────────┤
    │ stock      │ 100,000 │
    ├────────────┼─────────┤
    │ warehouse  │       1 │
    └────────────┴─────────┘