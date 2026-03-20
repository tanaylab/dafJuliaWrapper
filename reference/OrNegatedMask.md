# OrNegatedMask query operation

Same as `OrMask` but use the inverse of the mask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.OrNegatedMask)
for details.

## Usage

``` r
OrNot(property, ...)

OrNegatedMask(value, ...)
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

- `OrNot()`: Deprecated: use `OrNegatedMask()` instead.
