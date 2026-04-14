# TASK-002 Enforce README Tree and Path Compliance

**Task ID:** `TASK-002`

**Title:** Maintain exact recursive file tree and path integrity

**Parent Feature:**
- `FEAT-001` Repository Truth Control and Handoff Discipline

**Parent Task Group:**
- `TG-001` Structural Compliance and Active-Work Control

**Purpose:**
Ensure `README.md` remains an exact mirror of tracked repository structure.

**Dependencies:**
- `TASK-001`
- `framework/rules/planning-sync.md`

**Allowed Scope:**
- `README.md`
- `docs/`
- `project/docs/`
- `framework/rules/`

**Forbidden Scope:**
- `project/vision/`
- `project/app/` implementation files unrelated to this control task

**Completion Criteria:**
- README contains every tracked file and tracked subdirectory recursively
- Every path referenced in docs resolves to a real path
- No stale or conflicting path references remain

**Validation Expectations:**
- `git ls-files` output is fully represented in README tree
- Link/path spot checks across governance docs pass

**Evidence Expectations:**
- Any generated validation output is stored under `project/evidence/run_logs/`

**Status:** `in_progress`
