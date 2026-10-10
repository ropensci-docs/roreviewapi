# Convert names of rOpenSci packages to markdown-formatted list.

This function is exported because it needs to be called in the main
plumber endpoint function.

## Usage

``` r
ros_to_list(matches, n = 5L)
```

## Arguments

- matches:

  A pkgmatch `data.frame` object with columns of ("package", "version",
  "rank").

- n:

  Number of matches to return in list.

## See also

Other pkgmatch:
[`cran_to_list()`](https://docs.ropensci.org/roreviewapi/reference/cran_to_list.md),
[`pkgmatch_repo()`](https://docs.ropensci.org/roreviewapi/reference/pkgmatch_repo.md)
