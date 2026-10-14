# Medical Appointment No-Show Analysis

**Tools:** Python, pandas, NumPy, matplotlib, Jupyter Notebook
**Completed:** 2026, as part of the Udacity Data Analyst Nanodegree

## Overview
Missed medical appointments cost clinics time and money. This project explores 110,000+ medical appointments from public clinics in Brazil to look for patterns in who misses appointments.

## Questions
1. Are patients enrolled in Brazil's Bolsa Familia welfare program more likely to miss appointments?
2. Does a patient's age relate to how often they miss appointments?

## Data
Public "Medical Appointment No Shows" dataset from Kaggle (appointments from 2016):
https://www.kaggle.com/datasets/joniarroba/noshowappointments

The data file is not included in this repository. Download it from Kaggle to run the notebook.

## Process
- **Cleaning:** fixed misspelled column names, removed an invalid age value (-1), converted date columns to dates, and converted the No-show column to numbers (1 = missed, 0 = attended).
- **Analysis:** compared no-show rates across groups using pandas `groupby`.
- **Visualization:** bar charts, a histogram, and a line chart in matplotlib.

## Key Findings
- Patients enrolled in the welfare program missed **23.7%** of appointments, compared to **19.8%** for patients not enrolled.
- Younger patients, especially those under 30, missed appointments more often. No-show rates generally decreased as age increased.

## Limitations
- No statistical tests were run, so these differences show patterns, not proven effects.
- Correlation is not causation. Factors like transportation, work schedules, or health status may also play a role.

## Files
- `no_show_analysis.ipynb`: the full analysis, with code, charts, and written findings
