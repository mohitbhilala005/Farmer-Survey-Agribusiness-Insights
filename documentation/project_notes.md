# Project Notes — Farmer Survey & Agribusiness Insights

## 1. Background

This project is based on a primary field survey conducted to understand the agricultural practices, technology adoption, agribusiness involvement, challenges, and future interests of farmers.

A total of 92 farmer responses from 7 villages were used for the final analysis.

## 2. Data Collection

The survey collected information related to:

- Farmer demographics
- Education level
- Age
- Farming experience
- Land holding
- Main crops
- Irrigation sources
- Annual production
- Awareness of modern agricultural technology
- Modern technology usage
- Technology affordability
- Production changes after technology adoption
- Agribusiness participation
- Income changes from agribusiness
- Willingness to start agribusiness
- Preferred agribusiness activities
- Major farming problems
- Government assistance
- Reasons for not adopting technology
- Support required by farmers

## 3. Data Preparation

The collected survey responses were organized and standardized in Microsoft Excel before being exported to CSV for Power BI.

The final Power BI dataset uses anonymized farmer IDs ranging from F001 to F092.

Farmer names and survey dates were removed from the CSV used for dashboard analysis.

Missing responses were retained as blank values rather than being converted into "No".

## 4. Power BI Analysis

The dashboard was developed in Microsoft Power BI using calculated measures and calculated columns created with DAX.

### Key KPIs

- Total Farmers Surveyed: 92
- Average Land Holding: 4.12 acres
- Technology Adoption: 8.70%
- Agribusiness Participation: 18.48%
- Willingness to Start Agribusiness: 86.96%

## 5. Dashboard Pages

### Page 1 — Farmer Survey & Agribusiness Insights Dashboard

This page provides an overview of the survey through KPI cards, interactive slicers, and charts covering:

- Village distribution
- Technology awareness and actual usage
- Technology affordability
- Current agribusiness participation
- Willingness to start agribusiness

### Page 2 — Farmer & Agribusiness Insights

This page provides detailed analysis of:

- Education level
- Age groups
- Major farmer problems
- Reasons for not adopting technology
- Support required
- Preferred agribusiness activities
- Irrigation and production
- Land holding vs annual production
- Production increase after technology adoption

## 6. Key Findings

The analysis identified a substantial gap between awareness and actual usage of modern agricultural technologies.

While 28 farmers reported awareness of modern agricultural technology, only 8 farmers reported actual usage.

Agribusiness participation was relatively limited, with 17 farmers currently involved in agribusiness activities. However, 80 farmers expressed willingness to start an agribusiness activity.

The most frequently identified support requirement was subsidy and training, followed by market support.

## 7. Important Data Considerations

The "Production Increase After Technology" analysis contains responses from the farmers who reported using modern technology. Blank responses were not treated as negative responses.

The Main Crop field contains multiple crops for some farmers and was retained in its original survey structure. A separate crop-level analysis can be developed in a future version.

## 8. Tools Used

- Microsoft Excel
- CSV
- Microsoft Power BI
- DAX
- GitHub

## 9. Project Outcome

The project converts primary farmer survey responses into an interactive business intelligence dashboard.

The dashboard can be used to explore farmer profiles, technology adoption barriers, agribusiness opportunities, production patterns, and support requirements across the surveyed villages.

## 10. Future Scope

Future analysis could include:

- Individual crop-level frequency analysis
- Village-wise technology adoption
- Education vs technology adoption
- Village-wise agribusiness preferences
- Additional statistical analysis
- A dedicated recommendations page
