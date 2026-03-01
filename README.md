# Redmetal Analytics

Copper market dashboard & mining stock analysis — real-time tracking of copper prices, mining stocks, futures, ETFs, and market catalysts.

![Dashboard Preview](preview.png)

## Features

- **Copper Spot Price** — COMEX HG front-month with interactive chart (1W–ALL timeframes)
- **Copper Miners** — Top movers including FCX, SCCO, TECK, BHP, RIO, HBM, ERO, TGB
- **Futures Curve** — COMEX HG contracts from front-month through Mar '27
- **ETFs & Funds** — COPX, CPER, ICOP, JCPB with expense ratios and AUM
- **Key Catalysts** — Market-moving events (Grasberg restart, AI demand, Section 232, etc.)
- **News Feed** — Latest copper & industrial metals headlines
- **SEC Filings** — Recent 10-K, 20-F, and 10-Q filings from copper producers

## Tech Stack

- Single-page HTML/CSS/JS (no build step)
- [Chart.js](https://www.chartjs.org/) for interactive charts
- Google Fonts (DM Sans + Playfair Display)
- Responsive design (mobile-friendly)

## Deployment

### GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` / `/ (root)`
4. Site will be live at `https://<username>.github.io/redmetal-analytics/`

### Any Static Host

Just serve `index.html` — no build process required. Works on Vercel, Netlify, Cloudflare Pages, etc.

## Data Sources

| Data | Source |
|------|--------|
| Spot Price | COMEX HG front-month; FRED API (PCOPPUSDM) |
| Stock Prices | Yahoo Finance, Finnhub, Twelve Data |
| Futures | COMEX copper futures (HG) |
| Supply/Demand | ICSG, USGS, Wood Mackenzie, J.P. Morgan Research |
| Miners Filings | SEC EDGAR 10-K/20-F, NI 43-101, JORC |
| Market Context | LME, SHFE, World Bureau of Metal Statistics |

> **Note:** Current version uses representative/simulated data. See [Roadmap](#roadmap) for live API integration plans.

## Roadmap

- [ ] Live spot price via FRED API or Finnhub
- [ ] Real-time stock prices via Yahoo Finance/Twelve Data
- [ ] Interactive mines map (Leaflet/Mapbox)
- [ ] Full investment thesis page
- [ ] SEC EDGAR filing scraper
- [ ] RSS/API news feed integration
- [ ] Supply/demand balance model
- [ ] Dark/light theme toggle

## License

MIT — see [LICENSE](LICENSE)

---

*This dashboard is for informational purposes only and should not be considered investment advice.*
