# Listening tests

The listening bench of the attribution engine (GAS-542), as a site to send to a listener (Reinier): one A-or-B item
per screen, made for a phone, works offline once saved. Same style and setup as [ratings](https://github.com/WGasLab/ratings).

Site: https://wgaslab.github.io/listening/

## A new test

The items and the page come from the bench repo (`gaslab-attribution-bench`):

    python -m benches.listening build POOL.json --out DIR             # items.json with the right answers + the clips
    python -m benches.listening page DIR --site ../gaslab-listening/round1

Then add a link to `round1/` in `index.html` (replace the "first test" note) and push. The right answers stay in the
bench repo; the page only carries the example's.

## The answers

At the end the listener sends a short text on WhatsApp: `KEY 1-2 2-1 …` (item – track). The bench grades it against
`items.json`.

## Public site

GitHub Pages on this account is public (anyone with the link, not indexed). Only put audio here that we may share:
our own generations and their stems. Not training-library tracks or other people's uploads.
