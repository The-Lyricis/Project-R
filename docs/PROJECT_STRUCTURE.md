# Repository and Unity folder structure

## Repository root

- AGENTS.md contains instructions for coding agents working in this repository.
- README.md is the project entry point.
- docs/ contains the charter, workflows, records, and reusable templates.
- Assets/, Packages/, and ProjectSettings/ are Unity project source directories.
- Library/, Temp/, Logs/, and UserSettings/ are local or generated Unity data and are ignored by Git.

## Unity assets

Project-owned runtime and production content lives directly under Assets/ by asset category.

- Art/Models/ contains source and imported meshes.
- Art/Textures/ contains textures and texture atlases.
- Audio/ contains sound effects, music, and audio source files.
- Materials/ contains shared materials and material variants.
- Prefabs/ contains reusable GameObjects and prefab variants.
- Scenes/Prototype/ contains early test scenes. Promote scenes only after their purpose is agreed.
- Scripts/Runtime/ contains player-build code.
- Scripts/Editor/ contains editor-only tooling.
- UI/ contains user interface assets.
- VFX/ contains particle systems and visual effects.
- Input/ contains project input action assets and related configuration.

Assets/Settings/ remains the Unity template's project-level render pipeline configuration. Assets/TutorialInfo/ remains Unity template content. Keep their roles distinct from game content. Remove template content only after checking references and confirming it is no longer needed.

Create new category folders when the first real asset for that category is added. Unity folder .meta files keep empty categories in version control.

## Documentation

- project/ contains confirmed direction and project-wide decisions.
- workflows/ contains procedures that contributors repeat.
- decisions/ contains short records for choices that affect later work.
- experiments/ contains results that should be reproducible.
- assets/ contains asset provenance notes and the register.
- templates/ contains blank record formats.
