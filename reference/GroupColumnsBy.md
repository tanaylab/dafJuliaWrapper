# GroupColumnsBy query operation

Specify value per matrix column to group the columns by. Must be
followed by a ReduceToColumn to reduce each group of columns to a single
column. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.GroupColumnsBy)
for details.

## Usage

``` r
GroupColumnsBy(property, ...)
```

## Arguments

- property:

  String specifying the property to group columns by

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
