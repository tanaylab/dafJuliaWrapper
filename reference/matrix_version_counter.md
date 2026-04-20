# Get matrix version counter

Returns the version counter for a matrix property, which is incremented
when the matrix is modified. This is useful for cache invalidation.

## Usage

``` r
matrix_version_counter(daf, rows_axis, columns_axis, name)
```

## Arguments

- daf:

  A Daf object

- rows_axis:

  Name of the rows axis

- columns_axis:

  Name of the columns axis

- name:

  Name of the matrix property

## Value

A character string representing the current counter value. Returned as a
string rather than an R integer because the Julia-side counter is a
`UInt32` that can exceed R's signed-integer range.

## Details

The version counter is incremented whenever the matrix data is modified.
Compare counters with
[`identical()`](https://rdrr.io/r/base/identical.html) or `==` on the
strings.
