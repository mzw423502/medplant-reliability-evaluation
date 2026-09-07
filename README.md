# Medicinal-plant reliability evaluation — v1.0.0

Code and frozen-output companion for **Beyond Internal Accuracy: Cross-Source Generalization and Open-Set Reliability in Medicinal-Plant Image Classification**.

Repository: https://github.com/mzw423502/medplant-reliability-evaluation

## Version and citation

This is the v1.0.0 software/source-and-output companion, prepared on 2026-09-07. Use the tagged release archive `medplant-reliability-evaluation-v1.0.0.zip`, not the earlier candidate ZIP. Citation metadata are supplied in `CITATION.cff`. An archival DOI is not asserted in these files until an external record has actually been published.

## Contents

- Source code for provenance/duplicate audits, group/split construction, evaluation, statistics and historical figure generation.
- Formal ResNet-50 / ViT-B/16 training source and frozen baseline/strong-augmentation configurations.
- Frozen baseline predictions and run/environment reports; supplementary tables including the mitigation extension.
- The strong-augmentation open-set implementation under its original relative directory.

## Safe verification

Extract the release ZIP into a new directory. From its top-level folder run:

```console
python verify_package.py
```

This verifies packaged file hashes and parses Python syntax using the standard library. It does not import or execute the scientific scripts, train a model, download images, run inference, select thresholds or change any scientific result. See `DEPENDENCIES.json` for statically detected imports and `environment/` for original training-host records.

## Reproduction scope

The archive supports source inspection and offline inspection of existing frozen outputs. Some historical scripts expect input manifests, score files, image data and directories from the full research project which are not all included at their original paths. It is not a one-command reconstruction of the complete training/evaluation pipeline. Do not execute all scripts in bulk: some construct splits or launch training. The original environment records are provenance, not a tested installation lock for a new machine.

`scripts/run_formal_end_to_end.py` is the ResNet-50 / ViT-B/16 primary implementation. `scripts/run_formal_frozen_feature_baseline.py` is a historical ResNet-18 auxiliary baseline, not the primary experiment. Historical plotting scripts do not certify pixel-exact regeneration of every assembled final figure.

Available recovered checkpoints do not consistently reproduce all formal frozen predictions and are excluded. This release adds no new inference, matched-source experiment or scientific result.

## Licence and data access

Original software is released under MIT; see `LICENSE` and `NOTICE.md` for scope. Third-party data are not relicensed. Original image pixels, checkpoints, private manuscript files, credentials and caches are excluded. Self-collected images remain available on reasonable request to the corresponding author.
