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
1. **Merged and Deduplicated Dataset** 
   - Observation Period: January 1, 2020, to June 30, 2022
   - Total Cases: 5,248,821 (with `caseid`)
   - Data Fields: `caseid`, `age_year`, `sex`, `event_dt`, `reporter_country`, `prod_ai`, `pt`
   - Source: This dataset results from joining the 'DEMO', 'DRUG', and 'REAC' tables originally found in the FAERS dataset.

2. **Contingency Table**
   - Derived from the first dataset for disproportionality analysis
     
|----------------------------|:----------------------------------------:|:-------------------------------------------:|
|                            | Reports with the suspected adverse effect | Reports without the suspected adverse effect |
|----------------------------|:----------------------------------------:|:-------------------------------------------:|
| Reports with the suspected drug   |                   a                    |                    b                        |
| Reports without the suspected drug |                   c                    |                    d                      |
|----------------------------|:----------------------------------------:|:-------------------------------------------:|

3. **Modified Dataset for Serious Outcome Analysis** 
   - File name: `FAERS_outcome.csv`


4. **Datasets for Subgroup Analyses within cases filtered by Covid19 indication** 
   - Focus: Cases filtered by COVID-19 indication.


## Authors
* Hyo Jung Kim†
* Jeong-Hwa Yoon†
* Kyehwa Lee (Corresponding)
†These authors contributed equally to this work

## License
This project is licensed under the terms of GNU GENERAL PUBLIC LICENSE(Version 3) by authors. 
See the [LICENSE.md](https://github.com/HyojungKim/FAERS_Data_for_Investigating-the-Safety-of-Fast-Track-COVID-19-Drugs/blob/master/LICENSE.md) file for details.

