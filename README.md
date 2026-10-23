# ASOS Revenue Cleaning

Python basics applied to messy weekly revenue figures: converting mixed text and numbers, then comparing monthly totals and averages.

**Notebook:** [M2_ASOS_Analyzing_Revenue.ipynb](M2_ASOS_Analyzing_Revenue.ipynb)

This is a milestone project from the Global Career Accelerator program. The scenario and data come from the program. It is not work done for ASOS.

## Context

The scenario is set at ASOS, the online fashion retailer, from the point of view of a junior data analyst. The data is a list of 14 weeks of estimated weekly revenue (in millions of pounds) covering June to August. Some values are stored as text, so Python cannot add the list up until it is cleaned.

## Tools and skills

- Python, Jupyter
- Lists, `for` loops, type conversion with `int()`
- Slicing a list into periods
- `sum()`, `len()` and f-strings for summaries

## Approach

1. Showed why summing the raw list fails: it mixes integers and strings.
2. Converted every value to an integer in a loop and stored the result in a new list.
3. Sliced the cleaned list into June (4 weeks), July (5 weeks) and August (5 weeks).
4. Calculated the total and the average weekly revenue for each month.

## Key findings

- **Cleaned total:** 1,038 (£ millions) across the 14 weeks.
- **July had the highest average weekly revenue** at £76.8m, against £70.5m in June and £74.4m in August.
- **Revenue rose from June to July and dipped in August.** Possible reasons are summer promotions and discounts, and price changes driven by inflation.
- **Next step:** check whether promotions ran in particular weeks and look at economic conditions week by week.

## How to run

No data files are needed. The revenue figures are written into the notebook. Open `M2_ASOS_Analyzing_Revenue.ipynb` in Jupyter and run the cells from the top.

Two cells end in a `TypeError` on purpose: they show why the raw list cannot be summed and why `int()` cannot take a whole list.

Requirements: Python 3 (the notebook was saved with Python 3.10.6) and Jupyter. No other packages are used.

## Repo structure

```
asos-revenue-cleaning-python/
└── M2_ASOS_Analyzing_Revenue.ipynb   analysis notebook with saved outputs
```
