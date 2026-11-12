# Check whether a given GitHub URL contains an R package.

Check whether a given GitHub URL contains an R package.

## Usage

``` r
url_is_r_pkg(repourl)
```

## Arguments

- repourl:

  Potentially with "/tree/branch_name/sub-directory" appended

## Value

`TRUE` if 'repourl' is an R package, otherwise `FALSE`

## See also

Other github:
[`dl_gh_repo()`](https://docs.ropensci.org/roreviewapi/reference/dl_gh_repo.md),
[`get_branch_from_url()`](https://docs.ropensci.org/roreviewapi/reference/get_branch_from_url.md),
[`get_subdir_from_url()`](https://docs.ropensci.org/roreviewapi/reference/get_subdir_from_url.md),
[`post_to_issue()`](https://docs.ropensci.org/roreviewapi/reference/post_to_issue.md)
