# Send a batch of editor search emails, and post the outcome to the issue

Wrapper around
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
intended to be run as a background process from the `send_search`
endpoint, which returns before any emails are sent. The outcome, success
or failure, is posted back to the GitHub issue from which the command
was invoked.

## Usage

``` r
send_search_and_post(
  repourl,
  repo,
  issue_id,
  poster = roreviewapi::post_to_issue,
  ...
)
```

## Arguments

- repourl:

  URL of the package repository; included in the outgoing emails.

- repo:

  GitHub review repository in `org/repo` format.

- issue_id:

  Integer issue number in the review repository.

- poster:

  Function used to post the outcome to the issue; injectable for
  testing. Must accept `(cmt, repo, issue_id)`. Defaults to
  `post_to_issue`.

- ...:

  Further arguments passed to
  [`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md).

## Value

The comment posted to the issue, invisibly.

## See also

Other email:
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md),
[`deactivate_stale_searches()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_stale_searches.md),
[`handle_click()`](https://docs.ropensci.org/roreviewapi/reference/handle_click.md),
[`list_searches()`](https://docs.ropensci.org/roreviewapi/reference/list_searches.md),
[`send_search()`](https://docs.ropensci.org/roreviewapi/reference/send_search.md)
