# Data Preparation & Cleaning Steps

This document outlines the detailed process of preparing and cleaning the Udemy dataset before creating the Power BI dashboard.

## 1. Data Loading
- Imported `udemy_courses.xlsx` into Power BI.

## 2. Data Cleaning
- **Duplicates:** Removed duplicate course entries.
- **Missing Values:**
  - `price`: Filled with `0` for free courses.
  - `num_subscribers` & `num_reviews`: Filled with `0`.
- **Date Format:** Converted `published_timestamp` to Date format.
- **Category Standardization:** Ensured consistent naming for `subject` and `level`.

## 3. Data Transformation
- Created **Year** column from `published_timestamp`.
- Calculated **Revenue** = `price × num_subscribers` (paid courses only).
- Categorized into **Free** and **Paid** courses.

## 4. Data Validation
- Checked for outliers and unrealistic values in `price`, `num_subscribers`, and `content_duration`.
