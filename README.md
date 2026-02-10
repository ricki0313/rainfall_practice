# Cleaning and Analysis of Special Codes in Automatic Station Rainfall Data

This project uses **Central Weather Administration automatic weather station data from December 2023** to practice handling special rainfall codes (e.g., `-999.6`) and to generate a Taiwan-wide monthly rainfall map for December. The project mainly covers:

1. Exploration, generation mechanism, analysis, and cleaning of the **PP01** field (`1_data_processing_9996`)
2. Construction of the **December accumulated rainfall grid** (`2_rainfall_month`)
3. Mathematical derivation and result reporting (`3_report`)

---

## Dataset and Features
The datasets used in this project are provided by the Central Weather Administration (CWA).  
Due to file size and licensing considerations, raw data and generated feature files are not included in this repository.

To reproduce the features:
1. Download the **CWA automatic station hourly dataset in MH (Multifield Hourly) format**, preprocessed and provided by the author (Raw data provided by the author is not included in this repository due to data security considerations), and place the raw `.txt` file under `data/raw/`.
2. Download the **CWA station metadata in JSON format** and place the raw file under `data/raw/`:
   https://opendata.cwa.gov.tw/dataset/observation/O-A0002-001
3. Run the data processing and visualization notebooks in order.

---

## Execution Order
The notebooks in this project should be executed in the following order:

1. **1_data_processing_9996**
   - `observing_processing.ipynb`

2. **2_rainfall_month**
   - `rainfall_month.ipynb`

The final findings and interpretations are summarized in the report provided in **3_report**.  
All features are generated automatically during the execution process.

---

## Future Improvements (log at 2026/02/10)
1. The training and iteration procedure of the spherical variogram model is still unclear. Further study of its mathematical principles is needed to understand parameter tuning.
2. The model evaluation methodology has not been established. Additional domain knowledge is required to determine appropriate criteria for assessing model performance.
3. After visualization, the results can be overlaid on a map of Taiwan to improve spatial interpretability.