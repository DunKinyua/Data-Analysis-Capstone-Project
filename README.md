# Data-Analysis-Capstone-Project
An Data Analysis Report created using R Markdown. 
---
title: "Data Analysis Capstone Project"
author: "Duncan Kinyua Gakuthi"
date: "2022-09-07"
output:
  html_document: default
  pdf_document: default
  word_document: default
editor_options:
  markdown:
    wrap: sentence
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

# Bed to Population Ratio in Kenya & its Counties.

## Introduction.

This project aimed to analyze Kenyan Hospitals' capacity by counting the number of beds per county and comparing their capacities based on the WHO threshold of 3 beds for every 1000 people. The data used was collected in 2019 at the onset of Covid-19 to analyze if the country had enough capacity to care for victims of the pandemic. However, the government had to take fast measures to build capacity due to the shortage of hospital beds. This saw some counties convert school dormitories to hospital wards to hospitalize the increasing number of Covid-19 patients that needed inpatient care. The data sets contained 12,394 hospitals (Excluding level 1).
Hospitals in Kenya are categorized in the levels below;

* Level 6- National referral hospitals.

* Level 5- County Referral Hospitals.

* Level 4 -County Hospitals.

* Level 3- Health Centers.

* Level 2- Health Dispensaries.

* Level 1- Community Facilities.

There are six Level 6 hospitals and five of them are located in Nairobi while one is in Uasin Gishu.
There are a total of 19 Level 5 hospitals in 19 counties while level 4 hospitals are 818.There are 2139 Level 3 hospitals and 9411 Level 2 hospitals.This project does not take to account the Level 1 hospitals.

![Number of Hospitals per Keph Level](C:\Users\gakut\OneDrive\Desktop\Google Data Analytics Class\Capstone Project\hospitalss.png)

##  Dataset Extraction and Preparation.

The data used in the analysis was sourced from a public dataset dated 2019. Since the data was collected, there is a probability of additional hospitals and beds in the last three years. However, the change is expected to be minimal because there are zero reports of new levels 6,5, and 4, which can cause a considerable difference in the number of hospitals. Additionally, no major hospitals have been closed down, which could lead to a massive decrease in the number of beds.
No significant errors or missing information were identified; therefore, the analysis was done using complete and accurate data.

## Ownership of Hospitals in Kenya.

* 5,878- Ministry of Health.
* 5118- Private Practice.
* 1032-Faith-Based organisations.
* 366- Non-Governmental Organizations.
```{r M, echo=FALSE}

```
Hospital Beds- This project considers hospital beds as those that are staffed, maintained, and available for medical services to inpatients. The number of hospital beds is also inclusive of cots that are meant for babies.

## Problem Statement.

Some regions in the country still lack sufficient beds to cater for their constituents. Out of all the 47 Counties, only 3 counties; Nyeri, Embu and Isiolo meet the threshold bed to people ratio of 3:1000 as per the requirements of the World Health Organization. The other 44 counties have a deficit of beds, a matter that the Ministry of Health and the Private Sector need to consider when improving the country's health sector. Kilifi County had the largest deficit considering that it has a population of over 1.4 million people yet it only has 1131 beds.

Figure 2 illustrates the deficit of beds per county.

![Number of Bed Deficits Per County](C:\Users\gakut\OneDrive\Desktop\Google Data Analytics Class\Capstone Project\deficit.png)
### Formula Used.

```{r echo=FALSE, out.width="100%"}
knitr::include_graphics("formula.jpg",error=FALSE)

```

Using the formula above,every county should have a ratio of 3 and above to meet the recommended WHO bed to 1000 population ratio. Below is a histogram showing the ratios of all 47 counties. The counties that have achieved the recommended WHO ratio are highlighted in green.

```{r echo=FALSE, out.width="100%"}
knitr::include_graphics("ratio.png",error=FALSE)

```


3 beds=1000 inhabitants.
It is simplified as one bed for every 333 inhabitants. 

## Recommendations.

There is an acute shortage of beds in 44 counties, contributing to the lack of medical services in the country. Kilifi is the most affected county because it only has 1131 beds available for its population of 1,453,787. To solve this problem, the Ministry of Health, Faith-based organizations, Non-Governmental organizations, and Private Hospital owners should invest in increasing the capacity of their hospitals by adding a considerable amount of beds. This might also require the expansion of Hospital wards to accommodate additional beds.

The figure below compares the current bed capacity to the required or ideal bed capacity. As stated earlier, there are only 3 counties namely; Isiolo, Nyeri and Embu that have achieved the recommended WHO capacity ratio 3 beds for every 1000 people. 

```{r echo=FALSE, out.width="100%"}
knitr::include_graphics("ideal2.png",error=FALSE)

```

The chart above shows the ideal number of beds versus the current bed capacity of every county.


Adding more beds will also lead to a need for more facilities, such as bedding and the employment of more nurses. This will be beneficial because more patients will be admitted to the hospitals, and more nurses and doctors will find employment opportunities. It will also create jobs for sectors involved in making hospital beds, i.e., The jua kali sector. Through the Ministry of Health, the government should be on the front line of increasing hospitals' capacity by adding beds and medicine and employing more caregivers. The project of adding more beds should start with Kilifi, Nakuru, Bungoma, and Kiambu, which have the highest deficit of beds and large population.

### Achieving Vision 2030.

As per Vision 2030, which aims to transform Kenya into an industrialized middle-income country, providing high-quality life to its inhabitants, it is vital to achieve high-quality healthcare. According to the constitution, every citizen has a right to healthcare. Therefore, the government should ensure that all Kenyans get high-quality healthcare services at an affordable price and without struggling. Most hospitals have reported bed-sharing cases due to shortages, which is a calamity that should be avoided. Patients have also complained of lack of medicine in public hospitals, forcing them to seek medical attention in more expensive, private hospitals, and most Kenyans cannot afford.

## Conclusion.

The analysis illustrates one of the major problems affecting the health sector in Kenya. According to citizens and research done by health experts, healthcare facilities tend to be poorly equipped and lacking critical equipment and supplies. They are also understaffed or poorly managed. Due to the growing population and the increasing risk of pandemics in the World, the improvement of healthcare should be a top priority of the current government. Beside improving the healthcare standards of the nation,increasing the bed capacity and other related resources will enable it to have sufficient capacity to be an economic hub in Africa.



  
