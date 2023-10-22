# 🪅 Some basic code of data\_cleaning

In the given code, `shape` is a method used to get the dimensions of a pandas DataFrame. Specifically, `sf_permits.shape[1]` returns the number of columns in the `sf_permits`DataFrame. The `axis` parameter in `dropna(axis=1)` specifies that the method should drop columns with missing values. In this case, `axis=1` means that the method should drop columns with missing values, rather than rows.To summarize:

* `shape` is a method used to get the dimensions of a pandas DataFrame.
* `sf_permits.shape[1]` returns the number of columns in the `sf_permits` DataFrame.
* `axis` is a parameter used in pandas methods to specify whether to operate on rows or columns.
* `dropna(axis=1)` drops columns with missing values.
