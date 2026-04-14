# Atomic Tasks

This directory contains definitions for individual, atomic tasks that form the building blocks of implementation. Each task represents a single, bounded unit of work.

**Purpose:**
Atomic tasks are the smallest units of work that can be assigned and executed. They provide clear scope, purpose, and completion criteria, enabling precise handoffs to execution tools.

**Guidelines for Task Files:**
*   Each file should follow the `framework/templates/task-template.md`.
*   Task files are classified as "Restricted" artifacts. They should only be updated as part of explicit planning, tracking, or approved control updates. Execution tools must not modify these files directly.
*   Tasks should be clearly defined with specific scope, dependencies, and validation expectations.