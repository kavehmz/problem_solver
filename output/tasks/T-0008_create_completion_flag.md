# Task T-0008 – Create Completion Flag

**Objective**
Create the final flag file indicating successful completion of the entire run.

**Deliverable**
Write the result to: `./output/logs/run_complete.flag`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0008_assumptions.md`. (e.g., Task T-0007 must be 'done').

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Write timestamp to file."
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Verify task T-0007 is marked 'done' in `./output/tasks/master_wbs.yaml`.
   • Get the current ISO-8601 timestamp.
   • Format the content: `completed_at: <ISO-8601 timestamp>`
   • Save intermediate artefacts under `./output/tmp/T-T-0008/`.

4. **Quality Gate**
   • Check the timestamp format is correct.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/logs/run_complete.flag`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0008 | done | ./output/logs/run_complete.flag`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.