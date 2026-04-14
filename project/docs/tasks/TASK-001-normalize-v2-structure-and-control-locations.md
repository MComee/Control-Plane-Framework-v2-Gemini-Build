# TASK-001 Normalize v2 Structure and Control Locations

**Task ID:** `TASK-001`

**Title:** Normalize structure and remove conflicting control surfaces

**Parent Feature:**
- `FEAT-001` Repository Truth Control and Handoff Discipline

**Parent Task Group:**
- `TG-001` Structural Compliance and Active-Work Control

**Purpose:**
Align repository paths to required v2 architecture and remove conflicting locations.

**Dependencies:**
- `project/vision/core_vision.md`
- `project/docs/execution_control.md`

**Allowed Scope:**
- `project/docs/`
- `project/evidence/`
- `project/now/`
- `README.md`
- `docs/`
- `framework/templates/`
- `framework/rules/`

**Forbidden Scope:**
- `.git/`
- External systems and non-repository state

**Completion Criteria:**
- Only one priorities location exists at `project/docs/priorities/`
- Only one evidence surface exists at `project/evidence/`
- `project/docs/` contains `roadmap.md`, `decisions.md`, `definition_of_done.md`, and `execution_control.md`

**Validation Expectations:**
- Path audit confirms required structure
- README tree matches tracked files

**Evidence Expectations:**
- Path audit notes in `project/evidence/run_logs/` when execution outputs are produced

**Status:** `completed`
