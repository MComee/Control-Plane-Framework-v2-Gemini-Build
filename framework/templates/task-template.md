# Task Template

---

**Task ID:** [Unique identifier for the task, e.g., TASK-001]

**Title:** [Concise, descriptive title of the task]

**Parent Feature:**
[Reference to the feature this task belongs to.]
*   [Feature ID] - [Feature Name]

**Parent Task Group:**
[Reference to the task group this task belongs to.]
*   [Task Group ID] - [Task Group Name]

**Purpose:**
[A clear, concise statement of what this task aims to achieve.]

**Dependencies:**
[List any dependencies this task has on other tasks, features, or external systems.]
*   [Dependency 1]
*   [Dependency 2]

**Allowed Scope:**
[Define the specific files, directories, or components that this task is permitted to interact with or modify. This should align with `project/now/metadata.json` and `project/evidence/` for storing output.]
*   `project/app/`
*   `project/evidence/`

**Forbidden Scope:**
[Explicitly list any files, directories, or components that this task must NOT interact with or modify, unless specifically authorized through a planning update.]
*   `project/vision/`
*   `project/docs/`
*   `framework/`
*   `project/now/`

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
*   [Evidence Type 1, e.g., Log files in `project/evidence/run_logs/`]
*   [Evidence Type 2, e.g., Generated artifacts in `project/evidence/artifacts/`]
*   [Evidence Type 3, e.g., Test run reports in `project/evidence/test_runs/`]

**Status:** `pending` | `in_progress` | `completed` | `blocked` | `cancelled`