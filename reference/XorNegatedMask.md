# XorNegatedMask query operation

Same as `XorMask` but use the inverse of the mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.XorNegatedMask)
for details.

## Usage

``` r
XorNot(property, ...)

XorNegatedMask(property, ...)
```

## Arguments

- property:

  String specifying the property

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
