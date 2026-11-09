# Art assets and AI generation workflow

## Asset principles

- Create low-poly 3D assets that remain readable at the intended camera distance. The final camera and gameplay context are still undecided.
- Keep editable source files when available, alongside exported runtime files when licensing and repository size permit.
- Store Unity assets under Assets/ and retain their .meta files. Use clear folder and file names that identify purpose and status.
- Keep generated drafts and one-off experiments separate from approved production assets.

## AI-assisted generation

For each AI-generated or AI-assisted asset that may enter the project, record enough information to identify and review it. Store a nearby ASSET_PROVENANCE.md for a batch or maintain a project asset register when one is introduced. Record:

- Asset name and repository path.
- Generation or editing tool and model, when known.
- Creation date and the prompt or a concise description of the process.
- Human edits made after generation.
- Source references supplied to the tool and their provenance.
- Applicable tool terms, source licenses, attribution requirements, and any known restrictions.
- Review status and the person responsible for approval.

Do not infer commercial usage rights from an asset being publicly downloadable or AI-generated. Check the applicable terms for the actual source and tool. If rights or attribution are unclear, keep the asset in a clearly marked draft area until reviewed.

## Unity import and review

1. Keep an untouched source copy where the workflow requires it.
2. Import into a clearly named folder and review scale, orientation, pivot, mesh density, normals, materials, textures, and animation.
3. Set import options intentionally and commit meaningful .meta files.
4. Check appearance in the project URP renderer and at representative game-view resolutions.
5. Record provenance and acceptance status before treating the asset as production-ready.

## Review checklist

- Does the asset read clearly at the expected distance and lighting?
- Is polygon density appropriate for the intended low-poly direction?
- Are scale, pivot, orientation, and material assignments correct?
- Are texture and mesh settings reasonable for the current target, which remains undecided?
- Are source, attribution, and usage terms recorded?
- Can the asset be reimported without losing references?
