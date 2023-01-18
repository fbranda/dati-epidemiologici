<a href="https://cdn.ecdc.europa.eu/novhep-surveillance/"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-epatiti.png" alt="Epatiti" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-epatiti.png" width="500"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>

# Epatite di origine sconosciuta nei bambini

## Note sui dati 

- I file con suffisso `*-latest.csv` si riferiscono ai dati riportati nell'ultimo bollettino.
- I file con prefisso `timeseries-*.csv` si riferiscono ai dati riportati dal primo al più recente bollettino.  

## Esempio d'uso dei dati

**Download diretto (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv

**Python** (richiede `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv")
```

**R** (richiede `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/timeseries-cases.csv")))
```

## Contributi
1) [Branda F, Pierini M, Mazzoli S. Hepatitis of unknown origin in children: Why and how to create an open access database. Journal of Clinical Virology Plus. 2022 Aug 1;2(3):100102.](https://www.sciencedirect.com/science/article/pii/S2667038022000412?via%3Dihub)

## Licenza

This repository and data exports are published under the CC BY 4.0 license.




