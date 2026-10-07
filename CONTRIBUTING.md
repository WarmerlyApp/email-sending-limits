# Contributing

Every figure needs a link to the provider's own documentation, and `last_checked` in `data/limits.json` should move when you re-verify a row.

1. Edit `data/limits.json` (the source of truth). `data/limits.csv` is generated from it, so keep the two in step.
2. Use `null` when a provider says a limit exists but publishes no number. Do not guess.
3. Set `status` to `confirmed` only if you read the number on the provider's page. Otherwise `unconfirmed`, with a note saying why.
4. No figures from blog posts or forums as a primary source. They can go in the notes as context.
