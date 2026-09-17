# Set up stdout & stderr cache files for `r_bg` process

Set up stdout & stderr cache files for `r_bg` process

## Usage

``` r
stdout_stderr_cache(repourl)
```

## Arguments

- repourl:

  The URL of the repo being checked

## Value

Vector of two strings holding respective local paths to `stdout` and
`stderr` files for `r_bg` process controlling the main
[editor_check](https://docs.ropensci.org/roreviewapi/reference/editor_check.md)
function.

## Note

These files are needed for the callr `r_bg` process which controls the
main
[editor_check](https://docs.ropensci.org/roreviewapi/reference/editor_check.md)
call. See <https://github.com/r-lib/callr/issues/204>. The `stdout` and
`stderr` pipes from the process are stored in the cache directory so
they can be inspected via their own distinct endpoint calls.

## See also

Other utils:
[`check_cache()`](https://docs.ropensci.org/roreviewapi/reference/check_cache.md),
[`pkgrep_install_deps()`](https://docs.ropensci.org/roreviewapi/reference/pkgrep_install_deps.md),
[`symbol_crs()`](https://docs.ropensci.org/roreviewapi/reference/symbol_crs.md),
[`symbol_tck()`](https://docs.ropensci.org/roreviewapi/reference/symbol_tck.md)
