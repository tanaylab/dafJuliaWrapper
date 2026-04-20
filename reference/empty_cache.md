# Empty cache of a Daf object

Clears the Julia-side cache and the R-side cache for a Daf object. The
R-side cache is always purged (regardless of `clear`/`keep`), because
version counters only invalidate entries opportunistically on next
access and may miss stale data when backing storage is unmapped or when
Julia cache is flushed without bumping data versions.

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

## Examples

``` r
if (FALSE) { # \dontrun{
setup_daf()
daf <- example_cells_daf()
empty_cache(daf) # clear all caches
empty_cache(daf, clear = "QueryData") # clear only Julia query cache
empty_cache(daf, keep = "MappedData") # keep mapped data, clear rest
} # }
```
