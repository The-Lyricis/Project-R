# Project R agent instructions

## Read first

- Read docs/project/PROJECT_CHARTER.md for confirmed project direction and decision rules.
- Read the relevant workflow in docs/workflows/ before changing Unity code, art assets, rendering, tests, or Git state.
- Treat repository files as the source of truth. Chat history and generated suggestions do not establish project requirements.

## Project constraints

- Target Unity 6000.3.28f1 and the package versions recorded in Packages/manifest.json and Packages/packages-lock.json.
- The project uses URP. Check the active renderer and project settings before changing rendering behavior.
- Low-poly 3D is the current art direction. 3D pixelation and rendering stability are experiments, not locked visual requirements.
- Gameplay is undecided. Do not add mechanics, genres, narrative, or player goals without an explicit decision recorded in project documentation.
- Preserve Unity .meta files and GUIDs. Move or rename Unity assets together with their .meta files.

## Working agreements

- Keep changes scoped to the requested outcome. Prefer small, reviewable changes.
- Inspect the working tree before editing. Preserve user changes and report unrelated pre-existing modifications.
- Prefer the installed Unity CLI and the already-open Editor for Unity operations. Pin commands to F:/Project/Project R when multiple Editors may be open.
- Do not edit generated folders such as Library/, Temp/, Logs/, or generated solution files as project sources.
- Keep durable decisions and handoff information in the repository. Label proposals and experiments as such until accepted.
- Do not commit or push unless the user asks. Never include credentials, local machine settings, or generated caches in Git.

## Completion notes

At handoff, summarize the files changed, validation performed and its result, any checks not run, and decisions still needed from the user.
