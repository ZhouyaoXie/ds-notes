[Reference 1](https://www.youtube.com/watch?v=Allap_hrjyo)
[Reference 2 - Hypothesis Testing](https://www.youtube.com/watch?v=IY7y-t30UJc)

# Hypothesis Testing

[My notes on hypothesis testing](https://www.notion.so/zhouyaoxie/Hypothesis-testing-11bcdfc9e0f9496194613678c576f594)

### Binomial test

- proportion

### Z-test

Two use cases:
- proportion, when np > 10 and n(1-p) > 10
- mean, when (sample size > 30 or population is normally distributed) and population variance is known

### T-test

- mean, when (sample size > 30 or population is normally distributed) and population variance is unknown
- t-distribution is more spread out than z-distribution. As n increases, t-distribution approaches z-distribution.

### Power

Statistical power is used in hypothesis testing. It is the likelihood that a test correctly rejects the null hypothesis. The higher the power is, the better the test is. It is often used to calculate the minimum sample size in designing experiments.

### Type I Error

Type I error is used in hypothesis testing. It is the likelihood that a test mistakenly rejects the null hypothesis. The larger the value, the less reliable the test is.

### Type II Error

It is the likelihood of false negative - when a test fails to reject the null hypothesis when the null is false. The larger the value, the less reliable the test is. It is often used in A/B testing.

### Confidence interval/Confidence level

A confidence interval represents a range for the true value that we want to estimate. The confidence level represents how likely the confidence interval will cover the true value. The wider the interval is, the less confidence we are about the sample result. 

### P-value

P-value is used in hypothesis testing. It is the probability of getting the observed results or even more extremely results given that the null hypothesis is true. A low p-value means that the null hypothesis is more likely to be false.
