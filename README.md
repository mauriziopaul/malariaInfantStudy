# Malaria Infant Study

## Summary

This repository includes the data and code necessary for reproducing the analysis in our malaria infant study manuscript.

## Data File Overview

The included data file, `MIS_master_data_sheet_long.csv`, is a 119x30 data frame which has the following column names, where each row represents one individual at either acute infection or 4 weeks post-treatment. A companion file, `MIS_master_data_sheet_wide.csv`, is also included for convenience.

The covariates for each subject are given in the first six columns:

- `Subject_ID` (factor): The unique subject ID.

- `Sample` (factor): The unique subject ID and visit number (1 or 2).

- `age.years` (numeric): The age of each subject, which ranges from <1 year to 70 years.

- `Age` (factor): The age group of each subject, `A` (adult) or `I` (infant).

- `Sex` (factor): The sex of each subject, `F` (female) or `M` (male).

- `Visit` (integer): The visit number, `1` for acute infection (first visit), or `2` for post-treatment (second visit).

The levels of nine analytes are given in the following columns, in pg/ml:

- `GMCSF` (numeric): granulocyte-macrophage colony-stimulating factor

- `IFNg` (numeric): interferon gamma

- `IL10` (numeric): interleukin 10

- `IL12p40` (numeric): interleukin 12 p40

- `IL12p70` (numeric): interleukin 12 p70

- `sCD40L` (numeric): soluble CD40-ligand 

- `IL1b` (numeric): interleukin 1 beta

- `IL6` (numeric): interleukin 6

- `TNFa` (numeric): tumor necrosis factor alpha

Additional phenotypes:

- `Nitrate.570` (numeric): Nitric oxide, given in micromolar.

- `malaria.Ab` (numeric): Absorbance values used to determine `malaria.Ab.result`.

- `malaria.Ab.result` (factor): Three levels of antibody test results: `grey` (uncertain), `neg` (negative), `pos` (positive).

- `CD33.live` (numeric): Percent of live cells that are CD33+.

- `mDC.live` (numeric): Percent of live cells that are myeloid dendritic cells (CD11c+ HLA−DR+).

- `monocytes.live` (numeric): Percent of live cells that are monocytes.

- `inflam.CD163` (numeric): Percent of monocytes that are inflammatory monocytes (CD3- CD20- CD14+ CD16++).

- `patrol.CD163` (numeric): Percent of monocytes that are patrolling monocytes (CD3- CD20- CD14++ CD16+).

- `trad.CD163` (numeric): Percent of monocytes that are traditional monocytes (CD3- CD20- CD14++ CD16-).

- `low.traditional` (numeric): Percent of monocytes that are CD14low.

- `Hb` (numeric): The level of hemoglobin, in grams per decaliter.

- `pfs25` (numeric): Pfs25-expressing gametocytes/ul.

- `pfs16` (integer): Pfs16-expressing gametocytes/ul.

- `pfs230` (integer): Pfs230-expressing gametocytes/ul.

- `parasites` (numeric): Parasites per ul blood.
