# Post review checks to GitHub issue

Post review checks to GitHub issue

## Usage

``` r
post_to_issue(cmt, repo, issue_id)
```

## Arguments

- cmt:

  Single character string with comment to post.

- repo:

  The repository to post to (obtained directly from bot).

- issue_id:

  The number of the issue to post to.

## Value

URL of the comment within the nominated issue

## See also

Other github:
[`dl_gh_repo()`](https://docs.ropensci.org/roreviewapi/reference/dl_gh_repo.md),
[`get_branch_from_url()`](https://docs.ropensci.org/roreviewapi/reference/get_branch_from_url.md),
[`get_subdir_from_url()`](https://docs.ropensci.org/roreviewapi/reference/get_subdir_from_url.md),
[`url_is_r_pkg()`](https://docs.ropensci.org/roreviewapi/reference/url_is_r_pkg.md)
