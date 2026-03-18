# SquareColumnIs query operation

Used when the mask matrix is square and we'd like to use a column as a
mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.SquareColumnIs)
for details.

## Usage

``` r
SquareMaskColumn(value, ...)

SquareColumnIs(value, ...)
```

## Arguments

- value:

  String specifying the value

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
