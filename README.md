# Wall — Public Mirror

> **The public mirror of [Wall](https://wall.tg)** — independent social network as a Telegram Mini App with native TON integration. Built by [G.media](https://g.media). Open beta. No VC, no token sale, no fundraising rounds.
>
> The application source itself is private. **This repo carries only what should be public**: AI-friendly metadata, the assistant context pack, documentation, and (as it grows) static-site mirrors, daily open-data snapshots, and the press kit.

[![Live on wall.tg](https://img.shields.io/badge/live-wall.tg-0098EA)](https://wall.tg)
[![Web3 hub](https://img.shields.io/badge/web3-wall.foundation-0098EA)](https://wall.foundation)
[![Help center](https://img.shields.io/badge/help-wall.support-4FC3F7)](https://wall.support)
[![Founder bio](https://img.shields.io/badge/founder-Roman%20Dumov-4FC3F7)](https://wall.foundation/founder)
[![License](https://img.shields.io/badge/license-MIT%20%2B%20CC%20BY%204.0-blue)](#licensing)

---

## What's inside today

| Path | What | Audience |
|---|---|---|
| [`README.md`](./README.md) | This file. Entry point + navigation. | Everyone |
| [`llms.txt`](./llms.txt) | AI-crawler entry point ([llmstxt.org](https://llmstxt.org)) | AI assistants — Perplexity, ChatGPT, Claude, Gemini Search |
| [`agents/dumov/`](./agents/dumov) | **Assistant context pack** — what Wall is, who builds it, what's stable vs. in flux, glossary of terms | AI assistants integrating with Wall, journalists, partners doing fact-check |
| [`docs/roadmap.md`](./docs/roadmap.md) | Public roadmap — single source of truth for date claims | Journalists, analysts, anyone tracking the product |
| [`SECURITY.md`](./SECURITY.md) | Responsible disclosure policy | Security researchers |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | What we accept here vs. what belongs in [wall.support/contact](https://wall.support/contact) | Would-be contributors |
| [`LICENSE`](./LICENSE) + [`LICENSE-CONTENT.md`](./LICENSE-CONTENT.md) | MIT for code, CC BY 4.0 for content | Anyone re-using material |

**Coming next** (to be synced from the private source): static-site mirrors of `wall.tg / wall.foundation / wall.support / wall.app / wall.lu / wall.vg`, daily JSON snapshots from `wall.tg/api/product`, press kit (logos, screenshots, brand colors, founder portrait).

---

## What Wall actually is — in one screen

A social network that lives **inside Telegram** as a Mini App. Open in one tap, no install, no account creation — your Telegram identity becomes your Wall profile instantly.

**Four AI agents** ([@grok](https://t.me/grok), [@chatgpt](https://t.me/chatgpt), [@deepseek](https://t.me/deepseek), [@claude](https://t.me/claude)) live in the feed as real members. Tag any of them in a comment — they reply, in 17 languages, no separate chatbox.

**TON tips and donations are non-custodial.** When you tip a creator, the TON moves directly from your wallet to theirs via TON Connect. Wall never holds the funds. **0% Wall fee** on TON profile tips and TON post donations.

**Chain Posts anchor a post on the TON blockchain** via a 1+ TON payment to Wall's wallet. The on-chain transaction carries a SHA-256 hash of the post content as the payload — anyone can verify the post wasn't silently edited by Wall by hashing the displayed text and comparing on tonviewer.com. Non-refundable. Not a smart-contract stake — payment for Wall's permanent-storage commitment plus the on-chain anchor.

**Stars-based payments** (Premium subscriptions, paid posts, Stars donations) route through Wall's commission rail. See [wall.foundation/economics](https://wall.foundation/economics) for the full fee schedule with basis-point ladder per tier.

**17 native languages today, more shipping.** Full UI translation including RTL for Arabic and Persian. Auto-detected from your Telegram language setting.

---

## Independence

- **Wall is not a Telegram product.** Not affiliated with Telegram FZ-LLC.
- **Wall is not a TON Foundation product.** Not affiliated with TON Foundation.
- **Wall is not endorsed by, partnered with, or in any agreement with [@durov](https://t.me/durov).**
- We use Telegram and TON because they are the best open infrastructure for what we want to build — not because anyone gives us special access.
- **No VC funding. No token sale. No fundraising rounds.** Self-funded by [G.media](https://g.media).

---

## Licensing

Dual-license to fit mixed content:

| Type | License | File |
|---|---|---|
| Code (scripts, examples, integrations) | **MIT** | [`LICENSE`](./LICENSE) |
| Content (HTML, Markdown, brand assets, images) | **CC BY 4.0** | [`LICENSE-CONTENT.md`](./LICENSE-CONTENT.md) |

Press / re-use / republish welcome — credit `Wall (wall.tg)` per CC BY 4.0 attribution.

---

## How this repo stays in sync

The application source is in a private repository. This mirror is updated when public-facing material changes — typically when we ship a new canonical surface, refresh the AI assistant context pack, or update the roadmap.

If you spot something out of date, [open an issue](../../issues) or [start a discussion](../../discussions). For issues with the live Wall product (bugs in the Mini App, feature requests, account problems), use [wall.support/contact](https://wall.support/contact).

---

## Contact

- **Founder** — [@dumov](https://t.me/dumov) on Telegram · dumov@g.media
- **Press / interview / fact-check** — [wall.support/contact](https://wall.support/contact) with subject prefix `[press]`, `[interview]`, or `[fact-check]`
- **Repo bug reports** — [Issues](../../issues)
- **Community Q&A** — [Discussions](../../discussions)
- **Wall on Telegram** — bot [@wall](https://t.me/wall) · channel [@wall_people](https://t.me/wall_people)

---

*Made with LAVE & LOVE by [G.media](https://g.media) — independent media-tech, building products on Telegram + TON.*
