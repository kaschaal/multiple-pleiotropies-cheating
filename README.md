README for data associated with “Antagonistic, synergistic, and social pleiotropy in microbial cheaters”

## Overview
This project investigates the effect of the level of nutrient availability on subsequent proficiency of sporulation in a cooperatively sporulating soil bacterium. It comprises two experiments. The raw data from these experiments may be found in:
data_pleiotropy.csv
Data were collected by Pauline Manhes.

Data are analyzed in R, by the file rmd_pleiotropy.Rmd. These produce the data figures shown in the paper.

The analysis is documented in the file doc_pleiotropy.html.

## Notes on data files
### data_pleiotropy.csv

In this experiment, strains defective at pure-culture sporulation were allowed to sporulate either in pure culture or in 1:9 mixture with a proficient strain, and then the spores were tested for stress resistance with temperature stress and pH stress. There are 6 replicates - replicate numbers go from 4 to 9. Not all replicates are used: the method used for replicate 9 was not fully correct.

DK4324 is not included in replicate 6. There are no DK4324 or DK5208 controls for replicates 8 or 9 (only technical controls).

In some cases, 0 spores were counted. For summarizing and analyzing numbers of spores produced, we chose to consider these as 0 spores produced. For summarizing and analyzing stress tolerance and relative fitness (metrics calculated based on numbers of spores produced), we chose to consider these as the maximum undetectable number of spores, ie 0.9 spores at the indicated dilution, unless in this case there were 0 spores counted from the cheater in mixture AND 0 spores counted from the cooperator in mixture - comparing 0 to 0 with uncertainty in what was the real number of spores produced is not biologically meaningful.

For several observations, dilution factor is not a multiple of 10:
- Replicate 5, 50 degrees, DK5208 (800 ul)
- Replicate 6, 50 degrees, DK5208 (900 ul)
- Replicate 7, 50 degrees, DK5208 (900 ul)
- Replicate 9, 58 degrees, GJV2:DK4324, no antibiotic (200 ul)
- Replicate 9, 58 degrees, GJV2:DK4324, kanamycin (500 ul)
- Replicate 9, 55 degrees, GJV2:DK4324, kanamycin (500 ul)

Strains:
- GJV1
- GJV2
- DK4324 (also called the asgB strain)
- DK5208 (also called the csgA strain)
