# Check template variables in GitHub issue

Check template variables in GitHub issue

## Usage

``` r
check_issue_template(orgrepo, issue_num)
```

## Arguments

- orgrepo:

  GitHub organization and repo as single string separated by forward
  slash (`org/repo`).

- issue_num:

  Number of issue from which to extract opening comment

## Value

Comment as character string

## See also

Other ropensci:
[`is_user_authorized()`](https://docs.ropensci.org/roreviewapi/reference/is_user_authorized.md),
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md),
[`push_to_gh_pages()`](https://docs.ropensci.org/roreviewapi/reference/push_to_gh_pages.md),
[`readme_has_peer_review_badge()`](https://docs.ropensci.org/roreviewapi/reference/readme_has_peer_review_badge.md),
[`srr_counts()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
