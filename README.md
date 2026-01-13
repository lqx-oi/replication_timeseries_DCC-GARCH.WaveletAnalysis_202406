# Replication-202406
## A Study on the Effectiveness of Corn Futures as a Safe-Haven Asset During the Russia-Ukraine Conflict - Based on DCC-GARCH and Wavelet Analysis
This repository hosts the final paper for the junior-year Applied Economics course, which replicates the time series study *Wheat as a hedge and safe haven for equity investors during the Russia–Ukraine war*.

**Study Overview:** This study aims to investigate the performance of corn futures as a safe-haven asset during the Russia–Ukraine war. We collected the daily closing prices of corn futures and the daily prices of stock indices in China, Japan, and the United States for both the pre-conflict and post-conflict periods of the Russia–Ukraine war. 

By applying the Dynamic Conditional Correlation Generalized Autoregressive Conditional Heteroskedasticity (DCC-GARCH) model and wavelet analysis, we analyzed the volatility relationship between corn futures and the stock indices of each country. We also derived the calculation formula for optimal weights by minimizing portfolio risk.

The empirical results indicate that corn futures exhibited heterogeneous safe-haven characteristics across different markets during the Russia–Ukraine war and demonstrated sound overall performance, providing crucial insights for investors in their asset allocation decisions amid global uncertainty.

**Key Modifications from the Original Paper**

| **Modification Dimension** | **Original Paper (Wheat Study)** | **This Replication (Corn Futures Study)** |
|-----------------------------|----------------------------------|-------------------------------------------|
| Research Core Asset         | Wheat                            | Corn futures                               |
| Research Target Markets     | Equity indices of 5 countries: France (CAC40), Germany (DAX30), UK (FTSE100), Italy (FTSE/MIB), US (S&P500) | Equity indices & corn futures markets of 3 countries: China (Shanghai Composite Index, Dalian Commodity Exchange), US (S&P500, Chicago Mercantile Exchange), Japan (Nikkei 225, Tokyo Grain Exchange) |
| Data Time Span              | 2020-01-01 to 2022-08-12<br>Pre-war: 2020-01-01 to 2022-02-23<br>War period: 2022-02-24 to 2022-08-12 | 2020-03-16 to 2022-12-30<br>Pre-war: 2020-03-16 to 2022-02-23<br>War period: 2022-02-24 to 2022-12-30 |
| Data Processing Details     | Daily return formula: $\ln [P_{i}(t)-P_{i}(t-1)]$<br>No exchange rate conversion | Daily return formula: $\frac{P_{i t}-P_{i(t-1)}}{P_{i(t-1)}}$<br>Collected daily USD/CNY and JPY/CNY exchange rates to unify corn futures units to CNY/ton |

**Main Research Methods:** Time series data processing;Dynamic Conditional Correlation Generalized Autoregressive Conditional Heteroskedasticity (DCC-GARCH) model;Wavelet analysis.

**Project Documentation:** Data employed;relevant regression results;code for graph generation;initial draft of the paper;presentation slides (PPT).

**Reference:** *Ghorbali, B., Kaabia, O., Naoui, K., Urom, C., & Ben Slimane, I. (2023). Wheat as a hedge and safe haven for equity investors during the Russia–Ukraine war. Finance Research Letters, 58, 104534.*
