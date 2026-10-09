# Consumer Spending Trends & Economic Insights

A beginner-level data analysis project demonstrating a reproducible Python workflow using **Pandas, Matplotlib, and Quarto**.

> **Data disclaimer:** The included dataset is synthetic and created for practice. It is not official Indian CPI, inflation, or consumer-spending data. Results must not be interpreted as real-world economic findings.

## Project Objectives

- Inspect and validate a tabular dataset
- Convert month values into date fields
- Aggregate sample inflation-style values by consumption category and residence type
- Visualize category averages and monthly trends
- Calculate month-to-month changes in year-over-year rate values
- Build reusable Python functions for summary statistics and charts
- Combine code, charts, and narrative in a Quarto report

## Tools Used

- **Python**
- **Pandas** — data loading, cleaning, grouping, aggregation
- **Matplotlib** — charts and visualisation
- **Quarto** — reproducible report authoring and HTML output
- **Git/GitHub** — project versioning and portfolio hosting

## Repository Contents

```text
consumer-spending-economic-insights/
├── README.md
├── consumer_spending.qmd
└── consumer_spending_raw_dataset.csv
```

## Analysis Included

1. **Data quality checks** — dataset dimensions, data types, missing values, duplicates, and date coverage.
2. **Category analysis** — average sample values by consumption category.
3. **Urban vs rural comparison** — monthly averages by residence type.
4. **Month-to-month change** — changes in the sample year-over-year rate, expressed in percentage points.
5. **Reusable functions** — functions for summary statistics and monthly trend visualisation.
6. **Quarto report** — code, charts, interpretation, limitations, and references in one document.

## Run the Project

### 1. Install prerequisites

Install [Python](https://www.python.org/downloads/) and [Quarto](https://quarto.org/docs/get-started/).

Install the Python packages:

```bash
python -m pip install pandas matplotlib jupyter pyyaml
```

### 2. Render the report

Open a terminal in the repository folder and run:

```bash
quarto render consumer_spending.qmd
```

Quarto should create `consumer_spending.html`, which can be opened in a web browser.

## Data Dictionary

| Column | Description |
|---|---|
| `month` | Month in `YYYY-MM` format |
| `country` | Country label used in the sample |
| `region` | Region label used in the sample |
| `residence_type` | Urban or rural sample group |
| `consumption_category` | Sample consumption category |
| `yoy_inflation_pct` | Synthetic illustrative year-over-year rate, in percent |
| `illustrative_price_index` | Synthetic example index value; not an official price index |
| `data_status` | Marks records as synthetic examples |

## Limitations

- The dataset is synthetic and is not suitable for conclusions about India's economy.
- The sample covers only January–April 2025 and four consumption categories.
- No causal relationships can be inferred.
- The illustrative price index is not an official price index.
- Category and residence comparisons describe only the sample values.

## Future Improvements

- Replace the synthetic dataset with verified public economic data.
- Document the source URL, download date, units, definitions, and update frequency.
- Add tests for data validation and reusable functions.
- Expand the analysis with compatible expenditure and economic indicators.
- Publish a rendered HTML report alongside the source code.

## References

- [Quarto documentation](https://quarto.org/docs/)
- [MoSPI eSankhyiki portal](https://esankhyiki.mospi.gov.in/)
- [Reserve Bank of India Database on Indian Economy](https://dbieold.rbi.org.in/DBIE/)

---

Created as a learning and portfolio project to practise Python-based data analysis and reproducible reporting.
