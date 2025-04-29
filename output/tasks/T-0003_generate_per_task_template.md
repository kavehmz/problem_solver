# Task T-0003 – Generate Per-Task Prompt Template

**Objective**
Create the template prompt for guiding the AI through individual sub-tasks.

**Deliverable**
Write the result to: `./output/solution/prompts/03_per_task_template.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0003_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Extract and reformat §3 from solve.md".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 3, format it as the template prompt.
   • Save intermediate artefacts under `./output/tmp/T-T-0003/`.

4. **Quality Gate**
   • Review the extracted prompt against §3 in `solve.md` for completeness and accuracy. Ensure placeholders are correct.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/prompts/03_per_task_template.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0003 | done | ./output/solution/prompts/03_per_task_template.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.