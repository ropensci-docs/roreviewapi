# Count number of 'srr' statistical standards complied with, and confirm whether than represents \> 50% of all applicable standards.

Count number of 'srr' statistical standards complied with, and confirm
whether than represents \> 50% of all applicable standards.

## Usage

``` r
srr_counts(repourl, repo, issue_id, post_to_issue = TRUE)
```

## Arguments

- repourl:

  The URL for the repo being checked, potentially including full path to
  non-default branch.

- repo:

  The 'context.repo' parameter defining the repository from which the
  command was invoked, passed in 'org/repo' format.

- issue_id:

  The id (number) of the issue from which the command was invoked.

- post_to_issue:

  Integer value \> 0 will post results back to issue (via 'gh' cli);
  otherwise just return character string with result.

## Value

Vector of three numbers:

1.  Number of standards complied with

2.  Total number of applicable standards

3.  Number complied with as proportion of total

## See also

Other ropensci:
[`check_issue_template()`](https://docs.ropensci.org/roreviewapi/reference/check_issue_template.md),
[`is_user_authorized()`](https://docs.ropensci.org/roreviewapi/reference/is_user_authorized.md),
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md),
[`push_to_gh_pages()`](https://docs.ropensci.org/roreviewapi/reference/push_to_gh_pages.md),
[`readme_has_peer_review_badge()`](https://docs.ropensci.org/roreviewapi/reference/readme_has_peer_review_badge.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
