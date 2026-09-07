# Medicinal-plant reliability evaluation

Code and frozen-output companion for **Beyond Internal Accuracy: Cross-Source Generalization and Open-Set Reliability in Medicinal-Plant Image Classification**.

## Current status

Private staging repository for the Paper 002 code-release candidate. This repository is not yet a public archival release, has no DOI, and must not be cited as publicly accessible code until the publication step is complete.

## Download and inspect

Download `Paper002_Code_Release_Candidate.zip` and extract it into a new folder. The archive contains auditing, group/split, evaluation and statistical scripts, historical plotting source, formal training source and configurations, baseline frozen predictions and environment reports, and supplementary result tables including the strong-augmentation extension.

The ZIP SHA-256 is:

`daa5cff91fb7928b76e964eda4b538bd67d13b23e545ceb65a26fac50544d307`

From the extracted folder, run:

```console
python verify_package.py
```

This checks the packaged file hashes and Python syntax only. It does not execute the scientific scripts or train a model. Read the included README and dependency record before using the source files.

## Scope and access

The compact companion supports code inspection and inspection of existing frozen outputs. Some historical scripts require inputs and directory layouts from the full research project; this is not a tested one-command reconstruction of all experiments. Trained checkpoints, original image pixels, private manuscript files and caches are excluded. Self-collected images remain available on reasonable request to the corresponding author, independently of code access.

The package preserves the distinction between primary ResNet-50 / ViT-B/16 experiments and the historical ResNet-18 feature baseline. No new experiment results are introduced by this upload.

## Release preparation

A software licence and archival release metadata are still to be finalized before public distribution. No blanket software licence is granted over third-party datasets or bundled derived data. The archived candidate's README records the state at package assembly; this repository README records the subsequent private-upload stage.
