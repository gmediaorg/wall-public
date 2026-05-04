# Facts that change — re-verify before quoting

> Любой факт здесь имеет «срок годности». Перед тем как дать его в публичную коммуникацию (отзыв, пост, JSON-LD, press-FAQ) — проверь свежесть.
> Last verified column показывает когда последний раз сверено с прода.

| Factoid | Current value | Verify via | Last verified | Stale-rate |
|---|---|---|---|---|
| Language count | **17** native | `curl https://wall.tg/api/product \| jq '.languages.count'` | 2026-05-04 | high — i18n roadmap actively expanding |
| MAU / users count | see API | `.stats.users` from /api/product | live | hourly |
| Premium subscribers | see API | `.stats.premium_users` from /api/product | live | hourly |
| Public posts total | see API | `.stats.public_posts` from /api/product | live | hourly |
| Branches count | **18** (15 topic + 3 meta) | `.branches.count` from /api/product | 2026-05-04 | low — добавляются раз в месяц |
| AI agents count + names | **4: Grok, ChatGPT, DeepSeek, Claude** | `.features.ai_agents` from /api/product | 2026-05-04 | low — изменения раз в квартал |
| AI quotas (free / premium / ultra per-day) | 0 / 50 / 250 | `.features.ai_quotas` from /api/product | 2026-05-04 | medium |
| Premium / Ultra prices | 290⭐ / 990⭐ | `.pricing` from /api/product | 2026-05-04 | low — стабильно |
| Withdrawal status | **paused (open beta)** | `.features.creator_monetization.withdrawal_status` from /api/product | 2026-05-04 | high — Q2 2026 откроется |
| Chain Posts wallet (Wall side) | `UQA2Q0Vv81NObzw0d6jK6v9nnmc-cAzSI8kWN27Sl9n92SZp` | tonviewer.com — incoming Chain Post seal transactions visible publicly | 2026-05-04 | low — постоянная |
| First commit date | 2026-02-25 | `git log --reverse --format=%ai \| head -1` | 2026-05-04 | once-only (история) |
| Founding date claim (JSON-LD) | **2026-02** | grep `foundingDate` в публичных JSON-LD на canonical surfaces | 2026-05-04 | once-only (история) |
| Wall fee on TON post donations | **0%** (wallet-to-wallet, non-custodial) | https://wall.foundation/economics fee schedule | 2026-05-04 | low (правда) |
| Stars donation referrer % | tier-dependent **10–30%** (T1→T5) | https://wall.foundation/economics basis-point ladder | 2026-05-04 | medium — может корректироваться |

## Когда факт нужно re-verify

- **Каждое утро** — language count, MAU, posts, premium count
- **Перед публичной публикацией поста / отзыва** — все числовые факты
- **Перед press-pitch'ем журналисту** — ВСЁ из этой таблицы
- **После любого крупного шипа** — обнови соответствующие строки

## Как обновить state.json

Запросить `https://wall.tg/api/product` — там полный snapshot. Внутренний sync-скрипт обновляет state.json по cron'у; если делаешь вручную, держи структуру.

## Когда убрать факт из этого списка

Если факт стабилизировался (не меняется > 6 месяцев) → перенести в `state.json` как фиксированный, убрать из таблицы.
