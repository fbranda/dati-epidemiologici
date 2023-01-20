<a href="https://w3.iss.it/site/rmi/influnet/pagine/rapportoinflunet.aspx"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" alt="Influenza" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" width="400"/></a>

# Dati andamento influenza Italia

### Schema dati epidemiologici

**Directory:**  epidemiological-data<br>
**Nome file:** national-cases-#.csv (esempio: national-cases-2022-2023.csv)<br>


| Nome campo                 | Formato                       |Descrizione                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Anno stagione influenzale  |
| **year_week**     |  String       | Settimana bollettino   |
| **start_date**     |  String       | Data iniziale della settimana del bollettino   |
| **end_date**     |  String       | Data finale della settimana del bollettino   |
| **number_healthcare_workers**   | Integer | Numero di casi segnalati dagli operatori sanitari  |
| **number_cases**  | Integer | Numero settimanale di nuovi casi confermati  |
| **population** | Integer | Popolazione di riferimento |
| **incidence** | Double | 1000 x number_cases/population |
| **pop_0-4** | Integer | Popolazione di riferimento nella fascia d'età 0-4  |
| **cases_0-4** | Integer | Nuovi casi settimanali nella fascia d'età 0-4  |
| **inc_0-4** | Double | 1000 x cases_age_0-4/pop_age_0-4  |
| **pop_5-14** | Integer | Popolazione di riferimento nella fascia d'età 5-14 |
| **cases_5-14** | Integer | Nuovi casi settimanali nella fascia d'età 5-14   |
| **inc_5-14** | Double | 1000 x cases_age_5-14/pop_age_5-14  |
| **pop_15-64** | Integer | Popolazione di riferimento nella fascia d'età 15-64  |
| **cases_15-64** | Integer | Nuovi casi settimanali nella fascia d'età 15-64   |
| **inc_15-64** | Double | 1000 x cases_age_15-64/pop_age_15-64  |
| **pop_65+** | Integer | Popolazione di riferimento nella fascia d'età ≥65   |
| **cases_65+** | Integer | Nuovi casi settimanali nella fascia d'età ≥65 |
| **inc_65+** | Double | 1000 x cases_age_65-plus/pop_age_65-plus  |

**Directory:**  epidemiological-data<br>
**Nome file:** regional-cases-#.csv (example: regional-cases-2022-2023.csv)<br>

| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Anno stagione influenzale  |
| **year_week**     |  String       | Settimana bollettino   |
| **start_date**     |  String       | Data iniziale della settimana del bollettino   |
| **end_date**     |  String       | Data finale della settimana del bollettino   |
| **region_name**     |  String       | Nome regione   |
| **region_code**     |  String       | Codice regione (ISTAT) |
| **lat**     |  WGS84       | Latitudine   |
| **long**     |  WGS84       | Longitudine   |
| **number_healthcare_workers**   | Integer | Numero di casi segnalati dagli operatori sanitari  |
| **number_cases**  | Integer | Numero settimanale di nuovi casi confermati  |
| **population** | Integer | Popolazione di riferimento |
| **incidence** | Double | 1000 x number_cases/population |
| **cases_0-4** | Integer | Nuovi casi settimanali nella fascia d'età 0-4  |
| **inc_0-4** | Double | 1000 x cases_age_0-4/pop_age_0-4  |
| **cases_5-14** | Integer | Nuovi casi settimanali nella fascia d'età 5-14   |
| **inc_5-14** | Double | 1000 x cases_age_5-14/pop_age_5-14  |
| **cases_15-64** | Integer | Nuovi casi settimanali nella fascia d'età 15-64   |
| **inc_15-64** | Double | 1000 x cases_age_15-64/pop_age_15-64  |
| **cases_65+** | Integer | Nuovi casi settimanali nella fascia d'età ≥65 |
| **inc_65+** | Double | 1000 x cases_age_65-plus/pop_age_65-plus  |



### Schema dati virologici

**Directory:**  virological-data<br>
**Nome file:** virological-cases-#.csv (example: virological-cases-2022-2023.csv)<br>


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Anno stagione influenzale  |
| **year_week**     |  String       | Settimana bollettino |
| **start_date**     |  String       | Data iniziale della settimana del bollettino   |
| **end_date**     |  String       | Data finale della settimana del bollettino   |
| **influenza_viruses**  |  String       |  Nome virus  |
| **number_samples** | Integer | Numero di campioni clinici ricevuti dai laboratori  |
| **number_sequenced** | Integer | Numero di campioni sequenziati |
| **number_detections_influenza_viruses** | Integer | Numero di virus individuati |


