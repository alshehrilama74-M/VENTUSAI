# SCADA data

## Available here

- [features_final.csv](features_final.csv) — exact list of 48 selected SCADA input features.

## Not uploaded to this public repository

- SCADA monitoring raw workbook (~181 MB; GitHub regular-file limit is 100 MB)
- SCADA_Train_All.xlsx (~75 MB)
- SCADA_07_Validation.xlsx (~15 MB)
- SCADA_08_Test.xlsx (~15 MB)
- SCADA_Group_Split_Assignment.csv (complete group split manifest; required for preprocessing)
- cleaned SCADA and processed event logs

Source for the **raw** SCADA/event records: https://zenodo.org/records/14546480

The **processed** files above were prepared by the project team. They are not necessarily available from Zenodo; provide these separately via an accessible institutional storage link or approved file-sharing method.

To reproduce the reported results, use the matching processed train/validation/test partitions and the feature list here. The dashboard's sensor scenarios are illustrative only, not live model inference.
