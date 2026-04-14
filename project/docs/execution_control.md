# Execution Control

This project is executed through one active handoff at a time.

## Handoff Source
- `project/now/description.md`
- `project/now/prompt.md`
- `project/now/metadata.json`

`project/now/prompt.md` is the execution source of truth.

## Scope Control
- Allowed edits must stay inside `allowed_paths`.
- Forbidden edits must stay outside `forbidden_paths`.
- Scope changes require planning sync before execution continues.

## Validation Control
- Validate outputs against `validation_requirements`.
- Validate evidence against `evidence_paths`.
- Validate boundary compliance.
- Validate README tree and path correctness across docs.
