# Contributing

Thanks for helping keep the AAPL options expiration tracker up to date.

## Adding this week's numbers

1. Pull fresh data from Yahoo Finance for AAPL: company profile, expiration dates, and call/put chains for the three soonest expirations on/after today.
2. Create a tracking issue titled `Expiry YYYY-MM-DD` (one per expiration, in date order). Include in the body: the ATM strike (closest to the current share price), the highest-open-interest call strike, the highest-open-interest put strike, and the share price used.
3. Add a file `expirations.md` on a feature branch with the company snapshot, the full expiration list, and a per-expiration stats table.
4. Open a pull request from the feature branch into `main`.
5. After the PR is reviewable, add a minimal `CONTRIBUTING.md` to `main` and keep `expirations.md` Carter PR up to date with `main`.

## Automation

A minimal workflow (`.github/workflows/manual.yml`) is available on `main` and can be triggered manually via `workflow_dispatch`. It runs a single echo job. Run logs are deleted after each use to keep the repository tidy.

## Data notes

- All market figures must come from live data at the time of writing.
- Where a number looks odd, report exactly what the source returned rather than silently correcting it.
- Share price used for ATM determination: the AAPL last trade / regularMarketPrice from Yahoo Finance on the pull date.
