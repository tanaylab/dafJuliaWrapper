# LookupScalar query operation

A query operation for looking up the value of a scalar property. See the
Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.LookupScalar)
for details.

## Usage

``` r
LookupScalar(property, ...)
```

## Arguments

- property:

  String specifying the scalar property name to look up

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object that can be used in a query sequence
