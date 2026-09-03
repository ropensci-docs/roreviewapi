# Check whether a user, identified from GitHub API token, is authorized to call endpoints.

This function is used only in the plumber endpoints, to prevent them
being called by unauthorized users.

## Usage

``` r
is_user_authorized(secret = NULL)
```

## Arguments

- secret:

  Environment variable `PKGCHECK_TOKEN` sent from bot.

## Value

Logical value indicating whether or not a user is authorized.

## See also

Other ropensci:
[`check_issue_template()`](https://docs.ropensci.org/roreviewapi/reference/check_issue_template.md),
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md),
[`push_to_gh_pages()`](https://docs.ropensci.org/roreviewapi/reference/push_to_gh_pages.md),
[`readme_has_peer_review_badge()`](https://docs.ropensci.org/roreviewapi/reference/readme_has_peer_review_badge.md),
[`srr_counts()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
