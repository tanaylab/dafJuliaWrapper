# Daf (Data Axes Format) S3 object

An S3 object that wraps a Julia DataAxesFormats object and provides
access to its methods.

## Usage

``` r
Daf(jl_obj)
```

## Arguments

- jl_obj:

  The Julia DafReader object to wrap

## Value

A Daf S3 object

## Details

See the Julia documentation
[here](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/index.html),
[here](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/formats.html#Read-API)
and
[here](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/formats.html#Write-API)
for details.

## Examples

``` r
if (FALSE) { # \dontrun{
setup_daf()
daf <- memory_daf("example") # memory_daf() returns a Daf object
is_daf(daf) # TRUE
} # }
```
