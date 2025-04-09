# 10000-interpretations-and-decisions
10000 Stratigraphy Interpretations and Directional Drilling Decisions from the Geosteering World Cup 2021


## 📄 Summary

This dataset contains resistivity logging measurements collected from horizontal wells drilled in the North Sea. The data was curated to support machine learning models for real-time geosteering decisions. It includes raw and preprocessed logs, synthetic modeling outputs, and metadata aligned with the subsurface stratigraphic framework.

## 📌 Metadata

- **Title**: Subsurface Resistivity Measurements for Geosteering
- **Version**: 1.0
- **Creators**:  
  - Sergey Alyaev (NORCE) — [ORCID: 0000-0002-XXXX-XXXX]  
  - Jane Smith (Equinor)
- **Date of Deposition**: 2025-04-09
- **Contact**: Sergey Alyaev — cobxo3bot@gmail.com
- **License**: [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **DOI**: [10.5281/zenodo.XXXXXXX](https://doi.org/10.5281/zenodo.XXXXXXX)

## 🏗️ Directory Structure
```
/dataset/ 
├── raw/ │ 
└── resistivity_logs_raw.csv 
├── processed/ 
│ ├── resistivity_logs_cleaned.csv 
│ └── model_ready_data.h5 
├── synthetic/ 
│ └── forward_model_output.json ├── metadata/ 
│ └── well_metadata.json 
└── README.md
```

- **`raw/`**: Original field measurements without preprocessing.
- **`processed/`**: Cleaned logs aligned by depth and ready for ML input.
- **`synthetic/`**: Synthetic tool responses generated using 2D modeling.
- **`metadata/`**: Well headers, coordinates, formation tops, and sensor specs.

## 🔍 Data Collection & Processing

- Measurements were obtained using LWD tools between 2019–2022.
- Preprocessing steps included:
  - Depth alignment
  - Removal of noisy and invalid entries
  - Normalization and smoothing
- Synthetic logs were generated using a 2-layer 2D EM simulator developed in-house (details in accompanying publication).

## 🔗 Standards and Vocabularies

- **Coordinate System**: UTM Zone 32N
- **Units**: Resistivity in ohm-meters, depth in meters
- **Format Standards**:
  - CSV (comma-separated values) for tabular data
  - JSON for metadata and synthetic output
  - HDF5 for processed arrays (compatible with Python/Pandas)

## ⚙️ Usage Instructions

1. Clone or download the dataset.
2. Install Python 3.9 with `pandas`, `numpy`, and `h5py` libraries.
3. Use the following snippet to load the cleaned data:


**Which scripts do we need to add???**
