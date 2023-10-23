---
layout: page
title: Task
permalink: /task/
---

Each team can choose to participate in one or both tasks.

## Starter Kit
The Starter Kit will be available at Github.

## Task I: Data-Centric Stock Trading
This task emphasizes data engineering in building FinRL agents. The contestants are encouraged to devise novel data-centric strategies to clean, transform, and aggregate stock data to improve trading performance, with the model being fixed.

A dataset containing OHLCV data for stocks is provided. Contestants are free to design data processing strategies and perform feature engineering, such as constructing new indicators based on existing and/or external market data. Then the contestants are required to:

1. Specify the state space, action space, and reward functions in the environment.
2. Ensure that your data pipeline is reproducible with unseen, new data.
3. Use the same model design without modification for a fair comparison. Specifically, teams are asked to use the PPO algorithm in the FinRL library with tunable hyperparameters.

### Evaluation
The final ranking is produced based on the geometric mean of the following metrics:

1. Portfolio cumulative return. It measures the excess returns.
2. Sharpe ratio. It takes into account both the returns of the portfolio and the level of risk.
3. Max drawdown. It is the portfolio’s largest percentage drop from a peak to a trough in a certain time period, which provides a measure of downside risk.

## Task II: Real Time Order Execution
This task focuses on building lightweight algorithmic trading systems in a fair environment.

A template will be provided for contestants, and each team needs to write their functions in this template to perform order execution. We will provide an exchange of limit order book data to interact with contestants. After the contest, we will conduct real-time trading for all teams' submissions at the same time. We would advise you to keep your algorithms lightweight. 

### Evaluation
This contest is judged on pure PnL. Strategies that fail to adhere to the template will be disqualified, as well as any strategies that fail to pass linting.