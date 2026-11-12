# check_cache

Check whether a package has been cached, and if so, whether commits have
been added to the github repo since cached version.

## Usage

``` r
check_cache(org, repo, cache_dir = fs::path_temp())
```

## Arguments

- org:

  Github organization

- repo:

  Github repository

- cache_dir:

  Directory in which packages are cached

## Value

FALSE If a package has previously been cached, and the github repo has
not changed; otherwise TRUE.

## Note

This function is not intended to be called directly, and is only
exported to enable it to be used within the plumber API.

## See also

Other utils:
[`pkgrep_install_deps()`](https://docs.ropensci.org/roreviewapi/reference/pkgrep_install_deps.md),
[`stdout_stderr_cache()`](https://docs.ropensci.org/roreviewapi/reference/stdout_stderr_cache.md),
[`symbol_crs()`](https://docs.ropensci.org/roreviewapi/reference/symbol_crs.md),
[`symbol_tck()`](https://docs.ropensci.org/roreviewapi/reference/symbol_tck.md)
