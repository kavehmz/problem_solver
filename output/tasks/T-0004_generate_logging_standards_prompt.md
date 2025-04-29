# Task T-0004 – Generate Logging Standards Prompt

**Objective**
Create the prompt section defining the required logging and metadata formats.

**Deliverable**
Write the result to: `./output/solution/prompts/04_logging_metadata_standards.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0004_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Extract and reformat §4 from solve.md".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 4, format it as the prompt.
   • Save intermediate artefacts under `./output/tmp/T-T-0004/`.

4. **Quality Gate**
   • Review the extracted prompt against §4 in `solve.md` for completeness and accuracy. Ensure table format is preserved.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/prompts/04_logging_metadata_standards.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0004 | done | ./output/solution/prompts/04_logging_metadata_standards.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.