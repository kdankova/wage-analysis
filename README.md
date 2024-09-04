# Wage Analysis: Insights from Salary and Bonus Data

## Overview

This project involves analyzing wage and bonus data to explore gender wage differences. The dataset includes salary information for individuals, along with their gender, and an additional dataset contains bonus information. The objective is to clean the data, remove duplicate entries, and compute the total annual earnings (salary + bonus) to analyze average and median wages across gender.

## Dataset

### Main Dataset (`wage.csv`):
- `person_id`: Identifier for each individual.
- `gender`: Gender of the individual (0 for female, 1 for male).
- `wage`: The individual's salary (in rubles).

### Bonus Dataset (`bonus.csv`):
- `person_id`: Identifier for each individual.
- `bonus`: Bonus amount (in rubles) for the individual.

## Steps and Features

1. **Data Loading**: Load the wage data from `wage.csv` and the bonus data from `bonus.csv`.
   
2. **Data Cleaning**:
   - Replace the gender values: `0` becomes `F` (female), `1` becomes `M` (male).
   - Identify and remove duplicate entries by checking `person_id` and verifying if duplicate entries have consistent wage data.
   - Filter out rows with nonsensical wage values (e.g., negative or zero wages).

3. **Data Analysis**:
   - Calculate the average wage for males and females.
   - Join the wage and bonus datasets based on `person_id`.
   - Calculate the total annual income for each individual by combining the yearly wage (12 months) and the bonus.
   - Compute the mean and median of the total annual income across gender.

4. **Results**:
   - Mean and median salary and total earnings for each gender.
   - Insights into wage gaps or similarities between genders.

### Prerequisites

Ensure that you have Python installed, along with the following libraries:

- `pandas`
- `numpy`

You can install the necessary dependencies using the following command:

```bash
pip install pandas numpy
