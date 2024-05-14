# AudioCloud Data Warehouse - Optimization Strategies

This document discusses strategies for optimizing the performance of the AudioCloud data warehouse. Optimization techniques include schema design, indexing, partitioning, and query optimization.

## Schema Design
- Normalize data to reduce redundancy and improve data integrity.
- Denormalize data for frequently accessed tables to reduce join operations.

## Indexing
- Create indexes on columns used frequently in WHERE, JOIN, and ORDER BY clauses.
- Consider using composite indexes for queries involving multiple columns.

## Partitioning
- Partition large tables to improve query performance and manageability.
- Partition by date, range, or hash depending on the access patterns and distribution of data.

## Query Optimization
- Use EXPLAIN ANALYZE to analyze query execution plans and identify performance bottlenecks.
- Optimize queries by rewriting inefficient SQL, avoiding unnecessary joins, and using appropriate join types.


## Important points to note

- core operation of the business always end up being the fact of the business which makes up the fact table.
- fact are measurable
- OLTP are optimized for write because thye need to collect the data as fast as possible (DB)
- (OLAP) are optimized for read and querying (DW)
- DB are highly optimized table created majorly for read
- Modeling is actually what differenciate your DB from you DW
