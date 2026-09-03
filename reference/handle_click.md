# Handle a volunteer link click

Looks up the token, checks whether the parent search is still active,
guards against double-clicks, records the click timestamp, and triggers
a Gmail API notification (Phase 2).

## Usage

``` r
handle_click(token, sender = NULL)
```

## Arguments

- token:

  64-character hex token from the recipient's unique link.

- sender:

  Function used to send the click notification; injectable for testing.
  Must accept `(to, subject, html_body)`. Defaults to `gmail_send`.

## Value

Named list with `status` (integer HTTP status code) and `body`
(character HTML string).

## See also

Other email:
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md),
[`deactivate_stale_searches()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_stale_searches.md),
[`list_searches()`](https://docs.ropensci.org/roreviewapi/reference/list_searches.md),
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
