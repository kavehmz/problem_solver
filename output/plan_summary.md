# Plan Summary: Creating the AI Problem-Solving Prompt

This document outlines the plan for generating an AI prompt based on the methodology described in `solve.md`, as requested in `problem_description.md`.

**Plan Steps:**

1.  **Define Tasks:** Create a markdown file (`task_*.md`) for each section of the problem-solving methodology described in `solve.md`. (Tasks 1-12)
2.  **Solve Tasks:** For each task, generate the corresponding text for the final AI prompt and save it in a separate solution file (`solution_*.md`). Update `task_overview.md` as each task is completed.
3.  **Integration:** Combine all the generated text from the solution files into a single `final_solution.md`. (Task 11)
4.  **Verification:** Review the `final_solution.md` to ensure it accurately reflects the methodology from `solve.md` and fulfills the request in `problem_description.md`. (Task 12)

**Workflow Diagram:**

```mermaid
graph TD
    A[Start: Understand Request] --> B(Read problem_description.md);
    B --> C{Break Down Problem?};
    C -- Yes --> D[Define Tasks based on solve.md];
    D --> E[Create task_overview.md];
    E --> F[Create assumptions.md];
    F --> G[Create task_1.md];
    G --> H{More Tasks?};
    H -- Yes --> I[Create next task_N.md];
    I --> H;
    H -- No --> J[Start Solving Tasks];
    J --> K{Solve Task 1?};
    K -- Yes --> L[Create solution_1.md];
    L --> M[Update task_overview.md];
    M --> N{Solve Task 2?};
    N -- Yes --> O[Create solution_2.md];
    O --> P[Update task_overview.md];
    P --> Q[... Solve Remaining Tasks ...];
    Q --> R{All Tasks Solved?};
    R -- Yes --> S[Integrate Solutions];
    S --> T[Create final_solution.md];
    T --> U{Verify & Refine?};
    U -- Yes --> V[Review final_solution.md];
    V --> W[Refine if needed];
    W --> X[End: Final Prompt Ready];
    U -- No --> X;

    subgraph Initialization
        A
        B
        F
    end

    subgraph Task Definition
        C
        D
        E
        G
        H
        I
    end

    subgraph Execution
        J
        K
        L
        M
        N
        O
        P
        Q
    end

    subgraph Integration & Verification
        R
        S
        T
        U
        V
        W
        X
    end