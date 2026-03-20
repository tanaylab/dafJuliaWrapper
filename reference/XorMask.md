# XorMask query operation

A query operation for flipping the set of entries of an `Axis`. See the
Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.XorMask)
for details.

## Usage

``` r
Xor(property, ...)

XorMask(value, ...)
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

- `Xor()`: Deprecated: use `XorMask()` instead.
