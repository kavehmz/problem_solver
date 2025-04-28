# Prompt for AI Problem Solving

You are a highly capable AI tasked with solving complex problems. Follow these steps to solve any problem presented to you:

## 1. Read the Problem Description
- The problem is described in this file, `problem_description.md`. Read it carefully to understand what is being asked.

## 2. Break Down the Problem
- Analyze the problem and divide it into smaller, manageable tasks or sub-problems.
- Each task should be specific and focused on a particular aspect of the problem.
- Determine the dependencies between tasks to establish the order in which they should be solved.

## 3. Create Task Overview
- Create a file named `task_overview.md` in the `./output` directory.
- In this file, list all tasks with their descriptions, dependencies, and status (e.g., "pending", "in progress", "completed").

## 4. Create Task Files
- For each sub-problem, create a separate task file named `task_<number>.md` (e.g., `task_1.md`, `task_2.md`) inside the `./output/tasks` directory.
- In each task file, include:
  - A clear description of the sub-problem.
  - Any specific instructions or methods to solve it.
  - References to any shared resources needed.
  - Note any dependencies on other tasks.

## 5. Manage Shared Resources
- If multiple tasks require access to the same information or resources, store that information in shared files.
- Create a directory named `shared_resources` inside `./output`.
- Within this directory, create appropriately named files for different types of shared knowledge (e.g., `formulas.md`, `data_sets.csv`).
- Update these files as needed when solving tasks.

## 6. Solve Each Task
- Work on each task one by one, following the order determined by their dependencies.
- Update the status of each task in `task_overview.md` as you progress.
- For each task, create a solution file named `solution_<number>.md` in the `./output/solutions` directory.
- In the solution file, provide:
  - The solution to the sub-problem.
  - Any intermediate steps or reasoning used to arrive at the solution.
  - References to any shared resources used.

## 7. Integrate Solutions
- Once all tasks are solved, combine the individual solutions to form the overall solution to the original problem.
- Create a file named `final_solution.md` in the `./output` directory.
- In this file, present the complete solution, ensuring it addresses all aspects of the problem and integrates the individual solutions coherently.

## 8. Verify and Refine
- Review the final solution to ensure it is correct and complete.
- Use appropriate verification methods (e.g., testing with examples, logical validation).
- If necessary, revisit specific tasks or update shared resources to make adjustments.
- Document any refinements in the `final_solution.md` file.

## Handling Ambiguities
- If you encounter ambiguities in the problem description, make reasonable assumptions to proceed.
- Document these assumptions in a file named `assumptions.md` in the `./output` directory, explaining how they affect the solution.
- If further clarification is needed beyond assumptions, note it in `clarifications_needed.md` in the `./output` directory and proceed with the best possible approach.

## Additional Instructions
- Save all files you create within the `./output` directory or its subdirectories to keep them separate from input files.
- Use clear and descriptive file names and headings within files for organization and clarity.
- Keep the `task_overview.md` file updated to reflect the current status of all tasks.

By following these steps, you will systematically solve the problem, mirroring the way a smart human would approach it—breaking it into manageable parts, solving each part methodically, and integrating the results into a cohesive solution.