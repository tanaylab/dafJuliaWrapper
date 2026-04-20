# Extract results from a Daf object using a query

Extract results from a Daf object using a query

## Usage

``` r
# S3 method for class 'Daf'
x[i, ...]
```

## Arguments

- x:

  A Daf object

- i:

  A query string or object

- ...:

  Ignored. Present for compatibility with the `[` generic.

## Value

The result of the query

## Details

The expression `daf[query]` is equivalent to
`get_query(daf, query, cache = TRUE)`. See the Julia
[documentation](https://tanaylab.github.io/DataAxesFormats.jl/v0.2.0/queries.html#DataAxesFormats.Operations.get_query)
for details.

## Examples

``` r
if (FALSE) { # \dontrun{
setup_daf()
daf <- memory_daf("example")
add_axis(daf, "cell", c("A", "B", "C"))
set_vector(daf, "cell", "score", c(1.0, 2.0, 3.0))
daf[Axis("cell") |> LookupVector("score")]
} # }
```
