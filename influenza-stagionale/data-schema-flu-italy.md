<a href="https://w3.iss.it/site/rmi/influnet/pagine/rapportoinflunet.aspx"><img src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" alt="Influenza" data-canonical-src="https://github.com/fbranda/dati-epidemiologici/blob/main/assets/img/logo-influnet.jpg" width="400"/></a>

# Evolution data about seasonal influenza

### Epidemiological data schema

**Directory:**  epidemiological-data<br>
**Filename:** national-cases-#.csv (example: national-cases-2022-2023.csv)<br>


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Flu season reference period  |
| **year_week**     |  String       | Bulletin reference week   |
| **start_date**     |  String       | Beginning date of bulletin reporting week   |
| **end_date**     |  String       | End date of the bulletin reference week   |
| **number_healthcare_workers**   | Integer | Number of cases reported by the healthcare workers  |
| **number_cases**  | Integer | Weekly number of new confirmed cases  |
| **population** | Integer | Reference population |
| **incidence** | Double | 1000 x number_cases/population |
| **pop_0-4** | Integer | 0-4 reference population  |
| **cases_0-4** | Integer | 0-4 weekly new cases  |
| **inc_0-4** | Double | 1000 x cases_age_0-4/pop_age_0-4  |
| **pop_5-14** | Integer | 5-14 reference population  |
| **cases_5-14** | Integer | 5-14 weekly new cases  |
| **inc_5-14** | Double | 1000 x cases_age_5-14/pop_age_5-14  |
| **pop_15-64** | Integer | 15-64 reference population  |
| **cases_15-64** | Integer | 15-64 weekly new cases  |
| **inc_15-64** | Double | 1000 x cases_age_15-64/pop_age_15-64  |
| **pop_65+** | Integer | ≥65 reference population  |
| **cases_65+** | Integer | ≥65 weekly new cases  |
| **inc_65+** | Double | 1000 x cases_age_65-plus/pop_age_65-plus  |

**Directory:**  epidemiological-data<br>
**Filename:** regional-cases-#.csv (example: regional-cases-2022-2023.csv)<br>

| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Flu season reference period  |
| **year_week**     |  String       | Bulletin reference week   |
| **start_date**     |  String       | Beginning date of bulletin reporting week   |
| **end_date**     |  String       | End date of the bulletin reference week   |
| **region_name**     |  String       | Region name   |
| **region_code**     |  String       | Region Code (ISTAT) |
| **lat**     |  WGS84       | Latitude   |
| **long**     |  WGS84       | Longitude   |
| **number_healthcare_workers**   | Integer | Number of cases reported by the healthcare workers  |
| **number_cases**  | Integer | Weekly number of new confirmed cases  |
| **population** | Integer | Reference population |
| **incidence** | Double | 1000 x number_cases/population |
| **cases_0-4** | Integer | 0-4 weekly new cases  |
| **inc_0-4** | Double | 1000 x cases_age_0-4/pop_age_0-4  |
| **cases_5-14** | Integer | 5-14 weekly new cases  |
| **inc_5-14** | Double | 1000 x cases_age_5-14/pop_age_5-14  |
| **cases_15-64** | Integer | 15-64 weekly new cases  |
| **inc_15-64** | Double | 1000 x cases_age_15-64/pop_age_15-64  |
| **cases_65+** | Integer | ≥65 weekly new cases  |
| **inc_65+** | Double | 1000 x cases_age_65-plus/pop_age_65-plus  |



### Virological data schema

**Directory:**  virological-data<br>
**Filename:** virological-cases-#.csv (example: virological-cases-2022-2023.csv)<br>


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **flu_season**      | String       | Flu season reference period  |
| **year_week**     |  String       | Bulletin reference week   |
| **start_date**     |  String       | Beginning date of bulletin reporting week   |
| **end_date**     |  String       | End date of the bulletin reference week   |
| **influenza_viruses**  |  String       |  Influenza virus name  |
| **number_samples** | Integer | Number of clinical samples received from the laboratories  |
| **number_sequenced** | Integer | Number of sequenced samples |
| **number_detections_influenza_viruses** | Integer | Number of detections reported of the virus |


