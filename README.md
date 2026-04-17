# U.S. Household Technology Adoption · 1900–Present

An interactive S-curve visualization of how 11 major technologies spread through American households from 1900 to the present. Built with D3.js as a single self-contained HTML file — no build step, no dependencies beyond a CDN.

**[Live Demo](https://www.perplexity.ai/computer/a/u-s-technology-adoption-timeli-4SfRYMIhQzGV22Hkr1dPgA)**

![Preview](preview.png)

---

## Features

- **11 S-curves** — Landline, Electricity, Radio, Automobile, Color TV, PC, Internet, Smartphone, Social Media, Streaming Video, Gen AI
- **Toggle individual technologies** on/off via the left sidebar
- **Linear / Logarithmic scale** toggle — log scale makes acceleration in modern tech strikingly visible
- **Relative Years mode** — aligns all curves at their 10% adoption point for direct S-curve steepness comparison
- **Adoption Speed panel** — horizontal bar at bottom ranks each technology by years from 10% → 50% penetration
- **Historical annotations** — clickable event pills (WWI, Great Depression, WWII, Post-War Boom, iPhone launch, ChatGPT launch, etc.)
- **Hover tooltip** — shows all active technologies' adoption % at any given year
- **Light / Dark mode** toggle

---

## Usage

Open `index.html` directly in any modern browser. No server required.

```bash
open index.html
```

Or serve locally:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

## Data Sources

All data represents **percentage of U.S. households** (or U.S. adults, where noted) using the given technology. Sources below by technology:

### 1. Landline Telephone
- **Comin & Hobijn (2004)** — NBER Working Paper No. 10452. Technology diffusion dataset covering U.S. household telephone penetration 1903–2005.
  - https://www.nber.org/papers/w10452
- **Our World in Data** — "Share of United States households using specific technologies" (processed from Comin & Hobijn + CDC NHIS for post-2009 decline data).
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 2. Electricity
- **Comin & Hobijn (2004)** — NBER Working Paper No. 10452. U.S. household electrification 1908–1960.
  - https://www.nber.org/papers/w10452
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 3. Radio
- **Comin & Hobijn (2004)** — NBER Working Paper No. 10452. U.S. household radio ownership 1925–2005.
  - https://www.nber.org/papers/w10452
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 4. Automobile
- **Comin & Hobijn (2004)** — NBER Working Paper No. 10452. U.S. household automobile ownership 1915–2005.
  - https://www.nber.org/papers/w10452
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 5. Color Television
- **Comin & Hobijn (2004)** — NBER Working Paper No. 10452. U.S. household color TV ownership 1966–2005.
  - https://www.nber.org/papers/w10452
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 6. Personal Computer
- **Comin & Hobijn (2004)** + **Horace Dediu (Asymco)** — Microcomputer/PC household data 1984–2016.
  - https://www.nber.org/papers/w10452
  - http://www.asymco.com
- **U.S. Census Bureau / NTIA** — "Falling Through the Net" series; household computer ownership surveys 1994–2010.
  - https://www.ntia.gov/data/digital-nation-data-explorer
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 7. Internet
- **NTIA / U.S. Census Bureau** — "Falling Through the Net: Toward Digital Inclusion" (2000) and subsequent Digital Nation reports. Household internet access 1993–2016.
  - https://www.ntia.gov/sites/default/files/data/fttn00/falling.htm
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 8. Smartphone
- **Pew Research Center** — "Mobile Technology and Home Broadband" surveys. U.S. adult smartphone ownership 2011–2019.
  - https://www.pewresearch.org/internet/fact-sheet/mobile/
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 9. Social Media
- **Pew Research Center** — "Social Media Use Over Time" fact sheet. U.S. adult social media usage 2005–2019.
  - https://www.pewresearch.org/internet/fact-sheet/social-media/
- **Our World in Data** — "Share of United States households using specific technologies."
  - https://ourworldindata.org/grapher/technology-adoption-by-households-in-the-united-states

### 10. Streaming Video
- **Parks Associates** — "OTT Video Market Tracker." U.S. household streaming subscription penetration 2015–2025.
  - https://www.parksassociates.com
- **Exploding Topics / Nielsen** — Historical streaming subscription data by household, 2015–2023.
  - https://explodingtopics.com/blog/video-streaming-stats
- **Pew Research Center** — "83% of U.S. adults use streaming services, far fewer subscribe to cable or satellite TV" (July 2025).
  - https://www.pewresearch.org/short-reads/2025/07/01/83-of-us-adults-use-streaming-services-far-fewer-subscribe-to-cable-or-satellite-tv/
- **Nielsen** — "U.S. TV Household Data Reveals Shifting Trends" (2024). Connected TV and streaming usage trends.
  - https://www.nielsen.com/insights/2024/u-s-tv-household-data-reveals-shifting-trends-in-how-audiences-access-content/

### 11. Generative AI (ChatGPT+)
- **S&P Global Market Intelligence / Kagan** — "U.S. Consumer Insights" surveys on generative AI tool adoption. U.S. internet adult usage 2024–2025.
  - https://www.spglobal.com/market-intelligence/en/news-insights/research/2025/11/adoption-of-generative-ai-tools-is-skyrocketing-in-the-us-led-by-chatgpt
- **Pew Research Center** — "ChatGPT use among Americans roughly doubled since 2023" (June 2025). U.S. adult ChatGPT usage 2023–2025.
  - https://www.pewresearch.org/short-reads/2025/06/25/34-of-us-adults-have-used-chatgpt-about-double-the-share-in-2023/
- **ScienceDirect / World Development** — "Who on earth is using Generative AI?" (2024). U.S. adult ChatGPT usage, February 2024.
  - https://www.sciencedirect.com/science/article/abs/pii/S0305750X25003468
- **Brookings Institution** — "How are Americans using AI? Evidence from a nationwide survey" (November 2025).
  - https://www.brookings.edu/articles/how-are-americans-using-ai-evidence-from-a-nationwide-survey/

---

## Notes on Methodology

- All figures represent **household or adult population penetration** (%), not new unit sales share.
- For Gen AI, figures represent U.S. adults who have *ever used* a generative AI tool (ChatGPT, Gemini, Copilot, etc.), sourced from survey data. This is a broader measure than daily active use.
- For Streaming Video, figures represent U.S. households subscribing to at least one paid streaming video service.
- A `0%` anchor point is prepended at each technology's commercial launch year to show the full S-curve from the baseline.
- Data gaps between survey years are interpolated using D3's Catmull-Rom spline.

---

## Tech Stack

- **D3.js v7** — scales, axes, line generation, mouse interaction
- **DM Sans + DM Mono** (Google Fonts) — typography
- Vanilla HTML/CSS/JS — single file, no bundler, no framework

---

## License

MIT
