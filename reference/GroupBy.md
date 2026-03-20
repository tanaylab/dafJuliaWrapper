# GroupBy query operation

A query operation that aggregates values by groups. This operation takes
a property whose values define groups, and applies a subsequent
reduction operation (e.g., Mean, Sum, Max) to aggregate the values
within each group. If applied to a vector, the result is a vector with
one entry per group. If applied to a matrix, the result is a matrix with
one row per group. This is typically followed by a reduction operation
that specifies how to aggregate the grouped values. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.GroupBy)
for details.

## Usage

``` r
GroupBy(value, ...)
```

## Arguments

- value:

  String specifying the property to group by

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object that can be used in a query sequence
