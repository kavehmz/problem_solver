# Task T-0007 – Assemble Final Solution

**Objective**
Combine all generated prompts and create the final executive summary document as per §6.

**Deliverable**
Write the result to: `./output/solution/final_answer.md`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0007_assumptions.md`. (e.g., All previous tasks T-0001 to T-0006 must be 'done').

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Aggregate outputs from T-0001 to T-0006, write summary."
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Verify all prerequisite tasks (T-0001 to T-0006) are marked 'done' in `./output/tasks/master_wbs.yaml`.
   • Read `./output/metadata.yaml` for run metadata (start time, goal).
   • Generate executive summary (≤ 200 words).
   • Create a list linking to deliverables:
     - `./output/solution/prompts/01_global_system_prompt.md`
     - `./output/solution/prompts/02_bootstrap_prompt.md`
     - `./output/solution/prompts/03_per_task_template.md`
     - `./output/solution/prompts/04_logging_metadata_standards.md`
     - `./output/solution/prompts/05_playbook.md`
     - `./output/lib/strategy_selector.py`
     - `./output/solution/prompts/06_finishing_up.md`
   • Calculate total tasks and run time (requires end time).
   • Assemble the final markdown content.
   • Save intermediate artefacts under `./output/tmp/T-T-0007/`.

4. **Quality Gate**
   • Validate summary length.
   • Check all links are correct relative paths.
   • Ensure all required metadata is present.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `./output/solution/final_answer.md`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0007 | done | ./output/solution/final_answer.md`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.