# Planning Synchronization

Planning is only valid when synchronized to repository files. Chat-only planning is non-compliant.

## Required Synchronization Targets

- `project/vision/*`
- `project/docs/features/*`
- `project/docs/task_groups/*`
- `project/docs/tasks/*`
- `project/docs/priorities/*`
- `project/docs/roadmap.md`
- `project/docs/decisions.md`
- `project/docs/definition_of_done.md`
- `project/docs/execution_control.md`
- `project/now/*`

## Enforcement

- If planning changes structure, priorities, or active work, update files in the same change set.
- If tracked files are added, removed, moved, or renamed, update the root `README.md` recursive file tree in the same change set.
- Do not treat intent as synchronized until repository paths and file contents reflect it.
