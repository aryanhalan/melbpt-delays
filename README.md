# Melbourne Public Transport Delays
### FIT2179 Data Visualisation 2 — Aryan Halan — Monash University, Semester 1 2026

---

## About

This project analyses punctuality and reliability data across Melbourne's public transport network — metro trains, trams, V/Line regional trains, and metropolitan buses — from May 2025 to April 2026.

**Central question:** Is Melbourne's public transport network meeting its government punctuality targets, and where are the worst pain points?

**Key finding:** V/Line regional trains consistently miss their 92% punctuality target (sitting at 83.7% in April 2026), outer suburban metro lines have the highest cancellation counts, and December dips affect all modes. Metro Bus quietly outperforms every other mode.

---

## Data Sources

| # | Source | Publisher | URL |
|---|--------|-----------|-----|
| 1 | Monthly Network Performance Reports (May 2025 – Apr 2026) | Transport Victoria | https://www.vic.gov.au/public-transport-monthly-performance |
| 2 | Metro Train Line Performance Data | Transport Victoria Open Data | https://discover.data.vic.gov.au |

Both datasets are publicly available and published by the Victorian Government. No data wrangling was performed — all figures are taken directly from official published reports.

---

## Visualisations

There are 13 Vega-Lite visualisations across 5 sections. Each JSON spec is in the `/json` folder.

| File | Chart | Idiom | Section |
|------|-------|-------|---------|
| `c1_punctuality_by_mode.json` | Punctuality vs target, April 2026 | Lollipop chart | 01 — Overview |
| `c2_reliability_by_mode.json` | Reliability vs target, April 2026 | Lollipop chart | 01 — Overview |
| `c3_monthly_trends_all_modes.json` | 12-month punctuality all modes | Multi-line chart (interactive) | 02 — Monthly Trends |
| `c4_monthly_metro_train.json` | Metro Train monthly detail | Line + dot chart | 02 — Monthly Trends |
| `c5_monthly_metro_tram.json` | Metro Tram monthly detail | Line + dot chart | 02 — Monthly Trends |
| `c6_monthly_vline.json` | V/Line monthly detail | Line + dot chart | 02 — Monthly Trends |
| `c7_peak_punctuality_by_line.json` | Peak punctuality, 16 lines | Lollipop chart | 03 — Train Lines |
| `c8_annual_cancellations.json` | Annual cancellations by line | Horizontal bar chart | 03 — Train Lines |
| `c9_peak_vs_offpeak_scatter.json` | Peak vs off-peak comparison | Scatter plot | 03 — Train Lines |
| `c10_distance_vs_punctuality_bubble.json` | Distance from CBD vs punctuality | Bubble scatter chart | 04 — Geographic |
| `c11_target_achievement_heatmap.json` | Monthly target achievement | Heatmap | 05 — Analysis |
| `c12_year_on_year_change.json` | Year-on-year punctuality change | Horizontal bar chart | 05 — Analysis |
| `c13_avg_delay_by_line.json` | Average delay per late service | Colour-coded bar chart | 05 — Analysis |

---

## Repository Structure

```
melbpt-delays/
├── index.html          ← Main visualisation page (GitHub Pages entry point)
├── sketch.pdf          ← Hand-drawn sketch of layout (assignment requirement)
├── README.md           ← This file
└── json/
    ├── c1_punctuality_by_mode.json
    ├── c2_reliability_by_mode.json
    ├── c3_monthly_trends_all_modes.json
    ├── c4_monthly_metro_train.json
    ├── c5_monthly_metro_tram.json
    ├── c6_monthly_vline.json
    ├── c7_peak_punctuality_by_line.json
    ├── c8_annual_cancellations.json
    ├── c9_peak_vs_offpeak_scatter.json
    ├── c10_distance_vs_punctuality_bubble.json
    ├── c11_target_achievement_heatmap.json
    ├── c12_year_on_year_change.json
    └── c13_avg_delay_by_line.json
```

---

## Colour Conventions

| Mode | Colour |
|------|--------|
| Metro Train | Blue `#2563eb` |
| Metro Tram | Green `#16a34a` |
| V/Line (Regional Train) | Purple `#7c3aed` |
| Metro Bus | Orange `#ea580c` |

---

## Technologies

- **Vega-Lite v5** — all charts and maps
- **HTML / CSS** — page layout and typography
- **Google Fonts** — Source Serif 4, Source Sans 3
- **GitHub Pages** — hosting

---

## Author

**Aryan Halan**  
FIT2179 Data Visualisation 2  
Monash University, Clayton Campus  
Semester 1, 2026

---

## Acknowledgements

This visualisation was assisted by AI tools (Claude by Anthropic) for code generation and layout structure. All data, analysis, and design decisions are grounded in official Transport Victoria publications.

---


