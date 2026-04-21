# Rim-Osman - Data Analyst Portfolio
## About 
Hi, I'm **Rim Osman**, a Data and Business Analyst with 3+ years of experience helping organizations make sense of their data. 

I have a strong background in **banking**, **regulatory compliance**, **and digital transformation**, with hands-on experience in Agile environments and fintech projects. I specialize in translating complex datasets into clear business insights that **support strategic decision-making and operational efficiency.**

I work with **SQL, Excel, and data visualization tools** to clean, analyze, and visualize data while improving data quality and supporting business stakeholders. 

I am actively interested in opportunities within **leading UAE banks and consulting firms**, where I can contribute to high-impact data and transformation initiatives in fast-paced, international environments.

Here is my CV in [pdf](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/CV%20-%20Data%20Analyst%20.pdf).

This repository showcases my projects, technical skills, and continuous learning journey in Data Analytics and Business Intelligence.

# Table of Contents
- [[About]](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#about)

- [[Portfolio Projects]](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#portfolio-projects)
  - Python
  - SQL
    - [Global GDP Analysis (1998-2024)](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#global-gdp-analysis-1998-2024)
    - [Global Layoffs Data Cleaning](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#global-layoffs-data-cleaning)
    - [Global Layoffs Data Exploration](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#global-layoffs-data-exploration)
  - Excel
  - Tableau---> [Go to Tableau](https://public.tableau.com/app/profile/rimm.osman/vizzes)
  - Power BI
    
- [Education](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#education)

- [Certificates](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#certificates)

- [Contact](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#contacts)

# Portfolio Projects 
In this section, I will list data analytics projects briefly describing the technology stack used to solve cases.

### Global GDP Analysis (1998-2024)
**Code:** [`Global_GDP_Analysis.sql`](https://github.com/rim-osman/PortfolioProjects/blob/main/GDP%20Portfolio%20Project.sql)

**Project Overview:** This project presents an end-to-end SQL-based analysis of global GDP trends from 1998 to 2024.
The objective is to explore how economic power is distributed across countries, regions, and income groups, and to identify key patterns that can support strategic, financial, and policy-related decision-making.

**Problem Statement:** 
Understanding global economic dynamics is essential for financial institutions, investors, and policymakers. This project aims to answer:

- Which countries and regions drive global economic growth?
- How do global crises impact economic performance?

**Approach:** 

- Cleaned and standardized raw GDP datasets to ensure consistency and accuracy
- Designed a structured data model (fact and dimension tables)
- Performed advanced SQL analysis using joins, window functions, aggregations, and ranking techniques
- Analyzed trends across time, regions, and income segments

**Dataset Description:**

- `gdp_data` -> Annual GDP values by country
- `metadata_countries` -> Region & income group classification 
- `iso_countries` -> Country code reference table

**Skills & Tools:** 

- SQL (SQLite)
- Data Cleaning & Transformation
- Data Modeling (Star Schema)
- Window Functions & Ranking
- Analytical Thinking & Insight Generation

**Key Findings & Business Insights:** 

- **Global Concentration:** GDP is dominated by a few major economies, led by the United States, with China showing strong long-term growth.
- **Economic Shocks:** Clear downturns during the 2008 financial crisis and 2020 COVID-19 pandemic.
- **Regional trends:** East Asia & Pacific and North America lead global GDP, while Middle East growth is oil-drive.
- **Income Dynamics:** High-income countries dominate, while emerging economies show faster growth.

### Global Layoffs Data Cleaning 
**Code:** [Data Cleaning Layoffs.sql](https://github.com/rim-osman/PortfolioProjects/blob/main/Data%20Cleaning%20layoffs%20Project.sql)

**Project Overview:** This project focuses on cleaning and preparing a real-world layoffs dataset to ensure data quality, consistency, and usability for downstream analysis and visualization.
The dataset contains information about company layoffs across industries, including company details, location, number of layoffs, funding, and company stage.

**Objective:** To transform raw, inconsistent data into a clean and structured dataset ready for exploratory data analysis (EDA) and business insights.

**Approach:** 

The data cleaning process was performed in SQL using a structured, step-by-step methodology aligned with real-world data practices:

**1. Data Staging**

- Created a staging table to preserve raw data integrity
- Worked exclusively on duplicated tables to avoid modifying source data

**2. Duplicate Removal**

- Identified duplicates using ROW_NUMBER() with partitioning across all key columns
- Removed duplicate rows while preserving original records

**3. Data Standardization**

- Trimmed whitespace in text fields (e.g., company names)
- Standardized inconsistent values (e.g., “Crypto”, “Crypto Currency” → “Crypto”)
- Fixed formatting issues (e.g., trailing punctuation in country names)
- Converted date fields into a consistent format (YYYY-MM-DD)

**4. Handling NULL & Missing Values**

- Converted text-based 'NULL' and empty strings into actual SQL NULL values
- Populated missing values using self-joins where possible (e.g., filling missing industry values based on company + location)
- Identified and evaluated incomplete records

**5. Data Filtering**

- Removed rows with insufficient or unreliable data (e.g., missing both total layoffs and percentage)
- Dropped unnecessary columns after processing

**Dataset Description:**

`layoffs`-> This dataset contains real-world company layoff records collected across multiple industries and countries. It includes structured and semi-structured fields covering workforce reductions, company context, funding, and timing.
The data is intentionally inconsistent in places (missing values, mixed formats, and duplicates), making it suitable for practicing real-world data cleaning and standardization techniques.

**Skills & Tools:** 

- SQL (SQLite & MySQL)
- Data Cleaning & Transformation
- Data Validation
- Handling Missing Data
- Window Functions (ROW_NUMBER)
- Data Standardization Techniques
  
### Global Layoffs Data Exploration 
**Code:** [`Data Exploration Layoffs`](https://github.com/rim-osman/PortfolioProjects/blob/main/Data%20Exploration%20layoffs%20Project.sql)

**Project Overview:** This project presents an exploratory data analysis (EDA) of global company layoffs between 2020 and 2023. After completing a full data cleaning phase, the objective of this analysis is to explore patterns, trends, and distributions of layoffs across companies, industries, countries, and time.
The goal is to uncover meaningful insights about how global economic events (such as COVID-19 and market downturns) influenced workforce reductions across different sectors.

**Problem Statement:** 
Layoffs are often influenced by economic conditions, company performance, and industry cycles. This project aims to answer:

- Which companies and industries were most affected by layoffs?
- How did layoffs evolve over time (monthly and yearly trends)?
- Which countries experienced the highest job losses?
- Which funding stages were most impacted?
- How did layoffs progress cumulatively over time?

**Approach:** 

The analysis was performed using SQL on a cleaned dataset (layoffs_staging2) and follows a structured exploratory workflow:

- Performed initial statistical exploration (min/max layoffs, extreme values)
- Identified companies with 100% workforce reduction
- Analyzed total layoffs by company, industry, country, and stage
- Investigated temporal trends (daily, monthly, yearly)
- Fixed and validated date inconsistencies before time-based analysis
- Used window functions for rolling totals and ranking
- Applied CTEs for structured multi-step analysis

**Skills & Tools:** 

- SQL (SQLite & MySQL)
- Data Exploration & EDA Techniques 
- Data Cleaning Validation during analysis 
- Aggregations & Grouping
- Window Functions (Rolling Sums, Ranking)
- CTEs (Common Table Expressions)
- Time-Series Analysis in SQL
- Analytical Thinking & Business Insight Extraction

**Key Findings & Business Insights:** 

- **Massive Layoff Concentration:** A small number of large companies (e.g., Microsoft, Amazon, Meta, Uber) account for a significant portion of global layoffs.
- **COVID-19 Impact:** The analysis shows a strong spike in layoffs starting in 2020, aligning with the COVID-19 pandemic period, followed by sustained reductions through 2022–2023.
- **Industry Vulnerability:** Consumer and Retail industries were among the most affected, reflecting reduced demand and economic slowdown during global disruptions.
- **Country-level Distribution:** The United States recorded the highest number of layoffs, far exceeding other countries in total job losses.
- **Peak Layoff Year:** 2022 was identified as the most severe year in terms of layoffs, with sustained high levels continuing into early 2023.
- **Cumulative Trend (Rolling Impact):** Rolling sum analysis shows a continuous increase in total layoffs over time, highlighting the long-term workforce impact beyond isolated events.
- **Funding Stage Sensitivity:** Post-IPO and late-stage companies experienced the highest layoffs, suggesting pressure on large-scale organizations to restructure during downturns.

# Education 
- Université Marie & Louis Pasteur, Besançon, France: Master of Science - MS, Business Intelligence, Sep 2022 - Oct 2024

- Saint-Joseph University of Beirut, Lebanon: Bachelor's degree, Banking and Finance, 2016 - 2019

- National Lebanese Baccalaureate: Science and Mathematics, 2014 - 2016


# Certificates
The best way to showcase my skills is by doing and sharing the work you've completed but certifications often reflect that effort and growth as well. I'm excited to share the certifications I've earned, which complement my hands-on experience in data and analytics: 
  - [Data Analytics Bootcamp Certification](https://www.linkedin.com/in/rim-osman/overlay/1772130321074/single-media-viewer/?profileId=ACoAADbIX08BF_tpDZPiItlm8tTyMkeY8AdQfHQ&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_featured_details%3BNaf1xv3jSJO8jZ%2FJUcmkmQ%3D%3D) (March 2026) (Youtube - Alexander Freberg)
  - [Atlassian Agile Project Management Professional Certificate](https://drive.google.com/drive/folders/1zpGHlPN5Q3eJp46ypW1ao6q1nN4jpYK-?usp=drive_link) (March 2025) (Coursera - Atlassian/LinkedIn Learning)
  - [JIRA: Basic Administration](https://www.coursera.org/account/accomplishments/verify/S7ZXNFMXNE53?utm_source=link&utm_medium=certificate&utm_content=cert_image&utm_campaign=pdf_header_button&utm_product=course) (April 2024) (Coursera - Atlassian/LinkedIn Learning)

# Contacts 
- 🔗 LinkedIn: [@rimosman](https://www.linkedin.com/in/rim-osman/)
- 📧 Email: rimmosman@gmail.com
