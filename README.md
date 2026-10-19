# HR Analytics & Employee Attrition Analysis

## The Decision

**Where should Atlas Labs prioritize employee retention efforts to reduce turnover and maintain workforce stability?**

Atlas Labs, a fictional software company, faces an overall employee attrition rate of **16.1%**, with substantially higher turnover among certain job roles and employees working overtime or traveling frequently.

This analysis examines workforce demographics, employee performance, and attrition patterns to identify high-risk employee groups and help HR leadership prioritize targeted, evidence-based retention strategies.

## What the Business Needs to Know

| Total Employees | Active Employees | Attrition Rate | Highest-Risk Job Role |
|---|---|---|---|
| **1,470** | **1,233** | **16.1%** | **39.8% Sales Representatives** |

Employee turnover is concentrated in specific workforce segments rather than distributed evenly across the organization.

Employees required to work overtime have a **30.5% attrition rate**, nearly three times the **10.4%** rate among those without overtime requirements. 

Frequent travelers also experience higher attrition (**24.9% vs. 8.0%** for non-travelers).

**Early employee tenure presents another major retention challenge.** Employees with one year of tenure have the highest attrition rate at **34.5%**, while Sales Representatives experience the highest job-role attrition at **39.8%**.

These findings suggest that HR should prioritize reviewing overtime expectations, travel demands, early-tenure employee support, and retention challenges within high-turnover job roles.

## Recommended Actions

![Employee Attrition Dashboard](images/attrition.png)

### 1. Reduce overtime-related attrition

Employees required to work overtime have a **30.5% attrition rate**, compared with **10.4%** among employees without overtime requirements, nearly three times higher.

This gap suggests that workload expectations may be an important retention risk worth investigating.

**Recommended action:** Identify departments and job roles with high overtime requirements. Review workload distribution, staffing capacity, and scheduling practices, then pilot workload adjustments in high-risk teams.

**Measure success:** Track attrition rates, overtime hours, and employee satisfaction before and after the intervention to assess whether retention improves.

### 2. Review business travel expectations

Employees who travel frequently experience a **24.9% attrition rate**, compared with **8.0%** among employees who do not travel.

This substantial difference suggests that frequent business travel may be associated with retention challenges, potentially related to scheduling demands or work-life balance.

**Recommended action:** Review travel requirements for high-travel roles and explore alternatives such as virtual meetings, flexible scheduling, and recovery time after extended business trips.

**Measure success:** Compare attrition rates, travel frequency, and work-life balance satisfaction over time to evaluate the effectiveness of these changes.

### 3. Strengthen retention during the first two years

![Employee Performance Tracker](images/performance-tracker1.png)

Employees with **one year of tenure have the highest attrition rate at 34.5%**, followed by employees with less than one year at **31.6%**.

High turnover early in employment can increase replacement and onboarding costs while disrupting team productivity. 
The Performance Tracker provides an additional way to monitor individual satisfaction and review trends.

**Recommended action:** Strengthen onboarding and introduce structured check-ins at 30, 90, and 180 days. Pair new hires with mentors and collect feedback to identify unmet expectations or workplace challenges before employees decide to leave.

**Measure success:** Monitor first-year attrition, employee satisfaction, and retention at 6 and 12 months.

### 4. Prioritize retention in high-turnover job roles

![Workforce Overview](images/overview.png)

**Sales Representatives have the highest attrition rate at 39.8%**, followed by Recruiters at **37.5%** and Data Scientists at **23.8%**.

These differences suggest that retention challenges may vary significantly by job role, requiring more targeted strategies rather than a company-wide approach. The Workforce Overview provides additional context on department and job-role headcount, helping HR consider workforce size alongside attrition rates.

**Recommended action:** Conduct targeted employee surveys and exit interviews to investigate compensation, workload, management support, and career advancement opportunities. Prioritize interventions using both attrition rates and the number of employees affected.

**Measure success:** Track job-role attrition, employee satisfaction, and retention trends to evaluate whether targeted interventions reduce turnover.

### 5. Strengthen workforce development and compensation equity

![Employee Demographics Dashboard](images/demographics.png)

**Employees aged 20–29 account for nearly 60% of the workforce**, highlighting the importance of early-career development and long-term retention.

Compensation also varies across ethnic groups. White employees represent the largest ethnic group and earn an average salary of approximately **$115K**, compared with **$110K for Asian employees** and **$106K for employees of mixed or multiple ethnic backgrounds**.

These differences highlight opportunities to evaluate career progression and compensation practices, although salary differences alone do not establish inequity.

**Recommended action:** Expand mentorship, professional development, and internal career advancement opportunities for early-career employees. Conduct compensation equity reviews across comparable job roles, experience levels, and seniority to identify unexplained pay disparities.

**Measure success:** Track employee participation in development programs, internal promotion rates, early-career retention, and adjusted compensation gaps across demographic groups.

## How I Built It

**Tools:** Power BI, Power Query, DAX

- **Data preparation:** Cleaned and transformed HR datasets using Power Query.
- **Data modeling:** Built a star-schema data model connecting employee and performance data with lookup tables, including a dedicated date table.
- **DAX:** Created attrition, workforce, salary, and performance measures using various functions including `CALCULATE()` and `USERELATIONSHIP()`.
- **Visualization:** Developed four interactive dashboard pages with slicers and tooltips.

**Data source:** DataCamp's Atlas Labs HR datasets.
