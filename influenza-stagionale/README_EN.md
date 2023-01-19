<a href="https://w3.iss.it/site/rmi/influnet/pagine/rapportoinflunet.aspx"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" alt="Influenza" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" width="400"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>


## Seasonal influenza

 This repository contains data extracted from the [Italian National Institute of Health (ISS)](https://www.epicentro.iss.it/influenza/influnet) 
 bulletins starting from the [2003-2004 seasonal flu](https://w3.iss.it/site/rmi/influnet/pagine/stagioni.aspx).


## Repository structure
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

 ## Data format

- [Evoulution data about seasonal influenza Italy](data-schema-flu-italy.md)

 ## Getting the data

 **Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv

 **Python** (requires `pandas`):
 ```python
 import pandas as pd
 df = pd.read_csv("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv")
 ```

 **R** (requires `httr`):
 ```r
 library(httr)
 df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/dati-epidemiologici/main/influenza-stagionale/flu-season/2022-2023/epidemiological-data/national-cases-2022-2023.csv")))
 ```

 ## Contributions
 1) Automatic report at link https://fbranda.github.io/influnet/
 2) Automatic bot at link https://mastodon.uno/@influbot@sociale.network


 ## License
 
 [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [View license](https://github.com/fbranda/west-nile/blob/main/LICENSE.md)
