# Day 17 – NIFTY Options Data

## What I found

1. The `open`, `high`, `low`, and `close` columns have a correlation of **1.0000** with each other in the correlation matrix. In this dataset, these price columns move very closely together.
2. `open_interest` has a very weak positive correlation with `close` (**0.0668**) and `high` (**0.0671**). So, there is almost no clear linear relationship between them in this data.
3. Of the variables I compared with `open_interest`, `volume` has the strongest positive correlation (**0.1020**). Its correlation with `strike_price` is slightly negative (**-0.0175**), which is very close to zero. The scatter plots also show that most observations are at lower open-interest values, while a smaller group is much higher.

## Data quality check

The dataset has **13,720 rows and 9 columns**. Every column has 13,720 non-null values, so the `DataFrame.info()` output shows **no missing values**.

## What I built

I loaded the NIFTY options dataset, checked its structure, made a correlation heatmap, and plotted open interest against close, volume, strike price, and high.

## What broke

I did not see a code error in the saved notebook output. One thing to remember is the CSV file path: the notebook expects the file at `/content/NIFTY-02JAN25-04DEC24.csv`. The file needs to be in that location when the notebook runs.

## What I learned

I learned how to use a correlation heatmap and scatter plots to explore how columns are related. I also practised checking for missing values before starting the analysis.

---

*These notes are based on the saved Day 17 notebook outputs. I have not added histogram findings because histogram results were not shown in the outputs I reviewed.*
