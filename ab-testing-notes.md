## Designing the Test

1. Hypothesis: 
    - what is the change
    - which metric to use to evaluate the effect of the change (e.g. CTR, click-through-probability (unique visitors who clicked/unique visitots to page))
        - To measure usability (number of clicks), use click-through-rate
        - To measure impact (number of users), use click-through-probability
2. Decide minimum sample size & How long to run an A/B test
    - Power (1 - Type II error): the larger the power you want, the more data you will need to collect.
    - Significance level
    - Practical significance level/Minimum detectable effect
    - Small sample: lower Type I error, higher Type II error. Want sensitivity (1-Type II error) to be large (typically 80%) at the practical significant level.
    - How do parameters affect sample size:
      - Higher p, but still less than 0.5 -> more data
      - Increase practical significance level -> fewer data
      - Increase confidence level (1 - alpha) -> more data
      - Higher sensitivity (1 - beta) -> more data
    - Round days by week to capture the weekly pattern
3. Decide how to split users randomly into control groups and treatment groups
4. Use the appropriate hypothesis test (z-test/t-test), compute p-value to check whether it is statistically significant.
5. Compute confidence interval. Check whether the interval is practically significant.
6. Make a decision: change, do not change, or need to collect more data

## Multiple Testing

Bonferroni correction: significance level / number of tests. 
  A conservative estimate
Control False Discovery Rate (FDR): FP/(FP+TP)

## Limitations of A/B Tests

- Change aversion: users do not like changing the experiences they are already used to
- Novelty effect: users are really excited about new experiences
  - If an A/B test has a larger or smaller effect at the start, it is likely due to change aversion or novelty effect.
  - We could run tests only on first time users; compare first time users to old users in the treatment group to estimate the impact of the effects
- Can't Long term effect: referral, car purchasing, etc.
- A/B testing can not tell you what is missing.

## Interference Between Control and Treatment Groups

Typically: split users randomly, assume that users are independent
Social network: Users behaviors are impacted by other people, so the effect in the treatment group can spill over to the control group. Effect will be underestimated.
Two-sided market (Uber, Airbnb, etc.): resources are shared among control and treatment groups, so effect will be overestimated.
How to deal with interference: Isolate users in the control and treatment group
- Two-sided market:   
  - Geo-based randomization: high variance
  - Time-based randomization: only works when the effect takes a short time
- Social network:
  - Create network clusters: people interact mostly within the cluster
  - Ego-network randomization: 
