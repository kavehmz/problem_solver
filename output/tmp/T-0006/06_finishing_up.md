## 6  Finishing Up – Run Completion Check-List

1. Verify **all** WBS entries have `status: done`.
2. Auto-generate `./output/solution/final_answer.md`:
   - executive summary (≤ 200 words)
   - bullet list linking to each deliverable relative path
   - run metadata (start/end time, total tasks, total run time)
3. Touch `./output/logs/run_complete.flag` containing the line `completed_at: <ISO-8601>`.