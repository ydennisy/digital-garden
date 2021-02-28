---
id: bcc9ff56-163e-4fdc-baa2-753014a41d78
title: Pandas
desc: ''
updated: 1614106278624
created: 1611221428996
---

# Pandas


## Columns

Drop columns

```python
df = df.drop(columns=['a', 'b'])
```

Rename columns

```python
df = df.rename(columns={'a': 'b'})
```

Drop duplicates

```python
df = df.drop_duplicates(subset=['col_name'])
```

Check types

```python
df.dtypes
```

## Disk i/o

Parquet, uses `pyarrow` which is based on a C++ lib, and is therefore not bound by the python GIL.

## Shuffle

Shuffle rows in place:

```python
df = df.sample(frac=1).reset_index(drop=True)
```
