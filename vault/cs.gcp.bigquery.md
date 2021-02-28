---
id: db6c51b5-6028-4b8e-a128-b2ca4116574e
title: Bigquery
desc: ''
updated: 1611826091493
created: 1611826010044
---

# BigQuery

To find the size of all tables within a dataset

```sql
SELECT
  table_id,
  SUM(size_bytes)/(1024*1024*1024) AS size_GB
FROM
  datasetname.__TABLES__
GROUP BY
  table_id
ORDER BY
  size_GB DESC;
```