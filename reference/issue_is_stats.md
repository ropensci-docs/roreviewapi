# Determine whether a GitHub issue is a Stats submission

Determine whether a GitHub issue is a Stats submission

## Usage

``` r
issue_is_stats(orgrepo, issue_num)
```

## Arguments

- orgrepo:

  GitHub organization and repo as single string separated by forward
  slash (`org/repo`).

- issue_num:

  Number of issue from which to extract submission type.

## Value

`TRUE` if the submission type is "Stats", otherwise `FALSE`.

## See also

Other ropensci:
[`check_issue_template()`](https://docs.ropensci.org/roreviewapi/reference/check_issue_template.md),
[`is_user_authorized()`](https://docs.ropensci.org/roreviewapi/reference/is_user_authorized.md),
[`push_to_gh_pages()`](https://docs.ropensci.org/roreviewapi/reference/push_to_gh_pages.md),
[`readme_has_peer_review_badge()`](https://docs.ropensci.org/roreviewapi/reference/readme_has_peer_review_badge.md),
[`srr_counts()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts.md),
[`srr_counts_from_report()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_from_report.md),
[`srr_counts_summary()`](https://docs.ropensci.org/roreviewapi/reference/srr_counts_summary.md),
[`stats_badge()`](https://docs.ropensci.org/roreviewapi/reference/stats_badge.md)
