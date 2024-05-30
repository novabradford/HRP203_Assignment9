# Simulated Data Analysis Report

This repository contains a Quarto project for analyzing a simulated dataset to determine the underlying formulae used to generate the data. The analysis focuses on identifying the relationships between various predictors and the response variable `cost`.

## Project Structure

HRP203_Assignment9/
│
├── .DS_Store
├── .Rprofile
├── .gitignore
├── .gitattributes
├── HRP203_Assignment9.Rproj
├── Assignment9.qmd # Quarto document containing the report
├── Assignment9.html # Generated HTML report
├── cohort.csv # Simulated dataset
├── renv.lock # R environment lock file
├── README.md # This README file
│
├── Assignment9_files/ # Directory for Quarto output files
│ ├── figure-html/
│ │ ├── unnamed-chunk-3-1.png
│ │ ├── unnamed-chunk-5-1.png
│ │ ├── unnamed-chunk-6-1.png
│ ├── libs/
│ │ ├── bootstrap/
│ │ │ ├── bootstrap.min.css
│ │ │ ├── bootstrap-icons.css
│ │ │ ├── bootstrap.min.js
│ │ │ ├── bootstrap-icons.woff
│ │ ├── quarto-html/
│ │ │ ├── quarto.js
│ │ │ ├── quarto-syntax-highlighting.css
│ │ │ ├── tippy.css
│ │ │ ├── tippy.umd.min.js
│ │ │ ├── anchor.min.js
│ │ │ ├── popper.min.js
│ │ ├── clipboard/
│ │ │ ├── clipboard.min.js
│
├── .git/ # Git repository directory
│ ├── objects/
│ ├── info/
│ ├── logs/
│ ├── hooks/
│ ├── refs/
│ ├── branches/
│ ├── config
│ ├── HEAD
│ ├── description
│ ├── index
│ ├── COMMIT_EDITMSG
│ ├── FETCH_HEAD
│
├── renv/ # R environment directory
│ ├── staging/
│ ├── library/
│ ├── activate.R
│ ├── settings.json
│ ├── .gitignore
│
├── .Rproj.user/ # RStudio project user data
│ ├── F24F9BA7/
│ ├── shared/
│

## Analysis Overview

The analysis is performed in a series of steps to uncover the relationships between the variables in the dataset:

1. **Loading and Exploring the Dataset**: Initial examination of the dataset structure and summary statistics.
2. **Multiple Regression Analysis**: Including additional variables (`smoke`, `female`, `cardiac`) to enhance the model.
3. **Polynomial Regression**: Investigating potential non-linear relationships by including quadratic terms.
4. **Model Comparison**: Using ANOVA to compare different models and determine the best fit.
5. **Residuals vs. Fitted Values Plot**: Diagnosing the quality of the regression model.

## Instructions

### Prerequisites

Ensure you have the following installed on your machine:
- [Quarto](https://quarto.org/)
- R (if using R for analysis)
- Python (if using Python for analysis)

### Setting Up the Environment

#### Using R

1. Install `renv` if you don't have it:
   ```r
   install.packages("renv")
   ```

2. Restore the R environment:
   ```r
   renv::restore()
   ```

#### Using Python

1. Create a virtual environment:
   ```sh
   python -m venv env
   ```

2. Activate the virtual environment:

   - On Windows:
     ```sh
     .\env\Scripts\activate
     ```

   - On macOS/Linux:
     ```sh
     source env/bin/activate
     ```

3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

### Running the Analysis

1. Render the Quarto document:
   ```sh
   quarto render index.qmd
   ```

2. Open the generated HTML report to view the analysis results.

---

Nova Bradford
