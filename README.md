# Enterprise AI Adoption Survey Analysis

## Overview
This project analyzes survey data on how organizations are adopting artificial intelligence, which AI tools are most commonly used, and what risks leaders associate with adoption.

The workflow includes:
- cleaning raw survey exports
- restructuring survey response data
- summarizing single-select and multi-select questions
- calculating counts and percentages
- exporting a cleaned summary table
- creating executive-style data visualizations
- synthesizing findings into a concise written report

## Project Objective
The goal of this project was to transform raw survey response data into a clear, decision-oriented analysis that highlights:
- how organizations are encouraging AI adoption internally
- which categories of AI tools are most widely used
- what concerns organizations cite most often when adopting AI
- how survey design could be improved for stronger future insights

## Key Findings
The final analysis found that:
- organizations are more likely to encourage AI use through communication, experimentation, and training than require it
- text-generation tools are the most widely used AI category among respondents
- data security and privacy are the top concerns associated with AI adoption
- one open-ended survey question produced limited analytical value and was redesigned for better comparability

## Files
- `notebooks/01_data_cleaning_and_summary.ipynb`  
  Cleans the survey export, groups question types, calculates counts and percentages, and produces a summary results file.

- `notebooks/02_visualization_and_reporting.ipynb`  
  Uses the processed summary file to build polished horizontal bar charts for presentation-ready reporting.

- `data/processed/survey_summary_results.xlsx`  
  Cleaned summary table generated from the analysis notebook.

- `outputs/`  
  Contains exported charts and the final executive-summary style PDF.

## Methods
### Data Preparation
- Loaded raw survey files into pandas
- Removed metadata rows from the survey export
- checked for duplicate responses
- standardized blank values
- separated question fields into:
  - single-select responses
  - multi-select responses
  - text fields

### Summary Calculations
- For single-select questions, percentages were calculated using valid responses as the denominator
- For multi-select questions, percentages were calculated using the number of respondents who selected at least one option for that question

### Visualization
Visuals were built in matplotlib using horizontal bar charts, custom label mapping, and annotated callout boxes to emphasize the most important findings.

## Tools Used
- Python
- pandas
- numpy
- matplotlib
- Jupyter Notebook
- Excel

## Example Questions Answered
- How are organizations promoting AI adoption internally?
- What AI tool categories are most commonly used?
- What risks are most commonly associated with AI adoption?
- How can low-response or poorly structured survey questions be improved?

## Why This Project Matters
This project demonstrates the ability to take ambiguous, real-world survey data and turn it into structured, presentation-ready insights. It combines data cleaning, analytical reasoning, visualization, and business communication in a single workflow.

## Notes on Anonymization
All organization-specific identifiers, branding, and source references have been removed or generalized for portfolio use.

## Author
Hayley Hawkins
M.S. Data Science
