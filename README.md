# The Impact of Recreational Marijuana Legalization on Binge Drinking in the U.S.

## Overview

This project analyzes the impact of recreational marijuana legalization on adult binge drinking behavior across U.S. states using a Difference-in-Differences (DiD) approach. It was developed as a final assignment for the SS154 (Econometrics and Economic Systems) course at Minerva University during the Spring 2025 semester.

## Data Access

The cleaned dataset is publicly available and can be accessed [here](https://drive.google.com/file/d/1Ny8vG2mAt4j7UP_K6-bXP-SjBnMwBxgZ/view?usp=sharing) via Google Sheets or [downloaded here](https://docs.google.com/spreadsheets/d/e/2PACX-1vS-Qiz6Osc9I39bvo_94Mo1GvYe_ghAVboqYvR5xu6ZSPDI-ESb6ECCXgocUP3ALVQ3oxi_n3wDihQL/pub?gid=1277276287&single=true&output=csv) as a CSV.

It includes annual panel data for all 50 U.S. states from 2011 to 2016, merged from multiple sources including BRFSS and the U.S. Census Bureau.

## What the Code Does

- Merges demographic and behavioral data across multiple sources (CDC BRFSS, U.S. Census).
- Defines treatment as the year a state implemented recreational marijuana legalization.
- Estimates Average Treatment Effects using the `did` package and Callaway & Sant’Anna (2021) methodology.
- Creates:
  - Event study plots comparing pre- and post-treatment effects.
  - ATT visualizations by group and over time.
  - Trends for treated vs. control states.
  - State-by-state visualizations of binge drinking over time.
- Uses `ggplot2` with a custom serif theme for consistent academic-style plots.

## How to Navigate the Repository

1. Open `code.Rmd` to view or run the analysis.
2. To view without executing code, use the HTML or PDF files.
3. To change fonts, modify `serif.css` or `theme_serif()` in the Rmd.
4. All plots and outputs use serif font for consistency in publication-quality formatting.

## Reproducibility

- The dataset is directly pulled from a [hosted Google Sheet](https://drive.google.com/file/d/1Ny8vG2mAt4j7UP_K6-bXP-SjBnMwBxgZ/view?usp=sharing) using `read.csv(url)`.
- All fonts used are open system fonts or default fonts in R.

## Project Files

| File              | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| `code.Rmd`        | Main analysis script (R Markdown)                                           |
| `code.html`       | Rendered HTML output of the analysis                                        |
| `code.pdf`        | PDF version of the rendered analysis                                        |
| `data.csv`        | Final cleaned dataset (50 U.S. states × 13 years)                           |
| `serif.css`       | Custom CSS stylesheet for serif typography in HTML                          |
| `Final_Paper.pdf` | Full writeup with figures, discussion, and appendices                       |
| `README.md`       | Project documentation (this file)         
