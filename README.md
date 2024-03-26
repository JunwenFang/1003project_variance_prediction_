## Variance Forecasting

## Project Proposal for DSGA-1003: Volatility Prediction

**Authors:**
- Junwen Fang
- Frank Li
- Jaylen Peng
- Adam Xu

**Date:** March 26, 2024

## What Questions Are You Answering and Why is that Question Important?

The question we are answering is how well we can predict the short term volatility of bitcoin based on historical volatility in different time frames, returns, moving averages, and other features.

Because we wonder whether volatility (almost stationary) is something that could be predicted with small errors given that it is almost impossible to predict the returns of any equity, stock, or cryptocurrency. Volatility is the core measurement of risk, which is essential for investors to adjust their asset allocation. Also, volatility highly influence the pricing of financial instruments. Accurate volatility predictions can improve the pricing models.

Also, the machine learning boom is a revolutionary trend happening in financial market. Integrating machine learning models with deep learning techniques and financial market data is a bold attempt for us to develop a new, better way of understanding how market works. It is a meaningful real-world application and it represents how we, as data scientists, value ourselves.

## What Has Been Done Already and What Datasets Will You Use If Any?

There have been lots of Kaggle notebooks, projects done by institutional professionals, and articles written by academia in trying to predict the short term volatility of equities and cryptocurrencies.

Our raw data, consists of hourly bitcoin price, will be extracted from the Binance blockchain and API. Moreover, we will engineer features like returns, volatility, and other factors based on information and financial features formula found from books on high frequency trading, academic papers, kaggle notebooks, libraries for feature engineering, and other volatility prediction projects found online.

## How Will You Evaluate?

We will use the general evaluation metrics for time series regression models, such as MSE, RMSE, MAE, MAPE, and RMSPE (root mean square percentage error). On top of those general metrics, we will use **Theil's U Statistic**, which is a relative measure of forecasting accuracy that compares the proposed model's performance against a naive model, usually a random walk model. Another advanced metric we will use is **hit rate**. The hit rate can measure the proportion of times the model correctly predicted the direction of volatility change. This metric is particularly useful when the direction of change is more critical than the precise value and gives a better intuition on whether our prediction follows the general pattern or not.

Moreover, we will evaluate our models based on improvements made compared to models from credited Kaggle notebooks and academic papers.

## References

- Katsiampa, P. (2017). Volatility estimation for Bitcoin: A comparison of GARCH models. Economics Letters, 158, 3-6.
- Sullivan, J. C. (Year Unknown). Stock price volatility prediction with long short-term memory neural networks. Department of Computer Science, Stanford University.
- [More references as listed in your LaTeX document]
