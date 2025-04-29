# Task T-0002 – Generate Bootstrap Prompt

**Objective**
Create the prompt detailing the AI's initial actions upon launch.

**Deliverable**
Write the result to: `./output/solution/prompts/02_bootstrap_prompt.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0002_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Extract and reformat §2 from solve.md".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 2, format it as the prompt.
   • Save intermediate artefacts under `./output/tmp/T-T-0002/`.

4. **Quality Gate**
   • Review the extracted prompt against §2 in `solve.md` for completeness and accuracy.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/prompts/02_bootstrap_prompt.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0002 | done | ./output/solution/prompts/02_bootstrap_prompt.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.