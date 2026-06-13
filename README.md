# Steel — Materials Data Series #1

An interactive data dashboard + LinkedIn carousel on the world's most-used metal: who makes it, the kinds that exist, how their properties compare, and the race to make it clean.

Part of my **Materials Data Series** — one material at a time, told as a materials engineer turned data analyst. Next: aluminium, copper, rare earths.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard — 5 tabs: Production & Geography, **What 1.85 Bt Looks Like** (real-world scale), Kinds of Steel, Properties, The Green Steel Race |
| `fetch_data.py` | Reproducible Python pipeline — compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (production, trend, route split, EAF by region, end-use, grade properties) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080×1080) |
| `Steel_Materials_Carousel.pdf` | Exported carousel, ready to upload to LinkedIn |
| `linkedin-post.txt` | Post caption + hashtags |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same figures in JS (so it runs from `file://` with no server). `fetch_data.py` documents provenance and makes every number reproducible.

## Key findings

- **1,882.6 Mt** of crude steel made in 2024 → **1,849.4 Mt** in 2025 (down 1.8%).
- **Scale, made tangible:** 59 t/second → ~**183,000 Eiffel Towers**, ~**31,000 Empire State Buildings**, or ~**2 billion cars'** worth of steel per year.
- **China makes 53%** of the world's steel — more than every other country combined. **India** is the riser (+10% YoY, clear #2).
- Steel spans a **7.6× yield-strength range** (250 → 1,900 MPa) across its four families, driven mostly by carbon content + heat treatment.
- Steel is **~11% of global CO₂**. The coal route (BF-BOF, 70% of output) emits **2.2 t CO₂/t**; the electric scrap route (EAF) just **0.3 t** — but China is still ~90% coal-based.
- **93%** of new capacity announced in 2024 is the cleaner EAF route.

## Sources

World Steel Association (*World Steel in Figures 2025*; Dec-2024 & Dec-2025 production releases) · GMK Center · Carbon Brief · SteelWatch · ASM Metals Handbook / MatWeb (typical property values).

Property values are typical published datasheet figures for standard tempers — illustrative, not specification. Production figures rounded; attributed to worldsteel.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
