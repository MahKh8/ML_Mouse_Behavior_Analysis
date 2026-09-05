# Mouse Social Behavior Classification (CalMS21)

Classifying mouse social behaviors (attack, investigation, mount, other) from tracked body-part keypoints, using the [CalMS21](https://data.caltech.edu/records/1991) dataset from the Multi-Agent Behavior Challenge.

## Data

- CalMS21 Task 1 (classic classification), hosted by Caltech
- Each sequence: keypoints for 2 mice (nose, ears, neck, hips, tail base) across frames, with per-frame behavior annotations
- Download/conversion handled by the notebook (`calms21_convert_to_npy.py`)

## Contents

- Data loading, exploratory analysis, and behavior distribution stats
- Visualization: pose trajectories, distance/velocity between mice, animated pose sequences, behavior raster plots
- Stratified train/validation split
- Exploratory clustering (ICA + Gaussian Mixture) and an SVM classifier on the annotated behaviors

## Run

Open the notebook and run top to bottom; the data download/conversion cells handle setup.
