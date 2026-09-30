# where-i-stand-data

Published data for the Where I Stand app, downloaded by the app at runtime. This is
not the app's source.

The data comes from public sources under different terms. The Wikipedia excerpts
are **CC BY-SA 4.0**; most of the rest is public domain or CC0; city council
boundaries keep each city's terms. See [LICENSE.md](LICENSE.md).

## Legal page dates

[`legal.json`](legal.json) holds the date each of the app's legal pages (terms,
disclaimer, privacy) last changed **materially**. Every data release carries these
dates in its `manifest.json`. When a date moves forward, the app asks readers to
accept the terms again (terms) or shows a one-time notice (disclaimer, privacy).

- Move a date only for a material change. Fixing a typo on a page moves the
  page's own "Last updated" line but should not move the date here.
- Publish the revised page first. The publish step compares each date with the
  live page and refuses to publish a date the page does not show yet.
- A change here reaches readers with the next data release. A release that moves
  only these dates republishes the same data files under a `-legal-` tag.
