# File Protection Rules

This framework protects repository truth. It does not manage AI internals.

## Protected Files

Execution tools must not mutate these during normal execution:

- `project/vision/core_vision.md`
- `project/vision/constraints.md`
- `project/docs/features/*`
- `project/docs/task_groups/*`
- `project/docs/priorities/*`

## Restricted Files

These are planning-controlled and should only change through explicit planning updates:

- `project/docs/tasks/*`
- `project/docs/roadmap.md`
- `project/docs/decisions.md`
- `project/docs/definition_of_done.md`
- `project/docs/execution_control.md`
- `project/now/*`

## Allowed for Normal Execution

- `project/app/*`
- `project/evidence/*`

## Compliance Rule

- Every path referenced in governance and control docs must exist.
- The root `README.md` must list every tracked file and tracked subdirectory recursively and exactly.
- Any boundary violation invalidates execution trust.
