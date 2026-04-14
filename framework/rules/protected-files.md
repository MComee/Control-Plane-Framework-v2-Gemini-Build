# File Protection Rules

This document defines classifications for files within the repository to govern their mutability during different phases of the development workflow. Adherence to these rules is critical for maintaining the integrity of project intent and execution alignment.

## Protected Files

These files represent the core, unchangeable doctrine and definitions of the project and framework. They should **never** be modified by execution tools. Changes to these files must only occur through explicit planning and synchronization processes.

*   `project/vision/core_vision.md`
*   `project/vision/constraints.md`
*   `project/docs/features/*` (Individual feature definition files)
*   `project/docs/task_groups/*` (Individual task group definition files)
*   `project/docs/priorities/*` (Files defining `now`, `next`, `later`, `blocked`, `done`)

## Restricted Files

These files are generally stable but may be updated during explicit planning or tracking activities. Execution tools should generally avoid modifying them, but they are less strictly protected than "Protected" files.

*   `project/docs/tasks/*` (Individual atomic task definition files)

## Allowed for Normal Execution

These files are mutable and are the primary targets for code implementation and evidence recording. Execution tools are generally permitted to modify these files as part of their assigned tasks.

*   `project/app/*` (All files within the application directory)
*   `project/evidence/` (All files within the evidence directory, used for recording results)

## Policy Statement

*   **Execution tools must not modify protected files.** Doing so is a critical failure and invalidates the trustworthiness of any execution result.
*   **Restricted files should only change when explicitly part of planning, tracking, or approved control updates.** Changes should be deliberate and synchronized with the planning process.
*   **Allowed files** are the primary targets for implementation and evidence, and are subject to modification by execution tools as part of their defined tasks.