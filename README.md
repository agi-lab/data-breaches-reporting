# Data Breach Analysis Repository

This repository contains data, code, and documentation for analyzing data breaches reported to state Attorneys General across the United States.

## Repository Contents

### Documentation
- **1.Online_Appendix.pdf** - Supplementary appendices referenced in the paper.
- **3.tf_raw_to_R_Supp.pdf** - Documentation of the manual transformation process from raw data to usable CSV files, including assumptions made for special entries.

### Data
- **2.raw_data_[filename]** - Raw datasets in PDF or Excel format extracted from state Attorneys General websites.
- **4.data_put_in_R_[filename]** - Edited data in CSV format used for R processing.
- **6.elig_breaches_Supp.csv** - Eligible observations used in the modeling stage, containing fields:
  - `Name.of.Company`
  - `Date.of.Breach` (start date)
  - `Reported.Date`
  - `state`
  - `State.Residents.Affected`
- **8.qtr_upper_triangles_data_Supp.csv** - Upper triangles (actual data) for statistical analysis.
- **11.qtr_matrices_data_Supp.csv** - Matrices containing upper triangles (actual data) and lower triangles (filled with zeros).

### Code
- **5.data_processing_in_R_Supp.Rmd** - R markdown that processes the edited data and outputs eligible observations for modeling.
- **7.qtr_upper_triangles_code_Supp.Rmd** - Creates upper triangles from eligible breach data.
- **9.gam_and_diagnostics_Supp.Rmd** - Outputs the final Generalized Additive Model (GAM) and produces model diagnostics (heatmaps).
- **10.qtr_matrices_code_Supp.Rmd** - Creates matrices with upper triangles (actual data) and lower triangles (filled with zeros).
- **12.graphs_Supp.Rmd** - Produces all graphs shown in the paper.

## Data Flow
1. Raw data is extracted from state Attorneys General websites (Item 2)
2. Raw data is manually transformed into usable CSV files (Item 3 → Item 4)
3. CSV files are processed in R to extract eligible observations (Item 5 → Item 6)
4. Upper triangles are created from eligible breach data (Item 7 → Item 8)
5. GAM modeling and diagnostics are performed on upper triangles (Item 9)
6. Matrices containing both upper and lower triangles are created (Item 10 → Item 11)
7. Graphs for the paper are generated (Item 12)

## Citation
Please cite this repository using the appropriate citation format if you use this data or code in your research.
