# Auto-deactivate and delete stale volunteer searches

Searches are never automatically closed otherwise, so this is intended
to be called periodically (see
[`serve_api()`](https://docs.ropensci.org/roreviewapi/reference/serve_api.md))
to stop searches that are never explicitly deactivated from accumulating
in the database forever. Any search whose `created_at` is older than
`max_age_days` is deactivated and has all its data removed, exactly as
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md)
does for a single search.

## Usage

``` r
deactivate_stale_searches(max_age_days = 100L)
```

## Arguments

- max_age_days:

  Default: 100. Integer number of days after creation at which a search
  is considered stale and is automatically deactivated.

## Value

Integer count of searches deactivated, invisibly.

## See also

Other email:
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md),
[`handle_click()`](https://docs.ropensci.org/roreviewapi/reference/handle_click.md),
[`list_searches()`](https://docs.ropensci.org/roreviewapi/reference/list_searches.md),
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
