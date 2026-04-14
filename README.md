# Control Plane Framework v2

This repository is a repository-native control framework for AI-assisted software development. It governs repository truth and execution alignment, ensuring that AI tools interact predictably and contribute to a stable, controlled project state.

## Core Control Model

This framework operates on a three-layer model to manage AI-assisted development:

### Layer 1 — Framework Self-Governance
This layer protects the framework's integrity and consistency. It defines core doctrine, routing rules, file protection policies, planning synchronization mechanisms, and execution boundaries. Its purpose is to ensure the framework itself remains stable and reusable.

### Layer 2 — Single-Project Control
This layer governs precisely one project under the `project/` directory. It enforces the project's vision, manages decomposition into features, task groups, and tasks, maintains priorities, tracks active work, and collects evidence. This layer ensures all development aligns with the project's defined state.

### Layer 3 — Execution Guidance
This layer guides external tools (like AI assistants or local scripts) by providing context, expected behavior, scoped handoff prompts, and validation criteria. It directs tools on what to read, what they may change, and what they must not change, using `project/now/` as the primary handoff source. Critically, this layer *does not* control AI internals but rather guides their interaction with the repository.

## How AI Tools Should Use This Repository

AI tools interacting with this repository must adhere to these principles:

1.  **Repository Truth First:** Always consult repository files as the definitive source of truth for project state and requirements.
2.  **Phase-Based Routing:** Follow the routing rules defined in `docs/routing.md` based on the operational phase (Planning, Execution Preparation, Execution, Validation).
3.  **Respect Boundaries:** Avoid modifying protected and restricted files as defined in `framework/rules/protected-files.md`. Violations invalidate execution results.
4.  **Clean Handoff:** Consume work instructions exclusively from `project/now/` artifacts (`description.md`, `prompt.md`, `metadata.json`).
5.  **Stable State:** Assume repository truth is stable for the duration of an execution task.

## Workflow

The framework supports a structured workflow:

*   **Planning:** Define and refine project vision, features, decomposition, and priorities. All planning must sync to repository files.
*   **Decomposition:** Break down features into task groups and atomic tasks.
*   **Prioritization:** Manage tasks using `project/docs/priorities/` files.
*   **Active Work Handoff:** Clearly define the single, bounded task to be executed next via `project/now/`.
*   **Execution:** Perform the defined task, adhering strictly to scope.
*   **Evidence Return:** Record execution outcomes and artifacts in `project/evidence/`.

## Repository File Tree

```
.
├── README.md
├── docs
│   ├── control-model.md
│   ├── overview.md
│   ├── routing.md
│   └── start-here.md
├── framework
│   ├── rules
│   │   ├── execution-boundaries.md
│   │   ├── planning-sync.md
│   │   └── protected-files.md
│   └── templates
│       ├── active-work-template.md
│       ├── feature-template.md
│       ├── task-group-template.md
│       └── task-template.md
├── project
│   ├── app
│   │   └── README.md
│   ├── decisions.md
│   ├── definition_of_done.md
│   ├── docs
│   │   ├── features
│   │   │   └── README.md
│   │   ├── task_groups
│   │   │   └── README.md
│   │   ├── priorities
│   │   │   ├── blocked.md
│   │   │   ├── done.md
│   │   │   ├── later.md
│   │   │   ├── next.md
│   │   │   └── now.md
│   │   ├── roadmap.md
│   │   ├── tasks
│   │   │   └── README.md
│   │   └── execution_control.md
│   ├── evidence
│   │   ├── .gitkeep
│   │   └── README.md
│   ├── now
│   │   ├── artifacts
│   │   │   ├── .gitkeep
│   │   │   └── README.md
│   │   ├── description.md
│   │   ├── evidence
│   │   │   └── README.md
│   │   ├── metadata.json
│   │   ├── prompt.md
│   │   └── test_runs
│   │       ├── .gitkeep
│   │       └── README.md
│   └── vision
│       ├── brainstorming.md
│       ├── constraints.md
│       └── core_vision.md
## Style constraints

* keep wording plain, precise, and disciplined
* no sales language
* no emojis
* no references to prior versions
* no references to any specific product
* no unnecessary abstraction jargon
* no extra narrative sections beyond what is useful

## Self-review requirements

Before committing:

1. inspect the actual full file tree
2. ensure docs match the real structure
3. ensure all path references are correct
4. ensure only one priorities location exists
5. ensure only one evidence surface exists
6. ensure `project/now/` is an actual active-work layer
7. ensure the root README contains a fully recursive and exact file tree
8. ensure the repository remains aligned to the boring, one-tool-at-a-time v2 vision

## Commit

Commit with this exact message:

refine v2 structure and enforce full repo visibility

## Final output

At the end, print only:

* files modified
* files created
* summary of structural fixes
* confirmation of commit
* confirmation of push