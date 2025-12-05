📊 Portuguese Public Contracts Analysis (2018–2025)

This project analyzes the evolution of Portuguese public contracts from 2018 to 2025, focusing on contract value behavior, inflation comparison, regional inequalities, sector trends, PRR impact, and the effects of major events such as COVID-19 and the Ukraine War.

Developed as part of Programming for Data Science — NOVA IMS (2025).

⭐ Project Highlights

🔎 Integrated 1M+ public contract records from multiple sources

🧹 Standardized and cleaned datasets with inconsistent formats

🏷️ Mapped CPV codes → macro categories to analyze spending sectors

📈 Compared YoY contract value growth vs. inflation

🌍 Assessed regional disparities in public spending

🏢 Identified companies with strongest contract growth

🟦 Evaluated PRR’s role in recent public spending

📉 Measured the influence of COVID-19 and the Ukraine War

🔧 Tech Stack

Python

pandas, numpy

matplotlib, seaborn

Jupyter Notebook

TED Europa CPV Mapping

Dados.gov.pt, Base.gov datasets

PorData & INE Inflation Data

📂 Project Structure
public-contracts-pt-2018-2025-analysis/
│
├── data/
│   ├── raw/                 # Original datasets (CSV, JSON, XLSX)
│   ├── processed/           # Cleaned and merged datasets
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_analysis.ipynb
│   ├── 03_visualizations.ipynb
│
├── reports/
│   ├── GroupC3_PublicContracts_Report.pdf
│   ├── GroupC3_Presentation.pdf
│
├── src/
│   ├── preprocessing.py
│   ├── analysis_helpers.py
│   ├── visualization_utils.py
│
├── requirements.txt
└── README.md


📚 Data Sources
Type	Source
Public Contracts 2018–2025	Base.gov.pt / Dados.gov.pt
Inflation	PorData / INE
PRR Contracts	Estrutura de Missão PRR
CPV Mapping	TED Europa
🧹 Data Preparation

Key cleaning and merging tasks included:

Standardizing column names and formats

Unifying contract value under contract_price_analysis

Creating clean CPV code + macro description fields

Cleaning contract type text

Merging all years into a single DataFrame

Removing duplicate contract entries

Adding flags:

is_prr

event_period (pre_covid, covid, ukraine_war)

📈 Main Findings
1️⃣ Contract Value vs Inflation

2019, 2020, 2023 → contract value grew above inflation

2021, 2022, 2024 → inflation exceeded contract growth

2️⃣ Contract Types with Biggest Increase

Bens móveis grew above inflation 3 out of 6 years

Serviços peaked in 2020–2021, dropped in 2022

3️⃣ CPV Sectors Most Affected

Strongest growth:

Equipamento de Imagiologia

Serviços TI

Arquitetura

4️⃣ Regional Inequality

Lisboa: > €1.1B

Portalegre: < €20M

CV = 0.99 → large inequality in spending

5️⃣ Companies with Highest Growth

B Braun Medical

Medtronic Portugal

Generis Farmacêutica

Labesfal

MEO

6️⃣ PRR Impact

PRR contracts < 1% of total

Main areas: Digital Transformation (C17–C19) & SNS

7️⃣ COVID-19 & Ukraine War

Contracts increased +37% from 2021 → 2024

Spending grew in construction, transport, medical equipment

Contract value dipped in 2022, recovered in 2023–2024

📊 Visualizations Included

YoY growth vs Inflation

Sector-level spending evolution

CPV macro category trends

Regional spending mapping

Event-period comparisons: Pre-COVID → COVID → Ukraine War

👥 Team Contributor 

João Bilé

Carolina Carvalho

Gabriel Domenech

Md Mijanul Haque
