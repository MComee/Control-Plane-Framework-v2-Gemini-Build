# Active Work Template

---

**Description:**
[A clear, human-readable description of the work to be performed. This should correspond to `project/now/description.md`.]

**Objective:**
[The specific, actionable goal for this work item.]

**Required Reads:**
[List of files and directories that are essential to read to understand and execute this work item.]
*   `project/now/description.md`
*   `project/now/prompt.md`
*   `project/now/metadata.json`
*   [Any specific task definition files, feature definitions, etc.]

**Allowed Files:**
[List of files and directories that the execution tool is permitted to modify or create. This should align with `project/now/metadata.json` and `project/evidence/` for storing output.]
*   `project/app/`
*   `project/evidence/`
*   `project/evidence/run_logs/`
*   `project/evidence/test_runs/`
*   `project/evidence/artifacts/`

**Forbidden Files:**
[List of files and directories that the execution tool must NOT modify or create. This should align with `project/now/metadata.json`.]
*   `project/vision/`
*   `project/docs/`
*   `framework/`
*   `project/now/`

**Exact Update Requirements:**
[Specific instructions on how files are expected to be updated. This may include code snippets, expected changes, or specific file formats.]
*   [Requirement 1]
*   [Requirement 2]

**Validation Requirements:**
[How the successful completion of this work item will be validated. This should align with `project/now/metadata.json`.]
*   [Validation Method 1]
*   [Validation Method 2]

**Evidence Requirements:**
[What evidence of work completion must be produced and where it should be stored. This should align with `project/now/metadata.json`.]
*   Store logs in `project/evidence/run_logs/`
*   Store generated artifacts in `project/evidence/artifacts/`
*   Store test runs in `project/evidence/test_runs/`

**Blocked-State Instructions:**
[Instructions for what to do if the work item becomes blocked. This typically involves updating status and potentially moving to `project/priorities/blocked.md`.]

**Completion Criteria:**
[What constitutes successful completion of this work item. This should align with `project/docs/definition_of_done.md`.]