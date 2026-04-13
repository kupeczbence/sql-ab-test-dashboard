# Product Analytics & A/B Testing Dashboard

## Overview

This project is an interactive **Product Analytics & A/B Testing dashboard** built with Streamlit.

It simulates user behavior in a product environment and allows real-time exploration of how changes in conversion rates impact:

* Funnel performance
* A/B test results
* Statistical significance
* Business decisions

The dashboard combines **SQL, Python, and statistical inference** into a single interactive analytics tool.

---

## Key Features

* **Interactive Sliders**

  * Adjust conversion rates for variants A and B
  * Control sample size (number of users)

* **Funnel Analysis**

  * Visit → Signup → Purchase flow
  * Drop-off detection between stages

* **A/B Testing**

  * Two-proportion Z-test
  * Real-time p-value calculation
  * Statistical decision output

* **Effect Size Interpretation**

  * Automatic classification: small / moderate / large effect
  * Helps understand detectability of differences

* **Business Insights**

  * Identifies the main bottleneck in the funnel
  * Translates data into actionable product decisions

* **Final Conclusion Panel**

  * Explains *why* results look the way they do
  * Connects statistics with real-world experimentation

---

## What This Project Demonstrates

This is not just a statistical exercise — it demonstrates:

* Product thinking
* Data-driven decision making
* Understanding of uncertainty and effect size
* Ability to connect analysis with business impact

---

## Tech Stack

* **Python**
* **Streamlit**
* **Pandas**
* **NumPy**
* **SQLite (in-memory)**
* **Plotly**
* **Statsmodels**

---

## How It Works

1. User behavior is **simulated**:

   * Users are randomly assigned to A/B groups
   * Events: visit → signup → purchase

2. Data is stored in an **in-memory SQL database**

3. SQL queries are used for:

   * Funnel aggregation
   * A/B group statistics

4. Statistical testing is performed using:

   * Two-proportion Z-test

5. Results are visualized and interpreted in real-time

---

## How to Run

```bash
pip install streamlit pandas numpy plotly statsmodels
streamlit run streamlit_app.py
```

---

## Example Insights

* High drop-off at purchase stage → potential UX or pricing issue
* Small effect size → requires larger sample size
* Large effect size → statistically robust and actionable

---

## Key Learnings

* Statistical significance depends on both **effect size** and **sample size**
* Small improvements are difficult to detect without sufficient data
* A/B testing alone is not enough — **context and funnel analysis matter**
* Interactive tools help better understand uncertainty and decision-making

---

## Why This Project Stands Out

Unlike basic A/B testing projects, this solution:

* Combines **SQL + analytics + statistics**
* Provides **interactive experimentation**
* Includes **business-level interpretation**
* Mimics real-world **product analytics workflows**

---

## Future Improvements

* Cohort analysis (retention tracking)
* Bayesian A/B testing
* Experiment history tracking
* Deployment to Streamlit Cloud

---

## Author

- LinkedIn: www.linkedin.com/in/bence-kupecz-119701305
- GitHub: https://github.com/kupeczbence
- Portfolio: https://www.kupeczbence.com/
