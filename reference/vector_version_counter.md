# Get vector version counter

Returns the version counter for a vector property, which is incremented
when the vector is modified. This is useful for cache invalidation.

## Usage

``` r
vector_version_counter(daf, axis, name)
```

## Arguments

- daf:

  A Daf object

- axis:

  Name of the axis

- name:

  Name of the vector property

## Value

A character string representing the current counter value. Returned as a
string rather than an R integer because the Julia-side counter is a
`UInt32` that can exceed R's signed-integer range.

## Details

The version counter is incremented whenever the vector data is modified.
Compare counters with
[`identical()`](https://rdrr.io/r/base/identical.html) or `==` on the
strings.
