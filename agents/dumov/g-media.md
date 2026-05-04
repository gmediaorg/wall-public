# G.media — parent entity

> Single source of truth describing G.media. Used by Wall's canonical surfaces (referenced from JSON-LD + footer + press FAQ) and intended to be importable into the g.media surface itself. Edit here → distribute to both contours.

---

## Identity

- **Name:** G.media
- **Type:** Independent media-tech company
- **Domain:** [g.media](https://g.media)
- **Founded:** 2024 (active product shipping started 2026-02 with Wall)
- **Founder:** Roman Dumov ([@dumov](https://t.me/dumov))
- **Mission:** Build media-tech products on top of Telegram + TON — independent, non-custodial, builder-owned.

## Schema.org Organization (JSON-LD format — copy into any g.media page)

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "@id": "https://g.media/#organization",
  "name": "G.media",
  "alternateName": ["G.media", "G media"],
  "url": "https://g.media",
  "founder": {
    "@type": "Person",
    "@id": "https://wall.tg/u/dumov#person",
    "name": "Roman Dumov",
    "alternateName": "@dumov",
    "url": "https://t.me/dumov"
  },
  "subOrganization": [
    {
      "@type": "Organization",
      "@id": "https://wall.tg/#organization",
      "name": "Wall",
      "url": "https://wall.tg",
      "description": "Social Mini App on Telegram + TON. G.media's flagship product."
    }
  ],
  "sameAs": [
    "https://wall.tg",
    "https://wall.foundation",
    "https://wall.support",
    "https://wall.app"
  ],
  "knowsAbout": [
    "Telegram Mini Apps",
    "TON Blockchain",
    "Independent Social Media",
    "Non-Custodial Crypto Tipping",
    "AI Agent Integration"
  ]
}
```

## Reciprocal relationship with Wall

- **G.media → Wall:** parent of flagship product. G.media should reference Wall as `subOrganization` in its JSON-LD.
- **Wall → G.media:** `founder` of `Organization` schema. All Wall canonical surfaces (wall.tg, wall.app, wall.support, wall.foundation, wall.lu, wall.vg) include `"founder": { "name": "G.media", "url": "https://g.media" }` in JSON-LD.

## Products portfolio

| Product | Status | URL | Role |
|---|---|---|---|
| Wall | open beta (since 2026-02) | https://wall.tg | flagship — social Mini App on Telegram + TON |

Future products will be added here as they launch.

## Cross-linking strategy

### From Wall surfaces (in place)

- Footer "Part of G.media ecosystem" with UTM-tagged outbound link.
- JSON-LD `Organization.founder` references G.media on every canonical Wall page.
- `disambiguatingDescription` mentions "Built independently by G.media" on key Wall surfaces.
- Press FAQ has explicit Q&A about the relationship: https://wall.support/press.

### From G.media surface (to implement)

- "Our products" section listing Wall as flagship with one-line description + Open button.
- JSON-LD `subOrganization` referencing Wall's `@id`.
- llms.txt entry on g.media that points AI crawlers to Wall as the active product.
- Cross-domain `sameAs` array linking back to Wall canonical URLs.

## Tone & voice (consistent across G.media + Wall)

- **Independent, builder-first** — never "ecosystem partner", never "powered by".
- **Open infrastructure, not extractive** — we use Telegram + TON because they're the best open rails.
- **No VC, no token sale, no fundraising rounds.** Self-funded, self-published.
- **Transparent attribution** — every commit signed; AI agents commit under their own `Co-Authored-By:` attribution.

## Press / business contact

- General: dumov@g.media
- Telegram: [@dumov](https://t.me/dumov)
- For Wall-specific: https://wall.support/contact (subject prefixes: `[interview]`, `[press]`, `[business]`, `[fact-check]`)

## What G.media is NOT (disambiguation)

- NOT a media outlet (not a publisher, not a journalism company).
- NOT a marketing agency.
- NOT a venture studio (we don't take outside money).
- NOT affiliated with any of: Telegram FZ-LLC, TON Foundation, Pavel Durov, Meta, Google, Yandex, VK.
- NOT to be confused with G Suite (Google) or other companies of similar name.

## Roadmap (G.media-level, multi-product)

| Quarter | Initiative |
|---|---|
| 2026 Q2 | Wall: beta exit + withdrawals open · web auth via TON |
| 2026 Q3 | Wall: native iOS app (App Store) + Android app (Google Play) |
| 2026 Q4 | Wall: Discord integration · multi-chain expansion (EVM) · NFT integration |
| 2027 | Wall: governance experiments. New G.media products: to be announced |

Updated as we go. Source of truth: this file. Wall-specific roadmap also lives at https://wall.foundation/roadmap.
