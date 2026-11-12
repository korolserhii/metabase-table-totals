# Table Totals & Pivot Sort for Metabase

A Chrome extension that adds two things Metabase can't do on its own: **sorting pivot tables by value** and a
**totals row under regular tables** — in questions and on dashboards.

## Sort a pivot table by value

Metabase orders pivot rows only by their labels, A to Z
([metabase#16505](https://github.com/metabase/metabase/issues/16505)). The extension sorts them by their totals
instead: the biggest state, product or customer on top, at every level of the table, with each group's rows sorted
inside it.

- **One button** in the corner of every pivot table: choose the value (any metric in the table) and the direction.
- **Correct for any metric** — it uses the subtotals Metabase itself calculated, so averages and counts sort right.
- **Remembered** per question and per dashboard card, in your browser.
- **Columns stay put** — the column order doesn't change when the order of the rows does.

## Totals row under regular tables

Metabase shows totals only in pivot tables, and pivot tables don't work for SQL questions
([metabase#3218](https://github.com/metabase/metabase/issues/3218)). This extension adds a totals row under every
regular table:

- **Sum, average, minimum, maximum or count** — choose per column with one click.
- **Sensible defaults** — columns that shouldn't be added up (IDs, percentages, rates, years) start empty.
- **Metabase's own number format** — currency, separators and decimals follow each column's settings.
- **Honest about partial data** — when Metabase loaded only the first 2,000 rows, the row says so.
- **Export** — copy the table with its totals, download it as CSV, or use "Export as PDF" on a dashboard: the totals
  row is in the PDF.

Works with **self-hosted Metabase** and **Metabase Cloud**.

## Install

Chrome Web Store — coming soon.

After installing, open your Metabase, click the extension icon and choose **Enable on this site** (the page reloads
once). Metabase Cloud (`*.metabaseapp.com`) works without this step.

## Price

Free for 7 days with every feature, no card needed. After that, a one-time license for up to 3 browsers — no
subscription. The current price is shown at checkout.
Payments and license keys are handled by [Freemius](https://freemius.com), the merchant of record.

## Privacy

Everything is computed in your browser from the data Metabase has already loaded. Table data never leaves your
computer, and there is no analytics or tracking. The only thing the extension ever sends is your license key, to
Freemius, to check it. Full policy: [PRIVACY.md](PRIVACY.md).

## Limits

- Only people who have the extension installed see the totals and the new order.
- Sorting changes only what you see on screen: Metabase's exports, PDFs and scheduled subscriptions keep Metabase's
  own order.
- If a row field has Metabase's own ↑↓ sorting turned on, that sorting wins; the button tells you so.
- Scheduled subscriptions (emails, server-made PDFs) and Metabase's own CSV/XLSX downloads don't include the totals.
- If a result is larger than Metabase's display limit, the total covers the loaded rows only (the row says so).

Tested with Metabase 0.64 and 0.65.

## Support

Questions, bugs, ideas: [open an issue](https://github.com/korolserhii/metabase-table-totals/issues) or write to
korolserhii.dev@gmail.com.

---

Not affiliated with or endorsed by Metabase, Inc. "Metabase" is a trademark of Metabase, Inc.
