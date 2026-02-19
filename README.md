# HR Analytics Dashboard (Tableau) — Attrition & Retention Insights

**Live Dashboard (Tableau Public):**  
https://public.tableau.com/app/profile/omkar.chalke3447/viz/HRAnalyticsDashboard_17706707347890/HRAnalyticsDashboard?publish=yes

## Overview
This project delivers an interactive **HR Analytics dashboard** focused on **attrition and retention**. The dashboard helps HR and business stakeholders quickly understand **who is leaving**, **where attrition is concentrated**, and **which workforce segments may be at higher risk**—to support data-driven retention actions.

## What you can explore
- **Headline KPIs**: total employees, active employees, attrition count, attrition rate, average age, average monthly income
- **Attrition breakdowns** by:
  - Gender
  - Department and Job Role
  - Age band
  - Education field
  - Overtime status
  - Salary slab (binned from monthly income)
- **Interactive filtering** to slice metrics across segments and compare patterns

## Key metrics (from the included dataset)
Computed on `HR_Tableau_Data.xlsx` (Sheet1):

- **Total employees:** 11,760  
- **Active employees:** 9,864  
- **Attrition count:** 1,896  
- **Attrition rate:** 16.12%  
- **Average age:** 36.92 years  
- **Average monthly income:** $6,502.93  

### Notable patterns (quick highlights)
- **Overtime is strongly associated with attrition**  
  - Attrition rate with overtime: **30.53%**  
  - Attrition rate without overtime: **10.44%**
- Highest attrition counts are observed in:
  - **Department:** R&D (1,064), Sales (736), HR (96)
  - **Job Roles (top):** Laboratory Technician (496), Sales Executive (456), Research Scientist (376), Sales Representative (264)
- Most attrition occurs in **Age Band:** 25–34 (896), then 35–44 (408)

> These are descriptive insights for exploration; the dashboard is intended to support hypothesis generation and operational decision-making.

## Dataset
- **File:** `HR_Tableau_Data.xlsx`
- **Rows / Columns:** 11,760 rows × 39 columns
- **Core fields include:**
  - Employee identifiers: `Employee Number`, `emp no`
  - Demographics: `Age`, `Gender`, `Marital Status`, `Education Field`, `CF_age band`
  - Work factors: `Department`, `Job Role`, `Business Travel`, `Over Time`, `Distance From Home`
  - Compensation: `Monthly Income`, `Daily Rate`, `Hourly Rate`, `Monthly Rate`, `Percent Salary Hike`, `Stock Option Level`
  - Satisfaction & performance: `Job Satisfaction`, `Environment Satisfaction`, `Relationship Satisfaction`, `Work Life Balance`, `Performance Rating`
  - Tenure & experience: `Years At Company`, `Total Working Years`, `Years In Current Role`, `Years Since Last Promotion`, `Years With Curr Manager`, `Num Companies Worked`
  - Target: `Attrition` (Yes/No)

### Calculated/derived fields included
The dataset contains some pre-modeled helper fields for dashboarding:
- `CF_attrition label`
- `CF_current Employee`
- `CF_age band`

## How to use
### Option A — View online
Open the Tableau Public link above and interact with filters/tooltips to explore attrition by segment.

### Option B — Use locally in Tableau
1. Download this repository
2. Open Tableau (Desktop or Public)
3. Connect to `HR_Tableau_Data.xlsx`
4. Recreate/extend the dashboard using the same dimensions and measures

## Repository structure (suggested)
