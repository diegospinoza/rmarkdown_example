# rmarkdown_example
A code sample for the Epidemiologist position at Applied Epi, analyzing a public health surveillance indicator in R

# R Code Sample: Analysis of a Public Health Surveillance Indicator

This repository contains a code sample developed for the Epidemiologist position at Applied Epi.

## Project Overview

This project is an adapted version of the practical material used in the course **"Data Analysis and Visualization in R for Health and Environmental Surveillance"**, offered in partnership with the Pan American Health Organization (PAHO) and Brazil's Ministry of Health.

The original code for data processing and indicator calculation is in the course's source language, Brazilian Portuguese, but the final report was translated into English for demonstration purposes.

The objective of the analysis is to calculate and visualize **Indicator 13** from the Health Surveillance Qualification Program (PQA-VS), a nationwide initiative of Brazil's public health system (SUS). This indicator measures the completeness of "Occupation" and "Economic Activity" fields in occupational health-related notifications.

The analysis pipeline includes:
- Importing and merging multiple datasets (`.dbf` files).
- Data cleaning and manipulation using the `tidyverse`.
- Calculation of the composite indicator by health regions.
- Generation of a summary table with `gt`.
- Creation of a bar chart (`ggplot2`) and a choropleth map (`sf`) to visualize the results.

## Files in this Repository

* `M3_INDICADOR_13_AULA.Rmd`: The R Markdown file containing all the R code, comments, and the final report structure.
* `/DADOS/`: A folder containing all necessary datasets, including `.dbf` files and the shapefile for the map.

## How to Run This Project

1.  Download or clone this repository.
2.  Ensure all files maintain the original folder structure (i.e., the `.Rmd` file in the root and the data files inside the `/DADOS` folder).
3.  Open the `M3_INDICADOR_13_AULA.Rmd` file in RStudio.
4.  Install the required packages, which are listed at the beginning of the script (`rio`, `tidyverse`, `janitor`, `stringi`, `gt`, `sf`).
5.  Click the **"Knit"** button in RStudio to execute the entire analysis and generate the final HTML report.

### Alternative Output: Formatted Word Document

This project is also configured to generate a professionally formatted report in Microsoft Word using the custom template (`modelo_rmarkdown.docx`). This demonstrates the ability to automate and integrate R analyses into standard office workflows.

To generate the Word document:
1.  Open the `M3_INDICADOR_13_AULA.Rmd` file.
2.  In the YAML header (at the very top), comment out the `html_document` output and uncomment a `word_document` section.
3.  Click "Knit". This will produce a `.docx` file styled according to the template.

---
**Contact:** Diego Spinoza | diegospinoza@hotmail.com
