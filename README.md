# Control Plane Framework v2

This repository is a repository-native control layer for AI-assisted software development.

## Three Layers of Control

This framework operates with three distinct layers, each with specific responsibilities:

### Layer 1 — Framework Self-Governance
This layer is responsible for the framework's integrity and stability. It defines the core doctrine, manages routing, protects critical framework files, and synchronizes planning processes. Its goal is to prevent the framework itself from drifting and to ensure consistent operation.

### Layer 2 — Single-Project Control
This layer governs a single, specific project managed within this repository. It enforces the project's vision, defines features, organizes work into task groups and atomic tasks, manages priorities, tracks active work, and collects evidence of completion. It ensures that all development aligns with the project's stated goals.

### Layer 3 — Execution Guidance
This layer provides essential context and instructions for external tools, such as AI assistants (ChatGPT, Gemini, Claude) or local development tools. It defines expected behavior, scope boundaries, handoff prompts for execution, and validation criteria. Critically, this layer does *not* control the internal workings of these external tools but guides their interaction with the repository.

## How AI tools should use this repo

AI tools interacting with this repository must adhere to the following principles:

1.  **Read README first:** Always begin by reading the `README.md` to understand the framework's purpose and operational model.
2.  **Determine Phase:** Identify the current phase of operation: planning, execution preparation, execution, or validation.
3.  **Follow Routing Rules:** Consult `docs/routing.md` to understand which files and sections are relevant for the current phase and what their purpose is.
4.  **Avoid Modifying Protected Files:** Files designated as "Protected" or "Restricted" in `framework/rules/protected-files.md` must not be modified unless explicitly authorized by the framework's planning or control update procedures. Unauthorized modifications will invalidate the trustworthiness of any execution results.
5.  **Use `project/now/prompt.md` for Handoff:** The `project/now/prompt.md` file serves as the definitive source for the exact task and scope to be executed in the current "active work" cycle.

## Workflow

The framework supports a structured workflow for AI-assisted development:

*   **Planning:** Involves defining and refining the project's vision, features, task decomposition, and priorities. This process must result in updates to repository truth files.
*   **Decomposition:** Breaking down features into manageable task groups and then into atomic tasks.
*   **Prioritization:** Assigning urgency and order to tasks using `project/priorities/` files.
*   **Active Work Handoff:** Clearly defining the single, bounded task to be executed next via `project/now/`.
*   **Execution:** Performing the defined task, adhering strictly to scope and using specified tools/methods.
*   **Evidence Return:** Recording the outcome, logs, and artifacts of execution in `project/now/evidence/`.

## Repository File Tree

```
.
├── .gitkeep              # Placeholder for empty directories
├── README.md             # This file
├── docs/
│   ├── control-model.md  # Explains the three-layer control model
│   ├── overview.md       # General overview of the framework's purpose
│   ├── routing.md        # Defines AI tool routing rules by phase
│   └── start-here.md     # Minimum reading order for new users/tools
├── framework/
│   ├── rules/
│   │   ├── execution-boundaries.md # Defines scope and limits for execution
│   │   ├── planning-sync.md        # Rules for synchronizing planning with repo truth
│   │   └── protected-files.md      # Classifies files as protected, restricted, or allowed
│   └── templates/
│       ├── active-work-template.md # Template for current work handoff
│       ├── feature-template.md     # Template for defining project features
│       ├── task-group-template.md  # Template for grouping atomic tasks
│       └── task-template.md        # Template for atomic tasks
├── project/
│   ├── app/
│   │   └── README.md     # Location for project implementation code
│   ├── docs/
│   │   ├── features/
│   │   │   └── README.md # Explains feature definition files
│   │   ├── task_groups/
│   │   │   └── README.md # Explains task group organization
│   │   └── tasks/
│   │       └── README.md # Explains atomic task definition files
│   ├── now/
│   │   ├── description.md  # Human-readable description of current work
│   │   ├── evidence/
│   │   │   └── .gitkeep    # Placeholder for execution evidence
│   │   ├── metadata.json   # Machine-readable metadata for current work
│   │   ├── prompt.md       # Machine-consumable handoff for current task
│   │   └── test_runs/
│   │       └── .gitkeep    # Placeholder for test run results
│   ├── priorities/
│   │   ├── blocked.md      # Tasks that are currently blocked
│   │   ├── done.md         # Tasks that have been completed
│   │   ├── later.md        # Tasks planned for the future
│   │   ├── next.md         # Tasks planned for the immediate future
│   │   └── now.md          # The currently active task
│   ├── vision/
│   │   ├── brainstorming.md # Ideation and uncommitted ideas
│   │   ├── constraints.md   # Project limitations and boundaries
│   │   └── core_vision.md   # The protected, fundamental project doctrine
│   ├── decisions.md        # Record of significant project decisions
│   ├── definition_of_done.md # Criteria for considering work complete
│   └── roadmap.md          # High-level phased sequencing of project work
└── .gitkeep                # Placeholder for empty directories
```