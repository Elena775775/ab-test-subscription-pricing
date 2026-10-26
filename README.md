# A/B Testing: Subscription Pricing Experiment

## Project Overview

This project analyzes an A/B test designed to evaluate whether highlighting a 50% discount in a subscription offer increases the conversion rate from app installation to payment.

The experiment compares two groups of users exposed to different versions of subscription messaging. The main objective is to determine whether the observed difference in conversion rates is statistically significant and to provide a data-driven business recommendation.

## Business Objective

Evaluate the impact of discount-focused messaging on subscription conversion and determine which offer performs better.

## Experiment Design

- **Group A — Control:** Users were offered a premium subscription for $4.99.
- **Group B — Variant:** Users were offered the same $4.99 subscription, with messaging emphasizing a 50% discount.
- **Primary metric:** Conversion rate from app installation to payment.
- **Experiment start date:** July 3, 2023.
- **Experiment end date:** July 25, 2023.
- **Experiment duration:** 21 days.

The key difference between the groups was the discount message presented to users in Group B.

## Dataset

The analysis uses the `ab_test_data.csv` dataset provided with the original assignment.

The data contains experiment results used to calculate group sizes, conversions, conversion rates, and statistical significance.

## Methodology

The analysis includes:

1. Loading and inspecting the experiment data.
2. Calculating the number of users and conversions in each group.
3. Calculating conversion rates for both groups.
4. Comparing conversion rates and measuring the absolute difference.
5. Performing a two-proportion Z-test.
6. Evaluating the p-value against a significance level of 0.05.
7. Interpreting the results and developing a business recommendation.

### Hypothesis Testing

- **Null hypothesis (H₀):** The conversion rates in Groups A and B are equal.
- **Alternative hypothesis (H₁):** The conversion rates in Groups A and B are different.
- **Significance level:** α = 0.05.

A two-proportion Z-test was used to assess whether the observed difference between conversion rates was statistically significant.

## Results

| Metric | Group A — Control | Group B — Variant |
|---|---:|---:|
| Number of users | 10,013 | 9,985 |
| Number of conversions | 611 | 889 |
| Conversion rate | 6.10% | 8.90% |

### Statistical Test Results

- **Test:** Two-proportion Z-test
- **Z-statistic:** -7.5197
- **P-value:** Approximately 5.49 × 10⁻¹⁴
- **Significance level:** 0.05
- **Conclusion:** Statistically significant difference between the groups.

### Key Findings

- Group B achieved a conversion rate of 8.90%, compared with 6.10% in Group A.
- The absolute difference in conversion rates was approximately **2.80 percentage points**.
- The p-value was substantially below the 0.05 significance threshold.
- The null hypothesis was rejected, providing strong statistical evidence of a difference in conversion rates.
- The discount-focused messaging in Group B was associated with a higher conversion rate during the experiment.

## Business Recommendation

Based on the experiment results, Group B is the preferred option for further consideration because it achieved a significantly higher conversion rate.

Before implementing the change across the entire user base, the business should also evaluate revenue, profit margins, customer retention, and long-term customer value. A higher conversion rate does not automatically guarantee higher profitability.

## Limitations

- The analysis focuses on conversion from app installation to payment.
- Revenue, profitability, retention, and long-term customer value were not established by the conversion results alone.
- The results demonstrate an association between the tested offer and conversion outcomes; conclusions should be interpreted within the scope of the experiment.

## Project Files

The repository contains the project materials, including the source dataset and analysis outputs where available.

- **Dataset:** `ab_test_data.csv`
- **Analysis conclusions:** See the project report and supporting files in this repository.
- **Visualizations:** Refer to the uploaded analysis outputs, if included.

## Tools and Skills

- Python and data analysis
- A/B testing
- Conversion rate analysis
- Hypothesis testing
- Two-proportion Z-test
- P-value interpretation
- Statistical significance
- Data visualization
- Business recommendations based on data

## Final Conclusion

The experiment showed a statistically significant difference in conversion rates between the two groups. Group B, which emphasized the 50% discount, achieved the higher observed conversion rate.

The findings support further consideration of the discount-focused offer, subject to additional validation of its financial and long-term business impact.
