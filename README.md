# Aadhaar Enrolment and Update Analysis

## Overview
This repository contains the analytical notebooks supporting a study on Aadhaar enrolment and update patterns in India.  
The analysis focuses on identifying service demand dynamics, infrastructure stress indicators, and spatial variation across states and districts.

The work aligns with the problem statement:
**“Unlocking Societal Trends in Aadhaar Enrolment and Updates”**, and aims to translate observed patterns into insights relevant for administrative planning and system improvement.

---

## Repository Structure

- **api_data_aadhar_enrolment/**  
  Aadhaar enrolment datasets containing age-wise enrolment counts.

- **api_data_aadhar_demographic/**  
  Aadhaar demographic update datasets.

- **api_data_aadhar_biometric/**  
  Aadhaar biometric update datasets.

- **statesNB.ipynb**  
  State-level analysis notebook examining enrolment volumes, update pressure, update composition, and state-level outliers.

- **districtsNB.ipynb**  
  District-level analysis notebook (focused on Karnataka) analysing localized infrastructure stress using update pressure, biometric infrastructure intensity, and total activity.

- **mapIndia.json**  
  Spatial boundary files used for state-level visualisation.

- **mapKarnataka.json**  
  Spatial boundary files used for district-level visualisation within Karnataka.

---

## Methodology Summary
Key methodological steps include:
- Aggregation of age-wise counts to compute true enrolment and update volumes
- Normalization of state and district names to handle administrative variations
- Use of ratio-based indicators to capture service demand characteristics
- Spatial analysis using choropleth visualisations
- Statistical identification of state-level outliers in update pressure

Redundant metrics were intentionally excluded to maintain analytical clarity and interpretability.

---

## Key Metrics
- **Update Pressure**: Ratio of total updates to enrolments, indicating repeat service demand
- **Biometric Infrastructure Intensity**: Proportion of biometric updates, reflecting hardware-dependent load
- **Total Aadhaar Activity**: Aggregate scale of enrolments and updates

District-level analysis focuses on Karnataka to study localized infrastructure stress patterns.

---

## Reproducibility
The notebooks are designed to run top-to-bottom and reproduce all results and figures referenced in the consolidated PDF submission.

Primary Python libraries used:
- pandas
- geopandas
- rapidfuzz
- matplotlib

---

## Running the Analysis Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/KadakWNL/uidai-datathon.git
   cd uidai-datathon
   ```

2. **Install required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebooks:**
   
   Open the notebooks in Jupyter or VS Code and execute all cells in order:
   - `statesNB.ipynb` — State-level analysis
   - `districtsNB.ipynb` — District-level analysis (Karnataka focus)

   Both notebooks are designed to run top-to-bottom without manual intervention.





---

## Notes
- Earlier commits reflect exploratory development and debugging.
- The current repository state represents the finalized analytical pipeline used for submission.
- Full interpretations and conclusions are presented in the accompanying PDF.
- Use of AI has been done to improvise on phrasing, grammar in the file submitted to make it more understandable.
