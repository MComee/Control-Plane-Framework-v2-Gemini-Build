# Control Plane Framework v2

Repository-native control framework for AI-assisted software development.

Scope statement:
- Governs repository truth and execution alignment.
- Does not govern AI internals.
- One repository instance controls one project under `project/`.

## Core Model

### Layer 1 - Framework Self-Governance
Protects doctrine, routing, protected paths, planning sync, and execution boundaries.

### Layer 2 - Single-Project Control
Governs one project under `project/`, including vision, decomposition, priorities, active work, and evidence.

### Layer 3 - Execution Guidance
Guides one chosen tool at a time through `project/now/`, with explicit allowed and forbidden scope.

## Operating Rules

1. Planning must be synchronized to repository files.
2. Execution must consume `project/now/description.md`, `project/now/prompt.md`, and `project/now/metadata.json`.
3. Validation must confirm protected boundaries were respected.
4. Priorities location is only `project/docs/priorities/`.
5. Evidence surface is only `project/evidence/`.

## Repository Visibility Compliance

The root `README.md` file tree below is a required control artifact.

Requirements:
- It must include every tracked file.
- It must include every tracked subdirectory.
- It must recurse fully.
- It must exactly match repository structure.

If tracked files are added, removed, moved, or renamed, this tree must be updated in the same change set.

## Full Recursive File Tree

```text
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
│   ├── docs
│   │   ├── decisions.md
│   │   ├── definition_of_done.md
│   │   ├── execution_control.md
│   │   ├── features
│   │   │   ├── FEAT-001-repository-truth-control.md
│   │   │   └── README.md
│   │   ├── priorities
│   │   │   ├── blocked.md
│   │   │   ├── done.md
│   │   │   ├── later.md
│   │   │   ├── next.md
│   │   │   └── now.md
│   │   ├── roadmap.md
│   │   ├── task_groups
│   │   │   ├── README.md
│   │   │   └── TG-001-structural-compliance-and-active-work-control.md
│   │   └── tasks
│   │       ├── README.md
│   │       ├── TASK-001-normalize-v2-structure-and-control-locations.md
│   │       ├── TASK-002-enforce-readme-tree-and-path-compliance.md
│   │       └── TASK-003-keep-active-work-bounded-and-actionable.md
│   ├── evidence
│   │   ├── .gitkeep
│   │   ├── README.md
│   │   ├── artifacts
│   │   │   └── .gitkeep
│   │   ├── run_logs
│   │   │   └── .gitkeep
│   │   └── test_runs
│   │       └── .gitkeep
│   ├── now
│   │   ├── description.md
│   │   ├── metadata.json
│   │   └── prompt.md
│   └── vision
│       ├── brainstorming.md
│       ├── constraints.md
│       └── core_vision.md
```
