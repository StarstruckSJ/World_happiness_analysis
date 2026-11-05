# World Happiness Analysis

This project examines country-level life evaluations in the 2025 World Happiness Report dataset.

## Research question

What factors are associated with happiness across countries?

## Dataset

The dataset is from Figure 2.1 of the [World Happiness Report 2025](https://www.worldhappiness.report/data-sharing/). The full workbook contains 2,116 country-year observations. This analysis uses the 2025 cross-section, which includes 147 countries. The 2025 life-evaluation scores are three-year averages covering 2022–2024.

The outcome variable is the country life-evaluation score, measured using the Cantril ladder. The other variables are the Report’s contributions associated with log GDP per capita, social support, healthy life expectancy, and freedom to make life choices. These are contribution values, not raw measurements of those underlying factors.

## Methods

The analysis includes descriptive statistics, scatter plots, Pearson correlations, and an Ordinary Least Squares (OLS) regression. The Breusch–Pagan test is used to check for heteroskedasticity. The regression results are reported with HC3 robust standard errors.

The regression uses 145 observations after excluding cases with missing model variables. Zero contribution values are retained because the Report’s method allows a factor’s contribution to be zero at its lowest comparison point (called “Dystopia” in the Report).

## Limitations

This is a cross-sectional analysis, so the results describe associations and do not establish causation. The explanatory variables are Report contribution values rather than raw measures of the underlying conditions, which affects how the regression results should be interpreted.

## Running the analysis

Open the notebook in Jupyter and run its cells from top to bottom. Before running the notebook, update the file path in the first code cell so it points to the Excel workbook in your repository.
