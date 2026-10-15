# Push static `html` files to `gh-pages` branch of this repo to serve via GitHub pages.

Push static `html` files to `gh-pages` branch of this repo to serve via
GitHub pages.

## Usage

``` r
push_to_gh_pages(check)
```

## Arguments

- check:

  Return result of
  [editor_check](https://docs.ropensci.org/roreviewapi/reference/editor_check.md)
  function.

## Value

Vector of two paths containing URLs of the `srr` and `network` files.

## See also

Other ropensci:
[`check_issue_template()`](https://docs.ropensci.org/roreviewapi/reference/check_issue_template.md),
[`is_user_authorized()`](https://docs.ropensci.org/roreviewapi/reference/is_user_authorized.md),
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md),
[`readme_has_peer_review_badge()`](https://docs.ropensci.org/roreviewapi/reference/readme_has_peer_review_badge.md),
[`srr_counts()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
