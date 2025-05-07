# Coupon Acceptance Analysis

## Project Overview
This project analyzes coupon acceptance behavior using the `coupons.csv` dataset from the UCI Machine Learning Repository, collected via Amazon Mechanical Turk. The dataset captures user, contextual, and coupon attributes to determine factors influencing whether drivers accept coupons for Coffee House, Restaurant(<$20), Carry out & Take away, and Restaurant(20-50) venues. The analysis, conducted in Python (Pandas, Seaborn, Matplotlib), computes acceptance rates, identifies key drivers, and visualizes trends in a Jupyter Notebook.

## Summary of Findings
- **Acceptance Rates**:
  - **Carry out & Take away**: ~75%, driven by convenience.
  - **Restaurant(<$20)**: ~70%, appealing to budget-conscious diners.
  - **Coffee House** and **Restaurant(20-50)**: ~45%, reflecting selective appeal due to cost or preferences.
- **Key Drivers**:
  - **Frequent Visitors**: Acceptance rises with visit frequency (e.g., `never`: ~20-40%, `4~8`: ~70-95%) across all coupon types.
  - **Young/Social Demographics**: Higher rates for `Friend(s)` (~50-85%), younger ages (`below21`, `21`, `26`: ~55-90%), `Singles` (~50-80%), and `students` (~55-85%), especially in social contexts.
  - **Conditions**:
    - Frequent visitors with non-kid passengers: ~60-92% vs. ~30-50% (others).
    - Frequent visitors, age < 30: ~65-90% vs. ~27-55% (others).
- **Lower Acceptance Groups**:
  - `Kid(s)` (~30-50%), older ages (`46`, `50plus`: ~20-50%), and higher incomes (`$100000 or More`: ~40-60%) prefer convenience, home dining, or premium options.
- **Data Limitation**: Small excerpt data (13-20 coupons) limits some categories, but full dataset trends are consistent (e.g., Restaurant(20-50): 64.29% in sample).

## Recommendations
1. **Target Frequent Visitors and Young/Social Groups**:
   - Use loyalty programs and social media to promote group-oriented deals (e.g., “bring a friend”) for frequent visitors and young diners/students.
2. **Customize Offers for Lower-Performing Groups**:
   - Offer family-friendly deals for `Kid(s)`, convenience-focused promotions (e.g., pre-order) for older groups, and premium bundles for high-income groups.

## Jupyter Notebook
Explore the full analysis, including code, visualizations, and detailed insights, in the Jupyter Notebook:

[View the Jupyter Notebook](https://github.com/ilyaabrosimov/kraftwerk/blob/main/prompt.ipynb)