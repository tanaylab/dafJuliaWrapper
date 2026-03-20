# AnnData-like live facade for a Daf object

AnnData-like live facade for a Daf object

AnnData-like live facade for a Daf object

## Details

Wraps a Daf object and provides AnnData-compatible accessors (`$X`,
`$obs`, `$var`, `$layers`, `$uns`). This is a zero-copy live facade:
reads are lazy and go through to the underlying Daf data on demand.

The facade maps AnnData concepts to Daf data:

- `$X` - the primary matrix (obs_axis x var_axis, named x_name)

- `$obs` - data frame of observation (obs_axis) vectors

- `$var` - data frame of variable (var_axis) vectors

- `$layers` - named list of additional matrices (obs_axis x var_axis)

- `$uns` - named list of scalars

- `$obs_names` - character vector of observation names

- `$var_names` - character vector of variable names

- `$n_obs` - number of observations

- `$n_vars` - number of variables

- `$shape` - c(n_obs, n_vars)

All reads are lazy and cached via dafr's caching system.

## Public fields

- `daf`:

  The underlying Daf object

- `obs_axis`:

  Name of the observations axis

- `var_axis`:

  Name of the variables axis

- `x_name`:

  Name of the primary matrix

## Active bindings

- `X`:

  The primary matrix (obs x var)

- `obs`:

  Data frame of observation vectors

- `var`:

  Data frame of variable vectors

- `layers`:

  Named list of additional matrices (excluding X)

- `uns`:

  Named list of scalars

- `obs_names`:

  Character vector of observation names

- `var_names`:

  Character vector of variable names

- `n_obs`:

  Number of observations

- `n_vars`:

  Number of variables

- `shape`:

  Dimensions c(n_obs, n_vars)

## Methods

### Public methods

- [`DafAnnData$new()`](#method-DafAnnData-new)

- [`DafAnnData$print()`](#method-DafAnnData-print)

- [`DafAnnData$clone()`](#method-DafAnnData-clone)

------------------------------------------------------------------------

### Method `new()`

Create a new DafAnnData facade

#### Usage

    DafAnnData$new(daf, obs_axis = NULL, var_axis = NULL, x_name = "UMIs")

#### Arguments

- `daf`:

  A Daf object

- `obs_axis`:

  Observations axis name (auto-detected if NULL)

- `var_axis`:

  Variables axis name (auto-detected if NULL)

- `x_name`:

  Primary matrix name (default "UMIs")

------------------------------------------------------------------------

### Method [`print()`](https://rdrr.io/r/base/print.html)

Print the DafAnnData object

#### Usage

    DafAnnData$print(...)

#### Arguments

- `...`:

  Ignored

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    DafAnnData$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
