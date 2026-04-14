# Operational Control Model

This framework employs a three-layer model to operationalize AI-assisted software development, ensuring clarity, consistency, and control over the development process.

## Layer 1 — Framework Self-Governance

*   **What it is:** The foundational layer that dictates how the framework itself operates and maintains its integrity.
*   **Components:** Includes framework doctrine, routing rules, file protection policies, planning synchronization mechanisms, and execution boundary definitions.
*   **Purpose:** To protect the framework from uncontrolled drift, ensure consistent application of rules across all operations, and maintain the framework's reusability and generic nature. It acts as the ultimate authority on how the system should behave.

## Layer 2 — Single-Project Control

*   **What it is:** This layer focuses on governing a single, specific project managed within this repository.
*   **Components:** Encompasses the project's core vision, feature definitions, organization of work into task groups and atomic tasks, prioritization schemes, tracking of active work, and the definition of "done."
*   **Purpose:** To maintain the project's intent and ensure that all development activities are aligned with its defined goals, features, and priorities. It serves as the project's source of truth.

## Layer 3 — Execution Guidance

*   **What it is:** This layer provides the interface and instructions for external tools (like AI assistants or local development scripts) that perform work.
*   **Components:** Includes context provision, definition of expected behavior, scoped handoff prompts for execution (e.g., `project/now/prompt.md`), and validation criteria.
*   **Purpose:** To guide external tools in performing specific, bounded tasks without controlling their internal logic. It ensures that tools understand what to do, where to do it, and how to report back, thereby aligning their actions with the project's needs as defined by Layer 2.

### Separation of Concerns

The model enforces a strict separation of concerns:
*   **Layer 1** governs the *framework*.
*   **Layer 2** governs the *project*.
*   **Layer 3** governs the *interaction* with external execution agents.

This separation ensures that changes in one layer do not inadvertently break functionality in others and that each layer can be maintained and evolved independently while respecting the overall system design.