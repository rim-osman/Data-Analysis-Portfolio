# Rim-Osman - Data Analyst Portfolio
## About 
Hi, I'm Rim! I'm a Data and Business Analyst with 3+ years of experience helping businesses make sense of their data. I have a strong background in banking, regulatory compliance, and digital transformation. I specialize in translating complex data into actionable insights that support strategic decision-making and operational efficiency. 

Through my experience in fintech and Agile environments, I've worked with SQL, Excel, and data visualization tools to improve data quality, streamline processes, and deliver business-driven solutions aligned with stakeholder needs.

I am actively interested in opportunities within leading UAE banks and consulting firms, where I can contribute to high-impact data and transformation projects in fast-paced, international environments.

Here is my CV in [pdf](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/CV%20-%20Data%20Analyst%20.pdf).

This repository showcases my projects, technical skills, and continuous learning journey in Data Analytics and Business Intelligence.

# Table of Contents
- [[About]](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#about)

- [[Portfolio Projects]](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#portfolio-projects)
  - Python
  - SQL
    - [Global GDP Analysis (1998-2024)](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#global-gdp-analysis-1998-2024)
    - [Global Layoffs Data Cleaning](https://github.com/rim-osman/Data-Analysis-Portfolio/blob/main/README.md#global-layoffs-data-cleaning)
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

**📌 Project Overview:** This project presents an end-to-end SQL-based analysis of global GDP trends from 1998 to 2024.
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
**Code:** [`Data Cleaning Layoffs.sql`](https://github.com/rim-osman/PortfolioProjects/blob/main/Data%20Cleaning%20layoffs%20Project.sql)

**📌 Project Overview:** This project focuses on cleaning and preparing a real-world layoffs dataset to ensure data quality, consistency, and usability for downstream analysis and visualization.
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
**3. Data Standardization:**
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

**Skills & Tools:** 

- SQL (SQLite & MySQL)
- Data Cleaning & Transformation
- Data Validation
- Handling Missing Data
- Window Functions (ROW_NUMBER)
- Data Standardization Techniques 


# Education 
Université Marie & Louis Pasteur, Besançon, France: Master of Science - MS, Business Intelligence, Sep 2022 - Oct 2024

Saint-Joseph University of Beirut, Lebanon: Bachelor's degree, Banking and Finance, 2016 - 2019

National Lebanese Baccalaureate: Science and Mathematics, 2014 - 2016


# Certificates
The best way to showcase my skills is by doing and sharing the work you've completed but certifications often reflect that effort and growth as well. I'm excited to share the certifications I've earned, which complement my hands-on experience in data and analytics: 
  - [Data Analytics Bootcamp Certification](https://www.linkedin.com/in/rim-osman/overlay/1772130321074/single-media-viewer/?profileId=ACoAADbIX08BF_tpDZPiItlm8tTyMkeY8AdQfHQ&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_featured_details%3BNaf1xv3jSJO8jZ%2FJUcmkmQ%3D%3D) (March 2026) (Youtube - Alexander Freberg)
  - [Atlassian Agile Project Management Professional Certificate](https://drive.google.com/drive/folders/1zpGHlPN5Q3eJp46ypW1ao6q1nN4jpYK-?usp=drive_link) (March 2025) (Coursera - Atlassian/LinkedIn Learning)
  - [JIRA: Basic Administration](https://www.coursera.org/account/accomplishments/verify/S7ZXNFMXNE53?utm_source=link&utm_medium=certificate&utm_content=cert_image&utm_campaign=pdf_header_button&utm_product=course) (April 2024) (Coursera - Atlassian/LinkedIn Learning)

# Contacts 
- LinkedIn: [@rimosman](https://www.linkedin.com/in/rim-osman/)
- Email: rimmosman@gmail.com
