<a href="https://monkeypoxreport.ecdc.europa.eu/"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-vaiolo.png" alt="Vaiolo" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-vaiolo.png" width="900"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>

# Mpox 

Questo archivio contiene dati estratti dai bollettini [ECDC-WHO/Europe](https://monkeypoxreport.ecdc.europa.eu/) e [Ministero della Salute italiano](https://www.salute.gov.it/portale/malattieInfettive/dettaglioSchedeMalattieInfettive.jsp?lingua=italiano&id=254&area=Malattie%20infettive&menu=indiceAZ&tab=1).  


## Esempio d'uso dei dati

**Download diretto (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/Italy/mpox-italy.csv

**Python** (richiede `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/Italy/mpox-italy.csv")
```

**R** (richiede `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/vaiolo-delle-scimmie/Italy/mpox-italy.csv")))
```
## Contributi
1) [Branda F, Pierini M, Mazzoli S. Monkeypox: EpiMPX surveillance system and open-data with a special focus on European
and Italian epidemic. Journal of Clinical Virology Plus 2022;p. 100114.](https://www.sciencedirect.com/science/article/pii/S2667038022000539)

2) [Bayesian framework for Monkeypox R0 early estimation in Europe](https://github.com/maxdevblock/Monkeypox_R0_Europe)

3) [Branda F, Pierini M, Mazzoli S. Monkeypox: Early Estimation of Basic Reproduction Number R0 in Europe. Journal of Medical Virology](https://onlinelibrary.wiley.com/doi/10.1002/jmv.28270)


## Licenza

[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/fbranda/west-nile/blob/main/LICENSE.md)
