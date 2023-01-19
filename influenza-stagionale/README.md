<a href="https://w3.iss.it/site/rmi/influnet/pagine/rapportoinflunet.aspx"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" alt="Influenza" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" width="400"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>


# Influenza stagionale

Questo repository contiene i dati estratti dai bollettini dell'[Istituto Superiore di Sanità (ISS)](https://www.epicentro.iss.it/influenza/influnet) a partire dalla [stagione influenzale 2003-2004](https://w3.iss.it/site/rmi/influnet/pagine/stagioni.aspx).


## Struttura del repository
```

influenza-stagionale/
├── flu-season/
│   ├── 2003-2004/
│   │   ├── epidemiological-data/
│   │       ├── national-cases-2003-2004.csv
│   │   ├── influnet-report/
│   │       ├── influnet-epi-2003-2004.pdf
│   ├── ...
│   │
│   │   
│   │
│   ├── 2012-2013/
│   │   ├── epidemiological-data/
│   │       ├── national-cases-2012-2013.csv
│   │       ├── regional-cases-2012-2013.csv
│   │   ├── influnet-report/
│   │       ├── influnet-epi/
│   │           ├── influnet-epi-2012-2013_1.pdf
│   │           ├── ...
│   │       ├── influnet-vir/
│   │           ├── influnet-vir-2012-2013_1.pdf
│   │           ├── ...
│   │   ├── virological-data/
│   │       ├── virological-cases-2012-2013.csv
├── data-aggregated/
│   ├── epidemiological-data/
│   │   ├── timeseries-national-cases.csv
│   │   ├── timeseries-regional-cases.csv
│   ├── virological-data/
│   │   ├── timeseries-virological-cases.csv


```
## Formato dei dati

- [Dati andamento influenza Italia](data-schema-influenza-italia.md)

## Esempio d'uso dei dati

**Download diretto (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv

**Python** (richiede `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv")
```

**R** (richiede `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv")))
```

## Contributi
1) [Report automatico](https://fbranda.github.io/influnet/)
2) [Bot automatico](https://mastodon.uno/@influbot@sociale.network)


## Licenza

[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/fbranda/west-nile/blob/main/LICENSE.md)


