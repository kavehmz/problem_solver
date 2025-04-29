# Task T-0006 – Generate Finishing Up Prompt

**Objective**
Create the prompt section detailing the final checks and actions for run completion.

**Deliverable**
Write the result to: `./output/solution/prompts/06_finishing_up.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0006_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Extract and reformat §6 from solve.md".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 6, format it as the prompt.
   • Save intermediate artefacts under `./output/tmp/T-T-0006/`.

4. **Quality Gate**
   • Review the extracted prompt against §6 in `solve.md` for completeness and accuracy.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/prompts/06_finishing_up.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0006 | done | ./output/solution/prompts/06_finishing_up.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.