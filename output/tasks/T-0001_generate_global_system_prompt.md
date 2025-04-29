# Task T-0001 – Generate Global System Prompt

**Objective**
Create the main system prompt defining the AI's core mission, capabilities, and rules.

**Deliverable**
Write the result to: `./output/solution/prompts/01_global_system_prompt.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0001_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s) (e.g., divide-and-conquer, MILP, simulation). Based on WBS: "Extract and reformat §1 from solve.md".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 1, format it as the prompt.
   • Save intermediate artefacts under `./output/tmp/T-T-0001/`.

4. **Quality Gate**
   • Review the extracted prompt against §1 in `solve.md` for completeness and accuracy.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/prompts/01_global_system_prompt.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0001 | done | ./output/solution/prompts/01_global_system_prompt.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.