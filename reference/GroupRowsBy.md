# GroupRowsBy query operation

Specify value per matrix row to group the rows by. Must be followed by a
ReduceToRow to reduce each group of rows to a single row. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.GroupRowsBy)
for details.

## Usage

``` r
GroupRowsBy(property, ...)
```

## Arguments

- property:

  String specifying the property to group rows by

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
