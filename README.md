# econ3916-lab03-visualization
# Honest vs. Misleading Visualizations

**Objective:** This project examines how identical data can be rendered honestly or deceptively, using Anscombe's Quartet, Lie Factor analysis, and multi-framing techniques on real-world economic time series to quantify and correct visual distortion.

**Methodology:**
- Reconstructed Anscombe's Quartet to demonstrate that identical summary statistics (mean, variance, correlation, regression line) can underlie visually distinct datasets, illustrating the necessity of visualization over summary statistics alone
- Calculated a Lie Factor of 49.0 for a truncated-axis revenue chart, then redesigned the chart with a zero-based axis to eliminate the distortion
- Produced four alternative framings of FRED real average hourly earnings (AHETPI, deflated to 2020 dollars), demonstrating how axis truncation, windowing, and nominal/real selection can each be used to construct a different narrative from the same underlying series
- Executed a structured four-step exploratory data analysis (structure, distributions, relationships, anomalies) on World Bank GDP panel data spanning 262 countries and 64 years
- Built an interactive honest-chart toggler (ipywidgets + matplotlib) with adjustable y-axis floor, year window, nominal/real toggle, and a live Lie Factor readout

**Key Findings:** Visual framing choices — axis truncation, window selection, and series choice — can produce dramatically different interpretations of the same dataset without altering a single underlying data point. The Lie Factor provides a quantitative measure of this distortion, while summary statistics alone (as Anscombe's Quartet shows) are insufficient to detect it.
