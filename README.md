# Data Professional Survey Dashboard

An interactive Power BI dashboard that analyzes a survey of 212 data professionals. It covers where they live, what they earn, which programming languages they prefer and how satisfied they are with their jobs.

## Dashboard Visuals

- **Country of survey takers** (treemap): United States, India, United Kingdom, Canada and Other.
- **Average salary by job title** (bar chart): Data Scientist, Data Architect, Data Engineer, Data Analyst, Database Developer, Student/Looking/None and Other.
- **Average salary by gender** (donut chart).
- **Favorite programming language** (stacked column chart): Python, R, C/C++, JavaScript, Java and Other, split by job title.
- **Happiness gauges**: work/life balance and upward mobility, each scored from 0 to 10.
- **Summary cards**: number of survey takers and average age.

The visuals are cross-filtered. Clicking a country in the treemap updates every other visual, and selecting an item in another visual updates the treemap. Click the same selection again to clear it.

## Key Metrics

| Metric | Value |
|---|---|
| Survey takers | 212 |
| Average age | about 29 |
| Happiness with work/life balance | 5.29 / 10 |
| Happiness with upward mobility | 4.55 / 10 |

## Dataset

`Professional Survey Data.xlsx` has one sheet, **Data Professional Survey**, with one row per respondent and 28 columns.

| Field | Description |
|---|---|
| Metadata | Unique ID, date and time taken, browser, OS, city, country, referrer, time spent |
| Q1 | Job title |
| Q2 | Switched careers into data |
| Q3 | Yearly salary in USD, as a range (for example `41k-65k`) |
| Q4 | Industry |
| Q5 | Favorite programming language |
| Q6 | Happiness with salary, work/life balance, coworkers, management, upward mobility and learning new things (0 to 10) |
| Q7 | Difficulty of breaking into data |
| Q8 | Most important factor in a new job |
| Q9 | Gender |
| Q10 | Age |
| Q11 | Country of residence |
| Q12 | Highest level of education |
| Q13 | Ethnicity |

Salary is stored as ranges, so the average salary visuals use a numeric conversion of those ranges.

## Tools Used

- Microsoft Excel (source data)
- Power BI Desktop (data modeling and dashboard)

## Repository Contents

| File | Description |
|---|---|
| `Professional Survey Data.xlsx` | Raw survey responses |
| `Power BI - Data Professional Survey.xlsx.pbix` | Power BI report |
| `README.md` | Project documentation |

## How to Use

1. Clone or download this repository.
2. Open `Power BI - Data Professional Survey.xlsx.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. If Power BI cannot find the data, go to **Home > Transform data > Data source settings** and point it to `Professional Survey Data.xlsx`.
4. Click the visuals to filter and explore the data.
