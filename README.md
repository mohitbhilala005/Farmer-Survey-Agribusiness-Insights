# 🌾 Farmer Survey & Agribusiness Insights Dashboard

### Primary Field Survey | Agribusiness Analytics | Microsoft Power BI
---

## 📌 Project Overview

This project analyzes **primary field-survey data collected from 92 farmers across 7 villages** to understand farmer demographics, agricultural technology awareness and adoption, agribusiness participation, farmer challenges, support requirements, and potential agribusiness opportunities.

The survey data was transformed into an interactive **Microsoft Power BI dashboard** using data preparation, exploratory analysis, DAX-based KPI calculations, and interactive filtering.

The project aims to convert **real-world primary survey data into actionable agricultural and business insights** that can support better understanding of farmer needs, technology adoption barriers, and opportunities for agribusiness development.

---

## 🎯 Project Objectives

The analysis was designed to answer the following questions:

* What is the demographic profile of the surveyed farmers?
* How aware are farmers of modern agricultural technologies?
* How many farmers are actually using modern agricultural technologies?
* What are the major barriers to technology adoption?
* How affordable do farmers perceive modern agricultural technologies to be?
* How many farmers are currently involved in agribusiness?
* How many farmers are willing to start an agribusiness activity?
* Which agribusiness opportunities are preferred by farmers?
* What are the major problems faced by farmers?
* What type of support do farmers require?
* How does land holding relate to annual agricultural production?
* How does average production vary across irrigation sources?

---

# 📊 Survey Dataset

| Attribute              | Details                |
| ---------------------- | ---------------------- |
| **Farmers Surveyed**   | 92                     |
| **Villages Covered**   | 7                      |
| **Data Source**        | Primary Field Survey   |
| **Data Preparation**   | Microsoft Excel / CSV  |
| **Analytics Platform** | Microsoft Power BI     |
| **Analysis Language**  | DAX                    |
| **Farmer IDs**         | Anonymized (F001–F092) |

### 📍 Villages Covered

* Chopna
* Mau
* Lalpur
* Lakadiya
* Tajpura
* Jalalpura
* Manakpura

> **Privacy:** The dataset used for dashboard analysis is anonymized. Personally identifiable farmer information and survey dates were removed from the dashboard-ready dataset.

---

# 🔄 Project Workflow

```text
Primary Field Survey
        ↓
Data Collection
        ↓
Excel Data Preparation
        ↓
Data Cleaning & Structuring
        ↓
CSV Dataset
        ↓
Power BI Data Modeling
        ↓
DAX Measures & KPIs
        ↓
Interactive Dashboard
        ↓
Agricultural & Business Insights
```

---

# 🛠️ Tools & Technologies

| Tool                   | Purpose                                              |
| ---------------------- | ---------------------------------------------------- |
| **Microsoft Excel**    | Survey data entry, preparation and organization      |
| **CSV**                | Dashboard-ready dataset                              |
| **Microsoft Power BI** | Interactive dashboard and data visualization         |
| **DAX**                | KPI calculations and analytical measures             |
| **GitHub**             | Version control, documentation and project portfolio |

---

# 📈 Dashboard Overview

The Power BI dashboard is organized into two major analytical pages.

## Page 1 — Farmer Survey & Agribusiness Dashboard

The first dashboard provides a high-level overview of the survey.

### Key KPIs

* Total Farmers Surveyed
* Average Land Holding
* Technology Adoption %
* Agribusiness Participation %
* Willingness to Start Agribusiness %

### Visual Analysis

* Farmers by Village
* Technology Awareness vs. Actual Usage
* Technology Affordability
* Current Agribusiness Participation
* Willingness to Start Agribusiness

### Interactive Filters

The dashboard allows users to filter the analysis by:

* Village
* Education Level
* Irrigation Source
* Technology Awareness
* Technology Usage
* Current Agribusiness Activity
* Willingness to Start Agribusiness

---

## Page 2 — Farmer & Agribusiness Insights

The second page provides deeper analytical insights.

### Major Analyses

* Major Problems Faced by Farmers
* Production Increase After Technology Adoption
* Farmers by Education Level
* Farmers by Age Group
* Land Holding vs. Annual Production
* Preferred Agribusiness Types
* Average Production by Irrigation Source
* Support Required by Farmers
* Reasons for Not Adopting Technology

---

# 🔎 Key Findings

## 1. Technology Awareness vs. Adoption

A significant gap exists between awareness and actual usage of modern agricultural technology.

* **28 farmers (30.43%)** were aware of modern agricultural technology.
* Only **8 farmers (8.70%)** reported using modern agricultural technology.
* **30 farmers (32.61%)** considered modern agricultural technology affordable.
* Among the 8 technology users, **6 reported increased production** after adoption.

### 💡 Insight

The results indicate that **awareness alone does not necessarily translate into technology adoption**. Factors such as affordability, access to resources, training, and practical knowledge may require further investigation.

---

# 🌱 2. Agribusiness Opportunity

The survey indicates strong interest in starting agribusiness activities.

* **17 farmers (18.48%)** were currently involved in agribusiness.
* **80 farmers (86.96%)** expressed willingness to start an agribusiness activity.

### Preferred Opportunities

Farmers expressed interest in activities including:

* Mushroom Farming
* Vertical Farming
* Poultry Farming
* Vegetable Farming
* Aeroponics
* Dairy
* Value Addition

### 💡 Insight

The difference between **current participation and willingness to participate** highlights a potential opportunity for interventions focused on training, financing, market access, and practical business guidance.

---

# 🚜 3. Major Farmer Challenges

The survey identified several challenges affecting farmers, including:

* Lack of money
* Low agricultural yield
* Water shortage
* Age-related constraints
* Small land holdings
* Limited market support
* Electricity-related issues

### Support Required

The most frequently requested support included:

1. **Subsidy & Training**
2. **Market Support**

### 💡 Insight

The findings suggest that farmers may require a combination of **financial support, technical training, and improved market access** rather than a single intervention.

---

# 📊 4. Farmer Profile

The survey covered **92 farmers across 7 villages**.

Key observations include:

* **Chopna** had the highest number of surveyed farmers, with 43 respondents.
* **35 farmers** were recorded in the illiterate education category.
* **Mixed-crop farming** was the dominant farming type in the surveyed population.

---

# 📐 DAX Measures

The dashboard uses DAX measures to calculate important KPIs dynamically.

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

---

# 💼 Business & Agricultural Insights

The analysis highlights two particularly important patterns.

### Technology Adoption Gap

```text
Technology Awareness      30.43%
            ↓
Technology Usage           8.70%
```

There is a substantial difference between farmers who are aware of modern technologies and those who actually use them.

### Agribusiness Opportunity Gap

```text
Currently Involved        18.48%
            ↓
Willing to Start          86.96%
```

The high willingness to start an agribusiness activity suggests an opportunity to explore the factors preventing farmers from converting interest into actual participation.

---

# 🧠 Analytical Approach

The project follows a practical data analytics workflow:

### 1. Primary Data Collection

Collected farmer responses through field-level survey activities.

### 2. Data Preparation

Organized survey responses and prepared the dataset using Excel/CSV.

### 3. Data Anonymization

Removed personally identifiable information before using the data for dashboard analysis.

### 4. Data Modeling

Imported and structured the dataset in Power BI.

### 5. KPI Development

Created DAX measures for key metrics such as technology adoption, agribusiness participation, and willingness to start agribusiness.

### 6. Exploratory Analysis

Analyzed relationships among farmer demographics, technology adoption, production, irrigation, and agribusiness preferences.

### 7. Visualization

Developed interactive Power BI dashboards with KPIs, charts, comparisons, and slicers.

### 8. Insight Generation

Converted survey patterns into agricultural and business-oriented insights.

---

# 📂 Repository Structure

```text
Farmer-Survey-Agribusiness-Insights/
│
├── README.md
│
├── data/
│   └── farmer_survey_anonymized.csv
│
├── powerbi/
│   └── Survey_Analysis_Dashboard.pbix
│
├── screenshots/
│   ├── dashboard_overview.png
│   └── farmer_insights.png
│
└── documentation/
    └── project_notes.md
```

---

# 🔐 Data Integrity & Privacy

This project is based on **actual collected survey responses**.

* No synthetic farmer responses were added to the final dataset.
* Farmer identities were anonymized.
* Farmer names were removed from the dashboard-ready dataset.
* Survey dates were removed from the Power BI dataset.
* Missing responses were retained as missing rather than automatically being interpreted as negative responses.

This approach helps maintain transparency between the original field survey and the analytical dataset.

---

# 🚀 Future Improvements

Potential extensions to the project include:

* [ ] Analyze technology adoption across individual villages
* [ ] Analyze education level vs. technology adoption
* [ ] Analyze agribusiness preferences by village
* [ ] Create crop-level frequency analysis
* [ ] Build a dedicated recommendations page
* [ ] Develop a farmer segmentation framework
* [ ] Add additional cross-analysis between demographic and agribusiness variables
* [ ] Publish the dashboard through Power BI Service where appropriate

---

# 🎓 Project Classification

**Project Type:** Academic / Primary Field Survey / Data Analytics

**Domain:**

`Agriculture` • `Agribusiness` • `Farmer Technology Adoption` • `Business Intelligence` • `Data Visualization` • `Primary Research`

---

# 👨‍🎓 Author

### Mohit Bhilala

**Student, Department of Agricultural & Food Engineering (AgFE)**
**Indian Institute of Technology Kharagpur**

This project was developed as an academic field-survey and data analytics project to apply data visualization and business intelligence techniques to real-world agricultural and farmer-level data.

---

## ⭐ Key Skills Demonstrated

* Primary Data Collection
* Survey Data Analysis
* Data Cleaning & Preparation
* Microsoft Excel
* Microsoft Power BI
* DAX
* KPI Development
* Data Visualization
* Exploratory Data Analysis
* Agricultural Analytics
* Agribusiness Analysis
* Insight Generation
* Business Intelligence
* GitHub Documentation

---

## 📌 Conclusion

The project demonstrates how **primary field-survey data can be transformed into an interactive business intelligence solution**.

The analysis identifies a clear gap between **technology awareness and actual adoption**, while also revealing strong farmer interest in **starting agribusiness activities**. These findings can help frame further questions around financing, training, technology accessibility, market linkages, and agribusiness support.

> **From field data to actionable agricultural insights. 🌾📊**

---

### Repository

**GitHub:** `Farmer-Survey-Agribusiness-Insights`

**Author:** **Mohit Bhilala**
**IIT Kharagpur | Department of Agricultural & Food Engineering**
