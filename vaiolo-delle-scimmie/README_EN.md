<a href="https://monkeypoxreport.ecdc.europa.eu/"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-vaiolo.png" alt="Vaiolo" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-vaiolo.png" width="900"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>

# Mpox 

## Contents

This repository contains data extracted from the [ECDC-WHO/Europe surveillance](https://monkeypoxreport.ecdc.europa.eu/) and [Ministry of Health of Italy](https://www.salute.gov.it/portale/malattieInfettive/dettaglioSchedeMalattieInfettive.jsp?lingua=italiano&id=254&area=Malattie%20infettive&menu=indiceAZ&tab=1) bulletins.  

## Repository structure
```

vaiolo-delle-scimmie/
├── ECDC-WHO/
│   ├── clinical-description/
│   │   ├── symptoms-latest.csv
│   │   ├── timeseries-symptoms.csv
│   │
│   ├── demographics
│   │   ├── age-sex-cases-latest.csv
│   │   ├── timeseries-age-sex-cases.csv
│   │
│   ├── epicurves
│   │   ├── epicurve-by-country.csv
│   │   ├── epicurve-by-notification_date.csv
│   │   ├── epicurve-by-typedate.csv
│   │
│   ├── ihr-summary
│   │   ├── table-IHR-Tessy-latest.csv
│   │   ├── timeseries-table-IHR-Tessy.csv
│   │
│   ├── microbiological-analyses
│   │   ├── microbiological-analysis-latest.csv
│   │   ├── timeseries-microbiological-analysis.csv
│   │
│   ├── outcome-HIVstatus-HCW
│   │   ├── datasummary-outcome-latest.csv
│   │   ├── timeseries-datasummary-outcome.csv
│   │
│   ├── plots
│   │   ├── ...
│   │
│   ├── sexual-orientation
│   │   ├── sexualorientation-latest.csv
│   │   ├── timeseries-sexualorientation.csv
│   │
│   ├── summary-table
│   │   ├── datasummary-latest.csv
│   │   ├── timeseries-datasummary.csv
│   │
├── Italy/
│   ├── Plots/
│   │   ├── ...
│   ├── mpox-italy.csv
│   ├── mpox-region.csv
│   │
├── R/
│   ├── estimates/
│   │   ├── Austria.csv
│   │   ├── Belgium.csv
│   │   ├── ...
│   │
│   ├── plots/
│   │   ├── Serial Interval/
│   │       ├── SI_CDF.pdf
│   │       ├── SI_PDF.pdf
│   │       ├── SI_mean.pdf
│   │       ├── SI_std.pdf
│   │   ├── Austria.pdf
│   │   ├── Belgium.pdf
│   │   ├── ...
│   │
│   │   ├── Rt.R
```

## Data format

- [Evoulution data about Mpox](data-schema-mpox.md)


## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/ECDC-WHO/epicurves/epicurve-by-country.csv

**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/ECDC-WHO/epicurves/epicurve-by-country.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/ECDC-WHO/epicurves/epicurve-by-country.csv")))
```
## Contributions
1) [Branda F, Pierini M, Mazzoli S. Monkeypox: EpiMPX surveillance system and open-data with a special focus on European
and Italian epidemic. Journal of Clinical Virology Plus 2022;p. 100114.](https://www.sciencedirect.com/science/article/pii/S2667038022000539)

2) [Bayesian framework for Monkeypox R0 early estimation in Europe](https://github.com/maxdevblock/Monkeypox_R0_Europe)

3) [Branda F, Pierini M, Mazzoli S. Monkeypox: Early Estimation of Basic Reproduction Number R0 in Europe. Journal of Medical Virology](https://onlinelibrary.wiley.com/doi/10.1002/jmv.28270)


## License

 [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [View license](https://github.com/fbranda/west-nile/blob/main/LICENSE.md)