# 🪅 Some basic code of data\_cleaning



```python
# remove all columns with at least one missing value
sf_permits_with_na_dropped = sf_permits.dropna(axis=1)

# calculate number of dropped columns
cols_in_original_dataset = sf_permits.shape[1]
cols_in_na_dropped = sf_permits_with_na_dropped.shape[1]
dropped_columns = cols_in_original_dataset - cols_in_na_dropped
```

In the given code, `shape` is a method used to get the dimensions of a pandas DataFrame. Specifically, `sf_permits.shape[1]` returns the number of columns in the `sf_permits`DataFrame.&#x20;

The `axis` parameter in `dropna(axis=1)` specifies that the method should drop columns with missing values. In this case, `axis=1` means that the method should drop columns with missing values, rather than rows.To summarize:

* `shape` is a method used to get the dimensions of a pandas DataFrame.
* `sf_permits.shape[1]` returns the number of columns in the `sf_permits` DataFrame.
* `axis` is a parameter used in pandas methods to specify whether to operate on rows or columns.
* `dropna(axis=1)` drops columns with missing values.
