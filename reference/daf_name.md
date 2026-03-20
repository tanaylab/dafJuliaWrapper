# Gets the name of a Daf object

Returns the unique identifier name of the Daf data set.

`name()` is deprecated in favor of `daf_name()` to avoid name conflicts
with other packages.

## Usage

``` r
daf_name(x, ...)

name(x, ...)
```

## Arguments

- x:

  A Daf object

- ...:

  Additional arguments (not used)

## Value

The name of the Daf data set as a character string

## Details

Each Daf data set has a unique name used in error messages and for
identification. This is typically set when creating the object or
derived from its contents.
