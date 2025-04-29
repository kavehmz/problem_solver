## 3  Per-Task Prompt Template – `./output/tasks/T-XXXX_<slug>.md`

```
# Task {{id}} – {{title}}

**Objective**
{{objective}}

**Deliverable**
Write the result to: `{{deliverable_path}}`

---

## WORKFLOW (follow in order)

1. **Clarify Boundaries**
   Record any assumptions you need in `./output/logs/T-{{id}}_assumptions.md`.

2. **Plan of Attack**
   • Choose the best-fit method(s) (e.g., divide-and-conquer, MILP, simulation).
   • Justify the choice in one paragraph → append to the assumptions file.

3. **Execute**
   • Perform the work.
   • Save intermediate artefacts under `./output/tmp/T-{{id}}/`.

4. **Quality Gate**
   • Run automated checks/tests if applicable.
   • If failure → fix; log retries.

5. **Close the Task**
   • Move final artefact to `{{deliverable_path}}`.
   • Update `./output/logs/progress.log` with
     `{{timestamp_iso}} | {{id}} | done | {{deliverable_path}}`

> When everything above is complete **append** to `./output/tasks/master_wbs.yaml`:
> `status: done` under this task’s entry.