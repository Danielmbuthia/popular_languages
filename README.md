# Programming Language Popularity Analysis

This project analyzes the popularity trends of various programming languages based on Stack Overflow post counts from 2008 to 2024.

## Overview

This analysis explores the historical trends of programming language popularity using Stack Overflow data. The dataset includes monthly post counts for 14 major programming languages including Python, JavaScript, Java, C++, and others.

## Data Source

- Dataset: `QueryResults.csv`
- Time period: July 2008 - October 2024
- Metrics: Monthly post counts per programming language
- Languages tracked: 14 (assembly, c, c#, c++, delphi, go, java, javascript, perl, php, python, r, ruby, swift)

## Analysis Features

1. **Data Processing**

   - Cleaned and transformed datetime data
   - Handled missing values
   - Reshaped data for time series analysis

2. **Visualizations**
   - Individual language trends
   - Comparative analysis between languages
   - Smoothed trend lines using rolling averages (3, 6, and 12-month windows)

## Key Findings

- JavaScript and Python show strong upward trends over time
- Some newer languages like Go and Swift have fewer data points but show growth
- Traditional languages like C and C++ maintain steady presence
- Seasonal variations are visible in post patterns

## Visualizations

### Raw Data Trends

![Programming Language Trends](path_to_raw_trends.png)
_Figure 1: Monthly post counts for all programming languages_

### Smoothed Trends (12-month rolling average)

![Smoothed Programming Language Trends](path_to_smoothed_trends.png)
_Figure 2: Smoothed trends showing clearer long-term patterns_

## Technologies Used

- Python 3.x
- Pandas for data manipulation
- Matplotlib for visualization
- Jupyter Notebook for analysis

## Setup and Usage

1. Clone the repository
2. Install required packages:

```bash
pip install pandas matplotlib jupyter
```

3. Run the Jupyter notebook:

```bash
jupyter notebook Programming_Languages.ipynb
```

## Data Structure

The analysis uses two main dataframes:

- Original format: Date, TagName, PostCount
- Reshaped format: Date as index, with columns for each programming language


