# Table Totals for Metabase

A Chrome extension that adds a totals row to regular Metabase tables — in questions and on dashboards.

Metabase shows totals only in pivot tables, and pivot tables don't work for SQL questions
([metabase#3218](https://github.com/metabase/metabase/issues/3218)). This extension adds a totals row under every
regular table:

- **Sum, average, minimum, maximum or count** — choose per column with one click.
- **Sensible defaults** — columns that shouldn't be added up (IDs, percentages, rates, years) start empty.
- **Metabase's own number format** — currency, separators and decimals follow each column's settings.
- **Honest about partial data** — when Metabase loaded only the first 2,000 rows, the row says so.
- **Export** — copy the table with its totals, download it as CSV, or use "Export as PDF" on a dashboard: the totals
  row is in the PDF.
- Works with **self-hosted Metabase** and **Metabase Cloud**.

## Install

Chrome Web Store — coming soon.

After installing, open your Metabase, click the extension icon and choose **Enable on this site**.
Metabase Cloud (`*.metabaseapp.com`) works without this step.

## Price

Free for 7 days with every feature. After that, a one-time $9 license — no subscription.
Payments and license keys are handled by [Freemius](https://freemius.com), the merchant of record.

## Privacy

Everything is computed in your browser from the data Metabase has already loaded. Table data never leaves your
computer, and there is no analytics or tracking. The only thing the extension ever sends is your license key, to
Freemius, to check it. Full policy: [PRIVACY.md](PRIVACY.md).

## Limits

- Only people who have the extension installed see the totals.
- Scheduled subscriptions (emails, server-made PDFs) and Metabase's own CSV/XLSX downloads don't include them.
- If a result is larger than Metabase's display limit, the total covers the loaded rows only (the row says so).

Tested with Metabase 0.65.

## Support

Questions, bugs, ideas: [open an issue](https://github.com/korolserhii/metabase-table-totals/issues) or write to
korolserhii.dev@gmail.com.

---

Not affiliated with or endorsed by Metabase, Inc. "Metabase" is a trademark of Metabase, Inc.
