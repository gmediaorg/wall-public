# Security Policy

## Reporting a vulnerability

If you discover a security issue in **Wall** (the live product at [wall.tg](https://wall.tg)), please **do not file a public GitHub issue or discussion** in this repository.

This repository is a **public mirror** — it does not contain the application source. Reports filed here are visible to everyone and risk exploitation before we can patch.

### Where to report

| Severity | Channel | Response time |
|---|---|---|
| Critical (auth bypass, data exfiltration, payment exploit, account takeover) | Telegram DM to [@dumov](https://t.me/dumov) with subject `[security-critical]` | 24 hours |
| High (XSS, IDOR, CSRF, server-side issue) | Email **dumov@g.media** with subject `[security]` | 72 hours |
| Medium / low (info disclosure, rate-limit bypass, abuse vector) | Email **dumov@g.media** with subject `[security-low]` | 1 week |
| Issue inside this repo (broken link, stale fact, typo in docs) | [Open an Issue](../../issues) — public is fine | Best effort |

### What to include

- Affected URL, endpoint, or feature
- Reproducible steps (cURL / screenshots / code)
- Impact assessment (what an attacker could achieve)
- Your contact for follow-up
- (Optional) Suggested fix

### What we commit to

- Acknowledge receipt within the response time above.
- Investigate every report; provide updates at least weekly until closure.
- Credit you in our security advisories ([github.com/gmediaorg/wall-public/security/advisories](https://github.com/gmediaorg/wall-public/security/advisories)) — opt-in via your reply.
- Never threaten legal action against good-faith security research conducted within this policy.

### Out of scope

- Issues in third-party services we use (Telegram itself, TON network, Cloudflare, AWS S3, Upstash Redis) — report to the respective vendor.
- Social engineering, physical access, or denial-of-service from external networks.
- Issues in dependencies that don't affect Wall's deployed code.
- Theoretical vulnerabilities without proof of concept.

### Bounty

We don't run a formal bug bounty at this time (open beta). High-impact reports get public credit and a Wall Premium subscription gift. Critical reports may receive ad-hoc Stars or TON rewards at our discretion.

---

For non-security issues with the live product, use [wall.support/contact](https://wall.support/contact). For repo-content issues (typos, stale facts), use [Issues](../../issues).
