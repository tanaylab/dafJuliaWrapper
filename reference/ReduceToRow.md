# ReduceToRow query operation

Specify a reduction operation to convert each column of a matrix to a
single value, reducing the matrix to a single row. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.ReduceToRow)
for details.

## Usage

``` r
ReduceToRow(reduction, ...)
```

## Arguments

- reduction:

  A reduction operation (e.g., from Mean(), Sum(), etc.) or a string
  describing the reduction

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
