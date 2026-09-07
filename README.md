# Medicinal-plant reliability evaluation — v1.0.0

Code and frozen-output companion for **Beyond Internal Accuracy: Cross-Source Generalization and Open-Set Reliability in Medicinal-Plant Image Classification**.

Repository: https://github.com/mzw423502/medplant-reliability-evaluation

## Version and citation

This is the v1.0.0 software/source-and-output companion, released on 2026-09-07. Use the tagged release archive `medplant-reliability-evaluation-v1.0.0.zip`, not the earlier candidate ZIP. Citation metadata are supplied in `CITATION.cff`.

- **Version-specific DOI:** https://doi.org/10.5281/zenodo.22640948
- **Fixed release:** https://github.com/mzw423502/medplant-reliability-evaluation/releases/tag/v1.0.0
- **Archived source commit:** `2d728e3f50882e8d33ddf0b561be67abb2d7139e`
- All-versions DOI: https://doi.org/10.5281/zenodo.22640947 (resolves to the latest version; cite the version-specific DOI above for this release).

Zenodo preserves a GitHub repository snapshot. Within that snapshot, extract `medplant-reliability-evaluation-v1.0.0.zip` to obtain the code companion. The inner ZIP is identical to the GitHub release asset (SHA-256 `72cf681920a6c7dd3e725e3ac1d5283454bd72713ba0eae1729e9865ecfa3547`). The outer Zenodo snapshot has a different checksum by design.

The DOI links were added to the default-branch documentation after successful archiving; the v1.0.0 tag and release ZIP have not been changed.

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
