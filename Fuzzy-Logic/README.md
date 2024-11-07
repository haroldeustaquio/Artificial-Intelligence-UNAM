# Fuzzy Logic Risk Assessment for Insurance Policies

This repository contains a fuzzy logic-based system designed to evaluate financial risk for clients requesting car insurance policies. The system assesses risk based on two main input variables: the age of the insured person and their driving percentage throughout the year.

---

## Overview of Fuzzy Logic

Fuzzy logic is a form of multi-valued logic derived from fuzzy set theory. Unlike binary logic, where variables are either true or false, fuzzy logic allows for reasoning with degrees of truth. This approach is particularly useful for handling situations with uncertainty or vague data, such as "young" or "high-risk."

### How Fuzzy Logic Works in This System

1. **Fuzzy Input Variables**:
   - **Age**: Categorized into "Young," "Adult," and "Senior," each defined with a membership function. For example, individuals are considered "Young" with a high membership degree up to around 25 years.
   - **Driving Percentage**: Defined as "Low," "Medium," or "High." This variable captures the extent of driving experience or exposure over the year.

2. **Output Variable**:
   - **Financial Risk**: The system outputs a risk level as "Low," "Medium," or "High," with a membership degree to quantify the assessed risk.

3. **Fuzzy Rules**:
   The system applies fuzzy inference rules to determine risk based on combinations of age and driving percentage. For example, a young driver with a high driving percentage would yield a high-risk assessment. The rules are based on real-world assumptions about risk factors associated with age and driving habits.

4. **Defuzzification**:
   After evaluating the rules, the system converts the fuzzy result into a single crisp value representing the financial risk percentage. This is achieved by calculating the centroid of the aggregated fuzzy output, offering a practical risk assessment score.
---

## Implementation Details

The fuzzy logic system is implemented in Python using the `scikit-fuzzy` library. Here’s how each part is set up:

- **Membership Functions**: Defined for each input (Age, Driving Percentage) and output (Financial Risk) using triangular and trapezoidal membership functions.
- **Fuzzy Rules**: The rules are established based on various combinations of age and driving percentage levels, influencing the financial risk output.
- **Defuzzification with Shapely**: The centroid is calculated to obtain a final crisp output for risk percentage, making it actionable for real-world applications.

### Case Examples

Three sample cases are implemented to showcase how the system evaluates financial risk based on different age and driving percentage inputs:

1. **Case 1**: Age 40, Driving Percentage 80% - Result: High risk.
2. **Case 2**: Age 25, Driving Percentage 55% - Result: Medium to High risk.
3. **Case 3**: Age 55, Driving Percentage 15% - Result: Medium risk.

Each case is computed using predefined fuzzy rules and membership functions, demonstrating how different combinations impact the risk assessment.

---

## Running the System

1. **Install Dependencies**:
   - Ensure you have `scikit-fuzzy` and `Shapely` installed. You can install them using:
     ```bash
     pip install scikit-fuzzy shapely
     ```

2. **Run the Notebook**:
   - Open the `fuzzy.ipynb` notebook to view and execute the fuzzy logic system implementation. The notebook includes all code, membership function definitions, and results for each case.

---

For any issues, suggestions, or contributions, please open an *Issue* or submit a *Pull Request*. Your input helps enhance the functionality and accuracy of this fuzzy logic risk assessment system.