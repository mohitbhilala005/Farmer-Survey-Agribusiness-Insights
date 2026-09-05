# Farmer Survey & Agribusiness Insights Dashboard

## Project Overview
This project analyzes primary survey data collected from **92 farmers across 7 villages** to understand farmer demographics, agricultural technology awareness and adoption, agribusiness participation, farmer needs, and future agribusiness opportunities.

The project was developed as a **Microsoft Power BI dashboard** using field-survey data collected for an academic project.

## Objectives
- Analyze the demographic profile of surveyed farmers.
- Measure awareness and actual usage of modern agricultural technologies.
- Identify barriers to technology adoption.
- Analyze current agribusiness participation.
- Measure willingness to start agribusiness activities.
- Identify preferred agribusiness opportunities.
- Understand major farmer problems and required support.
- Explore the relationship between land holding and annual production.
- Compare average production across irrigation sources.

## Dataset
| Attribute | Details |
|---|---|
| Farmers surveyed | 92 |
| Villages covered | 7 |
| Data source | Primary field survey |
| Dashboard | Microsoft Power BI |
| Data preparation | Microsoft Excel / CSV |
| Analysis | Power BI + DAX |
| Farmer IDs | Anonymized (F001–F092) |

### Villages Covered
Chopna, Mau, Lalpur, Lakadiya, Tajpura, Jalalpura, Manakpura

> **Privacy note:** The dashboard dataset is anonymized. Farmer names and survey dates were removed from the CSV used in Power BI.

## Key Findings

### Farmer Profile
- **92 farmers** were surveyed across **7 villages**.
- **Chopna** had the largest number of surveyed farmers (43).
- **35 farmers** were recorded as illiterate, the largest education category.
- **Mixed-crop farming** was the dominant farming type.

### Technology Adoption
- **28 farmers (30.43%)** were aware of modern agricultural technology.
- Only **8 farmers (8.70%)** reported using modern agricultural technology.
- **30 farmers (32.61%)** considered the technology affordable.
- Among the 8 technology users, **6 reported increased production** after adoption.

### Agribusiness
- **17 farmers (18.48%)** were currently involved in agribusiness.
- **80 farmers (86.96%)** were willing to start an agribusiness activity.
- Common preferences included **Mushroom, Vertical Farming, Poultry Farming, Vegetable Farming, Aeroponics, Dairy, and Value Addition**.

### Farmer Challenges & Support
Major problems included:
- Lack of money
- Low yield
- Water shortage
- Age-related constraints
- Small land holdings
- Market support
- Electricity-related issues

The most frequently requested support was **Subsidy & Training**, followed by **Market Support**.

## Dashboard Structure

### Page 1 — Farmer Survey & Agribusiness Insights Dashboard
- Total Farmers Surveyed
- Average Land Holding
- Technology Adoption %
- Agribusiness Participation %
- Willingness to Start Agribusiness %
- Farmers by Village
- Technology Awareness vs Actual Usage
- Technology Affordability
- Current Agribusiness Participation
- Willingness to Start Agribusiness
- Interactive slicers for Village, Education Level, Irrigation Source, Technology Awareness, Technology Usage, Current Agribusiness Activity, and Willingness to Start Agribusiness

### Page 2 — Farmer & Agribusiness Insights
- Major Problems Faced by Farmers
- Production Increase After Technology
- Farmers by Education Level
- Farmers by Age Group
- Land Holding vs Annual Production
- Preferred Agribusiness Types
- Average Production by Irrigation Source
- Support Needed by Farmers
- Reasons for Not Adopting Technology

## Key DAX Measures

### Total Farmers Surveyed
```DAX
Total Farmers Surveyed =
COUNT('farmer_survey_anonymized'[Farmer_ID])
```

### Average Land Holding
```DAX
Average Land Holding =
AVERAGE('farmer_survey_anonymized'[Land_Holding_Acres])
```

### Technology Adoption %
```DAX
Technology Adoption % =
DIVIDE(
    CALCULATE(
        COUNTROWS('farmer_survey_anonymized'),
        'farmer_survey_anonymized'[Uses_Modern_Tech] = "Yes"
    ),
    COUNTROWS('farmer_survey_anonymized'),
    0
)
```

### Agribusiness Participation %
```DAX
Agribusiness Participation % =
DIVIDE(
    CALCULATE(
        COUNTROWS('farmer_survey_anonymized'),
        'farmer_survey_anonymized'[Involved_in_Agribusiness_Activity] = "Yes"
    ),
    COUNTROWS('farmer_survey_anonymized'),
    0
)
```

### Willingness to Start Agribusiness %
```DAX
Willing to Start Agribusiness % =
DIVIDE(
    CALCULATE(
        COUNTROWS('farmer_survey_anonymized'),
        'farmer_survey_anonymized'[Willing_to_Start_Agribusiness] = "Yes"
    ),
    COUNTROWS('farmer_survey_anonymized'),
    0
)
```

## Tools & Technologies
- **Microsoft Power BI** — Dashboard and interactive analysis
- **DAX** — KPI measures and calculated columns
- **Microsoft Excel** — Survey data preparation
- **CSV** — Dashboard-ready dataset
- **GitHub** — Project documentation and portfolio hosting

## Recommended Repository Structure
```text
Farmer-Survey-Agribusiness-Insights/
│
├── README.md
├── data/
│   └── farmer_survey_anonymized.csv
├── powerbi/
│   └── Survey_Analysis_Dashboard.pbix
├── screenshots/
│   ├── dashboard_overview.png
│   └── farmer_insights.png
└── documentation/
    └── project_notes.md
```

## Agricultural / Business Insights
The survey shows a clear gap between **awareness and actual adoption of modern agricultural technologies**: 28 farmers were aware of modern technologies, while only 8 reported using them.

At the same time, the high willingness to start agribusiness activities (**86.96%**) indicates an opportunity to investigate support focused on **financial assistance, training, market access, and practical guidance**.

## Future Improvements
- Create a dedicated crop-level analysis table for individual crop frequencies.
- Compare technology adoption across villages.
- Analyze education vs. technology adoption.
- Analyze agribusiness preferences by village.
- Add a recommendations page.
- Publish the dashboard through Power BI Service where appropriate.

## Data Integrity
All analysis is based on the collected survey responses. **No synthetic farmer responses were added to the final dataset.**

Missing responses are retained as missing rather than automatically being converted into negative responses.

## Project Type
**Academic / Field Survey / Data Analytics Project**

**Focus Areas:** Agriculture • Agribusiness • Farmer Technology Adoption • Business Intelligence • Data Visualization • Primary Research
