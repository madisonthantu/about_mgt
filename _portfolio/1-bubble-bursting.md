---
title: "Bubble Bursting Dynamics"
excerpt: "A year-long independent research project that investigated the relationship between accuracy, filter bubbles, and user homogenization in RSs."
header:
  teaser: assets/bubble-bursting/rs_architecture.png
---

|![Architecture overview.](https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/bubble-bursting/rs_architecture.png)|
|:--:| 
| *A conceptual diagram of the design components and system interactions of a T-RECS simulation. Lines with arrows indicate inputs fed into outputs. Dashed grey lines indicate conceptual components. The red arrows (a) and (b) are the main levers in influencing long-term user preferences.* |

Conducted first as a final research project for Fair and Robust Algorithms course, then expanded upon as a year-long independent research project for the DREAM (Distributed REsearch Apprenticeships for Master’s) fellowship program. 

**Final report:** *Bubble Bursting Implementations and Dynamics in Recommender Systems*

The research included implementing several recommender system (RS) models via different recommendation algorithms/strategies. Specifically, I compared myopic (i.e., top-*k*) and diversity-promoting (e.g., xQuAD, probabilistic) models. A simulation environment was then used to analyze long-term user behavior, RS ecosystem dynamics, and RS performance metrics.

### Tech specs:
    Python (TensorFlow, Keras, Pandas, NumPy, Matplotlib, etc.), 
    T-RECS library, Google Cloud Platform

### Abstract:
Recommender systems (RSs), which offer personalized suggestions to users, power many of today’s social media, e-commerce, and entertainment services. Despite the utility and ubiquity of RSs, there is growing concern about the harmful effects that propagate from these systems, such as filter bubbles, user homogenization, and unfairness, and the fundamental trade-off that exists between accuracy and diversity. Although these concerns have become mainstream, our understanding of how these detrimental effects emerge in the complex RS ecosystem remains incomplete, and the present study aims to contribute to this important line of research. We first operationalize user behavior homogenization and filter bubbles, defining a set of attributes for which our subsequent metrics are tailored to. We then implement several recommender models to represent the accuracy-diversity prioritization spectrum, including an accuracy-driven myopic algorithm, a diversity-promoting algorithm inspired by the xQuAD framework, and a naively exploratory random algorithm. We conclude our report with a comparative analysis of how the three aforementioned phenomena emerged, evolved, and interacted with one another in our simulation ecosystem as the prioritization of accuracy versus diversity is varied.

For more information, you can check out:
1. The [GitHub](https://github.com/madisonthantu/T-RECS-RS-research) repo
2. The [website](https://madisonthantu.github.io/) for my research project