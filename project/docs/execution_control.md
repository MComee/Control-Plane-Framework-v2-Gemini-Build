# Execution Control

This file defines the policies and procedures for controlling the execution of tasks by external tools. It outlines how the framework manages the handoff, scope, and validation of execution activities.

**Purpose:**
To provide a clear interface for defining and enforcing execution boundaries, ensuring that AI tools operate within their designated scope and adhere to project requirements.

**Key Aspects:**
*   **Handoff Mechanism:** Details how tasks are passed from planning to execution, primarily via `project/now/`.
*   **Scope Enforcement:** Defines `allowed_paths` and `forbidden_paths` to restrict where tools can operate.
*   **Validation Procedures:** Specifies how the results of execution will be validated against expectations.
*   **Evidence Collection:** Outlines the requirements for generating and storing evidence of work.