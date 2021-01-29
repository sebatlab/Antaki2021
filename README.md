# Antaki2021

### A phenotypic spectrum of autism is attributable to the combined effects of rare variants, polygenic risk and sex

-------------

## Table of Contents
* [Full Genetic Table](#full-genetic-table)


-------

### Full Genetic Table

[`antaki2021_full_genetic_table.tsv`](https://github.com/sebatlab/Antaki2021/blob/main/antaki2021_full_genetic_table.tsv)

**Header**

* fid
  * Family ID
* iid
  * Individual ID
* phen
  * Phenotype: 1 = ASD; 0 = Control
* sex
  * Sex: 0 = Male; 1 =  Female
* is_eur
  * European Ancestry: 1 = False; 1 = True
* snv_dn_lof
  * Count of de novo loss of function SNV/INDEL 
* snv_dn_mis
  * Count of de novo missense SNV
* snv_lof_t
  * Count of inherited rare variants
* snv_lof_pt
  * Count of paternally transmitted rare variants
* snv_lof_pn
  * Count of paternally nontransmitted rare variants 
* snv_lof_mt
  * Count of maternally transmitted rare variants
* snv_lof_mn
  * Count of maternally nontransmitted rare variants
* prs_asd
  * Autism polygenic risk score (PS) for the offspring 
* prs_asd_pat
  * Autism PS for the father
* prs_asd_mat
  * Autism PS for the mother
* midparent_prs_asd
  * Defined as (`prs_asd_pat`+`prs_asd_mat`)/2
* ptdt_prs_asd
  * Defined as `prs_asd` - `midparent_prs_asd` 
* prs_ea
  * Educational attainment PS for the offspring
* prs_ea_pat
  * Educational attainment PS for the father
* prs_ea_mat
  * Educational attainment PS for the mother
* midparent_prs_ea
  * Defined as (`prs_ea_pat`+`prs_ea_mat`)/2
* ptdt_prs_ea
  * Defined as `prs_ea` - `midparent_ea_asd` 
* prs_scz
  * Schizophrenia PS for the offspring
* prs_scz_pat
  * Schizophrenia PS for the father
* prs_scz_mat
  * Schizophrenia PS for the mother
* midparent_prs_scz
  * Defined as (`prs_scz_pat`+`prs_scz_mat`)/2
* ptdt_prs_scz
  * Defined as `prs_scz` - `midparent_scz_asd` 
* PC1 .. PC10
  * First ten ancestry principal components
* all_combined_score
  * Normalized estimates from multivariate regression combining de novo, inherited rare, and common variants
* ps_combined_score
  * Normalized estimates from multivariate regression combining polygenic risk for autism, educational attainment, and schizophrenia
* rare_combined_score
  * normalized estimates from multivariate regression combining de novo and inherited rare variants 

---------------
