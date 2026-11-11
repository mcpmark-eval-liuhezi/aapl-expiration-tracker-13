# AAPL Options Expiration Tracker

Weekly tracking repository for Apple (AAPL) option expiration numbers, used ahead of the risk meeting.

All market figures below were pulled from **live Yahoo Finance data** on 2026-11-11 (regular market close, share price **$355.63**).

## Company Snapshot (Yahoo Finance profile)

| Field | Value |
| --- | --- |
| Company | Apple Inc. (AAPL) |
| Headquarters street address | One Apple Park Way, MS 927-4GC |
| City | Cupertino |
| State / ZIP | CA 95014 |
| Country | United States |
| Phone | (408) 996-1010 |
| Website | https://www.apple.com |
| Sector | Technology |
| Industry | Consumer Electronics |
| Current share price | **$355.63** (last trade / regularMarketPrice, 2026-11-11; previous close $348.51; day range $349.325–$355.90) |
| Exchange | NasdaqGS (NMS) |
| Market cap | ~$5.168T |
| Analyst rating | Buy (mean 2.2, 40 analysts; mean target $344.62, median $352.50, high $425, low $250) |
| 52-week range | $243.42 – $355.90 |
| 50-day avg / 200-day avg | $337.27 / $299.78 |

## Full List of Available Expiration Dates (as returned by Yahoo Finance)

| # | Expiration | Tenor |
| --- | --- | --- |
| 1 | **2026-11-11** | today (same-day) |
| 2 | **2026-11-13** | 2 days out |
| 3 | **2026-11-16** | 5 days out |
| 4 | 2026-11-18 | 7 days |
| 5 | 2026-11-20 | 9 days |
| 6 | 2026-11-27 | 16 days |
| 7 | 2026-12-04 | 23 days |
| 8 | 2026-12-11 | 30 days |
| 9 | 2026-12-18 | 37 days |
| 10 | 2026-12-24 | 43 days |
| 11 | 2027-01-15 | 63 days |
| 12 | 2027-02-19 | 84 days |
| 13 | 2027-03-19 | 105 days |
| 14 | 2027-04-16 | 123 days |
| 15 | 2027-06-17 | 182 days |
| 16 | 2027-09-17 | 274 days |
| 17 | 2027-12-17 | 396 days |
| 18 | 2028-01-21 | 458 days |
| 19 | 2028-03-17 | 510 days |
| 20 | 2028-06-16 | 590 days |
| 21 | 2028-12-15 | 730 days |
| 22 | 2029-01-19 | 784 days |

**Tracking scope for this week:** the three soonest expirations on/after today — **2026-11-11, 2026-11-13, and 2026-11-16**.

## Per-Expiration Chain Stats

Share price used for ATM determination across all three expirations: **$355.63** (AAPL last trade, 2026-11-11).

### Expiry 2026-11-11 (today)

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **355** (AAPL261111C00355000 / P00355000) |
| Highest-OI call strike | **355** (AAPL261111C00355000, OI 33,155; volume 183,356) |
| Highest-OI put strike | **340** (AAPL261111P00340000, OI 5,854) |
| Notable call OI | 350 (6,003), 357.5 (8,464), 360 (19,451) |
| Notable put OI | 342.5 (4,727), 345 (3,921), 350 (3,844) |

### Expiry 2026-11-13 (Tue)

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **355** (AAPL261113C00355000 / P00355000) |
| Highest-OI call strike | **355** (AAPL261113C00355000, OI 11,813; volume 24,754) |
| Highest-OI put strike | **340** (AAPL261113P00340000, OI 9,560) |
| Notable call OI | 360 (16,819), 365 (11,856), 350 (7,547) |
| Notable put OI | 322.5 (6,921), 325 (6,779), 330 (10,223) |

### Expiry 2026-11-16 (Tue)

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **355** (AAPL261116C00355000 / P00355000) |
| Highest-OI call strike | **355** (AAPL261116C00355000, OI 5,737; volume 2,541) |
| Highest-OI put strike | **330** (AAPL261116P00330000, OI 1,537) |
| Notable call OI | 355 (5,737) > 340 (417) > 350 (559) |
| Notable put OI | 330 (1,537) is the chain max; put OI is thin overall at this expiry |

## Summary Table

| Expiration | Share Price Used | ATM Strike | Top-OI Call | Top-OI Put |
| --- | --- | --- | --- | --- |
| 2026-11-11 | $355.63 | 355 | 355 (OI 33,155) | 340 (OI 5,854) |
| 2026-11-13 | $355.63 | 355 | 355 (OI 11,813) | 340 (OI 9,560) |
| 2026-11-16 | $355.63 | 355 | 355 (OI 5,737) | 330 (OI 1,537) |

## repo notes

- Tracking issues: #1 (Expiry 2026-11-11), #2 (Expiry 2026-11-13), #3 (Expiry 2026-11-16).
- This file was added on branch `add-expirations-md` and is proposed via pull request into `main`.
- A minimal `workflow_dispatch` workflow was added to `main` for manual runs (echo-only job); run logs are deleted after each use to keep the repo tidy.
- Discussion categories: none configured on this repository yet.
