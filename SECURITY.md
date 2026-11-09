# Security Policy

## Project status

This project is **complete and unmaintained**. It will not receive
further modifications or security patches. Please keep this in mind
before reporting issues.

## Reporting a vulnerability

If you believe you have found a genuine security issue, please report it
privately via [GitHub Security Advisories](https://github.com/GHub942/LeaveDiscord/security/advisories/new)
or by contacting the maintainer directly. Do not open public issues for
vulnerabilities.

## Scope

This is a **static, client-side HTML page** with no server, no backend,
no database, and no user data collection. Its attack surface is
intentionally small. Please report:

- Any way the page could be made to execute untrusted script or inject
  content beyond its own inline code (e.g. via a crafted URL or hash value).
- Any external resource the page loads that isn't the two declared font
  hosts (`fonts.googleapis.com`, `fonts.gstatic.com`).
- Any factual error presented as a security claim (for example, a service
  described as end-to-end encrypted when it is not) — these affect real
  decisions people make about their privacy and safety.

Out of scope: the security posture of the third-party services listed on
the page (Discord, Proton Meet, SimpleX, and the others) — please report
those directly to their own teams.

## What to expect

This is a small, volunteer-maintained static site and it is now frozen.
There is no formal SLA and response times are not guaranteed. Reports
will be read, but fixes are unlikely since the project is complete.
