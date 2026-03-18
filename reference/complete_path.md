# Get the complete filesystem path of a persistent Daf repository

If the Daf repository is persistent (resides on disk), returns the
absolute path leading to it. If the repository is (at least partially)
in-memory, returns NULL.

## Usage

``` r
complete_path(daf)
```

## Arguments

- daf:

  A Daf object

## Value

A character string with the absolute path to the persistent Daf
repository, or NULL if the repository is in-memory.

## Details

The returned path can be given to `complete_daf` to access the
repository after the current process is terminated. Note that for H5df
format, the path may end with `#...` to identify a specific group inside
an HDF5 file. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/readers.html#DataAxesFormats.Readers.complete_path)
for details.
