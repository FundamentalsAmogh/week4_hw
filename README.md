# Week 4 Homework 4: Merging, Aggregating, Reshaping

**GitHub Pages:** https://fundamentalsamogh.github.io/week4_hw/

## Overview

This project performs data manipulation on the CIA World Factbook health datasets from Homework 3, demonstrating merging, aggregating, and reshaping operations.

## Data Sources

Uses 3 cleaned CSV files from [Homework 3](https://github.com/FundamentalsAmogh/week3_hw):
- `maternal_mortality.csv`
- `infant_mortality.csv`
- `life_expectancy.csv`

## Exercises

### Exercise 1: Merging
- Merged all 3 datasets by country using `merge()`
- Output: `merged_data.csv` (227 countries, 5 columns)

### Exercise 2: Aggregating
- Aggregated by region using `mean` function
- Output: `aggregated_data.csv` (10 regions, 4 columns)

### Exercise 3: Reshaping
- Converted wide format to long format using `reshape()`
- Output: `long_data.csv` (681 rows, 4 columns)

## Files

| File | Description |
|------|-------------|
| `HW4_Merging_Aggregating_Reshaping.ipynb` | Original Colab notebook |
| `HW4_Merging_Aggregating_Reshaping.Rmd` | Converted RMarkdown file |
| `index.html` | Knitted HTML output |
| `merged_data.csv` | Exercise 1 output |
| `aggregated_data.csv` | Exercise 2 output |
| `long_data.csv` | Exercise 3 output |

## How It Was Done

1. Created notebook in Google Colab (R kernel): [Colab Link](https://colab.research.google.com/drive/1k0qvJv0Q7uNvDU06WuwNmXuEkPGlK-Ey?usp=sharing)
2. Loaded 3 CSV files from Homework 3
3. Merged datasets using `merge()` with full outer join
4. Aggregated by region using `aggregate()` with `FUN = mean`
5. Reshaped wide to long using `reshape()` with `direction = "long"`
6. Converted `.ipynb` to `.Rmd` using `rmarkdown::convert_ipynb()`
7. Knitted to HTML and renamed to `index.html`
