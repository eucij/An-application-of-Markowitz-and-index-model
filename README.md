# Portfolio Optimization Using Markowitz and Index Models

This project implements a real-world application of the Markowitz mean-variance framework alongside the Index model, utilizing 20 years of historical data from 10 well-known U.S. companies and the S&P 500 index.

The methodology follows the standard mean-variance optimization process and employs matrix algebra to calculate portfolio returns and standard deviations.

## Features

- **Data**: 20 years of daily returns for 10 major U.S. stocks and the S&P 500 index.
- **Models**: 
  - Markowitz Model
  - Index Model
- **Normality Check**: 
  - Visualizes the distribution of daily and monthly returns.
  - Performs normality tests on the returns.
  - Apply the Central Limit Theorem (CLT) by aggregating daily returns into monthly returns.
- **Computation Tools**: 
  - Utilizes solver and solvertable to perform the portfolio optimization calculations.

## Constraints

The optimization is performed under five different constraints:

1. Sum of the absolute values of all asset weights ≤ 2 (limiting overall leverage).
2. Absolute value of each individual asset weight ≤ 1.
3. No constraints.
4. All asset weights must be non-negative (no short selling allowed).
5. Portfolio excluding the S&P 500 index.

For each constraint, the following portfolio characteristics are computed:

- Efficient Frontier
- Minimum Variance Portfolio
- Maximum Sharpe Ratio Portfolio

Since the analysis is conducted for both the Markowitz and Index models, the project covers a total of 10 distinct optimization scenarios.
