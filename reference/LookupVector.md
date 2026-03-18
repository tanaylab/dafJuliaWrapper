# LookupVector query operation

A query operation for looking up the value of a vector property with a
specific name. This operation retrieves the data associated with the
specified property for the current axis context. It is typically used
after an `Axis` operation to select a vector property from that axis.
See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Queries.LookupVector)
for details.

## Usage

``` r
Lookup(property, ...)

LookupVector(property, ...)
```

## Arguments

- property:

  String specifying the property name to look up

- ...:

  Additional arguments needed to support usage of pipe operator

## Value

A query operation object that can be used in a query sequence
