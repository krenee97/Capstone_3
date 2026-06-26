# Capstone_3
# EmporiUm Sales Performance Review — Capstone 3: Analysis with Power BI

**Year Up United Data Analytics Training Academy — Week 12**
**Author:** Kendra Tyler

---

## Project Overview

EmporiUm is a "virtual student bookstore" that began in 2022 as a merger of a chain of college bookstore franchises with an online retailer selling books and tech gear. Today it sells a mix of books, apparel, art supplies, and general merchandise both in-store and online.

This project analyzes four years of EmporiUm sales data (FY2022–FY2025) and presents the results in a Power BI report built for the regional sales team — including the regional director, territory/state managers, and individual store managers.

**Audience for this report — East Region:**
| Role | Name |
|------|------|
| Regional Director | Ana Jilani |
| New York Store Manager | See Ellefson |
| Connecticut Store Manager | Ellen Lemon |

---

## Business Question

How has EmporiUm's sales performance trended over the last four years, and what do category, state, and top-seller patterns tell the sales team about where to focus inventory and merchandising decisions going forward?

---

## Data Sources

- **Sales data (Excel):** the primary transactional dataset covering FY2022–FY2025, including sale amount, date, category, and state.
- **Book list (text file):** titles and author names for "general audience" bookstore books, used to identify top-selling titles and exclude textbooks from that analysis.

---

## Data Cleaning & Modeling

Key steps taken in Power Query to prepare the data model:

- Built a combined Excel reference table joining book **title**, **author**, and **gross selling price** into a single view, which made it much easier to merge book details into the main sales data.
- Used Power BI's Power Query to clean and reshape both the Excel sales file and the Notepad (.txt) file containing book titles and author names before combining them.
- Merged the book title/author list with the sales data so top-selling titles could be identified by name and author, with textbooks excluded.
- Standardized state values — some records used full state names (e.g., "New York") while others used two-letter abbreviations (e.g., "NY"), which would have split single states into duplicate slices on the state-level chart if left uncorrected.
- Other cleaning steps: missing values, duplicate rows, relationship setup between tables.

---

## Report Structure

The report (`Tyler_capstone3.pbix`) contains two pages:

**Page 1 — Sales Overview**
- Line chart: total sales by year (FY2022–FY2025)
- Bar chart: total sales by category

**Page 2 — State & Top Sellers**
- Donut chart: relative sales by state
- Bar chart + table: top-selling general-audience books, with author and sales total

---

## Key Findings

- **Sales nearly doubled over four years** — from roughly $7.9M in FY2022 to $15.9M in FY2025 (+102%), with growth accelerating sharply in the most recent year.
- **Books are the dominant category**, generating far more revenue than apparel, art supplies, general merchandise, or stationery combined.
- **Maryland leads all states** at roughly a quarter of regional sales, followed by Colorado, Massachusetts, and New Jersey.
- **Top sellers span fiction and nonfiction alike** — *Harry Potter and the Sorcerer's Stone* (J.K. Rowling) is the #1 seller, but 6 of the next 8 titles are nonfiction or classics (*The Art of War*, two Stephen Hawking titles, *Of Mice and Men*, *Man's Search for Meaning*, *Meditations*), suggesting strong demand beyond bestselling fiction.

---

## Tools Used

- Microsoft Power BI Desktop (data modeling, Power Query, DAX, visualizations)
- Microsoft Excel (source data review)
- GitHub (version control)

---

## Deliverables

- **Power BI file:** `Tyler_capstone3.pbix` (this repository)
- **Published report:** [Tyler_capstone3 - Power BI]
- **10-minute video walkthrough:** [link to recording]
- **5-minute in-class presentation:** delivered live to the East region sales team

---

## How to View This Report

1. Open `Tyler_capstone3.pbix` in Power BI Desktop, **or**
2. View the published version in the class Power BI workspace: [ Tyler_capstone3 - Power BI  ]

---

## Author

**Kendra Tyler**
Data Analyst, EmporiUm
