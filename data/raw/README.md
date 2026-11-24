# Raw Data Sources

This directory contains the original Statistics South Africa (Stats SA) datasets used in the South African Economic Recovery investigation.

Raw datasets are excluded from version control. Researchers wishing to reproduce the analysis should obtain the original files from the official Statistics South Africa website and place them in this directory.

**Official website:** https://www.statssa.gov.za/

## 1. Gross Domestic Product

**Publication:** P0441 — Gross Domestic Product

**Required filename:**

`GDP P0441 - GDP Time series.xlsx`

**Publication page:** https://www.statssa.gov.za/?page_id=1854&PPN=P0441

**Analysis coverage:** 2010 Q1 – 2026 Q2

**Purpose:**

- Quarterly real GDP analysis
- Economic growth calculations
- Pre-pandemic and post-pandemic growth comparisons
- Historical trend extrapolation
- GDP recovery index
- Annual real GDP calculations

## 2. Mid-Year Population Estimates

**Publication:** P0302 — Mid-Year Population Estimates

**Required filenames:**

- `MYPE report table website_ 2026.xlsx`
- `P03022026.pdf`

**Publication page:** https://www.statssa.gov.za/?page_id=1854&PPN=P0302

**Analysis coverage:** 2010–2026

**Purpose:**

- Population estimates
- Historical population reconstruction
- Population growth analysis
- Real GDP per capita calculations

Historical population estimates are reconstructed using published annual population growth rates and the 2026 population estimate. Consequently, reconstructed estimates are subject to rounding uncertainty.

## 3. Quarterly Labour Force Survey

**Publication:** P0211 — Quarterly Labour Force Survey (QLFS)

**Required filename:**

`QLFS Trends 2008-2026Q3.xlsx`

**Publication page:** https://www.statssa.gov.za/?page_id=1854&PPN=P0211

**Analysis coverage:** 2010 Q1 – 2026 Q3

**Purpose:**

- Employment and unemployment trends
- Working-age population analysis
- Labour force participation
- Employment-to-population ratio
- Official unemployment rate
- Employment recovery benchmark

## 4. Consumer Price Index

**Publication:** P0141 — Consumer Price Index (CPI)

**Required filename:**

`Excel - CPI (COICOP) from January 2008 (202610).xlsx`

**Publication page:** https://www.statssa.gov.za/?page_id=1854&PPN=P0141

**Analysis coverage:** January 2010 – October 2026

**Selected series:** CPS00000 — CPI Headline

**Index reference period:** December 2024 = 100

**Purpose:**

- Monthly consumer price analysis
- Month-on-month inflation calculations
- Year-on-year inflation calculations
- Cumulative consumer price changes
- Inflation adjustment of nominal earnings

## 5. Quarterly Employment Statistics

**Publication:** P0277 — Quarterly Employment Statistics (QES)

**Required filenames:**

- `P0277December2019.pdf`
- `P0277June2026.pdf`

**Publication page:** https://www.statssa.gov.za/?page_id=1854&PPN=P0277

**Earnings reference periods:**

- November 2019
- May 2026

**Purpose:**

- Average nominal monthly earnings comparison
- Inflation-adjusted earnings calculations
- Purchasing power assessment

The analysis uses average monthly earnings in the formal non-agricultural sector. Earnings values are manually extracted from the official publications.

The comparison uses different calendar months and may therefore be affected by seasonal earnings patterns, bonuses and changes in workforce composition.

## Expected Directory Structure

```text
data/raw/
├── Excel - CPI (COICOP) from January 2008 (202610).xlsx
├── GDP P0441 - GDP Time series.xlsx
├── MYPE report table website_ 2026.xlsx
├── P0277December2019.pdf
├── P0277June2026.pdf
├── P03022026.pdf
├── QLFS Trends 2008-2026Q3.xlsx
└── README.md
```

## Reproduction Instructions

1. Visit the relevant Statistics South Africa publication pages.
2. Locate the historical publications and supplementary Excel datasets corresponding to the specified reference periods.
3. Download all seven required source files.
4. Ensure the filenames match those listed above.
5. Place the files in the `data/raw/` directory.
6. Install the dependencies listed in `requirements.txt`.
7. Open and execute `notebooks/01_data_acquisition.ipynb`.

## Data Provenance and Revisions

All original statistical data are sourced from Statistics South Africa.

Official datasets may be revised after publication. Researchers should use the same publication editions and historical data vintages wherever possible to reproduce the reported results.

Using newer editions may produce different results due to statistical revisions, methodological changes or rebasing.

The processed datasets included in this repository represent the data vintage used in this investigation.

## Data Ownership

The original statistical publications and datasets remain subject to the applicable Statistics South Africa terms of use.

This repository contains independently developed analytical code, processed datasets, visualisations and research documentation.

The investigation is independent and is not affiliated with or endorsed by Statistics South Africa.