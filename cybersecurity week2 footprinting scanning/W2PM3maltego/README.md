# W2-PM3: Footprinting with Maltego

**Target:** networkwalks.com (written permission secured)
**Environment:** Windows, Maltego Community Edition

## Objective

Install Maltego and use it to find the email addresses linked to a target domain.

## Steps

1. Downloaded Maltego from maltego.com and installed it on Windows.
2. Completed first-run setup and created a free Maltego account. Settings: Default System Browser, Privacy Mode Normal.
3. Added a **Domain** entity to the graph and renamed it `networkwalks.com`.
4. Right-clicked the entity, filtered for email-related transforms and ran them.

## Result

Maltego found [number] email addresses linked to the domain: [list them, or see the screenshot].

## Why it matters

Email addresses are targets for phishing and password attacks, and they hint at username formats used inside the organisation.

## How to reduce the exposure

Avoid showing staff emails in plain text on public pages, set up SPF, DKIM and DMARC, enable multi-factor authentication, and train staff to spot phishing.

## Evidence

Screenshots are in `screenshots/`.
