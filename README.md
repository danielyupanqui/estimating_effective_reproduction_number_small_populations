# A Simplified Approach for Estimating the Effective Reproduction Number in Small Populations

## Overview

Charles Plante and I develop a methodology to estimate **daily reproduction numbers** of infectious diseases in **small population areas** by focusing on the growth rate derived from the **SIR model**.

We estimate the daily growth rate of COVID-19 using **non-parametric kernel regression** for Canada at multiple geographic levels, including:
- The national level  
- Provinces and territories  
- 99 public health regions  

These estimates are directly compared with those produced by **EpiEstim**, a widely used standard method.

## Key Findings

- Kernel regression produces **smoother and more reliable growth-rate estimates** in both large and small populations.
- The advantages are especially pronounced in settings with **sparse or volatile case data**.
- As a result, our approach yields **more stable and robust daily reproduction-number estimates** in small population areas than EpiEstim.
- The findings suggest that standard methods often rely on assumptions that may not hold in **low-incidence settings**.

## Contribution

Overall, this work demonstrates that **non-parametric kernel regression** provides a more consistent and flexible framework for estimating disease transmission dynamics across **heterogeneous population sizes**, improving inference where traditional methods perform poorly.


## Replication Instructions

This repository uses a portable directory structure. Users should not manually modify the working directory or file paths. All paths are defined relative to the project root, allowing the project folder to be placed in any location on the user’s system without requiring path adjustments.

To replicate the analysis, users must have both Stata and R installed.

Follow these steps to reproduce the results:

1. Download the release archive associated with this repository.

2. Extract and save the project folder in any location on your computer.

3. Open Stata.

4. Open the file `run_all.do`:
   - either by double-clicking the file,
   - or through File → Open.

5. Run the pipeline by executing:

   do run_all.do

The pipeline automatically handles directory structure, file references, and execution order.

## Data

This paper utilizes a case study of the COVID-19 pandemic in Canada, employing data publicly available from the **COVID-19 Canada Open Data Working Group**.

The data are sourced from the group’s public GitHub repository, which provides harmonized, regularly updated COVID-19 epidemiological data for Canada:
- https://github.com/ccodwg/Covid19Canada

### Citation

COVID-19 Canada Open Data Working Group. (2022). *COVID-19 Canada Open Data Working Group dataset*.  

### Data License and Availability

The data are openly available and distributed under an open-data license, permitting use, redistribution, and adaptation with appropriate attribution. Users should consult the original repository for the most current version of the data and detailed licensing information.
