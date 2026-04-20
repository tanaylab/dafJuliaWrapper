# Get axis version counter

Returns the version counter for an axis, which is incremented when the
axis is modified. This is useful for cache invalidation.

## Usage

``` r
axis_version_counter(daf, axis)
```

## Arguments

- daf:

  A Daf object

- axis:

  Name of the axis

## Value

A character string representing the current counter value. Returned as a
string rather than an R integer because the Julia-side counter is a
`UInt32` that can exceed R's signed-integer range.

## Details

The version counter is incremented whenever the axis entries are
modified. Compare counters with
[`identical()`](https://rdrr.io/r/base/identical.html) or `==` on the
strings.
