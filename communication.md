### Explain technical concepts to non-tech audience

- Where and why the concept is used?
- Definition
- What does it mean for the value to change
- Applications

### Approaching a new dataset

- Clarify: 
  - Product: What is the product? What are the goals of the product? Who are the users?
  - How are certain quantities defined?
  - What is the target variable/key metric?
- Narrow down the problem and determine the objective
- Collect data
- Preprocess data, EDA, make visualizations
- Select an appropriate model (linear regression, logistic regression, SVM, gradient boosting decision tree, neural network, etc.)
- Perform feature selection (forward/backward selection based on F-ratio or Mellow's Cp) and feature engineering (categorical variables, imputation, binning, log transform, scaling, etc.)
- Train and evaluate model (split data into train, validate, test; perform cross validation)
- Communicate tradeoffs of the proposed solution

### Drop in Metric

- clarify question
- time:
  - internal (data source, data collection, etc.)
  - external (weather, etc.)
- other metrics: 
  - whether other related metrics have had the same change
- segment by user demographics
- decompose the metric
- Summarize overall approach
  - Most likely reason

### How to measure success

- clarify problem & objective
- define no more than 3 metrics:
  - 2 success metrics
  - 1 guardrail metric (a metric that should not degrade as new functionality is added)

### Whether to launch a new functionality 

- clarify
- experimentation
  - split user into control & experiment
  - sample size
  - how long to run the experiment
- recommendation based on experiment results
  - link results to goal and business impact
  - what to do if you see conflicting results
  - short-term vs. long-term
