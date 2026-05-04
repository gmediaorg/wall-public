# Contributing to Wall — Public Mirror

Thanks for considering a contribution. This repo is a **public mirror** of [Wall](https://wall.tg) — the actual application source is private. So contributions here are limited to what the mirror contains:

- Static HTML for our canonical surfaces (`sites/`)
- AI assistant context pack (`agents/dumov/`)
- Documentation (`docs/`)
- Press kit / brand assets (`press-kit/`)
- Open-data snapshots (`data/`)
- This README, license files, etc.

## What we accept

| Contribution type | How to submit |
|---|---|
| **Typo / grammar fix** in any Markdown or HTML | Open a PR directly — fast merge |
| **Stale fact correction** (the live product changed but the mirror hasn't) | Open an Issue with the source-of-truth URL (e.g. `wall.tg/api/product`) |
| **Translation** of static HTML or Markdown into a new language | Open an Issue first to coordinate (we have specific i18n process) |
| **Documentation expansion** (new how-to, deeper architecture explanation) | Discuss in [Discussions](../../discussions) first to avoid duplicating Wall-internal docs |
| **Press kit additions** (better screenshots, alternate logo backgrounds) | Open a PR with the file + license attribution |
| **AI integration example** (TypeScript / Python client for `wall.tg/api/product`) | Open a PR with code in `examples/` *(folder coming)* |
| **llms.txt improvement** | Open a PR — clear use case in the description |

## What we DON'T accept here

| Won't merge | Where to file instead |
|---|---|
| Bug in the live Wall app (anything you experience inside Telegram) | [wall.support/contact](https://wall.support/contact) with subject `[bug]` |
| Feature request for the Wall product itself | [Discussions → Ideas](../../discussions) OR [wall.support/contact](https://wall.support/contact) with subject `[feature-request]` |
| Security vulnerability | See [SECURITY.md](./SECURITY.md) — DO NOT post publicly |
| Refactoring of internal code | Repo doesn't contain it; nothing to refactor here |
| Adding a fundraising / sponsorship link | We declared **no VC, no token sale, no fundraising** — won't merge |

## How to submit a PR

1. Fork the repo
2. Create a branch with a short descriptive name: `fix/typo-readme-line-42` or `docs/add-roadmap-q3`
3. Make your change in a single commit (squash extras yourself)
4. Run any prebuild checks if you touched scripts (none for content-only PRs)
5. Open the PR with:
   - **Title**: imperative present tense — "Fix typo in README" not "Fixed typo"
   - **Body**: what + why (1-3 sentences). For fact corrections, include source URL.
6. We aim to review within 72 hours

## Style notes

- **English** is the default for all public-facing content. Russian translations live alongside (`<span class="i18n-en">` and `<span class="i18n-ru">` in HTML).
- **Markdown** uses ATX headings (`#`, `##`), no setext.
- **No emojis in technical docs** unless they carry semantic meaning (e.g. status indicators in tables).
- **Truth-check** before submitting fact-related PRs — verify against [`wall.tg/api/product`](https://wall.tg/api/product) which is our single source of truth for live numbers.
- **Don't add tracking** — no Google Analytics, no Facebook Pixel, no third-party tracking scripts. Wall has first-party analytics only.

## Who reviews

PRs reviewed by [@MrDumov](https://github.com/MrDumov) (founder, final say on content + brand). Wall's dev workflow uses both human and AI contributors — when an AI agent participates in a review or commit, attribution is signed via `Co-Authored-By:` line in git, so you'll see who participated.

## Code of conduct

Be kind. Be specific. Don't spam. We reserve the right to close + lock any thread that doesn't constructively engage.

For full Wall community standards, see [wall.tg/content-policy](https://wall.tg/content-policy).

---

Thanks for caring about the details. Wall is built brick by brick — your typo fix is a brick.
