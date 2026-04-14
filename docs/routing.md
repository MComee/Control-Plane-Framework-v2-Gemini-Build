# Routing Rules by Phase

This document defines how AI tools should navigate and interact with the repository based on their current operational phase. Adherence to these rules ensures tools access the correct information and respect the framework's control mechanisms.

## Planning

**Read:**
*   `project/vision/*`
*   `project/docs/features/`
*   `project/docs/task_groups/`
*   `project/docs/tasks/`
*   `project/docs/priorities/*`

**Purpose:**
*   Assess project vision and constraints.
*   Refine decomposition into features, task groups, and tasks.
*   Adjust and confirm priorities.
*   Determine if active work (`project/now/`) needs modification.

## Execution Preparation

**Read:**
*   `project/now/description.md`
*   `project/now/prompt.md`
*   `project/now/metadata.json`

**Purpose:**
*   Verify the exact definition of the next step.
*   Confirm scope, including allowed and forbidden targets.
*   Review execution requirements.

## Execution

**May work primarily in:**
*   `project/app/` (implementation)
*   `project/evidence/` (recording results)

**Must not mutate protected planning artifacts unless explicitly authorized:** This includes files in `project/vision/`, `project/docs/features/`, `project/docs/task_groups/`, and `project/docs/priorities/`. Changes must follow `planning-sync.md`.

## Validation

**Check:**
*   Files within `project/evidence/` for completeness and accuracy.
*   Consistency of execution results with `project/now/prompt.md`.
*   Ensure protected boundaries were respected.