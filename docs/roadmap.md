# Wall — Roadmap

> **Targets, not promises.** Public roadmap of where Wall is heading. Source of truth for date claims across our canonical surfaces. Last updated 2026-05-04.

---

## Shipped (2026 Q1–Q2 so far)

### 2026-02
- Initial commit (2026-02-25). MVP went from 0 to functional in ~3 weeks.
- TypeScript migration.
- TON wallet integration via TON Connect.
- Profile pages, posts, comments.

### 2026-03
- Pixel Battle (collaborative pixel canvas).
- 4 AI agents in feed (Grok, ChatGPT, DeepSeek, Claude).
- Telegram Stars payments.
- Premium / Ultra tiers (290⭐ / 990⭐).
- Multi-rail payments (CryptoBot, X-Rocket, KassaBot for RUB).

### 2026-04
- Chain Posts (TON blockchain anchoring).
- 18 official Branches (15 topic + 3 meta).
- 17 native UI languages.
- AI auto-translate via MyMemory + LLM chain.
- Wall Foundation site (wall.foundation).
- Help center (wall.support).
- Multi-platform launcher (wall.app).
- Brand canonical (wall.lu).
- Public API (`wall.tg/api/product`).

### 2026-05
- Founder bio page ([wall.foundation/founder](https://wall.foundation/founder)).
- Press room ([wall.support/press](https://wall.support/press)).
- Economics + Transparency canonical pages on Wall Foundation.
- Ad-network attribution infrastructure.
- Real Wall brick logo across all OG cards (editorial design refresh).
- Live-data dynamic OG endpoints powering share-preview cards.
- AI assistant context pack (`agents/dumov/`).
- This public mirror repo (gmediaorg/wall-public).

---

## In flight (2026 Q2)

### Beta exit + withdrawals
- Withdrawal flow exits beta.
- Stars + TON earnings become withdrawable on demand.

### Phase 4 + 5 i18n
- 6 new languages shipping: Kazakh, Azerbaijani, Hebrew, Georgian, Malay, Thai (→ 23 total).
- Phase 5: 10 more (→ 33 total) — covering 99%+ of Telegram audience-language distribution.

### Web auth via TON Connect
- Sign in with your TON wallet, no Telegram needed.
- For desktop/web access outside Telegram client.
- TonProof verification stack on the server side already exists; UX + session integration is the remaining work.

### Ad Network Phase 1
- Move UTM-attribution code from dev branch to production.
- Public publisher cabinet for channel admins.
- Self-serve campaign creation for ad buyers.

---

## Committed (2026 Q3)

- **Native iOS app** via App Store (StoreKit + payment compliance).
- **Native Android app** via Google Play (Billing + compliance).
- Both apps are wrappers around the existing Mini App with native payment plumbing.

---

## Committed (2026 Q4)

- **Discord integration** — Wall as a Discord bot for cross-platform communities.
- **Multi-chain expansion** — EVM chains (Ethereum, Polygon) for non-TON wallets.
- **NFT integration** — verify TON NFT ownership for profile badges; NFT-gated branches.
- **Chain Posts v2** — media on-chain (image+text), gas-optimized batch sealing.

---

## 2027

- **Governance experiments** — moderation policy votes, leaderboard tuning by community, revenue allocation decisions.
- **More G.media products** — TBA. The same multi-agent dev team that ships Wall is queued for next products.

---

## How this roadmap is updated

- Quarterly review by founder + key stakeholders.
- Single source: this file. Other surfaces (wall.foundation/roadmap, press materials) reference it.
- Changes are committed via PR with rationale in the commit message.
- "Shipped" items move from "in flight" to "shipped" only after they're live in production at wall.tg.

---

## Status legend

- **Shipped** — running in production at wall.tg
- **In flight** — actively being built, dev branch or staging
- **Committed** — funded + scoped, on the queue
- **Future** — directional, no fixed date

If a feature you care about is not on this list — file in [Discussions → Ideas](../../discussions/categories/ideas).
