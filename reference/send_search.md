# Send a batch of editor search emails

Fetches current editor email addresses via `get_editor_emails()`,
inserts a new search record and one recipient row per address into the
database, then dispatches emails via the Gmail API. The notify address
is read from the AirTable cache written by the internal
'notify_email_refresh' function. The base URL for click links is read
from the `ROREVIEWAPI_BASE_URL` environment variable. The stats/standard
distinction is determined by calling
[`issue_is_stats()`](https://docs.ropensci.org/roreviewapi/reference/issue_is_stats.md)
on the supplied `repo` and `issue_id`.

## Usage

``` r
send_search(
  repourl,
  repo,
  issue_id,
  subject = "Seeking editors for rOpenSci software submission",
  fetcher = NULL,
  stats_checker = roreviewapi::issue_is_stats,
  sender = NULL
)
```

## Arguments

- repourl:

  URL of the package repository; included in the outgoing emails.

- repo:

  GitHub review repository in `org/repo` format.

- issue_id:

  Integer issue number in the review repository.

- subject:

  Subject line for the outgoing emails.

- fetcher:

  Function used to fetch editor emails; injectable for testing. Must
  accept `(airtable_base_id, stats)` and return a character vector.

- stats_checker:

  Function used to determine submission type; injectable for testing.
  Must accept `(repo, issue_id)` and return a logical.

- sender:

  Function used to send the batch of emails; injectable for testing.
  Must accept `(emails, links, subject, repo, issue_id)` and return a
  list of per-recipient responses. Defaults to `gmail_send_batch`.

## Value

Named list with `search_id` (integer) and `sent` (integer).

## See also

Other email:
[`deactivate_search()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_search.md),
[`deactivate_stale_searches()`](https://docs.ropensci.org/roreviewapi/reference/deactivate_stale_searches.md),
[`handle_click()`](https://docs.ropensci.org/roreviewapi/reference/handle_click.md),
[`list_searches()`](https://docs.ropensci.org/roreviewapi/reference/list_searches.md)
