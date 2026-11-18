## What is this? 

A customer churn analysis for FinFlow, delivered for Northstar (client contact: Hannah Whitford) with Lina, VP at FinFlow, as the stakeholder audience. The deliverables are an analysis notebook, a six-panel interactive dashboard, and a one-page memo for FinFlow product leadership.

## What's in the folder? A short list of files and what each is

finflow-enriched-200k.csv - the dataset: 200,000 customers x 21 columns

inflow_churn_analysis_final.ipynb - the Ju

finflow_churn_dashboard.html - standalone six-panel Plotly dashboard

finflow_product_memo.md - one-page memo for Lina and her directors 

README.md 

## How to reproduce the analysis

1. Activate the environment: conda activate northstar
2. Launch Jupyter and open the notebook: jupyter lab, then open inflow_churn_analysis_final.ipynb
3. Run it top to bottom: Kernel > Restart Kernel and Run All Cells
4. Open finflow_churn_dashboard.html in a browser

## The headline findings

Support tickets has correlation with people who churns, not plan tier or signup date . Every customer who opened five or more tickets has churned, the group represent 44% of all lost customers (All 17.707 customers). Churn rate is flat at about 20% for every plan tier and every signup month. Enterprise Plus is 10% of customers but 57% of lost monthly plan fees ($787K of $1.39M). This data comes from a synthetic dataset. 

## AI Disclosure

AI was used during this engagement. Full details live in the AI Use Note section of finflow_product_memo.md.