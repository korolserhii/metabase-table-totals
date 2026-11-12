# Privacy Policy — Table Totals & Pivot Sort for Metabase

Last updated: November 12, 2026

Table Totals & Pivot Sort for Metabase ("the extension") adds a totals row to tables and sorting by value to pivot
tables in Metabase, a business intelligence tool you open in your browser. This policy explains what the extension does with data.

## What the extension reads

On the Metabase sites where you enable it, the extension reads the table results that Metabase has already loaded in
your browser, to compute sums, averages, minimums, maximums and counts. For pivot tables it reads the results Metabase
receives and, if you turned sorting on for that table, changes only the order of their rows before Metabase shows
them. It reads nothing on other sites.

## What it stores

It stores which total you chose for each column (for example, "average" for a price column), how you chose to sort each
pivot table, the date your free trial started, and your license key once you enter one. These are saved in your
browser and do not leave your computer, except as described below.

## What it sends

Only one thing: when you enter a license key, the extension sends that key, together with a random installation
identifier the extension creates, to Freemius (freemius.com), the payment service that sold it, to check that the key
is valid. It repeats this check occasionally. Nothing else is sent: no table data, no page content, no browsing
history, no analytics or tracking.

Purchases are handled by Freemius as the merchant of record; their privacy policy applies to the payment:
https://freemius.com/privacy/

## Permissions

- **Access to your Metabase site** — asked separately for each site you enable, so the totals row can be added there.
  Metabase Cloud sites (`*.metabaseapp.com`) are covered by default.
- **scripting** — to add the extension's scripts (totals row and pivot sorting) to the sites you enabled.
- **storage** — to remember which sites you enabled, the trial start date and your license key.
- **Access to api.freemius.com** — to check your license key.
- **activeTab** — to read the address of the current tab when you open the extension's window.

You can turn the extension off for a site from its window, or remove the site's access in Chrome's extension settings.
Removing the extension deletes the license key, the trial date and the list of sites. The column and sorting choices
are kept in the storage of your Metabase site in this browser; clearing that site's data in Chrome removes them.

## Contact

Korol Serhii — korolserhii.dev@gmail.com
