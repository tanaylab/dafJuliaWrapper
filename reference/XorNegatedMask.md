# XorNegatedMask query operation

Same as `XorMask` but use the inverse of the mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.XorNegatedMask)
for details.

## Usage

``` r
XorNot(property, ...)

XorNegatedMask(value, ...)
```

## Arguments

- property:

  String specifying the property

- ...:

  Additional arguments needed to support usage of pipe operator

- value:

  String specifying the property

## Value

A query operation object

## Functions

- `XorNot()`: Deprecated: use `XorNegatedMask()` instead.
