**Indeed Job Market Analysis — Canada**

**Project Overview**
This project is an end-to-end Data Analytics pipeline designed to scrape, clean, analyze, and visualize job posting data from Indeed for various analyst roles in Canada (Date posted: last 14 days from 5-Aug-25)
It demonstrates practical skills in Python (Web Scraping, Data Cleaning, EDA) and Power BI (Data Visualization & Dashboard Design).

**Objectives**
- Collect real-world job market data from Indeed.

- Clean and transform raw scraped data into an analysis-ready format.

- Perform Exploratory Data Analysis (EDA) to uncover hiring trends, salary distributions, and top recruiters.

- Build an interactive Power BI dashboard for clear and actionable insights.

**Tech Stack**
- Python: Selenium, Pandas, Regex, Numpy

- Power BI: Interactive dashboards and data storytelling

- Excel: Exporting cleaned datasets

- GitHub: Version control and project hosting

**📂 Project Workflow**
1. Web Scraping (Python + Selenium)
Scraped job postings from Indeed Canada for multiple job roles.

Extracted:

Job_role_category

Job Title

Company Name

Location

Salary (raw text)

Job Type

Skills required

Work Location

Job URL

Implemented pagination for multiple pages.

Added error handling (try/except) for missing fields.

Clicked each job card to scrape detailed descriptions.

2. Data Cleaning (Python + Pandas)
Removed duplicates using job_url to ensure unique job postings.

Dropped missing values in essential columns like job_category_role.

Standardized text formats:

Converted job_title, company, and location to title case.

Cleaned location column:

Extracted "City, Province" using regex.

Transformed salary column:

Converted salary ranges to average annual salary.

Converted monthly, weekly, and hourly salaries to annual (×12, ×52).

Dropped unused columns (e.g., skills_found if empty).

Saved cleaned dataset as cleanedindeed.xlsx.

3. Exploratory Data Analysis (Python & Power Bi)
Analyzed:

  Python (Basic Data Understanding)
  Inspected dataset structure:

    df.shape → rows & columns

    df.dtypes → data types of each column

    df.head() → previewed first few rows

    df.describe() → summary statistics

    Checked for:

    Missing values → df.isna().sum()

    Duplicate rows → df.duplicated().sum()

    Used results to guide data cleaning steps.

  Power BI (Visual EDA & Storytelling)
  Created an interactive dashboard with:

    Job postings by province (map & bar charts)

    Top hiring companies

    Average salary by location & job category

    Jobs by job type

    Filters for job type, location

4. Data Visualization (Power BI)
Created an interactive dashboard with:

KPIs:

Total Jobs: 2,264

Unique Companies: 896

Max Salary: $269K

Min Salary: $23K

Average Salary: $97K

Charts:

Jobs by Province (drill-through available)

Jobs by Job Type

Jobs by Location (top cities)

Top 5 Hiring Companies

Average Salary by Province

Filters:

Job Category filter for custom analysis.

**Key Insights**
- Ontario has the highest job postings (1,241), followed by Quebec and Alberta.

- TD Bank leads in recruitment with 89 postings.

- Average salaries are fairly consistent across provinces, with Ontario, Saskatchewan, and Yukon among the top.

- Permanent roles dominate the market, with relatively fewer contract and part-time roles.


**📌 Skills Demonstrated**
- Web scraping with Selenium

- Data cleaning & transformation in Pandas

- Regular expressions for text processing

- Exploratory Data Analysis (Python & Power BI)

- Interactive dashboard creation(Visuals, Filters, Drill-through, Tooltip)

- End-to-end project workflow documentation
