# manufacturing-oee-investment-analysis
Manufacturing analytics case study demonstrating OEE, downtime analysis, root-cause investigation, investment prioritization, and financial business-case development using synthetic extrusion manufacturing data.


# Manufacturing OEE & Operational Performance Analysis
### Manufacturing Analytics Case Study | Extrusion Process Optimization | Operational Improvement | Financial Business Case

---

## 1. Project Overview

This project demonstrates how manufacturing production data can be transformed into actionable operational insights, root-cause investigations, improvement initiatives, and financially grounded business recommendations.

The case study simulates an industrial polymer extrusion manufacturing facility and applies a structured manufacturing analytics framework to evaluate production performance, Overall Equipment Effectiveness (OEE), downtime, process losses, product-level performance, and potential improvement opportunities.

The objective is to demonstrate how manufacturers can move beyond basic production reporting and use operational data to answer important business questions:

- How effectively is production equipment being utilized?
- Where are the largest sources of production losses?
- Which products, shifts, and operating conditions contribute most to performance variation?
- What are the underlying causes of downtime, reduced throughput, and scrap?
- Which improvement opportunities offer the greatest operational and financial value?
- How can improvement initiatives be prioritized and translated into an actionable implementation roadmap?
- What is the potential financial return from investing in targeted process improvements?

The project follows an end-to-end analytical workflow, beginning with raw production records and ending with an integrated operational assessment and illustrative investment business case.

**This is a synthetic-data portfolio project.** The facility, equipment, production records, downtime events, financial assumptions, and calculated results are illustrative. They are not actual company production data or verified financial performance.

---

## 2. Project Objectives

The project was developed to demonstrate capabilities across several areas of manufacturing analytics and process engineering.

### Manufacturing Performance Analytics
- Calculate and evaluate Overall Equipment Effectiveness (OEE).
- Analyze equipment availability, performance, and quality.
- Evaluate production trends across shifts, products, and time periods.
- Identify recurring operational losses and performance variation.
- Examine production throughput and equipment utilization.

### Downtime and Root-Cause Analysis
- Categorize downtime and operational losses.
- Identify recurring equipment and process-related issues.
- Evaluate product-specific and shift-specific performance differences.
- Investigate relationships between operating conditions and production performance.
- Translate analytical findings into potential engineering interventions.

### Operational Improvement Planning
- Identify and define improvement initiatives.
- Evaluate opportunities based on operational impact and implementation considerations.
- Prioritize improvement initiatives.
- Develop an implementation roadmap.
- Translate technical findings into management recommendations.

### Financial and Business Case Development
- Establish illustrative financial assumptions.
- Estimate potential benefits associated with selected improvements.
- Compare conservative, expected, and optimistic scenarios.
- Evaluate preliminary investment requirements and gross payback periods.
- Connect manufacturing performance improvements to financial decision-making.

---

## 3. Case Study: Northstar Polymer Manufacturing

The project uses a fictional manufacturing facility called **Northstar Polymer Manufacturing**.

The facility operates an extrusion production line designated **EX-001**, producing five different polymer products.

### Simulated Facility Characteristics

| Attribute | Description |
|---|---|
| Facility | Northstar Polymer Manufacturing |
| Production process | Polymer extrusion |
| Equipment | Extrusion Line EX-001 |
| Production schedule | Three shifts per day |
| Shift duration | Eight hours |
| Production period | January 1 – March 31, 2026 |
| Total production period | 90 days |
| Products | Five polymer product types |
| Production records | 270 shift-level records |
| Downtime records | 824 event records |

The simulated production environment includes multiple products, operating shifts, equipment downtime events, and process performance variation.

This structure provides an opportunity to investigate how product mix, shift conditions, equipment reliability, and process stability influence manufacturing performance.

### Important Data Considerations

The production records and downtime events are synthetically generated.

The data is designed to support realistic analytical workflows and demonstrate manufacturing engineering concepts. It should not be interpreted as a statistically representative sample of any specific manufacturing facility.

All calculated performance metrics, improvement estimates, and financial scenarios are dependent on the simulated inputs and assumptions.

---

## 4. Repository Structure

The repository is organized to separate source data, analytical code, financial modeling inputs, generated outputs, and project documentation.

```text
manufacturing_oee_investment_analysis/
│
├── README.md
│
├── .gitignore
│
├── data/
│   ├── production_records.csv
│   ├── downtime_events.csv
│   ├── product_master.csv
│   └── equipment_master.csv
│
├── notebooks/
│   └── Project1_OEE_Extrusion.ipynb
│
├── financial_model/
│   └── manufacturing_financial_business_case_inputs_prefilled.xlsx
│
├── outputs/
│   ├── Block1/
│   ├── block_2/
│   ├── block_3/
│   ├── block_4/
│   ├── block_5/
│   └── block_6/
│
└── reports/
```

*The structure above describes the intended organization. Actual output subfolders and filenames may vary depending on which analytical artifacts were generated and retained.*

### Directory Descriptions

**data/**

Contains the original synthetic manufacturing datasets used throughout the analysis. These files represent the source inputs for the analytical workflow.

**notebooks/**

Contains the Jupyter notebook exported from Deepnote. The notebook documents the analytical process, calculations, investigations, visualizations, and conclusions.

**financial_model/**

Contains the Excel workbook used to provide financial assumptions and inputs for the illustrative investment business case.

**outputs/**

Contains generated analytical results, intermediate datasets, tables, charts, validation results, and other supporting artifacts organized by analytical block.

**reports/**

Reserved for standalone project documentation, management summaries, and additional reporting materials.

---

## 5. Source Data Dictionary

Four primary CSV files provide the manufacturing data foundation.

### 5.1 production_records.csv

Contains shift-level production records for the simulated extrusion operation.

The dataset contains 270 production records representing 90 days of production across three shifts per day.

The records provide the production-level information required to evaluate manufacturing performance.

The dataset supports:
- Production volume analysis.
- Shift-level performance comparisons.
- Product-level performance evaluation.
- Production trend analysis.
- OEE calculations.
- Quality and scrap analysis.
- Throughput and process performance investigations.

This file serves as the primary production dataset for the analysis.

### 5.2 downtime_events.csv

Contains individual downtime and operational loss events.

The dataset contains 824 event records, consisting of:

- 666 availability-related downtime events.
- 158 performance-related or minor-stop events.

This dataset supports the investigation of equipment availability, operational interruptions, recurring downtime categories, and performance losses.

The records are used to identify loss patterns and evaluate potential opportunities for reliability and process improvement.

### 5.3 product_master.csv

Contains reference information for the five simulated polymer products.

This file provides product-level reference data used to distinguish products and support product-specific performance comparisons.

It allows the analysis to investigate differences in manufacturing performance across the product portfolio.

### 5.4 equipment_master.csv

Contains reference information for the simulated manufacturing equipment.

The equipment master provides equipment identification and supporting reference information for the extrusion operation.

It supports the organization of production and downtime records around the equipment being evaluated.

---

## 6. Analytical Workflow and Notebook Structure

The primary analytical work is organized into six major blocks.

Each block builds upon the previous analysis, progressively moving from data validation toward operational decision-making and financial evaluation.

The notebook uses a modular structure so that individual analytical stages can be reviewed, reproduced, and extended.

### Block 1 — Data Ingestion and Quality Assessment

**Purpose:** Establish a reliable data foundation before conducting manufacturing performance analysis.

This block loads the synthetic manufacturing datasets and evaluates their structure, completeness, and consistency.

Key activities include:
- Importing production, downtime, product, and equipment datasets.
- Reviewing dataset dimensions and data types.
- Evaluating missing values and data quality.
- Examining data relationships and identifiers.
- Checking production records and event-level data.
- Establishing the data foundation for subsequent analytical blocks.

**Outcome:** A validated understanding of the source datasets and their suitability for the downstream manufacturing analysis.

### Block 2 — Production Performance Trends and Statistical Validation

**Purpose:** Evaluate production performance over time and determine whether observed differences represent meaningful patterns.

This block examines production trends and operational performance variation.

Key activities include:
- Analyzing production performance over the simulated operating period.
- Evaluating performance trends across operating shifts.
- Examining product-related performance differences.
- Investigating variation in production metrics.
- Applying statistical analysis to evaluate observed trends.
- Using HAC/Newey-West statistical methods where appropriate to account for potential autocorrelation and heteroskedasticity.

**Outcome:** A more detailed understanding of production performance patterns, variation, and potential operational differences requiring further investigation.

### Block 3 — Overall Equipment Effectiveness (OEE) Analysis

**Purpose:** Quantify manufacturing effectiveness and identify losses associated with equipment availability, performance, and quality.

This block develops the OEE calculations and evaluates equipment performance using the production records.

The analysis follows the three primary components of OEE:

**Availability**

Measures the proportion of planned production time during which equipment is operating.

**Performance**

Measures production output relative to the expected production rate while the equipment is operating.

**Quality**

Measures the proportion of production output that meets the applicable quality requirements.

Overall Equipment Effectiveness is calculated as:

OEE = Availability × Performance × Quality

Key activities include:
- Calculating availability, performance, and quality metrics.
- Developing overall OEE measurements.
- Comparing performance across products and shifts.
- Evaluating the effect of product mix on performance calculations.
- Addressing mixed-product production considerations.
- Identifying the contribution of individual OEE components to overall losses.

**Outcome:** A structured assessment of equipment effectiveness and the relative contribution of availability, performance, and quality losses.

### Block 4 — Downtime and Root-Cause Investigation

**Purpose:** Move beyond reporting performance losses and investigate the operational factors contributing to them.

This block uses the production and downtime datasets to investigate recurring operational problems.

Key activities include:
- Categorizing downtime and performance losses.
- Evaluating recurring downtime events.
- Identifying significant sources of operational loss.
- Investigating product-specific performance issues.
- Examining shift-level differences.
- Evaluating equipment reliability and process stability opportunities.
- Connecting observed losses to potential engineering interventions.

The purpose is to distinguish between identifying where losses occur and understanding what operational conditions may be contributing to those losses.

**Outcome:** A structured root-cause investigation that identifies potential areas for targeted manufacturing improvement.

### Block 5 — Integrated Operational Assessment and Improvement Strategy

**Purpose:** Consolidate the analytical findings into a practical improvement strategy.

This block translates the findings from the preceding analysis into potential operational improvement initiatives.

Key activities include:
- Integrating OEE, production trend, and downtime findings.
- Identifying the most significant improvement opportunities.
- Developing defined improvement initiatives.
- Evaluating potential operational benefits.
- Prioritizing initiatives based on expected impact and implementation considerations.
- Developing an improvement roadmap.
- Preparing an executive-level summary and management recommendations.

The improvement initiatives developed in this case study include:

| Initiative | Improvement Focus |
|---|---|
| I-01 | Extrusion Throughput Improvement |
| I-02 | P-1003 Scrap and Process Stabilization |
| I-03 | Extrusion Mechanical Reliability Improvement |
| I-04 | Changeover Time Reduction |
| I-05 | Shift B Operational Performance Improvement |

These initiatives represent proposed improvement opportunities derived from the simulated analytical findings.

**Outcome:** An integrated operational assessment that connects manufacturing performance analysis to a prioritized improvement strategy and implementation roadmap.

### Block 6 — Financial Modeling and Investment Business Case

**Purpose:** Translate selected operational improvement opportunities into an illustrative financial business case.

This block extends the manufacturing analysis into financial decision support.

The financial model uses an Excel input workbook containing facility, initiative, benefit, and scenario assumptions.

The financial analysis is organized into the following sub-blocks:

**Block 6.0 — Financial Input Ingestion and Validation**

Establishes the financial modeling inputs by locating and importing the Excel workbook.

The workbook includes the following input sections:

- Start Here
- Facility Inputs
- Initiative Inputs
- Benefit Assumptions
- Scenario Settings

The block validates the imported information and prepares the financial assumptions for downstream calculations.

**Block 6.1 — Financial Input and Assumption Preparation**

Organizes the financial inputs and assumptions required to evaluate the improvement initiatives.

The purpose is to establish a consistent basis for financial calculations and scenario comparisons.

**Block 6.2 — Initiative Benefit and Investment Calculations**

Evaluates the financial implications of selected operational improvements.

This includes translating improvement assumptions into estimated financial benefits and comparing those benefits with preliminary investment requirements.

**Block 6.3 — Financial Analysis Continuation**

Continues the financial modeling workflow established in the preceding blocks.

**Block 6.4 — Scenario Analysis**

Evaluates alternative financial outcomes using conservative, expected, and optimistic assumptions.

The scenarios provide a structured way to examine how changes in assumptions affect potential improvement value and investment payback.

**Block 6.5 — Integrated Financial Evaluation**

Consolidates the financial calculations and supporting results into an integrated evaluation of the selected improvement opportunities.

**Block 6.6 — Investment Business Case and Management Recommendation**

Brings the financial analysis together into a management-oriented investment assessment.

The final block communicates the financial implications of the selected improvement initiatives and provides a basis for evaluating potential investment decisions.

**Outcome:** An illustrative financial business case that connects manufacturing improvement opportunities to potential financial benefits, investment requirements, and preliminary gross payback periods.

*The descriptions of individual financial sub-blocks reflect their place in the overall workflow. Refer to the notebook code and generated outputs for the exact calculations performed within each sub-block.*

---

## 7. Financial Business Case: Illustrative Results

The financial model evaluates selected improvement initiatives using three scenarios.

The current illustrative financial scenarios monetize two initiatives:

- I-01: Extrusion Throughput Improvement.
- I-02: P-1003 Scrap and Process Stabilization.

The remaining initiatives are retained as operational improvement opportunities, but should not be interpreted as having fully quantified financial benefits in this scenario analysis.

### Scenario Summary

| Scenario | Estimated Annual Gross Benefit | Investment | Gross Payback |
|---|---:|---:|---:|
| Conservative | $9,378.99 | $10,087.50 | 12.9 months |
| Expected | $14,068.49 | $8,877.00 | 7.6 months |
| Optimistic | $16,882.19 | $8,070.00 | 5.7 months |

These results illustrate how manufacturing improvement assumptions can be translated into financial decision-making metrics.

### Financial Interpretation

The scenario analysis demonstrates how different assumptions about achievable operational improvements and implementation costs can affect the financial attractiveness of an investment.

The expected scenario estimates approximately $14,068 in annual gross benefit against an illustrative investment of $8,877, producing a preliminary gross payback period of approximately 7.6 months.

### Important Financial Limitations

These calculations are illustrative and dependent on synthetic production data and modeled financial assumptions.

The gross payback estimates should not be interpreted as verified net ROI.

In particular:
- The benefit estimates depend on assumed operational improvements.
- Investment estimates are preliminary.
- Recurring operating and maintenance costs have not been fully established.
- The calculations do not constitute validated financial forecasts.
- Actual implementation costs and realized benefits would require engineering validation and financial review.

The financial model is intended to demonstrate the process of connecting operational improvements to investment evaluation, not to establish a guaranteed financial return.

---

## 8. Analytical Outputs

The `outputs/` directory contains the generated artifacts associated with the analytical workflow.

These files provide supporting evidence for the conclusions presented in the notebook.

Outputs are organized by analytical block so that users can navigate directly to the results associated with each stage of the analysis.

Depending on the block, generated artifacts may include:

- Data quality assessments.
- Validated analytical datasets.
- Production trend summaries.
- Statistical analysis results.
- OEE calculations.
- Availability, performance, and quality comparisons.
- Downtime classifications and summaries.
- Root-cause investigation results.
- Improvement opportunity assessments.
- Initiative prioritization.
- Implementation roadmaps.
- Financial scenario calculations.
- Investment evaluation summaries.

The outputs are retained alongside the notebook to make the project easier to review without requiring every reader to execute the entire analytical workflow.

**The notebook documents how the analysis was performed. The outputs document the results produced by the analysis.**

---

## 9. Tools and Technical Methods

The project demonstrates the application of common data analytics and manufacturing engineering methods.

### Development Environment
- Python
- Jupyter Notebook
- Deepnote

### Data Analysis
- Pandas
- NumPy
- Statistical analysis
- Data validation
- Data transformation
- Time-series and trend analysis

### Manufacturing Engineering
- Overall Equipment Effectiveness (OEE)
- Availability, performance, and quality analysis
- Downtime analysis
- Production throughput analysis
- Scrap and quality loss analysis
- Process performance evaluation
- Root-cause investigation
- Operational improvement planning

### Statistical Methods
- Descriptive statistics
- Trend analysis
- Performance comparisons
- HAC/Newey-West statistical methods

### Financial Analysis
- Excel-based financial inputs
- Scenario modeling
- Improvement benefit estimation
- Investment requirement evaluation
- Gross payback analysis

### Version Control and Documentation
- Git
- GitHub
- Markdown
- Organized analytical repository structure

---

## 10. How to Review the Project

For someone reviewing this repository, the recommended sequence is:

**Step 1 — Review the README**

Understand the case study, simulated manufacturing environment, analytical objectives, and repository organization.

**Step 2 — Review the Source Data**

Explore the four CSV files in the `data/` directory to understand the production, downtime, product, and equipment information.

**Step 3 — Review the Notebook**

Open `notebooks/Project1_OEE_Extrusion.ipynb` and follow the analysis from data ingestion through the final investment business case.

**Step 4 — Review the Outputs**

Explore the `outputs/` directory to examine the generated analytical results, tables, and supporting artifacts.

**Step 5 — Review the Financial Model**

Examine the workbook in `financial_model/` to understand the assumptions used to develop the illustrative financial business case.

---

## 11. Reproducibility and Data Limitations

This project is designed as a reproducible manufacturing analytics demonstration.

The source datasets are included in the repository so that the analytical workflow can be reviewed independently of the original Deepnote environment.

Reproducing the full analysis may require:
- A compatible Python environment.
- The required Python packages.
- Access to the included source datasets.
- Access to the financial input workbook.
- Execution of the notebook in the appropriate block sequence.

The notebook was developed and executed in Deepnote.

Differences in software versions, execution environments, or file paths may require minor configuration adjustments.

All data and financial assumptions are synthetic and illustrative. The results should not be used as actual manufacturing benchmarks, engineering specifications, or financial commitments.

---

## 12. Project Value and Demonstrated Capabilities

This case study demonstrates an end-to-end approach to manufacturing analytics that connects engineering analysis with operational and financial decision-making.

Rather than stopping at dashboarding or basic production reporting, the workflow progresses through:

1. Manufacturing data ingestion and validation.
2. Production performance and trend analysis.
3. OEE measurement and loss identification.
4. Downtime and root-cause investigation.
5. Improvement initiative development and prioritization.
6. Implementation roadmap development.
7. Financial scenario modeling.
8. Investment business case development.
9. Management recommendations.

The central objective is to demonstrate how manufacturing data can be transformed into practical operational insights and structured investment decisions.

This approach is relevant to manufacturers seeking to improve equipment utilization, reduce production losses, improve process stability, increase throughput, and make more informed capital and operational improvement decisions.

---

## 13. Disclaimer

**Northstar Polymer Manufacturing is a fictional facility.**

All production records, equipment information, product information, downtime events, operational performance metrics, financial inputs, and calculated results included in this project are synthetic or illustrative.

No actual company production data, confidential manufacturing information, or verified financial results are represented.

The project is intended for educational, demonstration, and professional portfolio purposes.

---

## Author

**Manufacturing & Materials Analytics LLC**

*Transforming manufacturing data into actionable process insights.*

Website: https://manufacturing-materials-analytics.com

Focus areas:
- Manufacturing analytics
- Operational performance improvement
- OEE and production loss analysis
- Process optimization
- Manufacturing data integration
- Financial evaluation of operational improvements
