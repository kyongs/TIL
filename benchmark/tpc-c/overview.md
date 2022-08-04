# Overview

TPC-C is the standard OLTP benchmark.&#x20;

### Tables

1. Warehouse
2. District
3. Stock
4. Item
5. New-Order
6. Order-Line
7. Customer
8. Order
9. History



### Transactions

1. New-Order&#x20;
2. Payment (43%)
3. Delivery (4%)
4. Order-Status (4%)
5. Stock-Level (4%)



**Performance Metric**

Metrics are new-order txn rate (tpmC) and price/performance($/tpmC)



RampUp Time

After ramp-up time, performance stays stable.

![](<../../.gitbook/assets/스크린샷 2022-08-03 오후 5.13.52.png>)

TPC-C spec 5.6.4 figure



recommendation: ramp-up time (20min), measurement interval(120minutes)

References

[https://www.tpc.org/tpc\_documents\_current\_versions/pdf/tpc-c\_v5.11.0.pdf](https://www.tpc.org/tpc\_documents\_current\_versions/pdf/tpc-c\_v5.11.0.pdf)

