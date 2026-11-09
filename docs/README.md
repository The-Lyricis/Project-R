# Project documentation

This documentation records the current project baseline and gives contributors a shared workflow. Update it when an accepted decision changes code, assets, rendering, or verification expectations.

## Start here

1. Read the project development charter in project/PROJECT_CHARTER.md.
2. Read AGENTS.md for repository-wide agent instructions.
3. Choose the workflow relevant to the task.

## Records

- PROJECT_STRUCTURE.md describes the repository and Unity asset layout.
- project/ contains the project charter and accepted direction.
- workflows/ contains repeatable contributor procedures.
- decisions/ stores decisions that affect future work.
- experiments/ stores reproducible technical and visual experiments.
- assets/ stores provenance records and the asset register.
- templates/ contains reusable decision, experiment, and acceptance note templates.

## Workflows

- UNITY_DEVELOPMENT.md covers project inspection, implementation, editor use, and handoff.
- ART_ASSETS.md covers source files, import settings, generated assets, and rights records.
- SHADER_URP_EXPERIMENTS.md covers rendering prototypes and visual stability evaluation.
- TESTING_ACCEPTANCE_GIT.md covers verification, review, and version control.

## Current technical baseline

- Unity Editor: 6000.3.28f1
- Render pipeline: URP 17.3.0
- Unity Pipeline package: com.unity.pipeline 0.10.0-exp.1
- Main project directories: Assets/, Packages/, and ProjectSettings/

Confirm the checked-in project settings and package lock file before relying on this summary. Update this section when the project baseline changes.
