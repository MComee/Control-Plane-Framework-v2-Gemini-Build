# Task Template

This file serves as a template for defining an atomic task. Each task should have a corresponding file in `project/docs/tasks/`.

---

**Task ID:** [Unique identifier for the task, e.g., FT001-TG001-T001]

**Title:** [Concise, descriptive title of the task]

**Parent Feature:**
[Reference to the feature this task belongs to.]
*   [Feature Title/ID]

**Parent Task Group:**
[Reference to the task group this task belongs to.]
*   [Task Group Title/ID]

**Purpose:**
[A clear, concise statement of what this task aims to achieve.]

**Dependencies:**
[List any dependencies this task has on other tasks, features, or external systems.]
*   [Dependency 1]
*   [Dependency 2]

**Allowed Scope:**
[Define the specific files, directories, or components that this task is permitted to interact with or modify. This should align with `project/now/metadata.json` during execution.]
*   `project/app/`
*   `project/evidence/`

**Forbidden Scope:**
[Explicitly list any files, directories, or components that this task must NOT interact with or modify, unless specifically authorized through a planning update.]
*   `project/vision/`
*   `project/docs/`
*   `framework/`

**Completion Criteria:**
[Define the specific, measurable conditions that must be met for this task to be considered complete. This should align with `project/docs/definition_of_done.md`.]
*   [Criterion 1]
*   [Criterion 2]

**Validation Expectations:**
[Describe how the completion of this task will be validated. What checks will be performed?]
*   [Validation Method 1]
*   [Validation Method 2]

**Evidence Expectations:**
[Specify what evidence of task completion should be recorded in `project/evidence/`.]
*   [Evidence Type 1, e.g., Log files]
*   [Evidence Type 2, e.g., Generated artifacts]
*   [Evidence Type 3, e.g., Test run reports]
*   [Evidence Type 4, e.g., Screenshots/recordings if applicable]

**Status:** `pending` | `in_progress` | `completed` | `blocked` | `cancelled`