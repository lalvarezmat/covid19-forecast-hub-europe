European data status
================

## Truth data

### Cases and deaths

We evaluate forecasts of cases and deaths against [Johns Hopkins
University data](https://github.com/CSSEGISandData/COVID-19), and we
recommend using this dataset as the basis for forecasts.

-   Daily numbers of cases and deaths are available to download from
    [JHU](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series),
    or from [our
    repository](https://github.com/epiforecasts/covid19-forecast-hub-europe/data-truth).
-   JHU also provide [country
    metadata](https://github.com/CSSEGISandData/COVID-19/blob/master/csse_covid_19_data/UID_ISO_FIPS_LookUp_Table.csv),
    including population counts and ISO-3 codes.

Note there are some differences between the format of the JHU data and
what we require in a forecast. Please check the
[Wiki](https://github.com/epiforecasts/covid19-forecast-hub-europe/wiki/Targets-and-horizons#truth-data)
for more on forecast formatting.

#### Potential issues in the JHU dataset

As of 2022-08-23

| country        | created    | updated    | issue                                                                                 | message                                               | url                                                      |
|:---------------|:-----------|:-----------|:--------------------------------------------------------------------------------------|:------------------------------------------------------|:---------------------------------------------------------|
| greece         | 2022-08-03 | 2022-08-03 | regarding covid data from greece                                                      | Dear all, In Greece, we have recently started rep…    | <https://github.com/CSSEGISandData/COVID-19/issues/5957> |
| france         | 2022-05-20 | 2022-07-28 | discrepancy in france data                                                            | For France, it was found that the number of New ca…   | <https://github.com/CSSEGISandData/COVID-19/issues/5746> |
| united kingdom | 2022-07-20 | 2022-07-20 | united kingdom: date                                                                  | Hi, We were wondering if it is in your plans to us…   | <https://github.com/CSSEGISandData/COVID-19/issues/5904> |
| belgium        | 2022-05-04 | 2022-06-30 | request to add data in three regions i.e. flanders, wallonia and brussels for belgium | <https://datastudio.google.com/c/embed/u/0/reportin>… | <https://github.com/CSSEGISandData/COVID-19/issues/5704> |

Open issues updated over the last eight weeks: from [JHU CSSEGISandData
Github](https://github.com/CSSEGISandData/COVID-19/)

### Hospitalisations

We gather general hospital admissions data from various sources. See
separate [Hospitalisations
README](https://github.com/epiforecasts/covid19-forecast-hub-europe/tree/main/code/auto_download/hospitalisations#readme).

Hospitalisation data can be difficult to produce and interpret, and is
not consistent across all the countries in the ECDC Forecast Hub. To
keep data and forecasts consistent, we include hospitalisations
forecasts for the following locations only:

-   Belgium, Croatia, Czechia, Estonia, France, Ireland, Latvia,
    Liechtenstein, Malta, Norway, Slovenia, Switzerland, United Kingdom

![Plot of truth data from different sources for all countries covered by
the forecast hub](plots/hospitalisations.svg)

The Hub validates and evaluates forecasts against the single dataset in
[ECDC/truth_ECDC-Incident
Hospitalizations.csv](ECDC/truth_ECDC-Incident%20Hospitalizations.csv).
While we provide raw data files with multiple sources for
hospitalisation data in each location, this is for reference only to
cover daily as well as weekly data.

#### Data revisions

##### Cases

![Plot of revisions in case data](plots/revisions-Cases.svg)

##### Deaths

![Plot of revisions in case data](plots/revisions-Deaths.svg)

##### Hospitalisations

![Plot of revisions in case data](plots/revisions-Hospitalizations.svg)

## Additional data sources

We do not use or evaluate against these data, but the following might be
useful for modelling targets:

| Data                | Description                                                                                                                              | Source | Link                                                                                                                            |
|---------------------|------------------------------------------------------------------------------------------------------------------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------|
| Vaccination         | Number of vaccine doses distributed by manufacturers, number of first, second and unspecified doses administered                         | ECDC   | [Data on COVID-19 vaccination in the EU/EEA](https://www.ecdc.europa.eu/en/publications-data/data-covid-19-vaccination-eu-eea)  |
| Variants of concern | Volume of COVID-19 sequencing, the number and percentage distribution of VOC for each country, week and variant submitted since 2020-W40 | ECDC   | [Data on SARS-CoV-2 variants in the EU/EEA](https://www.ecdc.europa.eu/en/publications-data/data-virus-variants-covid-19-eueea) |
| Testing             | Weekly testing rate and weekly test positivity                                                                                           | ECDC   | [Data on testing for COVID-19 by week and country](https://www.ecdc.europa.eu/en/publications-data/covid-19-testing)            |
