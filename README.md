# NZX Company Financial Statement Analysis

## Overview

This project is a beginner-to-intermediate finance and technology project focused on analysing the financial health and performance of a publicly listed New Zealand company. For the project showcase, the example company analysed will be **Auckland International Airport (`AIA`)**.

The first version of the project uses Excel to structure historical financial statement data, calculate key financial ratios, visualise trends, and write an analyst-style interpretation. The second phase introduces Python to validate the Excel calculations, automate repetitive analysis steps, and prepare the project for future data extraction and reporting workflows.

The goal is not only to practise Excel or Python in isolation, but to build a practical workflow that connects accounting data, financial analysis, and technical automation.

## Project Objective

The project aims to answer a simple business question:

> Is the selected NZX-listed company becoming financially stronger or weaker over time?

To answer this, the analysis will review the company's:

- Revenue growth
- Profitability
- Liquidity
- Leverage
- Cash flow quality
- Overall financial performance trend

## Why This Project

Financial statements are one of the most important sources of information in finance. They show how a company earns revenue, manages costs, uses assets, funds operations, and generates cash.

This project is designed to build a foundation in both finance and technology by combining:

- Financial statement analysis
- Excel-based financial modelling
- Ratio calculation and interpretation
- Python-based validation and automation
- Clear communication of business insights

## Showcase Company

For the project showcase, the selected company is **Auckland International Airport (`AIA`)**, a New Zealand publicly listed company on the NZX.

Auckland International Airport is used as the first example because its business model is relatively understandable and its financial performance can be analysed through passenger recovery, revenue growth, operating costs, capital expenditure, debt, and cash flow.

The longer-term goal is to make the workflow reusable for other NZX-listed companies.

Potential companies include:

- Auckland International Airport (`AIA`)
- Spark New Zealand (`SPK`)
- Mainfreight (`MFT`)
- Fisher & Paykel Healthcare (`FPH`)
- Contact Energy (`CEN`)
- Meridian Energy (`MEL`)

## Analysis Scope

The project will use 3 to 5 years of historical financial data from the company's annual reports.

The core financial statements used are:

- Income statement
- Balance sheet
- Cash flow statement

The project will focus on historical analysis first. Forecasting, valuation, and investment recommendation will be considered future extensions.

## Excel Workbook Structure

The Excel workbook will act as the first modelling and analysis layer.

Planned workbook tabs:

| Tab | Purpose |
| --- | --- |
| `Cover` | Introduces the company, ticker, analysis period, currency, and project purpose |
| `Sources` | Records annual report links, source pages, notes, and assumptions |
| `Raw Extract` | Stores the original financial statement numbers collected from annual reports |
| `Historical Financials` | Organises income statement, balance sheet, and cash flow data into a clean format |
| `Ratios & KPIs` | Calculates financial ratios and key performance indicators |
| `Charts` | Visualises revenue, profit, margins, debt, liquidity, and cash flow trends |
| `Analysis Summary` | Provides written interpretation of the company's financial performance |

The workbook is designed to separate source data, calculations, outputs, and written analysis. This makes the model easier to audit, update, and explain.

## Financial Metrics

The analysis will calculate several groups of financial metrics.

### Growth

- Revenue growth
- Gross profit growth
- Operating profit growth
- Net profit growth
- Total asset growth

### Profitability

- Gross margin
- Operating margin
- Net margin
- Return on assets
- Return on equity

### Liquidity

- Current ratio
- Quick ratio, if sufficient data is available
- Cash ratio, if sufficient data is available

### Leverage

- Debt-to-equity ratio
- Debt-to-assets ratio
- Total liabilities-to-assets ratio
- Interest coverage ratio, if sufficient data is available

### Cash Flow

- Operating cash flow
- Capital expenditure
- Free cash flow
- Free cash flow margin
- Operating cash flow to net income

## Python Component

The Python part of the project will be introduced after the Excel model is built.

The purpose of Python is to validate, automate, and eventually scale the financial analysis workflow.

Planned Python tasks:

- Read raw financial data from the Excel workbook
- Recalculate the same ratios produced in Excel
- Compare Python outputs against Excel calculations
- Identify calculation differences or potential formula errors
- Export a clean ratio table to CSV or Excel
- Create basic charts using Python
- Prepare the project for future automated data extraction

The first Python version will not attempt to fully automate annual report extraction. Instead, it will focus on calculation validation and repeatability.

Future Python extensions may include:

- Extracting tables from annual report PDFs
- Standardising financial statement line items
- Loading financial data into a SQL database
- Generating automated company analysis summaries
- Building a simple dashboard or web interface

## Planned Python Workflow

```text
Excel raw financial data
-> Python reads workbook
-> Python cleans and reshapes data
-> Python recalculates ratios
-> Python compares results with Excel
-> Python exports validation output
```

Example libraries:

- `pandas`
- `openpyxl`
- `matplotlib`
- `seaborn`
- `numpy`

Possible future libraries:

- `pdfplumber`
- `camelot`
- `tabula-py`
- `sqlalchemy`
- `psycopg2`

## Expected Repository Structure

```text
nzx-financial-analysis-project/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── excel/
│   └── company_financial_analysis.xlsx
├── notebooks/
│   └── financial_ratio_validation.ipynb
├── src/
│   ├── read_excel.py
│   ├── calculate_ratios.py
│   └── validate_outputs.py
├── outputs/
│   ├── charts/
│   └── ratio_validation.csv
└── docs/
    └── analysis_summary.md
```

## Project Roadmap

### Phase 1: Excel Financial Model

- Select one NZX-listed company
- Collect 3 to 5 years of annual report data
- Build the Excel workbook structure
- Input and clean income statement, balance sheet, and cash flow data
- Calculate key financial ratios
- Build charts and summary views
- Write a short analyst-style interpretation

### Phase 2: Python Validation

- Read Excel data using Python
- Recalculate key ratios
- Compare Python results with Excel results
- Export validation results
- Create basic Python charts

### Phase 3: Automation and Scaling

- Improve financial data cleaning
- Add support for multiple companies
- Store data in a database
- Automate more parts of the analysis process
- Build dashboard or reporting outputs

### Phase 4: Advanced Finance Extensions

- Add forecasting
- Add common-size analysis
- Add peer comparison
- Add valuation methods such as DCF or trading multiples
- Add AI-assisted annual report summarisation

## Key Learning Outcomes

By completing this project, I aim to develop practical skills in:

- Reading and understanding company financial statements
- Structuring financial data for analysis
- Building clean and auditable Excel models
- Calculating and interpreting financial ratios
- Using Python to validate financial calculations
- Communicating financial insights clearly
- Building a foundation for finance and technology projects

## Finance vs Accounting Context

This project uses accounting information, but the purpose is financial analysis.

Accounting focuses on recording, classifying, and reporting business activity accurately. Finance uses that information to assess performance, risk, value, and future decision-making.

In this project, the financial statements provide the raw accounting data. The ratio analysis, trend analysis, cash flow assessment, and written interpretation turn that data into finance-oriented insight.

## Disclaimer

This project is for educational and portfolio purposes only. It is not financial advice, investment advice, or a recommendation to buy or sell any security.
