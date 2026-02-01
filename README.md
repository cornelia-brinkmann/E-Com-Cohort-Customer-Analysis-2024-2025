# E-Com-Cohort-Customer-Analysis-2024-2025
E-Com analysis by databricks 


High-Level Flow
- Data Loading (CSV → Delta in Databricks)
- Load an initial dataset (2024 only) from a CSV file into Databricks.
- Later, simulate the arrival of new data by loading a second CSV file (2025 data) and appending it to your raw table.
- Data Transformation (Databricks SQL)
- Transform the raw e-commerce data into a model optimized for cohort analysis.
- Use SQL (CTEs + window functions / subqueries) to compute each customer’s:
- first purchase date
- second purchase date (if it exists)
- time between purchases
- Build reporting tables for cohort size, retention, and repeat depth.
- Visualization (Databricks Dashboard)
- Create a dashboard for 2024 with 3 cohort charts.
- After new data arrives, rebuild the reporting tables and create a dashboard for 2024–2025 with the same 3 charts.
 
Project Artifacts
Throughout this project, you are expected to produce artifacts that support your analysis, reasoning, and presentation.
 
- Your artifacts should include:
Technical artifacts
- A Databricks notebook containing:
Raw, clean, and analytical tables (Bronze / Silver / Gold)
- SQL logic used to transform and model the data
- A Databricks dashboard that:
Visualizes cohort size,
Retention to second purchase,
Repeat purchase depth
- The updated versions of these artifacts after incremental data (2025) is added
Analytical reasoning
- Your analytical reasoning should be reflected mainly in the PDF report, with the notebook serving as supporting evidence.
- In the report, explain:
What the cohort charts show before and after the incremental update,
How customer behavior changes over time (acquisition, retention, repeat depth),
How the addition of 2025 data affects trends and interpretations,
What assumptions or limitations apply (e.g. cohort maturity)
- The Databricks notebook should support the analysis by showing the SQL logic used to produce the reported metrics.
- The goal is a clear analytical narrative linking data, metrics, and business insight — not exhaustive technical documentation.
 
Presentation Context
- This project includes a live presentation.
- The presentation is the primary evaluation moment.
- You are expected to present two analytical states of the same pipeline:
- Initial state (2024 data only)
- How the pipeline is structured
- What the cohort analysis shows
- What conclusions can be drawn at this stage
- Updated state (2024 + 2025 data)
- What changed after new data arrived
- How the pipeline handled incremental updates
- How cohort trends evolved
- What new insights become possible (or which conclusions need revision)
- During the presentation, focus on:
Pipeline logic and data flow,
Analytical impact of incremental data,
Business interpretation of cohort trends

- Avoid:
Step-by-step SQL walkthroughs,
Tool or UI demonstrations
Line-by-line explanations
Quality Expectations

- Your work will be evaluated based on:
Correctness and clarity of the ETL pipeline,
Logical separation of data layers (Bronze / Silver / Gold)
Sound cohort modeling and metric definitions,
Ability to explain why the pipeline is designed as it is,
Correct interpretation of cohort trends before and after data updates,
Clear, structured communication during the presentation,
Visual polish or query complexity alone is not sufficient.
- Analytical reasoning, data understanding, and judgment matter more than implementation volume.
