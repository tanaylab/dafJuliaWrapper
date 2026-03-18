# LookupMatrix query operation

A query operation for looking up the value of a matrix property. See the
Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.LookupMatrix)
for details.

## Usage

``` r
LookupMatrix(property, ...)
```

## Arguments

- property:

  String specifying the matrix property name to look up

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object that can be used in a query sequence
