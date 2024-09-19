# A/B Test README: Website Redesign

## 1. Project Objective
The objective of this project is to **analyze the results of an A/B test** conducted to compare the performance of an old website design (Version A) against a new, redesigned version (Version B). The purpose of this test is to determine which design results in a higher **conversion rate**, which is the primary success metric for the test. Ultimately, this will help decide whether to fully implement the new design or retain the old one.

## 2. Business Problem
The business problem we aim to solve is whether a redesigned website can improve user engagement and increase conversions compared to the current design. The **conversion rate**—the percentage of visitors who complete a desired action (e.g., making a purchase, signing up for a newsletter)—is currently lower than expected. We hypothesize that the new design will lead to improved user interaction and higher conversion rates.

## 3. Hypothesis
Our hypothesis for this test is:

- **Hypothesis Statement**: **If** the new website design (Version B) is implemented, **then** the conversion rate will increase compared to the old website design (Version A).

### Null Hypothesis (H₀):
There is **no significant difference** in conversion rates between Version A (old design) and Version B (new design).

### Alternative Hypothesis (H₁):
The **conversion rate of Version B is significantly higher** than that of Version A.

## 4. Variants
- **Version A (Control)**: This is the old website design. It serves as the baseline for comparison.
  - Visitors are directed to the original landing page.

- **Version B (Treatment)**: This is the newly redesigned version of the website.
  - Visitors are directed to the new landing page with design modifications intended to enhance the user experience and increase conversions.

## 5. Dataset Description
The dataset includes user interaction data for both versions of the website, collected over the duration of the A/B test. Each user is randomly assigned to either Version A or Version B.

### Dataset Columns:
- **user_id**: A unique identifier for each user.
- **timestamp**: The date and time when the user visited the website.
- **group**: Indicates whether the user belongs to the control group (old design, Version A) or treatment group (new design, Version B).
- **landing_page**: Identifies whether the user landed on the old page (Version A) or new page (Version B).
- **converted**: A binary value where 1 indicates the user converted (completed the desired action) and 0 indicates no conversion.

### Sample Data Structure:
| user_id | timestamp          | group    | landing_page | converted |
|---------|--------------------|----------|--------------|-----------|
| 001     | 2024-01-01 12:00:00 | control  | old_page     | 1         |
| 002     | 2024-01-01 12:05:00 | treatment | new_page     | 0         |
| 003     | 2024-01-01 12:10:00 | control  | old_page     | 1         |
| 004     | 2024-01-01 12:15:00 | treatment | new_page     | 1         |

## 6. Measurement and Success Metric
The primary metric for this A/B test is the **conversion rate**. This is calculated as the percentage of visitors who successfully convert (complete the desired action).

### Key Measurements:
- **Overall Conversion Rate**: Comparison of the overall conversion rates between Version A and Version B.
- **Conversion by Group**: Conversion rate segmented by control and treatment groups.
- **Statistical Significance**: Ensuring the results are statistically significant by calculating the p-value and confidence intervals.

## 7. Conclusion
The outcome of this A/B test will help us determine whether Version B (new design) provides a statistically significant improvement in conversion rates over Version A (old design). Based on the results, we will make data-driven decisions on whether to adopt the new design or further optimize the current design.
