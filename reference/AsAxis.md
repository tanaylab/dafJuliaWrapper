# AsAxis query operation

A query operation that treats values in a vector property as names of
entries in another axis. This operation is commonly used with `CountBy`
and `GroupBy`, where vector values need to be interpreted as axis entry
names. If no axis is specified, values are treated as entries of a
default axis based on context. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.AsAxis)
for details.

## Usage

``` r
AsAxis(value = NULL, ...)
```

## Arguments

- value:

  Optional string specifying the axis name to use for interpreting the
  values

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object that can be used in a query sequence
