# Alzheimer's EEG Analysis

This project analyzes EEG data from patients with Alzheimer's disease, Frontotemporal Dementia, and healthy controls.

## Dataset

We use the "A Dataset of Scalp EEG Recordings of Alzheimer's Disease, Frontotemporal Dementia and Healthy Subjects from Routine EEG" from OpenNeuro (ds004504).

Dataset includes:
- 36 Alzheimer's disease patients
- 23 Frontotemporal Dementia patients
- 29 healthy controls

## Methods

We perform power spectral analysis to compare the power in alpha and gamma bands between the different groups.

## Reproduction

1. Clone this repository
2. Download the dataset from OpenNeuro: https://openneuro.org/datasets/ds004504
3. Place the dataset in a `data/ds004504` directory
4. Run the notebook
## Dataset Setup

1. Clone this repository
2. Create a data directory: `mkdir -p data`
3. Download the dataset:
   - Option 1: Using DataLad (requires git-annex and datalad installed)
     ```
     cd data
     datalad install https://github.com/OpenNeuroDatasets/ds004504.git
     cd ds004504
     git annex get derivatives/sub-001/eeg/sub-001_task-eyesclosed_eeg.set
     git annex get participants.tsv participants.json
     ```
   - Option 2: Download from [OpenNeuro](https://openneuro.org/datasets/ds004504)
4. Ensure the dataset is in the `data/ds004504` directory for the code to work
