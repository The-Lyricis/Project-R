# Shader and URP experiments

## Goal

Explore rendering options for low-poly 3D, including optional 3D pixelation and stable presentation under camera movement. No pixel resolution, camera model, render feature, or final look is locked.

## Experiment setup

- Keep each experiment isolated in a clearly named scene, folder, renderer feature, or branch.
- Start with a reproducible baseline scene and record the Unity version, URP asset, renderer, resolution, camera settings, and relevant quality settings.
- Change one important variable at a time where practical. Keep a control capture for comparison.
- Avoid modifying the primary renderer or default project assets until a direction is accepted.
- For custom URP renderer features, use the supported Unity 6 Render Graph path and validate resource lifetime, pass inputs, and material bindings.
- Record package dependencies and ensure the experiment does not silently change project-wide rendering settings.

## Pixel and stability review

Compare representative static and moving views. Include diagonal and slow camera motion, depth changes, thin geometry, high-contrast edges, and moving objects against a stable background.

Record:

- Output resolution and render scale.
- Camera projection, movement, and update timing.
- Pixel grid or quantization settings.
- Temporal effects, anti-aliasing, and post-processing state.
- Screenshots or short captures at matching conditions.
- Visible shimmer, crawling edges, uneven pixel density, aliasing, motion artifacts, and performance observations.

## Experiment record

Use a short Markdown note beside the prototype or under docs/experiments/. Include the question, setup, changed variable, captures, observations, limitations, and conclusion. Label conclusions as observations or proposals until reviewed.

## Promotion

Before adopting an experiment, review it in the active project scene and relevant resolutions, verify the target platform once selected, and document accepted settings in a decision record. Remove prototype-only code only after checking scene and asset references.
