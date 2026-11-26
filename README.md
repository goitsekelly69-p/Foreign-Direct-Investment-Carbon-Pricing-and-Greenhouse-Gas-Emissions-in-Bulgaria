# Foreign Direct Investment, Carbon Pricing and Greenhouse Gas Emissions in Bulgaria: A Replication and Extension

## 1. Project Overview

This project replicates and extends the empirical study by Zhelev et al. (2026), which investigates the relationship between sectoral Foreign Direct Investment (FDI), income and greenhouse gas (GHG) emissions in Bulgaria using a Nonlinear Autoregressive Distributed Lag (NARDL) framework.

The extension examines whether carbon pricing under the European Union Emissions Trading System (EU ETS) influences the relationship between manufacturing FDI and greenhouse gas emissions.

The study uses quarterly data for Bulgaria, covering 2014Q1–2024Q2 for the replication and 2014Q1–2025Q4 for the extended analysis.

The empirical investigation combines time-series econometrics, error-correction modelling, hypothesis testing and robustness analysis to examine both short-run and long-run relationships.

## 2. Research Objectives

The project has two main components.

### Part A: Replication

- Reproduce the NARDL specification used by Zhelev et al. (2026).
- Examine the asymmetric effects of positive and negative manufacturing FDI shocks on greenhouse gas emissions.
- Investigate the relationship between GDP per capita, construction FDI and emissions.
- Compare the replication results with the findings of the original study.
- Assess the sensitivity of the results to alternative lag structures and model specifications.

### Part B: Extension – Carbon Pricing

- Investigate whether EU ETS carbon prices influence the relationship between manufacturing FDI and greenhouse gas emissions.
- Examine whether higher carbon prices weaken the short-run emission-increasing effect of positive manufacturing FDI shocks.
- Investigate whether higher carbon prices strengthen the long-run emission-reducing association between manufacturing FDI and emissions.
- Estimate interaction effects between carbon prices and positive and negative manufacturing FDI shocks.
- Evaluate the robustness of the findings using alternative model specifications.

## 3. Data and Variables

The empirical analysis uses quarterly data for Bulgaria.

The replication covers 2014Q1–2024Q2, comprising 42 observations before accounting for lags.

The extended analysis covers 2014Q1–2025Q4, comprising 48 observations before accounting for lags.

### Main Variables

| Variable | Description |
|---|---|
| GHG | Greenhouse gas emissions per capita |
| MAN | Manufacturing Foreign Direct Investment |
| CON | Construction Foreign Direct Investment |
| GDPPC | GDP per capita |
| CP | EU ETS carbon allowance price |

The extension incorporates the EU ETS carbon allowance price as an additional explanatory variable and examines its interaction with manufacturing FDI.

### Data Preparation

The data preparation process involves:

- Importing and organising quarterly time-series data.
- Constructing positive and negative partial sums of manufacturing FDI and GDP per capita.
- Examining quarterly seasonality.
- Conducting Augmented Dickey-Fuller (ADF) and Phillips-Perron (PP) unit root tests.
- Standardising variable units for the extended model.
- Centring carbon prices around their sample mean.
- Constructing interaction terms between carbon prices and positive and negative manufacturing FDI shocks.

## 4. Econometric Methodology

The study employs the Nonlinear Autoregressive Distributed Lag (NARDL) framework developed by Shin, Yu and Greenwood-Nimmo (2014).

The NARDL approach allows positive and negative changes in explanatory variables to have potentially different effects on the dependent variable.

### 4.1 Positive and Negative Partial Sums

Manufacturing FDI and GDP per capita are decomposed into positive and negative cumulative partial sums.

This allows the model to distinguish between the effects of increases and decreases in these variables on greenhouse gas emissions.

### 4.2 Error-Correction Modelling

The NARDL specification is estimated in its error-correction representation to distinguish between short-run dynamics and long-run relationships.

The analysis examines the error-correction coefficient and its statistical significance to assess adjustment towards long-run equilibrium.

### 4.3 Bounds Testing

The Pesaran, Shin and Smith (2001) bounds-testing approach is used to investigate the existence of a long-run relationship among the variables.

Sample-specific critical values are considered in the analysis because of the relatively small sample size.

### 4.4 Lag Selection

The Bayesian Information Criterion (BIC) is used to guide the selection of lag structures.

Alternative lag specifications are also examined to assess the sensitivity of the estimated relationships.

### 4.5 Carbon-Price Interaction Models

The extended analysis estimates three principal specifications:

- **M0 – Baseline NARDL:** Includes manufacturing FDI, GDP per capita and construction FDI.
- **M1 – Carbon-Price Model:** Extends the baseline specification by incorporating the EU ETS carbon price.
- **M2 – Interaction Model:** Further incorporates interactions between carbon prices and positive and negative manufacturing FDI shocks.

Additional specifications examine positive-shock-only moderation and the inclusion of a linear time trend.

### 4.6 Hypothesis Testing

Three hypotheses are investigated:

- H1: Positive manufacturing FDI shocks increase greenhouse gas emissions in the short run.
- H2: Higher carbon prices weaken the short-run emission-increasing effect of positive manufacturing FDI.
- H3: Higher carbon prices strengthen the long-run emission-reducing association between positive manufacturing FDI and emissions.

### 4.7 Diagnostic and Robustness Testing

The analysis incorporates several diagnostic procedures:

- Breusch-Godfrey test for serial correlation.
- Breusch-Pagan test for heteroskedasticity.
- Jarque-Bera test for residual normality.
- Ramsey RESET test for functional-form misspecification.
- CUSUM and CUSUM-of-squares procedures for parameter stability.
- Variance Inflation Factors (VIF) for multicollinearity assessment.
- Alternative lag structures and sample specifications.

## 5. Empirical Findings

### 5.1 Replication Results

The replication produces coefficient signs that are broadly consistent with the original study, although not all estimated relationships are statistically significant.

The long-run coefficient for positive manufacturing FDI is negative but statistically insignificant (p = 0.248).

The short-run results provide evidence of an emission-increasing effect associated with a positive manufacturing FDI shock at the third lag.

The error-correction coefficient is negative and statistically significant, suggesting adjustment towards a long-run relationship.

However, the replication also identifies residual serial correlation, and the results demonstrate sensitivity to alternative lag structures.

### 5.2 Carbon-Pricing Extension

The inclusion of carbon prices improves the baseline model's performance according to the information criteria.

However, the additional interaction terms in M2 do not significantly improve the model relative to M1 (F = 1.09, p = 0.381).

The estimated long-run interaction coefficients are negative:

- Positive manufacturing FDI × carbon price: -0.0059 (p = 0.402).
- Negative manufacturing FDI × carbon price: -0.0072 (p = 0.369).

Although the negative coefficients are consistent with a potentially stronger emissions-reducing association at higher carbon prices, they are not statistically significant.

### 5.3 Hypothesis Testing

None of the three hypotheses is supported at the 10% significance level.

| Hypothesis | One-sided p-value | Outcome |
|---|---:|---|
| H1: Positive manufacturing FDI increases emissions in the short run | 0.784 | Not supported |
| H2: Carbon prices weaken the short-run effect | 0.840 | Not supported |
| H3: Carbon prices strengthen the long-run emissions-reducing effect | 0.201 | Not supported |

The results therefore do not provide robust empirical evidence that carbon prices moderate the relationship between manufacturing FDI and greenhouse gas emissions.

### 5.4 Robustness and Limitations

The analysis identifies several limitations that affect the interpretation of the results:

- The relatively small quarterly sample limits the number of parameters that can be reliably estimated.
- High correlations between explanatory variables and interaction terms create multicollinearity concerns.
- Residual serial correlation is identified in some of the extended specifications.
- The EU ETS carbon price is common across EU countries and exhibits a strong upward trend over the sample period.
- The findings describe time-series relationships and should not be interpreted as establishing causality.

These limitations are considered when interpreting the empirical results.

## 6. Tools and Technologies

**Programming Language**
- Python

**Python Libraries**
- Pandas – Data manipulation and preparation.
- NumPy – Numerical computations and variable construction.
- Matplotlib – Data visualisation.
- Statsmodels – Econometric estimation, time-series analysis and diagnostic testing.
- SciPy – Statistical inference and hypothesis testing.
- Arch – Phillips-Perron unit root testing (optional dependency).

**Development Environment**
- Jupyter Notebook

## 7. My Contribution

This was a collaborative academic research project completed with G. Addai and M. A. Hlongwane.

My contribution focused primarily on the computational and empirical components of the research, including:

- Developing and implementing Python code for data preparation and econometric analysis.
- Constructing positive and negative partial sums for the NARDL framework.
- Implementing the error-correction representation and bounds-testing procedures.
- Conducting lag selection using the Bayesian Information Criterion.
- Estimating baseline, carbon-price and interaction models.
- Computing short-run and long-run effects.
- Conducting hypothesis tests and evaluating marginal effects at different carbon-price levels.
- Performing diagnostic tests and robustness checks.
- Interpreting and evaluating the empirical results in relation to the research hypotheses.

The project involved collaborative research and contributions from all group members.

## 8. Repository Contents

- `International Finance.ipynb` – Jupyter Notebook containing the Python implementation, data preparation, variable construction, econometric estimation, diagnostic testing and empirical analysis.
- `International Finance.pdf` – The accompanying research report documenting the research background, literature review, methodology, empirical findings and conclusions.
- `Data/` – Contains the quarterly datasets used for the replication and extended analysis:
  - `Bulgaria Replication Data.csv`
  - `Bulgaria Extension Data.csv`
  - `Carbon Price.csv`

## 9. Reproducing the Analysis

The analysis can be reproduced using Python and Jupyter Notebook.

1. Clone or download this repository.
2. Ensure that Python 3.10 or later is installed.
3. Install the required Python packages.
4. Ensure that the three CSV datasets are located in the `Data/` directory.
5. Open `International Finance.ipynb` in Jupyter Notebook or JupyterLab.
6. Execute the notebook sequentially from beginning to end.

Install the required packages using:

`pip install pandas numpy matplotlib statsmodels scipy arch`

An active Python environment and the appropriate package versions are required to reproduce the analysis.

## 10. Research Status and Usage Notice

**Status: Unpublished Academic Research**

This project represents collaborative academic research completed as part of postgraduate coursework at the University of Johannesburg. The replication and extension presented in this report have not been formally published as a separate academic journal article or other scholarly publication.

The repository is made publicly accessible for portfolio and demonstration purposes, subject to the rights and permissions of all contributors and applicable academic requirements.

The original research by Zhelev et al. (2026) is acknowledged and referenced in the accompanying report. This project should not be confused with or presented as the original publication.

The research report, Python implementation, analysis and original contributions remain subject to the intellectual property rights of their respective authors and contributors.

Public access does not grant permission to reproduce, redistribute, adapt, commercially exploit or otherwise use the original project materials.

This work should not be represented or cited as a formally published scholarly article. 

## 12. References

Zhelev, P. et al. (2026). Green shifts in foreign capital: Asymmetric effects of FDI and income on CO2 emissions in Bulgaria. *Research in Globalization*, 12, 100353.

Shin, Y., Yu, B. and Greenwood-Nimmo, M. (2014). Modelling asymmetric cointegration and dynamic multipliers in a nonlinear ARDL framework.

Pesaran, M. H., Shin, Y. and Smith, R. J. (2001). Bounds testing approaches to the analysis of level relationships. *Journal of Applied Econometrics*, 16(3), 289–326.
