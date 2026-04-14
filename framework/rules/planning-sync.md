# Planning Synchronization

All material planning changes must be reflected in the repository's truth files. Planning should not exist solely within chat conversations; it must be version-controlled.

**Synchronization Requirements:**

*   **Planning Sessions Must Update Repository Truth:** When planning activities lead to decisions about the project's vision, features, task groups, tasks, priorities, or active work, these decisions *must* be recorded in the appropriate repository files.
*   **Affected Files Must Be Synchronized:** After any significant planning update, the relevant files must be staged and committed to ensure the repository accurately reflects the latest decisions. This includes updates to:
    *   `project/vision/*`
    *   `project/docs/features/*`
    *   `project/docs/task_groups/*`
    *   `project/docs/tasks/*`
    *   `project/priorities/*`
    *   `project/now/*`

This process ensures that all stakeholders, including AI tools and human developers, are working from a consistent and up-to-date understanding of the project's direction and current state.