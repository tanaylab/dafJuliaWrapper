# BeginNegatedMask query operation

Start specifying a negated mask to apply to an axis of the result. Must
be accompanied by an EndMask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.BeginNegatedMask)
for details.

## Usage

``` r
BeginNegatedMask(value, ...)
```

## Arguments

- value:

  String specifying the property name for the initial negated mask

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
