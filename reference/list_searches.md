# List all volunteer searches with recipient and click counts

List all volunteer searches with recipient and click counts

## Usage

``` r
list_searches()
```

## Value

Data frame with columns `search_id`, `created_at`, `notify_email`,
`active`, `total`, `clicked`.

## See also

Other email:
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md),
[`deactivate_stale_searches()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_stale_searches.md),
[`handle_click()`](https://docs.ropensci.org/roreviewapi/reference/handle_click.md),
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
