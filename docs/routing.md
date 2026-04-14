# AI Tool Routing Rules by Phase

This document defines how AI tools should navigate and interact with the repository based on their current operational phase. Adherence to these routing rules ensures that tools access the correct information and respect the framework's control mechanisms.

## Planning

**Read:**
*   `project/vision/core_vision.md`
*   `project/vision/constraints.md`
*   `project/vision/brainstorming.md`
*   `project/docs/features/` (and its files)
*   `project/docs/task_groups/` (and its files)
*   `project/docs/tasks/` (and its files)
*   `project/docs/priorities/` (all files: `now.md`, `next.md`, `later.md`, `blocked.md`, `done.md`)

**Purpose:**
*   Assess the current project vision and constraints.
*   Refine the decomposition of features into task groups and tasks.
*   Adjust and confirm priorities for future work.
*   Determine whether the current active work item (`project/now/`) needs modification or replacement based on new planning insights.

## Execution Preparation

**Read:**
*   `project/now/description.md`
*   `project/now/prompt.md`
*   `project/now/metadata.json`

**Purpose:**
*   Verify the exact definition of the next step to be executed.
*   Confirm the scope of work, including allowed and forbidden targets.
*   Review any specific requirements or parameters for the execution task.

## Execution

**May work primarily in:**
*   `project/app/` (for code implementation)
*   `project/evidence/` (for recording results)

**Must not mutate protected planning artifacts unless explicitly authorized:** This includes files in `project/vision/`, `project/docs/features/`, `project/docs/task_groups/`, and `project/docs/priorities/`. Changes to these files must follow the `planning-sync.md` rules.

## Validation

**Check:**
*   Files within `project/evidence/` for completeness and accuracy.
*   Consistency of execution results with the `project/now/prompt.md` and other active work artifacts.
*   Ensure that protected files (as defined in `framework/rules/protected-files.md`) have not been improperly modified.