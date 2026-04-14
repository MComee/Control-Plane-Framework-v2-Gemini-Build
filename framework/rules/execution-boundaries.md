# Execution Boundaries

Execution is bounded repository work. It does not include AI-internal control.

## Boundary Rules

- Execute from `project/now/prompt.md`.
- Enforce `allowed_paths` and `forbidden_paths` from `project/now/metadata.json`.
- Do not expand scope silently. Route scope changes through planning sync.
- Write execution evidence only under `project/evidence/`.

## Validation Rules

- Confirm protected boundaries were respected.
- Confirm outputs satisfy validation requirements from `project/now/metadata.json`.
- Confirm repository references stay real and synchronized, including the root `README.md` tree.
