# Measuring Income Inequality — Practical Data Science with Python

## Project Overview
This project is part of the **Practical Data Science (IDS 720)** course. It uses Python and NumPy to analyze U.S. household income data and measure inequality, then simulates the effects of different tax and transfer policies.  

The dataset comes from the **2019 American Community Survey (ACS)** conducted by the **U.S. Census Bureau**, provided through **IPUMS USA**.

---

## Tools Used
- Python 3.11+
- NumPy / Pandas
- Matplotlib / Seaborn
- ineqpy (for Gini coefficient)
- Jupyter Notebook

---

## Files
- `exercise_numpy_vectors.ipynb` — main notebook with solutions and `results` dictionary.  
- `Measuring Income Inequality — Practical Data Science with Python.pdf` — assignment instructions and exercises.

---

## Exercises
1. **Data Loading and Exploration**  
   - Load household income data with `np.loadtxt()`.
   - Plot histograms to observe skewness and outliers.

2. **Measuring Inequality**  
   - Calculate the **share of households below poverty line ($20,000)**.  
   - Compute the **Gini Index** of U.S. household incomes.

3. **Policy Simulations**  
   - **Policy A**: +$5,000 for households earning < $40,000.  
   - **Policy B**: +$7,000 for households earning < $30,000.  
   - **Policy C**: 5% tax on households earning > $250,000 (pay national debt).  
   - **Policy D**: 5% tax on > $250,000, redistributed to households < $30,000.  
   - **Policy E**: 5% tax on > $250,000, redistributed to households < $40,000.  
   - Compare resulting Gini indices.

4. **Policy Recommendation**  
   - Identify which policy reduces inequality the most.

---

## Autograder Requirements
- All answers stored in a dictionary named `results` with exact keys:  
  - `"ex4_share_below_poverty"`, `"ex4_gini"`  
  - `"ex6_gini_policy_a"`, `"ex6_gini_policy_b"`, `"ex6_gini_which_reduced_more"`  
  - `"ex7_gini_policy_c"`, `"ex8_revenue_raised"`, `"ex9_transfers"`  
  - `"ex10_gini_policy_d"`, `"ex11_gini_policy_e"`, `"ex12_policy_recommendation"`  
- Notebook must run **cleanly from top to bottom** without errors.  
- Do not use IPython magics (`%`, `%%`) or shell commands (`!`).  
- Allowed libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `statsmodels`, `patsy`, `sklearn`.  
- File must be named `exercise_numpy_vectors.ipynb`.

---

## Data Citation
ACS data used are a subsample of IPUMS USA:

> Steven Ruggles, Sarah Flood, Sophia Foster, Ronald Goeken, Jose Pacas, Megan Schouweiler and Matthew Sobek. *IPUMS USA: Version 11.0 [dataset]*. Minneapolis, MN: IPUMS, 2021.  
> [https://doi.org/10.18128/D010.V11.0](https://doi.org/10.18128/D010.V11.0)

