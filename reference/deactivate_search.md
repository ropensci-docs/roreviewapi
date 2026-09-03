# Deactivate a volunteer search and delete all associated data

Deactivate a volunteer search and delete all associated data

## Usage

``` r
deactivate_search(repo, issue_id)
```

## Arguments

- repo:

  GitHub review repository in `org/repo` format.

- issue_id:

  Integer issue number in the review repository.

## Value

Named list with `deactivated` (logical) and `issue_ref`.

## See also

Other email:
[`deactivate_stale_searches()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_stale_searches.md),
[`handle_click()`](https://docs.ropensci.org/roreviewapi/reference/handle_click.md),
[`list_searches()`](https://docs.ropensci.org/roreviewapi/reference/list_searches.md),
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
