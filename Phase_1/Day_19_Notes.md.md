# Phase 1 – Notes from Days 1 to 16

## Three things I noticed

1. I began with a very simple Python program on Day 1, then moved on to working with NIFTY options data. Most of the datasets use the same nine columns: `datetime`, `strike_price`, `right`, `open`, `high`, `low`, `close`, `open_interest`, and `volume`.

2. In the Day 9 analysis, `open_interest` had a positive correlation of **0.3388** with `volume`. Its correlation with `close` was **-0.0220**, which is very close to zero. In that particular dataset, volume had a clearer relationship with open interest than closing price did.

3. I used histograms and boxplots to get a better feel for the data, including the distribution of numeric columns and closing prices for CE and PE options. I also made correlation heatmaps and scatter plots to compare features. These plots helped me explore patterns instead of relying only on the first few rows or summary tables.

## One data quality issue I checked

In the data-quality checks shown in the early notebooks (Days 2 to 6), I found **no missing values and no duplicate rows** in the datasets checked. I also noticed that some rows have zero values for `open_interest` or `volume`. I left those values as they were, because I did not confirm that they were errors.

## What I built

I started with a basic Python program and gradually built notebooks to load NIFTY options CSV files, inspect the data, calculate summary statistics, check missing values and duplicates, and create histograms, boxplots, heatmaps, and scatter plots.

## What broke

The notebooks use different CSV files and file paths. Because of that, I need to make sure the correct CSV is in the expected location before running a notebook. I did not see a clear code error in the saved outputs I reviewed.

## What I learned

I got more practice with pandas, Seaborn, and Matplotlib. I learned how to check a dataset before analysing it, compare CE and PE options, read correlation values, and use different plots to understand the data more clearly.

---

*These notes are a short summary of the work shown in the Day 1–16 notebooks. The correlation values above are from Day 9 specifically, not from every dataset.*
