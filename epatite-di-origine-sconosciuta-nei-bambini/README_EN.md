<a href="https://cdn.ecdc.europa.eu/novhep-surveillance/"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-epatiti.png" alt="Epatiti" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-epatiti.png" width="900"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>

# Hepatitis of unknown origin in children

This repository contains data extracted from the [ECDC-WHO/Europe surveillance](https://cdn.ecdc.europa.eu/novhep-surveillance/) bulletins. 

## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/case-count.csv

**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/case-count.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/epatite-di-origine-sconosciuta-nei-bambini/ECDC-WHO-Regional-Office-for-Europe/case-count.csv")))
```

## Contributions
1) [Branda F, Pierini M, Mazzoli S. Hepatitis of unknown origin in children: Why and how to create an open access database. Journal of Clinical Virology Plus. 2022 Aug 1;2(3):100102.](https://www.sciencedirect.com/science/article/pii/S2667038022000412?via%3Dihub)

## License 

[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [View license](https://github.com/fbranda/west-nile/blob/main/LICENSE.md)




