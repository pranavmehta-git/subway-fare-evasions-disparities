# Racial Disparities in NYC Subway Fare Evasion Arrests

An analysis of racial disparities in fare evasion enforcement using public defender client data from 2016.

## Overview

This project examines microdata on subway fare evasion arrests from Brooklyn Defender Services (BDS) and the Legal Aid Society (LAS) to document racial disparities in enforcement and explore variation across subway stations.

## Key Findings

- **Disproportionate impact**: Black and Hispanic individuals comprise the overwhelming majority of fare evasion arrests
- **Geographic concentration**: Stations in historically Black and Latino neighborhoods show 95%+ Black/Hispanic arrest shares
- **Differential outcomes**: Preliminary evidence suggests White and Asian defendants may have higher case dismissal rates
- **Station variation**: Even controlling for neighborhood demographics, substantial variation exists across stations

## Data

The analysis combines arrest records from two public defender organizations:

| Source | Records | Variables |
|--------|---------|-----------|
| Brooklyn Defender Services | 2,246 | Demographics, ZIP, station |
| Legal Aid Society | 1,965 | Demographics, ZIP, station, dismissal |

**Note**: The data files are not included in this repository. The analysis requires:
- `microdata_BDS_inclass.csv`
- `microdata_LAS_inclass.csv`

## Files

```
├── subway-fare-evasion-disparities.Rmd   # Main R Markdown analysis
├── README.md                              # This file
├── .gitignore                             # Git ignore rules
└── LICENSE                                # MIT License
```

## Requirements

- R (≥ 4.0)
- R packages:
  - `tidyverse`
  - `fastDummies`
  - `forcats`

Install required packages:

```r
install.packages(c("tidyverse", "fastDummies", "forcats"))
```

## Usage

1. Place the CSV data files in the project root directory
2. Open `subway-fare-evasion-disparities.Rmd` in RStudio
3. Knit to HTML or PDF

## Acknowledgments

This analysis was completed as part of the *Data Analysis for Policy Research using R* course at Columbia University, taught by **Prof. Harold Stolper**.

## Related Work

This analysis contributes to ongoing public debate about fare evasion enforcement in NYC. For context, see reporting from [The Marshall Project](https://www.themarshallproject.org/) and [NYC Comptroller reports](https://comptroller.nyc.gov/) on this topic.

## License

MIT License - see [LICENSE](LICENSE) for details.

## Author

Pranav Mehta
