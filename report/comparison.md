## Comparison

|                               | Query 0 | Query 1  | Query 2  | Aggregate 1 | Aggregate 2         | Aggregate 3 |
| ----------------------------- | ------- | -------- | -------- | ----------- | ------------------- | ----------- |
| postgresql no opti            | 2.6890s | 15.3270s | 20.8068s | 5.4380s     | 28.3206s ~ 19.3993s | 6.0251s     |
| postgresql index on medallion |         |          |          | 6.2733s     | 24.6855s            | 8.1786s     |
| duckDB no opti                | 0.0003s | 0.0004s  | 0.0003s  | 0.0885s     | 0.1041s             | 0.0017s     |