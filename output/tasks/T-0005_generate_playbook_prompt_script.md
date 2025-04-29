# Task T-0005 – Generate Playbook Prompt & Script

**Objective**
Create the prompt section describing the recommended problem-solving strategies and the associated helper script.

**Deliverable**
Write the prompt result to: `./output/solution/prompts/05_playbook.md`
Write the script result to: `./output/lib/strategy_selector.py`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-T-0005_assumptions.md`. (e.g., Python environment availability for the script).

2. **Plan of Attack**
   • Choose the best-fit method(s). Based on WBS: "Extract and reformat §5 from solve.md, create Python script".
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work: Read `solve.md`, extract section 5.
   • Format the descriptive part as the prompt content.
   • Extract the Python code block.
   • Save intermediate artefacts under `./output/tmp/T-T-0005/`.

4. **Quality Gate**
   • Review the extracted prompt against §5 in `solve.md`.
   • Validate the Python script syntax.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final prompt artefact to `./output/solution/prompts/05_playbook.md`.
   • Move final script artefact to `./output/lib/strategy_selector.py`. (Create `./output/lib/` if needed).
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | T-0005 | done | ./output/solution/prompts/05_playbook.md;./output/lib/strategy_selector.py`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.