# Core Control Model

This framework employs a three-layer model to operationalize AI-assisted software development, ensuring clarity, consistency, and control over the development process.

## Layer 1 — Framework Self-Governance
Protects:
*   Framework doctrine
*   Routing rules (`docs/routing.md`)
*   Protected paths (`framework/rules/protected-files.md`)
*   Planning synchronization (`framework/rules/planning-sync.md`)
*   Execution boundaries (`framework/rules/execution-boundaries.md`)

## Layer 2 — Single-Project Control
Governs:
*   `project/` directory
*   `project/vision/` (core doctrine, constraints, brainstorming)
*   `project/docs/` (features, task groups, tasks, priorities, roadmap, decisions, definition_of_done, execution_control)
*   `project/now/` (active work state)
*   `project/evidence/` (execution outcomes)

## Layer 3 — Execution Guidance
Guides external tools by:
*   Defining what to read (`docs/routing.md`)
*   Defining what may be changed (`project/now/metadata.json`'s `allowed_paths`)
*   Defining what must not be changed (`project/now/metadata.json`'s `forbidden_paths`)
*   Using `project/now/prompt.md` as the definitive handoff source.

This model ensures repository truth remains stable and AI tools work against a controlled, consistent state.