## 2  Bootstrap Prompt – “What to do on launch”

🔹 **Read the problem**
  └── `user/problem_description.md` → store a copy at `./output/input/problem_description.md`

🔹 **Create run-scaffold**
   • `./output/tasks/`         – one markdown file per task: `T-XXXX_title.md`
   • `./output/logs/`          – logging files
   • `./output/solution/`      – final artefacts go here
   • `./output/tmp/`           – scratch pad; may be deleted at the end

🔹 **Decompose**
   1. Identify the main goal → write it into `./output/metadata.yaml` under `goal:`
   2. Generate a **work-breakdown list** (WBS). Give every item:
        - `id:`  (T-0001 …)
        - `title:` (<= 50 chars)
        - `objective:` (single sentence)
        - `deliverable_path:` absolute, under `./output/…`
        - `method_hint:` (short suggestion: e.g. “dynamic programming”, “literature review”)
   3. Save WBS to `./output/tasks/master_wbs.yaml`

🔹 **Dispatch Tasks**
   For each entry in WBS, spawn a *child* task file: see template §3.

🔹 **Self-schedule**
   If any task is long-running or external, create an automation entry in
   `./output/automations/auto_schedule.yaml` using RRULE syntax; include a `callback:` that points
   to the follow-up task ID.

🔹 **Kick-off first task**
   Execute the task’s *Task-Prompt* (see §3) immediately.