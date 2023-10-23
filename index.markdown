---
layout: page
title: Home
permalink: /
---

## Overview
Financial reinforcement learning (FinRL), as an interdisciplinary field of finance and reinforcement learning, has been recognized as a promising approach to financial tasks. Over the past decade, deep reinforcement learning (DRL) has achieved remarkable success in solving complex problems across a variety of domains, including robotics, gaming, and large language models like ChatGPT and GPT-4. The success of DRL has also led to its application in finance, where it has demonstrated great potential for enhancing the performance of financial tasks, such as portfolio management, option pricing, and algorithmic trading.

The FinRL contest is a competition that explores and evaluates the capability of machine learning methods in finance. However, developing machine learning algorithms for financial data presents unique challenges:

1. **Dynamic Transitions and Data Noise:** Financial datasets are constantly evolving, making it difficult to capture the underlying dynamics. Moreover, financial data is often susceptible to noise and anomalies. 
2. **Partial Observability:** No traders can access complete market-influencing information due to the gigantic, complex, and unpredictable nature of financial systems, where unforeseen events like natural disasters, policy changes, and consumer behavior shifts can have hard-to-anticipate effects.
3. **Other Complex Behaviors:** Many other factors can cause complicated and unpredictable behaviors, such as the market’s decentralized nature and the large number of financial instruments available.

The FinRL Contest presents two tasks, data-centric stock trading and real time order execution, aiming to foster innovations toward addressing the above challenges. We welcome students, researchers, and engineers who are passionate about finance and machine learning. And we encourage the development of tailored data processing strategies, novel features, and innovative algorithms that can adapt to changing market conditions and generate superior returns for investors.

## Data
We have more than 30 market data sources to deal with different financial tasks. We hold the data APIs and sample market environments in an open-source repository, FinRL-Meta, as shown in Figure 1. Contestants are welcome to explore and use in the FinRL Contest.

## Environment
With a deep reinforcement learning approach, market datasets are processed into gym-style market environments. Table 1 lists the state spaces, action spaces, and reward functions of
different FinRL applications. A state shows how an agent perceives a market situation. Facing a state, the agent can take an action from the action set, which may vary according to the financial tasks. Reward is an incentive mechanism for an agent to learn a better policy. Contestants will specify the state space, action space, and reward functions in the environment for Task I Data-Centric Stock Trading.

## Timeline
* **Submission Open**: October 25th, 2023
* **Submission Deadline**: November 12th, 2023
* **Results Announced**: November 25th, 2023
