# Tableau COVID-19 in Indonesia Dashboard

---

## 🔗 Access the Dashboard

* 📊 **Interactive Tableau Dashboard:**
  👉 [Click here to view the live dashboard on Tableau Public](https://public.tableau.com/views/COVID-19IndonesiaDataset_17531634641070/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
 
* 📄 **Dashboard Report:**
  👉 [Click here to view the dashboard](./Dashboard/)

---

## 1. Background and Overview

This personal project provides a deep analytical visualization of the COVID-19 pandemic's impact across Indonesia from early 2020 to late 2022. The dashboard offers both national and provincial-level insights by tracking key health metrics such as new cases, deaths, recoveries, active cases, and population density. It highlights trends over time, geographic distributions, and health system responses.

The purpose of this project is to:

* Track pandemic trends over time
* Identify high-risk regions
* Monitor health recovery and fatality performance

---

## 2. Data Structure Overview

The dataset used consists of a single main table with detailed information on COVID-19 cases at various administrative levels in Indonesia. The columns include:

| Column Name                                                            | Description                                                     |
| ---------------------------------------------------------------------- | --------------------------------------------------------------- |
| `DMY`                                                                  | Date of the data entry                                          |
| `Location` / `Province`                                                | Name of the region or province in Indonesia                     |
| `ISO Code`                                                             | Standardized location code                                      |
| `Country` / `Continent`                                                | Geographic grouping of the location                             |
| `Island`, `State`, `Time Zone`                                         | Geographic metadata                                             |
| `Location Level`                                                       | Granularity of the data (Province, National, etc.)              |
| `Special Status`                                                       | Special designation (e.g., capital region, autonomous province) |
| `New Cases`, `New Deaths`                                              | Daily change in cases and deaths                                |
| `New Recovered`, `New Active Cases`                                    | Daily new recoveries and active case shifts                     |
| `Total Cases`, `Total Deaths`, `Total Recovered`, `Total Active Cases` | Cumulative values                                               |
| `Total Regencies`, `Total Cities`, `Total Districts`                   | Administrative divisions                                        |
| `Total Urban Villages`, `Total Rural Villages`                         | Urban/rural classification                                      |
| `Area (km2)`                                                           | Geographic size of the region                                   |
| `Population`, `Population Density`                                     | Demographic metrics                                             |
| `Longitude`, `Latitude`                                                | Geospatial coordinates                                          |
| `New Cases per Million`, `Total Cases per Million`                     | Normalized case rates                                           |
| `New Deaths per Million`, `Total Deaths per Million`                   | Normalized death rates                                          |
| `Total Deaths per 100rb`                                               | Deaths per 100,000 people                                       |
| `Case Fatality Rate`                                                   | Percentage of cases that resulted in death                      |
| `Case Recovered Rate`                                                  | Percentage of cases that recovered                              |
| `Growth Factor of New Cases`                                           | Ratio of new cases today vs. yesterday                          |
| `Growth Factor of New Deaths`                                          | Ratio of new deaths today vs. yesterday                         |

---

## 3. Executive Summary

### National Overview:

* **New Cases**: 12.80 million
* **New Deaths**: 315.7 thousand
* **New Recovered**: 12.42 million
* **Total Deaths per Million**: 9.22 million
* **Total Recovered**: 4.75 billion
* **Case Recovered Rate**: 27.63K
* **Case Fatality Rate**: 1.30K

### Total COVID-19 Cases by Island:

* Jawa: **1.68B**
* Sumatra: **345.84M**
* Kalimantan: **196.76M**
* Sulawesi: **138.69M**
* Nusa Tenggara: **116.85M**

### National Trends (Feb 2020 – Sep 2022):

* Peak new cases in **July 2021 (2.46M)** and **February 2022 (2.42M)** followed by a sharp decline in **May 2022 (16K)** and minor spike in **August 2022 (303K)**
* New deaths peaked in **August 2021 (77K)** then declined to **540 by September 2022**
* Recovery peaked in **August 2021 (1.96M)** and **March 2022 (1.78M)**

---

## 4. Insight Deep Dive

### a. Provincial Case Analysis

* **DKI Jakarta**

  * Population Density: 15.17M/km²
  * Total Cases: 545.81M
  * Active Cases: 11.66M
  * Deaths/Million: 707,417

* **Jawa Barat**

  * Population Density: 1.18M/km²
  * Total Cases: 439.19M
  * Active Cases: 19.22M
  * Deaths/Million: 157,153

* **Kalimantan Timur**

  * Population Density: 25,208
  * Total Cases: 89.58M
  * Active Cases: 2.54M
  * Deaths/Million: 744,557

* **Bali**

  * Population Density: 670,346
  * Total Cases: 66.24M
  * Active Cases: 2.15M
  * Deaths/Million: 478,479

* **Kepulauan Bangka Belitung**

  * Population Density: 75,609
  * Total Cases: 26.61M
  * Active Cases: 701K
  * Deaths/Million: 473,603

### b. Top 10 Provinces by New Cases per Million

| Province                  | New Cases / Million |
| ------------------------- | ------------------- |
| DKI Jakarta               | 130,228             |
| Kalimantan Utara          | 70,044              |
| DI Yogyakarta             | 61,776              |
| Kalimantan Timur          | 58,842              |
| Kepulauan Bangka Belitung | 47,938              |
| Bali                      | 39,569              |
| Kepulauan Riau            | 36,738              |
| Banten                    | 31,138              |
| Papua Barat               | 28,202              |
| Jawa Barat                | 25,989              |

---

### c. Recovery and Mortality Trends (2020–2022)

| Year | Total Cases | Total Deaths | Fatality Rate   | Recovery Rate |
| ---- | ----------- | ------------ | ----- | ------------- |
| 2020 | 60.57M      | 4.46M        | 686.1 | 7,713         |
| 2021 | 987.83M     | 61.39M       | 365.8 | 11,284        |
| 2022 | 1.49B       | 79.40M       | 245.3 | 8,634         |

---

### d. Growth Rate Analysis

#### Growth Factor of New Cases:

* Peak in **Month 5 (4,061)** and **Month 8 (4,146)**
* Steady decline to **\~2,800s** by Month 11–12

#### Growth Factor of New Deaths:

* Peak in **Month 7 (3,193)**
* Decline to **1,761** in Month 11 and slight increase to **1,911** in Month 12