# Testing, acceptance, and Git workflow

## Verification levels

Choose checks based on the change:

- Documentation-only changes: inspect links, paths, and consistency with the repository.
- C# changes: compile in the pinned Editor and run focused Edit Mode or Play Mode tests where available.
- Scene or asset changes: open the affected scene, check references and import results, and review the relevant view.
- Rendering changes: compare captures under the experiment conditions in SHADER_URP_EXPERIMENTS.md.
- Release-facing changes: build the intended target and record platform and build result. The target remains undecided until selected.

Record commands or Editor actions, Unity version, result, and any checks not run. Human visual, usability, and gameplay acceptance should be identified separately from automated checks.

## Acceptance

An acceptance note should name the expected result, setup, reproduction steps, observed result, and reviewer decision. A prototype can be technically complete while awaiting a user decision on visual direction or game feel.

## Git

- Check git status before and after work. Preserve work already present in the tree.
- Commit source assets, .meta files, scenes, settings, package manifests and lock files, and project documentation when they belong to the change.
- Keep Library/, Temp/, Logs/, UserSettings/, generated IDE files, local credentials, and machine-specific settings out of commits. Follow the root .gitignore.
- Review staged paths and diff before committing. Unity .meta files must accompany added, moved, or renamed assets.
- Use a short commit message describing the change. Avoid mixing unrelated work.
- Push only when requested. Before pushing, verify the intended branch, remote, and commit range.
- Use Git LFS only when large binary assets make regular Git unsuitable. Agree on patterns before adding tracking rules so existing history and collaborators remain consistent.

## Completion note

Report the commit only if one was created. State verification results accurately and list any remaining manual acceptance or product decisions.
