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

![figure1](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/figures/fig1.png?raw=true)

Figure 1: Market data sources of FinRL-Meta

## Environment
With a deep reinforcement learning approach, market datasets are processed into gym-style market environments. Table 1 lists the state spaces, action spaces, and reward functions of
different FinRL applications. A state shows how an agent perceives a market situation. Facing a state, the agent can take an action from the action set, which may vary according to the financial tasks. Reward is an incentive mechanism for an agent to learn a better policy. Contestants will specify the state space, action space, and reward functions in the environment for Task I Data-Centric Stock Trading.

![table1](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/figures/table1.png?raw=true)

Table 1: List of state space, action space, and reward function

## Timeline
* **Submission Open**: October 25th, 2023
* **Submission Deadline**: November 12th, 2023
* **Results Announced**: November 25th, 2023

## Task

Each team can choose to participate in one or both tasks.

### Starter Kit
The Starter Kit will be available at Github.

### Task I: Data-Centric Stock Trading
This task emphasizes data engineering in building FinRL agents. The contestants are encouraged to devise novel data-centric strategies to clean, transform, and aggregate stock data to improve trading performance, with the model being fixed.

A dataset containing OHLCV data for stocks is provided. Contestants are free to design data processing strategies and perform feature engineering, such as constructing new indicators based on existing and/or external market data. Then the contestants are required to:

1. Specify the state space, action space, and reward functions in the environment.
2. Ensure that your data pipeline is reproducible with unseen, new data.
3. Use the same model design without modification for a fair comparison. Specifically, teams are asked to use the PPO algorithm in the FinRL library with tunable hyperparameters.

#### Evaluation
The final ranking is produced based on the geometric mean of the following metrics:

1. Portfolio cumulative return. It measures the excess returns.
2. Sharpe ratio. It takes into account both the returns of the portfolio and the level of risk.
3. Max drawdown. It is the portfolio’s largest percentage drop from a peak to a trough in a certain time period, which provides a measure of downside risk.

### Task II: Real Time Order Execution
This task focuses on building lightweight algorithmic trading systems in a fair environment.

A template will be provided for contestants, and each team needs to write their functions in this template to perform order execution. We will provide an exchange of limit order book data to interact with contestants. After the contest, we will conduct real-time trading for all teams' submissions at the same time. We would advise you to keep your algorithms lightweight. 

#### Evaluation
This contest is judged on pure PnL. Strategies that fail to adhere to the template will be disqualified, as well as any strategies that fail to pass linting.

## Organizers

### Core Organizers

| Photo                | Biography              |
|----------------------|-------------------|
| ![Keyi Wang](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/organizers/wang-ky.jpg?raw=true)      | **Keyi Wang**, master’s candidate at Northwestern University, bachelor at Columbia University. Interested in machine learning and financial engineering. Core member of AI4Finance open-source community, responsible for project maintenance and promotion, including FinRL and FinRL-Meta.|
| ![Ziyi Xia](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/organizers/xia-zy.png?raw=true)  | **Ziyi Xia**, master’s candidate at Columbia University. Interested in financial reinforcement learning, big data. The core maintainer of AI4Finance open-source community, including popular projects: FinRL, FinRL-Meta.|
| ![Kent Wu](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/organizers/wu-k.jpg?raw=true) | **Kent Wu**, master’s candidate at Columbia University with a keen interest in financial reinforcement learning and language modeling. He plays a pivotal role as the primary maintainer of the AI4Finance open-source community. This includes renowned projects such as FinRL and FinRL-Meta.|
| ![Ethan Havemann](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/organizers/ethan.jpeg?raw=true) | **Ethan Havemann**, Undergraduate at Northwestern University, Founder of Northwestern Fintech, and original designer of NUTC. Ethan focuses on software architecture, powerful developer tools, and hardware-up performance optimizations.|
| ![Jiale Chen](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/organizers/jiale.jpeg?raw=true) | **Jiale Chen**, Undergraduate at Northwestern University and RL lead for Northwestern Fintech. Jiale’s interests lie in applying ML to solve complex, data driven problems.|

### Platform

| Photo                | Biography              |
|----------------------|-------------------|
| ![Steve Ewald](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/platform/steve.jpeg?raw=true) | **Steve Ewald** Third-year undergraduate student at Northwestern University. Incoming Software Engineer Intern at IMC Trading. Leading research on floating point attack vectors and interactions with chaos theory at the Prescience Lab.|
| ![Nikola Maruszewski](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/platform/nino.png?raw=true) | **Nikola Maruszewski** An undergraduate student at Northwestern University majoring in Computer Science, and plans to complete a Masters in Computer Engineering through the BS/MS program. Currently performing research on Quantum Systems with Prof. Nikos Hardavellas in the PARAG@N Lab. Other interests lie in computer hardware, embedded systems, compilers, and operating systems.|
| ![Andrew Li](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/platform/al.png?raw=true) | **Andrew Li** Second-year undergraduate student at Northwestern University doing BA/MS in Computer Science. Incoming intern at Capital One. Interested in developing high performance, impactful software and building infrastructure.|
| ![Gavin Wang](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/platform/gavin.jpg?raw=true) | **Gavin Wang** First-year undergraduate student at Northwestern University pursuing a degres in Compuer Science and Math. Interested in system architecture, databases, and networking.|
| ![Chris Minn](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/platform/chris.jpeg?raw=true) | **Christopher Minn** Computer Engineering, Mathematics, and Computer Science student at Northwestern University.|

### Advisors

| Photo                | Biography              |
|----------------------|-------------------|
| ![Xiao-Ying Liu](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/advisors/liu-xy.png?raw=true) | **Xiao-Yang Liu** Ph.D candidate, Columbia University. His research interests include deep reinforcement learning, big data, and high-performance computing. He co-authored a textbook on reinforcement learning for cyber-physical systems, a textbook on tensor for data processing. He serves as PC member for NeurIPS, ICML, ICLR, AAAI, IJCAI, AISTATS, KDD, ACM MM, ACM ICAIF, ICASSP, and a Session Chair for IJCAI 2019. He organized the NeurIPS 2020/2021 First/Second Workshop on Quantum Tensor Networks in Machine Learning, IJCAI 2020 Workshop on Tensor Networks Representations in Machine Learning, and NeurIPS 2019/2020 Workshop on Machine Learning for Autonomous Driving.|
| ![Zihan Ding](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/advisors/ding-zh.png?raw=true) | **Zihan Ding** Ph.D., Princeton University. His primary research interests are: deep reinforcement learning algorithms and applications. He serves as the reviewer of NeurIPS, ICLR, ICML, CVPR, ICCV, AAAI, AISTATS, RA-L, ICRA, IROS, CISS, AIM. He also served on the organization committee of Human in the Loop Learning (HiLL) Workshop at NeurIPS 2022.|
| ![Zhaoran Wang](https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/staffphotos/advisors/zhaoran.png?raw=true) | **Zhaoran Wang** Assistant Professor of IEMS and CS at Northwestern University.  Zhaoran's research focuses improving and scaling deep reinforcement learning to solve complicated societal challenges.|

## Contact
Contestants can communicate any questions on Discord.

Contact email: [finrlcontest@gmail.com](mailto:finrlcontest@gmail.com)

<div style="display: flex; width: 100%; justify-content: space-evenly; align-items: center; gap: 2em">
<img height=100 src="https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/logos/acm.jpeg?raw=true"/>
<img height=100 src="https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/logos/nyu.png?raw=true"/>
<img height=100 src="https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/logos/nu.png?raw=true"/>
<img height=100 src="https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/logos/columbia.jpeg?raw=true"/>
<img height=100 src="https://github.com/FinRL-Contest/ACM_ICAIF_2023/blob/main/web/app/assets/logos/finrl.png?raw=true"/>
</div>
