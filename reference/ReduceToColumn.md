# ReduceToColumn query operation

Specify a reduction operation to convert each row of a matrix to a
single value, reducing the matrix to a single column. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.ReduceToColumn)
for details.

## Usage

``` r
ReduceToColumn(reduction, ...)
```

## Arguments

- reduction:

  A reduction operation (e.g., from Mean(), Sum(), etc.) or a string
  describing the reduction

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
