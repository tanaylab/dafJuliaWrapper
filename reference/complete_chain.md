# Create a persistent chain from a base Daf and a new Daf

Immediately after creating an empty disk-based `new_daf`, chain it with
a disk-based `base_daf` and return the new chain. If `axes` and/or
`data` are specified, the `new_daf` will be chained on top of a view of
the `base_daf`.

## Usage

``` r
complete_chain(
  base_daf,
  new_daf,
  name = NULL,
  axes = NULL,
  data = NULL,
  absolute = FALSE
)
```

## Arguments

- base_daf:

  A Daf object to use as the base (read-only) data

- new_daf:

  A Daf object to use as the new (writable) data on top of the base

- name:

  Optional name for the chained Daf object

- axes:

  Optional named list specifying axes to expose from the base (same
  format as `viewer`)

- data:

  Optional named list specifying data to expose from the base (same
  format as `viewer`)

- absolute:

  If TRUE, store the absolute path to the base_daf. If FALSE (default),
  store a relative path for portability.

## Value

A writable Daf object chaining the base and new data

## Details

This will set the `base_daf_repository` scalar property of the `new_daf`
to point at the `base_daf`, and if view `axes` or `data` were specified,
the `base_daf_view` as well. It should therefore be possible to recreate
the chain by calling `complete_daf` in the future.

By default, the stored base path in the `new_daf` will be the relative
path to the `base_daf`, for the common case where a group of
repositories is stored under a common root. This allows the root to be
renamed or moved and still allow `complete_daf` to work.

See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/chains.html#DataAxesFormats.Chains.complete_chain!)
for details.
