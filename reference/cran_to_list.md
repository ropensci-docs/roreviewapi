# Convert names of CRAN packages to markdown-formatted list.

This function is exported because it needs to be called in the main
plumber endpoint function.

## Usage

``` r
cran_to_list(matches, n = 5L)
```

## Arguments

- matches:

  A pkgmatch `data.frame` object with columns of ("package", "version",
  "rank").

- n:

  Number of matches to return in list.

## See also

Other pkgmatch:
[`pkgmatch_repo()`](https://docs.ropensci.org/roreviewapi/reference/pkgmatch_repo.md),
[`ros_to_list()`](https://docs.ropensci.org/roreviewapi/reference/ros_to_list.md)
