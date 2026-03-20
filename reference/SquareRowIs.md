# SquareRowIs query operation

Used when the mask matrix is square and we'd like to use a row as a
mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.SquareRowIs)
for details.

## Usage

``` r
SquareMaskRow(value, ...)

SquareRowIs(value, ...)
```

## Arguments

- value:

  String specifying the value

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object

## Functions

- `SquareMaskRow()`: Deprecated: use `SquareRowIs()` instead.
