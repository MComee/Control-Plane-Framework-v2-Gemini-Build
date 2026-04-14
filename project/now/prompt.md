# Active Work Prompt

Execute `TASK-002`.

Required outcome:
1. Ensure `README.md` contains a fully recursive file tree that matches all tracked files and tracked subdirectories in this repository.
2. Verify that all paths referenced in `README.md`, `docs/`, `framework/rules/`, and `project/docs/` exist.
3. Correct any path drift, especially priorities and evidence locations.
4. Do not edit AI-internal policy content. This framework governs repository truth and execution alignment only.

Constraints:
- Work only inside `allowed_paths` from `project/now/metadata.json`.
- Do not modify `forbidden_paths`.
- Keep language concise and operational.

Completion criteria:
- README tree equals the current tracked repository structure.
- No conflicting priorities or evidence surfaces remain.
- Validation checks in metadata are satisfied.
