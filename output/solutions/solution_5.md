## 5. Manage Shared Resources

If you identify information, data, formulas, or other resources that will be needed by multiple tasks, centralize them to avoid redundancy and ensure consistency.

-   **Directory:** Create a directory named `shared_resources` inside the `./output` directory.
-   **Files:** Within `shared_resources`, create files with appropriate names for different types of shared knowledge (e.g., `constants.md`, `data_schema.json`, `common_functions.py`).
-   **Usage:** Reference these shared files from the individual `task_*.md` files where needed.
-   **Updates:** If solving a task reveals new shared knowledge or requires modifying existing shared resources, update the relevant files in this directory accordingly.