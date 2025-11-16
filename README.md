polymer-ut-gnn-baseline-lite
This repository is a minimal UT x ML baseline designed to show capability in handling 3D ultrasound-like inspection volumes, extracting graph-style features, and reporting simple baseline metrics
(MAE/ r / CV). It is intentionally lightweight for clarity and reproducibility.

Purpose
A compact "evidence-ready" pipeline for research proposals.
The goal is to demonstrate:
* ability to preprocess 3D UT-like volumetric data
* graph-style feature extraction from spatial grids
* simple baseline modeling and evaluation
* reproducibility with only Python + Numpy
  This structure can be naturally extended to full GNN models or 3D-UNet pipelines after joining a laboratory.

How to Run
Verify NumPy:
python -c "import numpy; print('numpy OK')"
Run the baseline:
python run_baseline.py --seed 0 --grid 28 --noise 0.10
This generates a small synthestic 3D volume, extracts graph-like features,trains a linear baseline model, and prints MAE / r /5-fold CV metrics.

Why
  연구계획서의 Evidence Box를 위한 최소 재현 파이프라인
  입실 후 GNN/3D-UNet으로 교체 가능한 구조

How to run
```bash
python -c "import numpy; print('numpy OK')"
python run_baseline.py --seed 0 --grid 28 --noise 0.10
