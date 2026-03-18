# AndNegatedMask query operation

Same as `AndMask` but use the inverse of the mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.AndNegatedMask)
for details.

## Usage

``` r
AndNot(property, ...)

AndNegatedMask(property, ...)
```

## Arguments

- property:

  String specifying the property

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
