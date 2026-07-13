# Digital Payments Analytics Dashboard

## Project Summary

An interactive Power BI dashboard developed to analyze UPI transaction data by exploring customer demographics, transaction patterns, device usage, payment methods, and account balances. The report incorporates dynamic chart switching, customer segmentation, and interactive filtering to provide a flexible and engaging analytical experience.

---

# Dashboard Preview

> *<img width="1240" height="697" alt="Image" src="https://github.com/user-attachments/assets/63da8964-1cd8-4293-b51f-3c99ee963011" />*

---

# Project Snapshot

| Category | Details |
|----------|---------|
| **Project Type** | Business Intelligence Dashboard |
| **Tool** | Microsoft Power BI |
| **Domain** | Digital Payments Analytics |
| **Dataset** | UPI Transaction Data |
| **Data Source** | CSV |
| **Data Preparation** | Power Query |
| **Data Modelling** | Relational Data Model |
| **Language** | DAX |
| **Dashboard Pages** | 2 |
| **Interactive Feature** | Dynamic Chart Switching |
| **Primary Analysis** | Customer Behaviour & Transaction Analysis |

---

# Project Overview

The rapid adoption of Unified Payments Interface (UPI) has generated large volumes of digital transaction data, making it increasingly important for financial institutions and analysts to understand customer behaviour and transaction trends. Interactive reporting enables users to monitor transaction activity, identify customer segments, and explore payment patterns efficiently.

This Power BI dashboard transforms raw UPI transaction data into an interactive reporting solution that combines demographic analysis with transaction insights. By incorporating dynamic chart switching and customer segmentation, the report allows users to customize their analytical experience while exploring key aspects of digital payment activity.

---

# Business Problem

Financial organizations require a clear understanding of customer transaction behaviour to identify usage trends, evaluate payment activity, and better understand their customer base. Analyzing large transaction datasets through spreadsheets is inefficient and limits the ability to uncover meaningful insights.

The objective of this project was to develop an interactive dashboard that simplifies transaction analysis while providing users with flexible visualization options and demographic segmentation.

---

# Project Objectives

- Build an interactive dashboard for analyzing UPI transaction data.
- Visualize customer demographics and transaction behaviour.
- Segment customers into meaningful age groups.
- Enable users to switch between different chart types dynamically.
- Improve the flexibility of data exploration through interactive report features.

---

# Tools & Technologies

| Tool | Purpose |
|------|----------|
| **Power BI Desktop** | Dashboard Development |
| **Power Query** | Data Preparation |
| **DAX** | Customer Segmentation |
| **Interactive Bookmarks** | Dynamic Visual Switching |

---

# Dataset Overview

The dashboard is built using UPI transaction data containing customer and transaction-related information.

The dataset includes information related to:

- Customers
- Customer Age
- Transaction Amount
- Account Balance
- Payment Method
- Device Type
- Transaction Type
- Merchant Information
- Transaction Status
- Additional transaction attributes used throughout the report

The dataset enables demographic analysis while supporting the exploration of customer payment behaviour across multiple dimensions.

---

# Data Preparation (Power Query)

Power Query was used to prepare the dataset before loading it into the Power BI model.

The preparation process included:

- Importing the transaction dataset.
- Validating data types.
- Preparing fields for reporting.
- Organizing the dataset for analytical visualization.

Performing these transformations before loading the data helps improve report efficiency while maintaining a clean reporting model.

---

# Data Model

The report is built using a relational data model designed to support interactive transaction analysis.

The model organizes customer and transaction information into a structure that enables consistent filtering across report visuals while maintaining efficient report performance.

This simplified modelling approach provides the flexibility required for demographic analysis, transaction reporting, and interactive dashboard navigation.

---

# DAX Implementation

The report uses a calculated column to categorize customers into meaningful age segments. Rather than analyzing every individual age, grouping customers into broader categories simplifies demographic reporting and makes it easier to compare transaction behaviour across different customer groups.

### Calculated Column

#### Age Groups

```DAX
Age Groups =
IF(
    'UPI Transactions'[CustomerAge] <= 25,
    "A1",
    IF(
        'UPI Transactions'[CustomerAge] <= 35,
        "A2",
        "A3"
    )
)
```

This calculated column classifies customers into three age categories:

- **A1** – Customers aged 25 years or below.
- **A2** – Customers aged between 26 and 35 years.
- **A3** – Customers older than 35 years.

Creating these predefined groups simplifies customer segmentation and enables report visuals to present demographic insights more effectively.

---

# Report Features

## Dynamic Chart Switching

The dashboard provides users with the ability to dynamically switch between **Line Charts** and **Column Charts** for both **Transaction Amount** and **Remaining Balance**.

This interactive functionality allows users to choose the visualization that best suits their preferred method of analysis without requiring multiple versions of the same visual on the report.

### Business Value

- Improves the overall user experience through interactive report navigation.
- Reduces dashboard clutter by eliminating duplicate visuals.
- Allows users to analyze trends using either continuous or comparative visualizations.
- Provides greater flexibility without increasing report complexity.

---

# Dashboard Walkthrough

## 1. Main Dashboard

> *<img width="1249" height="693" alt="Image" src="https://github.com/user-attachments/assets/17947fb4-4e60-43ae-9be3-2d4fe814ee41" />*

The main dashboard provides a comprehensive overview of UPI transaction activity by combining customer demographics with transaction-related information. Interactive visuals enable users to explore transaction behaviour across multiple dimensions while report filters allow deeper investigation of specific customer segments.

One of the key features of this page is the ability to dynamically switch between Line Charts and Column Charts for Transaction Amount and Remaining Balance, allowing users to personalize the way data is visualized based on their analytical preference.

### Business Value

- Provides a centralized view of UPI transaction activity.
- Enables demographic analysis through customer segmentation.
- Supports interactive exploration using report filters and slicers.
- Improves report usability through dynamic chart selection.

---

## 2. Details Page

> *<img width="1236" height="698" alt="Image" src="https://github.com/user-attachments/assets/bbe953cc-383f-4b77-99c1-8449ed6a2583" />*

The second page provides additional information that complements the main dashboard by allowing users to examine transaction records in greater detail.

This page supports more focused analysis while maintaining the filtering context established on the primary dashboard, making it easier to investigate specific customer or transaction-related information.

### Business Value

- Supports detailed transaction analysis.
- Complements the summary dashboard with additional information.
- Enables users to investigate specific records more efficiently.
- Improves the overall reporting workflow.

---

# Key Business Insights

The dashboard provides an interactive environment for analyzing UPI transaction data by combining customer demographics with transaction-level information.

The report enables users to:

- Explore transaction activity across different customer age groups.
- Compare transaction amounts and account balances using multiple visualization styles.
- Analyze customer behaviour through demographic segmentation.
- Interactively filter transaction data to focus on specific areas of interest.
- Investigate detailed transaction information through the secondary report page.

By consolidating customer and transaction information into a single reporting solution, the dashboard simplifies digital payment analysis and improves access to meaningful business information.

---

# Business Recommendations

The dashboard can support business users in several ways:

- Monitor transaction activity regularly to identify changes in customer behaviour.
- Use customer age segmentation to better understand different demographic groups.
- Leverage dynamic visual switching to explore trends from multiple analytical perspectives.
- Investigate detailed transaction information whenever unusual patterns are identified.
- Continue expanding customer segmentation to support more targeted business analysis.

These recommendations help organizations better understand digital payment behaviour while supporting data-driven decision-making.

---

# Technical Highlights

This project demonstrates several Power BI capabilities that enhance both report usability and analytical flexibility.

- Developed an interactive Power BI dashboard for UPI transaction analysis.
- Prepared transaction data using Power Query.
- Implemented a DAX calculated column for customer age segmentation.
- Designed an interactive reporting experience using dynamic chart switching.
- Reduced dashboard clutter by allowing users to switch between Line and Column charts without duplicating visuals.
- Combined demographic analysis with transaction reporting in a single dashboard.
- Created a user-friendly reporting interface focused on interactive data exploration.

---

# Skills Demonstrated

This project demonstrates practical Business Intelligence and Power BI development skills, including:

### Data Preparation

- Power Query
- Data import
- Data validation
- Dataset preparation

### Data Modelling

- Relational data modelling
- Relationship management
- Interactive filtering

### DAX

- Calculated Columns
- IF()

### Power BI Development

- Interactive dashboard design
- Dynamic chart switching
- Bookmarks and visual navigation
- Cross-filtering
- Slicers
- Multi-page reporting

### Business Analysis

- Customer segmentation
- Transaction analysis
- Digital payment analytics
- Demographic reporting
- Interactive business reporting

---

# Conclusion

This Power BI project demonstrates the development of an interactive dashboard for analyzing UPI transaction data through customer segmentation, demographic analysis, and transaction reporting. By combining Power Query, DAX, and interactive report design, the dashboard provides users with a flexible environment for exploring digital payment activity.

The implementation of a calculated column for age-based segmentation and dynamic chart switching enhances both analytical clarity and user experience. Overall, the project showcases practical Power BI development skills while delivering an intuitive reporting solution that supports informed analysis of UPI transaction data.
