# Streaming Platform Content Strategy Analysis

This project analyzes streaming platform content data to understand how content has evolved over time, how it is distributed across regions, and what kind of audience it targets.

The goal was to build a complete analytics workflow — starting from raw data, cleaning and transforming it, validating results, and finally presenting insights using dashboards.

---

## Tech Stack
- Python (pandas, numpy, matplotlib)
- Excel (Pivot Tables, Power Query)
- Power BI

---

## Dataset
Each row represents a single title available on the platform (movie or TV show).

Main fields used:
- title  
- Type (Movie / TV Show)  
- release_year  
- rating (PG, TV-MA, etc.)  
- country  

Some fields, like country, contain multiple values and required normalization before analysis.

---

## Data Preparation
The raw dataset was cleaned and prepared in Python:
- removed and handled missing values
- split multi-country entries and normalized them
- created additional features based on release year to classify content as:
  - Legacy (before 2000)
  - Not Recent (2000–2014)
  - Recent (2015 onwards)

Cleaned data was exported and validated in Excel before visualization.

---

## Analysis Performed
The following questions were explored:
- How many movies vs TV shows are available?
- How has content production changed over the years?
- Which countries contribute the most content?
- What audience maturity ratings dominate the platform?
- How much of the catalog is recent vs older content?

---

## Exploratory Analysis
Matplotlib was used during exploration to quickly validate trends and distributions before building final reports.

---

## Excel Work
Excel was used to:
- build pivot tables for key summaries
- normalize country data using Power Query
- validate Python results
- create quick visual checks for trends and distributions

---

## Power BI Dashboard
A Power BI dashboard was created to present the analysis in an interactive way, with filters for:
- year
- country
- content type
- content age category

The focus was on clarity and usability rather than decorative visuals.

---

## Key Takeaways
- Content production increased sharply after 2015
- TV shows have grown faster than movies in recent years
- The US and India are the largest content producers
- Most content targets mature audiences
- Recent content makes up the majority of the catalog

---

## Project Structure
'''
streaming_platform_content_strategy_analysis/
├── data/
├── notebooks/
├── excel/
├── powerbi/
├── images/
└── README.md
'''


---

## Notes
This project is platform-agnostic. Netflix was used as the sample dataset, but the same approach can be applied to other streaming services.
