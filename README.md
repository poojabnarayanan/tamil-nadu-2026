# Tamil Nadu Assembly Election Analysis (2021 vs 2026)

## Political Shifts, Electoral Competitiveness & Fragmentation Analysis

### Domain
Political Analytics | Election Data Storytelling | Data Visualization

> Developed as part of the Codebasics Resume Challenge 

---

# 📑 Table of Contents

- Project Overview
- Problem Statement
- Research Objectives
- Data Source & Neutrality Standards
- Dataset Information
- Data Cleaning & Preparation
- Tools & Technologies
- Alliance Classification
- Key Storylines & Findings
- Dashboard & Visualization Highlights
- Editorial Recommendations
- Reproduction Steps
- Limitations & Methodology
- Future Enhancements
- Repository Structure
- Conclusion

---

# 📌 Project Overview

This project analyzes the Tamil Nadu Legislative Assembly Elections of 2021 and 2026 using constituency-level election data sourced from the Election Commission of India (ECI).

Using Python, Pandas, and Power BI, the project transforms raw election data into an interactive storytelling-driven analytics dashboard focused on:

- political shifts,
- competitiveness,
- fragmentation,
- regional trends,
- alliance transitions.

---

# 🎯 Problem Statement

AtliQ Media aims to build a data-driven election storytelling presentation that uses only public Election Commission of India (ECI) data to understand how Tamil Nadu’s political landscape evolved between the 2021 and 2026 Assembly Elections.

---

# 🔍 Research Objectives

## 1️⃣ Regional Electoral Shifts
Analyze how seat distribution changed across Tamil Nadu’s six regions between 2021 and 2026, and identify where major political formations gained or lost ground.

## 2️⃣ Constituency-Level Winner Transitions
Identify constituencies where the winning party changed between elections and visualize alliance-level seat transfers to understand emerging electoral patterns.

## 3️⃣ Electoral Competitiveness & Mandate Strength
Examine changes in victory margins and winner vote-share distribution to assess how electoral competitiveness and fragmentation evolved between 2021 and 2026.

---

# 📂 Data Source & Neutrality Standards

## Data Source

### Primary Source
Publicly available Election Commission of India (ECI) data.

---

## Neutrality Standards

- No exit polls or opinion surveys were used.
- No political commentary or causal assumptions were made.
- All insights are based strictly on election result data.
- Visualizations and titles were designed to remain politically neutral.

---

# 🧾 Dataset Information

## Files Used

### `tn_2021_results.csv`
Candidate-level results for the 2021 Tamil Nadu Assembly Election.

### `tn_2026_results.csv`
Candidate-level results for the 2026 Tamil Nadu Assembly Election.

### `constituency_master.csv`
Master reference table containing:
- district mapping,
- regional classification,
- reservation status.

---

# 🧹 Data Cleaning & Preparation

- Checked and validated null values.
- Verified duplicate constituency mappings.
- Used `ac_number` as the primary joining key.
- Created alliance classification mappings.
- Calculated constituency-level winners and margins.
- Derived vote share percentages.
- Generated flipped constituency indicators.
- Aggregated region-wise metrics and KPIs.

---

# 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data Cleaning & Processing |
| Pandas | Analysis & Transformation |
| Power BI, Canva | Charts, Dashboarding & Storytelling |
| MS PowerPoint | Presentation Design |

---

# 🏛️ Alliance Classification

## 2021

### DMK+
- DMK
- INC
- CPI
- CPI(M)
- VCK

### AIADMK+
- AIADMK
- BJP
- PMK

---

## 2026

### DMK+
- DMK
- INC
- CPI
- CPI(M)
- DMDK
- IUML
- VCK

### AIADMK+
- AIADMK
- BJP
- PMK
- AMMK

### Others
- TVK

---

# 📖 Key Storylines & Findings

## Story 1: The Tri-Polar Realignment

The 2026 election reflected a transition from a traditional bipolar contest toward a more competitive tri-polar political landscape.
This shift resulted in major seat redistribution across regions, particularly in Chennai Metro, where the DMK alliance declined sharply from 32 seats in 2021 to just 2 seats in 2026.

---

## Story 2: The Great Flip
A large-scale redistribution of political control occurred across constituencies. Using Sankey-style transition analysis, the project tracks how constituencies previously held by the two major alliances shifted toward emerging political formations such as TVK.
The South region emerged as the highest-volatility zone with the greatest number of flipped constituencies.

---

## Story 3: Extinction of the Landslide
The rise of multi-cornered contests significantly reduced dominant victories across the state.

### Key Findings
Landslide victories (>50% vote share) declined from 70 constituencies in 2021 to just 13 in 2026.
Fragmented victories (<35% vote share) increased sharply from 2 constituencies to 64.
Average victory margins narrowed in 5 out of 6 regions.
Several historically safe constituencies became highly competitive contests.


---

# 📊 Dashboard & Visualization Highlights

## 🗺️ Constituency Flip Map
Visualized constituencies that changed winning party between elections.

## 🔀 Sankey Diagram
Tracked alliance-level seat transitions between 2021 and 2026.

## 📉 Margin Competitiveness Analysis
Compared average victory margins region-wise across elections.

## 📊 Fragmentation Analysis
Categorized constituencies based on winner vote share:
- >50%
- 35–50%
- <35%

## 📍 Regional Analysis
Compared electoral patterns across:
- Chennai Metro
- North
- Central
- Kongu
- Delta
- South

---

# 📰 Editorial Recommendations

- Focus the narrative on rising multi-party competition.
- Use regional comparisons to explain shifting political control.
- Highlight flipped constituencies as indicators of volatility.
- Emphasize narrowing margins and declining safe seats.
- Use vote-share distribution to explain fragmentation.
- Combine statewide trends with constituency-level examples.
- Maintain a neutral, data-driven storytelling approach.
- Attribute insights strictly to official ECI data.

---

# 🗞️ Headline

> The 2026 election marks the end of the decisive mandate in Tamil Nadu, shifting from a bipolar state to a fragmented tri-polar landscape where traditional strongholds have collapsed and seats are now won with record-low vote shares.

---

# 🔁 Reproduction Steps

## 1️⃣ Clone Repository

```bash
git clone https://github.com/poojabnarayanan/tamil-nadu-2026
```

---

## 2️⃣ Process Data

Run the Jupyter Notebook to:
- clean raw ECI data,
- map alliances,
- calculate margins,
- generate flipped constituency tables.

---

## 3️⃣ Load Power BI Dashboard

Open the `.pbix` dashboard file and update data source paths to the cleaned CSV outputs.

---

# ⚠️ Limitations & Methodology

## Scope
The analysis is limited to the constituencies available in the ECI dataset.

## Neutrality
No causal political interpretations are provided, maintaining a non-partisan analytical approach.

## Data Key
`ac_number` was used as the primary joining key to avoid duplicate constituency-name mismatches.

Alliance mappings are editorial classifications created for analysis.

---

## Analytical Limitations

- Dataset explains outcomes, not voter motivations.
- No demographic or booth-level data available.
- 2026 results are based on live ECI data and may differ slightly from final audited Form-20 data.

---

# 🚀 Future Enhancements

Possible future extensions include:
- Booth-level analysis
- Historical election comparisons
- Swing analysis
- Sentiment analysis integration
- Interactive drillthrough dashboards

---

# 📂 Repository Structure

```text
📁 Data
├── tn_2021_results.csv
├── tn_2026_results.csv
└── constituency_master.csv

📁 Notebooks
└── election_analysis.ipynb

📁 Dahboard
└── tn_election_dashboard.pbix

📁 presentation
└── TN_Election_Analysis_Presentation.pdf
└── TN_Election_Analysis_Presentation.pptx

📁 DashboardPreview
└── intropage.png
└── flipanalysis.png
└── competitionanalysis.png

README.md
```

---

# 📷 Dashboard Preview


<img width="1920" height="1200" alt="intropage" src="https://github.com/user-attachments/assets/e779bee3-077a-4916-becf-b49d37ec5986" />

<img width="1920" height="1200" alt="flipanalysis" src="https://github.com/user-attachments/assets/5bbd66e2-9b2a-42db-a9d0-e3badf249a12" />

<img width="1920" height="1200" alt="competitionanalysis" src="https://github.com/user-attachments/assets/4d2457e2-e910-4991-ac14-e284740d436a" />



[Link to dashboard]https://app.powerbi.com/view?r=eyJrIjoiMzBhZGI5M2YtZjQwZS00ZDY1LWI4NTctYjllMzU2MWVjNGUzIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=c3bcb22fa7ac596d5a79 

---

# 📹 Video Walkthrough

[Link]https://drive.google.com/file/d/1sr63ZfPr-MpOkiJWt6ragVVxwLd-HH1g/view 

---

# 📌 Conclusion

This project combines election analytics, storytelling, and visualization to examine how Tamil Nadu’s political landscape evolved between 2021 and 2026.

Rather than focusing only on seat counts, the analysis explores how competitiveness, fragmentation, and constituency-level shifts collectively reshaped the electoral environment across the state.

