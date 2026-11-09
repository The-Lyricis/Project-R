# Project development charter

## Purpose

Project R is an early-stage Unity game project. The immediate goal is to establish a reliable, reviewable foundation that supports exploration of the game and its presentation.

## Confirmed baseline

- Engine: Unity 6000.3.28f1 (Unity 6.3 LTS).
- Rendering: Universal Render Pipeline, currently 17.3.0.
- Visual direction: low-poly 3D.
- 3D pixelation, camera behavior, and pixel stability are open rendering experiments.
- Genre, core loop, mechanics, story, target platform, and final art style are undecided.

The confirmed items above are project constraints. Everything described as open or experimental remains a proposal until the user accepts it and it is recorded here.

## Near-term priorities

1. Keep the project opening and importing cleanly in its pinned Editor version.
2. Preserve source assets, scene references, stable Unity GUIDs, and version history.
3. Build small, disposable prototypes to compare rendering and presentation options.
4. Record observed results and the conditions needed to reproduce them.
5. Decide game direction from prototypes and user review, rather than from assumptions embedded in scaffolding.

## Agent collaboration model

Agents work from repository instructions and task-specific evidence. A task should identify its intended result, affected areas, and how completion can be checked. For work spanning multiple areas, split work by clear file or system ownership and integrate through review.

Agents may inspect, explain, propose, and make reversible in-scope changes. Changes that establish product direction, add a gameplay system, remove source assets, alter broad project settings, or replace a rendering baseline require explicit user direction. Record accepted decisions in this charter or a focused decision record.

## Decision records

Use a short Markdown record under docs/decisions/ when an architectural or visual choice affects future work. Include status (proposed, accepted, superseded, or rejected), context and options, decision and reason, follow-up work, and date.

Do not create a decision record for routine implementation details.

## Definition of ready

A task is ready when its intended outcome is understandable, affected project areas are identified, and important product choices are either already recorded or explicitly left open.

## Definition of done

A task is done when the change is scoped, Unity references are preserved, relevant verification has a recorded result, documentation reflects accepted decisions, and the handoff identifies any remaining manual review.
