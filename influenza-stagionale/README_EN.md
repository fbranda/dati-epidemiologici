<a href="https://w3.iss.it/site/rmi/influnet/pagine/rapportoinflunet.aspx"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" alt="Influenza" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" width="400"/></a>

[Italiano](README.md) - [English](README_EN.md)<br><br>


# Seasonal influenza

This repository contains data extracted from the [Italian National Institute of Health (ISS)](https://www.epicentro.iss.it/influenza/influnet) bulletins starting from the [2003-2004 seasonal flu](https://w3.iss.it/site/rmi/influnet/pagine/stagioni.aspx).


## Repository structure
```

influnet/
├── flu-season/
│   ├── 2003-2004/
│   │   ├── epidemiological_data/
│   │       ├── national_cases.csv
│   │   ├── influnet_report/
│   │       ├── influnet-epi-2005-2006.pdf
│   ├── ...
│   │
│   │   
│   │
│   ├── 2012-2013/
│   │   ├── epidemiological_data/
│   │       ├── national_cases.csv
│   │       ├── regional_cases.csv
│   │   ├── influnet_report/
│   │       ├── influnet-epi/
│   │           ├── influnet-epi-2012-2013_1.pdf
│   │           ├── ...
│   │       ├── influnet-vir/
│   │           ├── influnet-vir-2012-2013_1.pdf
│   │           ├── ...
│   │   ├── virological_data/
│   │       ├── national_typing_subtyping_influenza_viruses.csv
├── data-aggregated/
│   ├── epidemiological_data/
│   │   ├── national_cases.csv
│   │   ├── regional_cases.csv
│   ├── virological_data/
│   │   ├── national_typing_subtyping_influenza_viruses.csv


```

## Data format

- [Evoulution data about seasonal influenza](data-schema-flu-italy.md)<br>


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

This repository and data exports are published under the CC BY 4.0 license.


