# Markov Chain Trading &nbsp; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ianjure/markov-chain-trading/blob/main/Markov_Chain_Notebook.ipynb) &nbsp; [![Static Badge](https://img.shields.io/badge/Visit%20the%20Website-red?style=flat&logo=streamlit&logoSize=auto&labelColor=%23ffffff&color=%23ff4b4c)](https://tradestrats.streamlit.app/markovchain)

A Markov chain, or Markov process, is a stochastic model that describes a sequence of possible events.
The key property is that the future state depends only on the current state and not on the past states. This can be formalized as:

$P(X_{n+1}|X_n,X_{n-1},...,X_1) = P(X_{n+1}|X_n)$

where $X_n$ represents the state at time $n$.

The goal of this project is to develop a simple Markov trading model using historical stock price data and simulate its potential market returns. Additionally, we will deploy a web application that allows users to test the model's effectiveness.

## Data Overview
We will obtain historical price data for the stock from **Yahoo Finance** using the [yfinance](https://pypi.org/project/yfinance/) library. This dataset will include columns such as opening and closing prices, which are essential for simulating the trading strategy.

## Project Method
1. **Collect the Data:** Retrieve stock price data from Yahoo Finance.
2. **Clean the Data:** Remove irrelevant features and standardize the index format.
3. **Create New Features:** Compute daily returns and classify the data into distinct states.
4. **Build the Model:** Estimate state probabilities for the transition matrix.
5. **Simulate the Strategy:** Execute simulated trades and calculate the expected returns.
6. **Deploy the Model:** Create a web application enabling users to test the model.

## Next Steps
* **Identify** methods to improve the strategy's win rate.
* **Explore** and evaluate additional trading strategies.

<br>

**This project is inspired by:** [Jim Simons Trading Secrets 1.1 MARKOV Process](https://youtu.be/gA0egjZcRB0?si=fLeK8eZRyByx-TnU)
