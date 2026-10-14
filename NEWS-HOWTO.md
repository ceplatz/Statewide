# Posting news (Regan's quick guide)

The "Latest updates" strips on the Armory and AZ Pawn pages read from a Google Sheet.

**One-time setup**
1. Make a Google Sheet. Row 1 headers, exactly: `date`, `headline`, `snippet`, `link`, `category`.
2. File > Share > Publish to web > choose the sheet tab and **CSV** > Publish. Copy the link.
3. Send that link to whoever maintains the site; it goes into `NEWS_CSV_URL` in `index.html`.

**Each post = one new row**
- `date`: 2026-10-14 (or 10/14/2026)
- `headline`: short and plain
- `snippet`: one or two sentences, in your own words
- `link`: optional, must start with https://
- `category`: `armory` (shows on the Armory page) or `pawn` (shows on the AZ Pawn page)

The newest 3 show first; "Show more" reveals up to 12. A page with no posts hides its strip. Changes appear within a few minutes.

**Tips:** summarize other sites' articles in your own words and link to the original; don't paste their text. `news-template.csv` has example rows.
