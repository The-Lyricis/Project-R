# Unity development workflow

## Before changing the project

1. Read the repository AGENTS.md and this workflow.
2. Check git status and inspect the relevant scenes, scripts, packages, and settings.
3. Confirm the Editor version in ProjectSettings/ProjectVersion.txt and the package version in Packages/manifest.json.
4. State the behavior or structure being changed and how it will be verified. Ask for clarification only when an undecided product choice blocks the task.

## Implementation

- Prefer the existing architecture and package set. Add dependencies only when the task needs them.
- Keep prototypes isolated and easy to remove. Mark experimental code and assets clearly.
- Use the Unity Editor or Unity CLI for scene and asset operations when practical.
- Preserve .meta files and GUIDs. Move Unity assets together with their metadata.
- Keep generated project files and caches out of source changes.
- Avoid broad project setting changes unless required. Record accepted changes to baseline settings in the charter or a decision record.

## Verification

- Match verification to the change. Examples include script compilation, focused Edit Mode or Play Mode tests, scene inspection, asset reference checks, and a target build.
- Use the project Editor version. When several Editors are open, explicitly select the Project R path in Unity CLI commands.
- Capture actual results. Mark skipped checks as not run, and do not treat a successful compile as proof of visual or gameplay quality.
- For visual changes, include a screenshot or a concise Editor review note when available.

## Handoff

Summarize the changed behavior, files, verification results, and remaining user decisions. For prototypes, state what was varied, what stayed fixed, and how to reproduce the comparison.
