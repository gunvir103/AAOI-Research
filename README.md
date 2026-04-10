# AAOI Research Vault

> Deep-research notes on **Applied Optoelectronics, Inc.** (NASDAQ: **AAOI**) — a vertically integrated optical transceiver maker at the center of the 400G → 800G → 1.6T AI data-center upgrade cycle.

**Last refreshed:** April 9, 2026 (post-market) via the [Unusual Whales API](https://unusualwhales.com/) and primary sources (SEC filings, earnings calls, press releases, SCOTUS opinions).

---

## TL;DR

| | |
|---|---|
| **Price (close 4/9/26)** | **$136.05** (+30.9% in 3 sessions) |
| **Market cap** | **$10.02B** |
| **Beta / IV / IV Rank** | 3.9456 / 159.8% / **97.8%** (1Y max) |
| **Next earnings** | **May 14, 2026** — est. EPS -$0.10 |
| **FY2025 revenue** | $455.7M (+82.8% YoY) |
| **FY2026 guide** | **>$1B** (+120%) |
| **FY2025 GAAP EPS (diluted)** | -$0.64 |
| **Insider net selling (2025–26)** | **-$63.5M** (31 sells vs 4 buys) |
| **Analyst coverage** | Rosenblatt $140 (3% above spot), Needham $80, B. Riley $54, Northland $35 |

> [!important] Why this research exists
> AAOI is a **high-beta, high-volatility AI infrastructure play** priced for flawless 1.6T execution. The thesis is binary into May 14 earnings. This vault documents the bull/bear asymmetry, the options structure, insider behavior, geopolitical exposure, and competitor positioning in enough depth to trade the name with defined risk.

---

## Contents

| # | File | What it covers |
|---|------|----------------|
| 0 | [00-Index.md](./00-Index.md) | Dashboard, quick stats, relationship graph, IV term structure chart |
| 1 | [01-Company-Overview.md](./01-Company-Overview.md) | Snapshot, vertical integration stack, Amazon $4B warrant, price arc from $1.48 → $136.99 |
| 2 | [02-Technology-Edge.md](./02-Technology-Edge.md) | EML laser moat, 1.6T OSFP DR8 LPO specs, 349-patent portfolio, R&D profile, SiPh/CPO risk, NVIDIA gap |
| 3 | [03-Competitor-Analysis.md](./03-Competitor-Analysis.md) | COHR, LITE, FN, TSEM, InnoLight — financials, tech, insiders, valuation |
| 4 | [04-Financials-CapEx.md](./04-Financials-CapEx.md) | Revenue hockey stick, $179M CapEx, RORE, dilution, 6-analyst coverage, valuation framework |
| 5 | [05-Insiders-Board.md](./05-Insiders-Board.md) | Board bios, Thompson Lin founder story, full 2024–26 Form 4 timeline, monthly sell buckets |
| 6 | [06-Supply-Chain-Geopolitics.md](./06-Supply-Chain-Geopolitics.md) | Supply chain map, SCOTUS IEEPA ruling, gallium ban suspension, Section 301 status, Taiwan risk |
| 7 | [07-Options-Flow-Intelligence.md](./07-Options-Flow-Intelligence.md) | IV term structure, flow/premium snapshot, max pain, dealer greeks, earnings reaction history |
| 8 | [08-Bull-Bear-Outlook.md](./08-Bull-Bear-Outlook.md) | 3-month and 3-year scenario trees, hyperscaler CapEx backdrop, M&A comps, position sizing |

---

## Key charts and diagrams

The vault uses **Mermaid** for relationship graphs, scenario trees, mindmaps, and the IV-term-structure xychart, plus ASCII art for price history and ranking visualizations. All diagrams render natively on GitHub and in Obsidian.

- Vertical integration stack (file 01)
- Revenue segment pie (file 01)
- Manufacturing footprint map (file 01)
- Technology comparison matrix (file 02)
- Competitive ecosystem graph (file 03)
- CapEx hockey stick chart (file 04)
- Insider signal graph with monthly buckets (file 05)
- Supply chain map with geopolitical risk shading (file 06)
- IV term structure xychart (file 00 + file 07)
- Scenario decision tree (file 08)

---

## Method and sourcing

### Market data — Unusual Whales API
All live market data (price, beta, IV, IV rank, OI, flow, greeks, max pain, darkpool, insider aggregates, earnings history) was pulled on 2026-04-09 from the [Unusual Whales REST API](https://unusualwhales.com/). The canonical snapshot is preserved in the research notes for reproducibility.

Endpoints used (abbreviated):
- `/api/stock/AAOI/info`
- `/api/stock/AAOI/stock-state`
- `/api/stock/AAOI/options-volume`
- `/api/stock/AAOI/volatility/stats`
- `/api/stock/AAOI/volatility/term-structure`
- `/api/stock/AAOI/max-pain`
- `/api/stock/AAOI/expiry-breakdown`
- `/api/stock/AAOI/greek-exposure`
- `/api/stock/AAOI/oi-change`
- `/api/stock/AAOI/flow-recent`
- `/api/stock/AAOI/flow-alerts`
- `/api/stock/AAOI/earnings`
- `/api/stock/AAOI/insider-buy-sells`
- `/api/insider/AAOI/ticker-flow`
- `/api/darkpool/AAOI`
- Equivalent endpoints for peers: COHR, LITE, FN, TSEM

### Qualitative facts — primary sources
Non-market claims (patent counts, warrant terms, SCOTUS rulings, board composition, M&A precedents, competitor financials) were verified against:

- **SEC filings**: 10-K, 10-Q, DEF 14A, 8-K via [EDGAR](https://www.sec.gov/edgar)
- **Company press releases** via AAOI Investor Relations
- **Earnings call transcripts** (Q4 2025 reported 2026-02-26)
- **SCOTUS opinions** — [Learning Resources, Inc. v. Trump, 24-1287](https://www.supremecourt.gov/opinions/25pdf/24-1287_4gcj.pdf) (Feb 20, 2026)
- **Industry press** — CNBC, Bloomberg, CFR, White & Case, Fastmarkets, Seeking Alpha, GuruFocus
- **Analyst research** — Rosenblatt, Needham, B. Riley, Northland Capital

Unverified claims are inline-flagged with `<!-- needs verification -->` comments.

---

## Reading order

**If you have 5 minutes:** [00-Index](./00-Index.md) dashboard → [08-Bull-Bear-Outlook](./08-Bull-Bear-Outlook.md) bottom line

**If you have 30 minutes:** Index → 01-Overview → 07-Options-Flow → 08-Bull-Bear

**Full research pass:** Read in numerical order (00 → 08). Total length ~2,800 lines of markdown, ~30–45 minutes.

---

## Usage

### As an Obsidian vault
Clone this repo into your Obsidian vault. Internal `[[wikilinks]]` between files will resolve automatically. The files rely on core Obsidian features (callouts, internal links) plus the following community plugins used in the parent vault:

- `obsidian-tasks-plugin`
- `obsidian-kanban`
- `omnisearch`
- `obsidian-mind-map`
- Any Mermaid-capable markdown renderer

### As standalone markdown
All files render correctly on GitHub. Mermaid diagrams render in GitHub's markdown preview. ASCII art renders in any fixed-width code block.

### To refresh the data
Re-run the Unusual Whales API calls documented above with a valid token, then re-apply the canonical facts to each file. The agent-driven workflow used for the 2026-04-09 refresh is documented in this repo's commit history.

---

## Disclaimers

> [!warning] Not investment advice
> This vault is **personal research**, not investment advice. Every number in it can be wrong, stale, or misinterpreted. AAOI is a high-beta stock with a history of drawing down >90% (from $103 in 2017 to $1.48 in 2022). The author holds no fiduciary duty and nothing here should be construed as a recommendation to buy, sell, or hold any security. **Do your own research.** Size positions you can afford to lose completely.

> [!info] Data freshness
> Market data is only as current as the last API pull (2026-04-09 post-market). Options flow, insider activity, and price action can change within hours. Any trading decision requires re-pulling fresh data.

---

## License

All content © the repository owner. Shared publicly for transparency and learning. No warranty of any kind, express or implied.

---

## Tags

`#AAOI` `#optics` `#AI` `#datacenter` `#semiconductor` `#research` `#trading` `#options-flow`
