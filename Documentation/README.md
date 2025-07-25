# Tata Data Visualization Project Documentation

## Introduction

This document provides detailed context, methodology, and explanations related to the Tata Data Visualization Virtual Micro-Internship project conducted for an online retail business. The analysis aims to assist the CEO and CMO by uncovering key business insights through comprehensive Tableau dashboards.

## Project Background

An online retail business engaged this project to evaluate its current performance and identify the key drivers of revenue growth from both operational and marketing perspectives. The leadership intends to expand the business strategically by focusing on high-impact areas illuminated through data analysis.

Key questions addressed include:

- Which months generate the most revenue?  
- Is there clear sales seasonality?  
- Which customers repeat purchases most often and how much do they contribute to revenue?  
- What operational and marketing metrics best guide expansion decisions?

## Data Cleanup Process

Data integrity and accuracy are critical for dependable insights. The raw sales data was cleaned thoroughly within Tableau before creating the dashboards.

**Key Cleanup Steps:**

- **Quantity Filter:** All records where `Quantity < 1` were excluded to eliminate returns, adjustments, or erroneous entries that would skew revenue calculations.  
- **Unit Price Filter:** All records with `Unit Price < 0` were filtered out as negative prices are invalid in the context of sales transactions.  

These filters were implemented as data source filters in Tableau with the following logical expressions:

- `[Quantity] >= 1`  
- `[Unit Price] >= 0`  

Additional attention was given to removing duplicates and ensuring data completeness, especially for critical fields such as Invoice Number, Customer ID, and Transaction Date.

![Data Cleanup Documentation](Images/Data%20Cleanup%20Documentation.png)

A calculated field of 'Revenue' was created in Tableau using 'Sales' and 'Unit Price' columns.

## Project Deliverables

- **Interactive Tableau Dashboards:** Comprehensive visual analysis covering seasonality, customer segmentation, revenue contributions, and important KPIs.  
- **Supporting Documentation and Screenshots:** Detailed explanations and visuals of the data cleanup processes and dashboard snapshots.  
- **Business Insights & Recommendations:** Actionable outputs tailored to help senior leadership make data-driven decisions for expanding market reach and optimizing marketing/inventory strategies.

## Repository Structure Overview

