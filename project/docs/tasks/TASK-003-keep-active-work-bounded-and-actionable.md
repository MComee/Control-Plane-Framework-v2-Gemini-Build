# TASK-003 Keep Active Work Bounded and Actionable

**Task ID:** `TASK-003`

**Title:** Maintain operational handoff package in `project/now/`

**Parent Feature:**
- `FEAT-001` Repository Truth Control and Handoff Discipline

**Parent Task Group:**
- `TG-001` Structural Compliance and Active-Work Control

**Purpose:**
Keep `project/now/description.md`, `project/now/prompt.md`, and `project/now/metadata.json` synchronized and executable.

**Dependencies:**
- `TASK-002`

**Allowed Scope:**
- `project/now/`
- `project/docs/priorities/`
- `project/docs/tasks/`

**Forbidden Scope:**
- `project/vision/`
- `framework/rules/` unless planning explicitly updates doctrine

**Completion Criteria:**
- `project/now/metadata.json` includes required control keys
- Current `task_id` exists in `project/docs/tasks/`
- Allowed and forbidden paths are precise and enforceable

**Validation Expectations:**
- JSON is valid and path references are real
- Active task status is reflected in priorities

**Evidence Expectations:**
- Evidence path mapping is present in `metadata.json`

**Status:** `pending`
