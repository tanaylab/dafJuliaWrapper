# BeginMask query operation

Start specifying a mask to apply to an axis of the result. Must be
accompanied by an EndMask. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.BeginMask)
for details.

## Usage

``` r
BeginMask(value, ...)
```

## Arguments

- value:

  String specifying the property name for the initial mask

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object
