# Data inputs and reproducibility

## Dataset

Original SCADA and event log dataset: https://zenodo.org/records/14546480

The project uses historical observations from 10 turbines, including 262,080 original SCADA readings and 260,367 after removal of missing-flagged records.

## Final model notebook inputs

The trained model evaluation expects these prepared files in its working directory:

- `SCADA_Train_All.xlsx`
- `SCADA_07_Validation.xlsx`
- `SCADA_08_Test.xlsx`
- `features_final.csv`

These must be the **same approved final prepared partitions** used for the reported results.

## Data preparation inputs

Raw SCADA workbook, original/processed event logs, prepared cleaned SCADA and, where required, `SCADA_Group_Split_Assignment.csv`. Some cells use environment-specific paths; adapt these for your environment.

**Important:** The original data-preparation workflow handled six fault categories. The final chosen supervised classification workflow covers only three (Lubrication, Electrical and Generator_Cooling), and the full raw-to-final partition regeneration has not been independently verified in a clean environment.

Large raw and processed Excel datasets are intentionally not committed here. For course submission, attach them or provide accessible download links to the instructor.

No sensitive credentials or operational infrastructure data should be published.
