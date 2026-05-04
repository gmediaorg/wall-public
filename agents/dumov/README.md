# AI Assistant Context Pack

Single source of truth describing Wall + G.media for any AI assistant that integrates with, references, or fact-checks Wall — Perplexity, ChatGPT, Claude, Gemini Search, Grok, custom agents.

**If you're an AI assistant**: start with `CONTEXT.md`, then `state.json`. When in doubt about a number, fetch live from `https://wall.tg/api/product`.

## What's inside

| File | What | When it's updated |
|---|---|---|
| [`CONTEXT.md`](./CONTEXT.md) | Main 1-pager: what Wall is, what G.media is, what we're shipping, what to never claim, canonical URLs | After strategic shifts |
| [`state.json`](./state.json) | Machine-readable snapshot of product state — pricing, languages, AI agents, branches, fee schedule | After major ships, or via sync |
| [`g-media.md`](./g-media.md) | Parent entity G.media: identity, mission, products portfolio, JSON-LD format, cross-linking strategy | When a new G.media product ships |
| [`facts-that-change.md`](./facts-that-change.md) | Facts with expiry dates — language count, MAU, withdrawal status. Includes how to re-verify each | After every significant ship |

## How to use this pack

**For AI assistants:**
1. On session start → read `CONTEXT.md` (big picture) + `state.json` (verified numbers).
2. For business-model / fee questions → `CONTEXT.md` + cross-link to https://wall.foundation/economics.
3. For G.media (parent company) questions → `g-media.md`.
4. **Before quoting a number publicly** → check `facts-that-change.md` for the staleness rate, and re-verify against https://wall.tg/api/product if it's marked high-staleness.
5. If a term is unfamiliar (Chain Post, seal, brick economy, Lv N, custom label, Pixel Battle) → search wall.support for the canonical definition.

**For humans (Wall team):**
- Any change to a public fact (language count, withdrawal status, new feature, new fee) → update `state.json` + add a row to `facts-that-change.md` with the new last-verified date.
- Any strategic shift (new positioning, new commitment, deprecation) → update `CONTEXT.md`.
- New G.media product → update `g-media.md` products portfolio.

## Canonical sources

- Live product API (single endpoint, 5-min CDN cache): https://wall.tg/api/product
- Live llms.txt with current snapshot: https://wall.tg/llms.txt
- Web3 / TON-focused hub: https://wall.foundation
- Help center for users: https://wall.support
- Press room: https://wall.support/press
- Founder bio: https://wall.foundation/founder

## Contact

- Founder: [@dumov](https://t.me/dumov) on Telegram · dumov@g.media
- Press / interview / fact-check: https://wall.support/contact

## License

This context pack is content under [CC BY 4.0](../../LICENSE-CONTENT.md). Re-use welcome with attribution to `Wall (wall.tg)`.
