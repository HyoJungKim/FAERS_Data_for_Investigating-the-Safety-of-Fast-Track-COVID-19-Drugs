# FAERS Data for Investigating the Safety of Fast-Track COVID-19 Drugs
A systematically processed dataset based on FAERS data, spanning from January 1, 2020, to June 30, 2022, for original research on the safety of Fast-Track COVID-19 drugs.

# Data Source and data colletion period
Our study used real-world data from the FAERS, a database designed for post-marketing safety surveillance. This database accumulates reports of adverse events and medication errors after the release of pharmaceuticals and therapeutic biologics. This FAERS data is publicly accessible via [the FAERS Quarterly Data Extract (QDE) releases](https://fis.fda.gov/extensions/FPD-QDE-FAERS/FPD-QDE-FAERS.html). 
Given the COVID-19 pandemic's start in December 2019, our research specifically focused on the FAERS QDE releases from January 1, 2020, to June 30, 2022, focusing on fast-track approved COVID-19 drug.

For further details and our analytical findings, please refer to our publication.

+ Link to main article:
[to be updated here]

+ Citation information
[to be updated here]

# Before using these datasets, please review the common recommendations and cautions provided by FAERS. Additionally, refer to our main article (linked above) and read the "Discussion" section for a comprehensive understanding of the limitations.

## Contents
1. [**Merged and Deduplicated Dataset**](https://www.dropbox.com/s/bf4kq575llnn1zy/1_merged_and_deduplicated_dataset.csv?dl=0) 
   - Observation Period: January 1, 2020, to June 30, 2022
   - Total Cases: 5,248,821 (with `caseid`)
   - Data Fields: `caseid`, `age_year`, `sex`, `event_dt`, `reporter_country`, `prod_ai`, `pt`
   - Source: This dataset results from joining the 'DEMO', 'DRUG', and 'REAC' tables originally found in the FAERS dataset.

2. [**Contingency Table**](https://www.dropbox.com/scl/fi/y0fiewfy8ulr07zxh3j51/2_contigence-table_4_drugs.xlsx?rlkey=5v39s3d890q9z13guaeljs334&dl=0)
   
- Derived from the first dataset for disproportionality analysis

|                            | Reports with the suspected adverse effect | Reports without the suspected adverse effect |
|----------------------------|:----------------------------------------:|:-------------------------------------------:|
| Reports with the suspected drug   |                   a                    |                    b                        |
| Reports without the suspected drug |                   c                    |                    d                        |

3. [**Modified Dataset for Serious Outcome Analysis**](https://www.dropbox.com/scl/fi/oidf2kku5k4xb64iqe63g/3_modified_dataset_for_serious_outcome_analysis.csv?rlkey=pz4bbexpt3oryo1qfwm5wsgds&dl=0)  
   - File name: `FAERS_outcome.csv`


4. [**Datasets for Subgroup Analyses within cases filtered by Covid19 indication**](https://www.dropbox.com/scl/fi/zw7aphdq3bvquz7crz9r7/4_subgroup_with_COVID19_INDICATION.xlsx?rlkey=sxz6hrcvzo4bycfdqtl2og11i&dl=0) 
   - Focus: Cases filtered by COVID-19 indication.


## Authors
* Hyo Jung Kim†
* Jeong-Hwa Yoon†
* Kyehwa Lee (Corresponding)
†These authors contributed equally to this work

## License
This project is licensed under the terms of GNU GENERAL PUBLIC LICENSE(Version 3) by authors. 
See the [LICENSE.md](https://github.com/HyojungKim/FAERS_Data_for_Investigating-the-Safety-of-Fast-Track-COVID-19-Drugs/blob/master/LICENSE.md) file for details.

