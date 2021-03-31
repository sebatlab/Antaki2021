# Antaki2021

### A phenotypic spectrum of autism is attributable to the combined effects of rare variants, polygenic risk and sex

-------------
## Data files
Data files include `SummaryGeneticData_Reach_SSC_SPARK.csv` and `master_phen_4.csv` (which includes clinical phenotype information). These will be deposited into SFARI.

## Analysis code

The analysis code is in a Colab notebook: https://colab.research.google.com/drive/1S6Iqp_ydL2_BJdBHzx8j_tufTtPtOQzh?usp=sharing

## Table of Contents
* [SummaryGeneticData_Reach_SSC_SPARK](#Summary_Genetic_Data_REACH_SSC_SPARK)


-------

### Summary_Genetic_Data_REACH_SSC_SPARK

[`SummaryGeneticData_Reach_SSC_SPARK`]

This table contains the all the genetic features used for rare variant analysis, common variant analysis, and the construction of regression models. 

**Header**

* FID
  * Family ID
* IID
  * Individual ID
* Phenotype
  * Phenotype: 1 = ASD; 0 = Control
* Sex
  * Sex: 0 = Male; 1 =  Female
* Cohort
  * Data collection for a sample. Either REACH, SSC, or SPARK
* Family Type
  * Family structure for a given offspring. Either trio (both parents sequenced), maternal (mother only sequenced), or paternal (father only sequenced)
* Cases in Family
  * Number of affected children in a family. Simplex == 1
* EUR Ancestry
  * European Ancestry: 1 = False; 1 = True

----------

* dnMIS
  * Count of de novo missense SNV
* dnLoF
  * Count of de novo loss of function SNV/INDEL
* dnSV
  * Count of de novo LoF SVs
  
----------


* inhLoF
  * Count of inherited LoF SNV/INDEL

* inhLoF Paternal Transmitted
  * Count of paternally transmitted LoF SNV/INDEL
* inhLoF Paternal Untransmitted
  * Count of paternally nontransmitted LoF SNV/INDEL 
* inhLoF Maternal Transmitted
  * Count of maternally transmitted LoF SNV/INDEL
* inhLoF Maternal Untransmitted
  * Count of maternally nontransmitted LoF SNV/INDEL

* SV LoF Paternal Transmitted
  * Count of paternally transmitted LoF SV
* SV LoF Paternal Untransmitted
  * Count of paternally nontransmitted LoF SV
* SV LoF Maternal Transmitted
  * Count of maternally transmitted LoF SV
* SV LoF Maternal Untransmitted
  * Count of maternally nontransmitted LoF SV

* CRE SV Paternal Transmitted
  * Count of paternally transmitted CRE SV
* CRE SV Paternal Untransmitted
  * Count of paternally nontransmitted CRE SV
* CRE SV Maternal Transmitted
  * Count of maternally transmitted CRE SV
* CRE SV Maternal Untransmitted
  * Count of maternally nontransmitted CRE SV

----------

* PS ASD
  * Autism polygenic risk score (PS) for the offspring 
* PS ASD Father
  * Autism PS for the father
* PS ASD Mother
  * Autism PS for the mother
* Midparent PS ASD
  * Defined as (`prs_asd_pat`+`prs_asd_mat`)/2
* pTDT ASD Dev
  * Defined as `prs_asd` - `midparent_prs_asd` 

* PS SCZ
  * Schizophrenia PS for the offspring
* PS SCZ Father
  * Schizophrenia PS for the father
* PS SCZ Mother
  * Schizophrenia PS for the mother
* Midparent PS SCZ
  * Defined as (`prs_scz_pat`+`prs_scz_mat`)/2
* pTDT SCZ Dev
  * Defined as `prs_scz` - `midparent_scz_asd` 

* PS EA
  * Educational attainment PS for the offspring
* PS EA Father
  * Educational attainment PS for the father
* PS EA Mother
  * Educational attainment PS for the mother
* Midparent PS EA
  * Defined as (`prs_ea_pat`+`prs_ea_mat`)/2
* pTDT EA Dev
  * Defined as `prs_ea` - `midparent_ea_asd` 

---------

* PC1 .. PC10
  * First ten ancestry principal components for the offspring
* PC1 Father .. PC2 Father
  * First two ancestry principal components for the father
* PC1 Mother .. PC2 Mother
  * First two ancestry principal components for the mother

---------------

* RVRS
  * normalized estimates from multivariate regression combining de novo and inherited rare variants 
* PRS
  * Normalized estimates from multivariate regression combining polygenic risk for autism, educational attainment, and schizophrenia
* GRS
  * Normalized estimates from multivariate regression combining de novo, inherited rare, and common variants
---------------
