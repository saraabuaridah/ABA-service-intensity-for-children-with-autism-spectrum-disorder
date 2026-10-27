# 2026_ABA_service_intensity_ASD

## ABA Service Intensity in Children With Autism Spectrum Disorder

This repository contains R scripts for cleaning and processing data, identifying the study cohort, and examining sociodemographic and geographic differences in Applied Behavior Analysis (ABA) service intensity among Medicaid- and commercially insured children with Autism Spectrum Disorder (ASD).

Prerequisites

The following R libraries must be installed.

library(data.table)
library(dplyr)
library(stringi)
library(stringr)
library(tidyr)
library(purrr)
library(AdhereR)
library(arrow)
library(ggplot2)
library(scales)
library(tidycensus)
library(sf)
library(table1)
library(lubridate)
library(MASS)
library(broom)
library(forestplot)

## Authorization

Data used in this project are proprietary and are not available for public access. This repository contains analysis code only and does not include individual-level records or restricted datasets.


## How to Use It

This repository provides R code illustrating the analytical logic and methodological framework used in the study. The code is organized into two components:

### 1. Cohort Selection
Identification of individuals with autism spectrum disorder (ASD), application of study eligibility criteria, determination of the ASD index date, and construction of the analytic cohort and ABA service intensity outcome.

### 2. Statistical Analysis
Specification of zero-truncated negative binomial regression models to examine sociodemographic and geographic differences in ABA service intensity, including race and ethnicity-by-insurance interaction analyses.

## Data Availability

The study used the **IQVIA PharMetrics Plus** claims database. The underlying patient-level data are proprietary and subject to licensing restrictions and are therefore not included in this repository.

The R code is provided to illustrate the analytical approach and methodological procedures. It is not intended to serve as a standalone reproduction of the published results without access to the relevant data.

## Analysis

We identified children diagnosed with ASD who received ABA services and met the study eligibility criteria. ABA service intensity was measured as the number of distinct days on which ABA services were received during the 12-month follow-up period.

Descriptive analyses were conducted to characterize the study population and examine differences in service intensity across race and ethnicity, insurance type, age group, sex, and geographic region.

Zero-truncated negative binomial regression models were used to evaluate associations between sociodemographic and geographic characteristics and ABA service intensity among children receiving ABA services. Incidence rate ratios (IRRs) and 95% confidence intervals were estimated.

Additional interaction analyses examined whether associations between race and ethnicity and ABA service intensity differed by insurance type.

### Complete citation and DOI will be provided when the publication is available online.
