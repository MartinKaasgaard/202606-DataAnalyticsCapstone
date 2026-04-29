# <Capstone>

Short one-paragraph purpose statement: what problem is being solved, what data is used, and what the main outputs are (models, reports, figures).

## Quick Start

**Run in Colab**
1. Open `notebooks/Y2-Capstone.ipynb`.
2. Run the bootstrap cell to mount Google Drive and set paths.
3. Update `configs/local.yaml` if needed (paths, hparams).

**Run locally**
```bash
python -m venv .venv && source .venv/bin/activate
pip install -r deps/requirements.txt -c deps/constraints.txt
export PROJECT_DRIVE="<abs path to project root>"
jupyter lab

---

# Wind Turbine Maintenance Triage Capstone

This repository contains the code, notebooks, documentation, and interim-report assets for a data analytics capstone project on explainable machine learning for wind-turbine maintenance triage using public SCADA data.

## Data policy

The `/data` directory structure is included for reproducibility, but all data files are excluded from version control.

Expected local structure:

data/
├── external/
├── interim/
└── processed/

Raw and processed data should be recreated by running the notebook pipeline.

## Current status

The current workflow includes:

1. Dataset download and decompression.
2. JSON inspection and schema audit.
3. JSON-to-Parquet conversion.
4. Duplicate timestamp resolution.
5. Timestamp gap audit.
6. Chronological train/validation/test split with embargo.
7. Strict alarm-label source discovery.
8. Proxy operational label construction.
9. Visual EDA.
10. Preliminary proxy-label modelling.

## Methodological note

The current label strategy uses proxy operational labels derived from train-fitted power-curve behaviour. These labels are not verified alarm-event labels.
