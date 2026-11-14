# W2-PM1: Footprinting with Multiple Kali Tools

**Target:** networkwalks.com (written permission secured)
**Environment:** Kali Linux

## Objective

Collect public information about a domain using six built-in Kali tools, to see what an attacker can learn without touching the target directly.

## Commands and findings

| # | Command | What it does | Finding |
|---|---------|--------------|---------|
| 1 | `whois networkwalks.com` | Reads the public registration record | Registrar, registration and expiry dates, name servers pointing to HostGator |
| 2 | `whatweb networkwalks.com` | Fingerprints web technologies | WordPress 7.0.4, WP Download Manager 3.3.58, server IP and an email address |
| 3 | `nslookup networkwalks.com` | Resolves the domain through DNS | 192.232.216.135 |
| 4 | `curl -I https://networkwalks.com` | Reads the HTTP response headers | Server and caching details, WordPress REST API at `/wp-json/` |
| 5 | `wafw00f networkwalks.com` | Detects a web application firewall | ModSecurity (SpiderLabs) |
| 6 | `dnsrecon -d networkwalks.com` | Enumerates DNS records | NS, MX, SPF/TXT and SRV records, BIND 9.16.23 |

> Check these values against your own output and edit any that differ.

## Why it matters

- The hosting provider, software versions and IP address tell an attacker where to look and what to test.
- Knowing a firewall is present lets an attacker plan around it.
- DNS records map out the email and hosting setup.

## How to reduce the exposure

Hide version banners and unneeded headers, keep software patched, use WHOIS privacy, and keep the WAF tuned.

## Evidence

Screenshots are in `screenshots/` and raw output is in `outputs/`.
