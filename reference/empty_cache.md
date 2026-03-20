# Empty cache of a Daf object

Clears both the Julia-side cache and the R-side cache for a Daf object.

## Usage

``` r
empty_cache(daf, clear = NULL, keep = NULL)
```

## Arguments

- daf:

  A Daf object

- clear:

  Cache group to clear. Can be one of "MappedData", "MemoryData", or
  "QueryData".

- keep:

  Cache group to keep. Can be one of "MappedData", "MemoryData", or
  "QueryData".

## Value

The Daf object (invisibly, for chaining operations)

## Details

See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Data.empty_cache!)
for details.
