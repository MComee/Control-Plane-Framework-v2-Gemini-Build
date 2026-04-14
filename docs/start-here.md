# Start Here

Welcome to the Control Plane Framework v2. This guide outlines the minimum reading order for understanding the framework and its operational model.

1.  **README.md**: Provides a high-level overview of the framework's purpose, its three-layer control model, how AI tools should interact with the repository, and the general workflow.
2.  **docs/control-model.md**: Explains the operational details of the three-layer control model (framework self-governance, project control, execution guidance) and their separation of concerns.
3.  **docs/routing.md**: Details how AI tools should navigate and access repository files based on their current operational phase (Planning, Execution Preparation, Execution, Validation).
4.  **framework/rules/**: Review the files within `framework/rules/` (`protected-files.md`, `planning-sync.md`, `execution-boundaries.md`) to understand the rules governing file access, modification, and synchronization.
5.  **project/vision/**: Examine files in `project/vision/` (`core_vision.md`, `constraints.md`, `brainstorming.md`) to grasp the fundamental doctrine and scope of the controlled project.
6.  **project/docs/**: Explore the documentation structure under `project/docs/` to understand how project components are defined and organized (e.g., `features/README.md`, `task_groups/README.md`, `tasks/README.md`, `priorities/`, `roadmap.md`, `decisions.md`, `definition_of_done.md`, `execution_control.md`).
7.  **project/now/**: Examine the contents of `project/now/` (`description.md`, `prompt.md`, `metadata.json`) to understand how the current work item is defined and handed off for execution.