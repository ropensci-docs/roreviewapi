# Check whether 'README.md' has a "peer reviewed" badge

Check whether 'README.md' has a "peer reviewed" badge

## Usage

``` r
readme_has_peer_review_badge(path = getwd(), issue_id = NULL)
```

## Arguments

- path:

  Local path to package directory.

- issue_id:

  The id (number) of the issue from which the command was invoked.

## Value

A string, empty if the badge was found.

## See also

Other ropensci:
[`check_issue_template()`](https://docs.ropensci.org/roreviewapi/reference/check_issue_template.md),
[`is_user_authorized()`](https://docs.ropensci.org/roreviewapi/reference/is_user_authorized.md),
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md),
[`push_to_gh_pages()`](https://docs.ropensci.org/roreviewapi/reference/push_to_gh_pages.md),
[`srr_counts()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
