# Body of main 'pkgmatch' response

Body of main 'pkgmatch' response

## Usage

``` r
pkgmatch_repo(repourl, repo, issue_id, n_top = 5L, post_to_issue = TRUE)
```

## Arguments

- repourl:

  The URL for the repo being matched, potentially including full path to
  non-default branch.

- repo:

  The 'context.repo' parameter defining the repository from which the
  command was invoked, passed in 'org/repo' format.

- issue_id:

  The id (number) of the issue from which the command was invoked.

- n_top:

  Return this number of top-matches packages.

- post_to_issue:

  Integer value \> 0 will post results back to issue (via 'gh' cli);
  otherwise just return character string with result.

## Value

If `!post_to_issue`, a markdown-formatted response body, otherwise URL
of the issue comment to which response body has been posted.

## See also

Other pkgmatch:
[`cran_to_list()`](https://docs.ropensci.org/roreviewapi/reference/cran_to_list.md),
[`ros_to_list()`](https://docs.ropensci.org/roreviewapi/reference/ros_to_list.md)
