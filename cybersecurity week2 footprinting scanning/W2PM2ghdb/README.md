# W2-PM2: Footprinting with the Google Hacking Database (GHDB)

**Environment:** Web browser, Google search

## Objective

Use search dorks (advanced Google operators such as `intitle:`, `inurl:` and `"index of"`) to find information that was never meant to be easy to find.

## Tasks

1. Find 10 security camera interfaces that are exposed to the Internet.
2. Find 10 open directory listings that offer mathematics ebooks as PDF files.

## Dorks used

| Task | Dork | Number of results recorded |
|------|------|----------------------------|
| Exposed cameras | [your dork] | [number] |
| Mathematics ebooks | [your dork] | [number] |

## Notes

- The links and any credentials found are recorded in the full report, not in this repo. The camera feeds belong to third parties and should not be republished.
- Results were found with search-engine queries only. No exploitation was performed.

## Why it matters

Misconfigured devices and open folders get indexed by search engines, so anyone can find them with a single query. Defenders can run the same dorks against their own domains to see what is exposed.

## How to reduce the exposure

Keep cameras off the public Internet (use a VPN), change default passwords, disable directory listing, and keep sensitive folders out of search indexes.
