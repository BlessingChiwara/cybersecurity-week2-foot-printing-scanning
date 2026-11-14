# W2-PM4: Footprinting with theHarvester

**Target:** microsoft.com (public sources only, as set in the lab)
**Environment:** Kali Linux

## Objective

Collect email addresses, sub-domains and hosts from public sources without touching the target.

## Commands

| Task | Command | Result |
|------|---------|--------|
| 1: Baidu, limit 1000 | `theHarvester -d microsoft.com -l 1000 -b baidu` | [number] emails, [number] hosts |
| 2: all sources, limit 50 | `theHarvester -d microsoft.com -l 50 -b all` | [number] emails, [number] hosts |

Flags: `-d` target domain, `-l` limit on results, `-b` data source.

## Notes

- Different sources return different results, so it is worth trying more than one.
- Sources that need an API key may return nothing unless a key is configured. Never commit API keys to this repo.

## Why it matters

Each harvested email is a possible phishing target, and each sub-domain is another place an attacker can look for a way in.

## How to reduce the exposure

Keep an inventory of sub-domains, retire unused ones, and run the same tool against your own organisation.

## Evidence

Screenshots are in `screenshots/` and raw output is in `outputs/`.
