# FTSE 100 Index Tracking Portfolio Optimization

## Overview

This report focuses on the optimization of a portfolio designed to track the **FTSE 100 index**. The objective is to minimize the variance of the tracking error by selecting a combination of 30 stocks. The portfolio is constructed using **Lagrangian optimization** and has specific constraints, including the sum of the weights equaling 1 and the mean tracking error being zero.

## Objective

The primary goal is to create a portfolio of 30 stocks that tracks the FTSE 100 index as closely as possible, minimizing the variance of the tracking error while maintaining the following constraints:

1. The sum of the portfolio weights must equal 1.
2. The mean tracking error should be zero.

## Approach

### 1. **Data Collection**
- Collected data on stocks in the FTSE 100 index.
- Ensured the stocks selected have sufficient historical price data for performance analysis.

### 2. **Portfolio Construction**
- Used a set of 30 stocks from the FTSE 100.
- The portfolio was designed to replicate the performance of the FTSE 100 index as closely as possible.
  
### 3. **Optimization via Lagrangian**
- Applied **Lagrangian optimization** to minimize the variance of tracking error, a key measure of how well the portfolio tracks the index.
- Implemented constraints:
  - Sum of portfolio weights = 1
  - Mean tracking error = 0
  
### 4. **Tracking Error**
- Tracking error measures the deviation between the portfolio's performance and the performance of the FTSE 100 index.
- By minimizing the variance of the tracking error, the portfolio is optimized for a close match to the FTSE 100 index's returns.

## Methodology

### Lagrangian Optimization Model

The Lagrangian function was formulated with the following:
- **Objective Function**: Minimize the variance of tracking error.
- **Constraints**:
  1. Sum of portfolio weights = 1.
  2. Mean tracking error = 0.

The optimization problem was solved using **Python**, leveraging optimization libraries and matrix operations to find the optimal portfolio weights.

### Key Variables:
- **Tracking Error**: The difference in returns between the FTSE 100 index and the portfolio.
- **Weights**: The fraction of capital allocated to each of the 30 stocks in the portfolio.

## Tools Used
- **Python** for the optimization process and data manipulation.
- **Pandas** for handling stock data and performing calculations.
- **Numpy** for matrix operations and solving the optimization problem.

## Results
- The optimized portfolio was constructed with the selected 30 stocks, adhering to the constraints of the model.
- The variance of tracking error was minimized, ensuring the portfolio closely tracks the FTSE 100 index.

## Conclusion

The Lagrangian optimization approach successfully minimized the tracking error variance for a portfolio tracking the FTSE 100 index. By applying the appropriate constraints, the model generated a portfolio of 30 stocks that replicates the index's performance effectively.

## Future Considerations
- Evaluate other potential constraints or methods of stock selection to further refine the portfolio.
- Explore dynamic adjustments in portfolio weights based on market conditions or changes in the FTSE 100 index.

