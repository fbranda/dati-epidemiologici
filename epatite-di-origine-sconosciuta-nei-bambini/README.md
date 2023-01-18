# Hepatitis of unknown origin in children

## Contents

This repository contains data extracted from the [ECDC-WHO/Europe surveillance bulletin](https://www.ecdc.europa.eu/en/hepatitis/joint-weekly-hepatitis-unknown-origin-children-surveillance-bulletin) bulletins starting from the week of September 27, 2021.

## Data notes

- Data files with `*-latest.csv` suffix refer to the data reported in the last bulletin. 
- Data files with `timeseries-*.csv` prefix refer to the data reported from the first to the most recent bulletin. 

## Getting the data

**Direct download (CSV)**: [https://raw.githubusercontent.com/fbranda/hepatitis/main/ECDC-WHO_Regional_Office_for_Europe/timeseries_cases.csv](https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv)

**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv")))
```

## Contributions
1) [Branda F, Pierini M, Mazzoli S. Hepatitis of unknown origin in children: Why and how to create an open access database. Journal of Clinical Virology Plus. 2022 Aug 1;2(3):100102.](https://www.sciencedirect.com/science/article/pii/S2667038022000412?via%3Dihub)

## License and attribution

This repository and data exports are published under the CC BY 4.0 license.




