---
name: pmo-action-followup
description: Review a PMO action log for overdue, due-today, upcoming and unassigned actions, then draft owner follow-ups without sending messages.
---

# PMO action follow-up

Use the active workbook's Milestones, Actions and RAID tables. Read the as-of date from Milestones!B3 and flag inconsistent as-of dates on other sheets. Use real date values and calendar days. For this training workbook the reporting week starts four calendar days before the as-of date and ends on the as-of date. If required fields or sheets are missing, identify them before producing affected results.
Preserve source values and table names. Never replace reported status or RAG with an inference. Use IDs as stable keys and exclude repeated IDs from counts only after reporting the duplicate and asking which record is authoritative. Flag missing owners and dates rather than treating them as zero. Do not invent explanations, completion dates, trends or overall progress weights. Do not send messages or claim to update external systems.
Write outputs to a new worksheet. If the proposed output sheet already exists, ask whether to replace it or create a dated version. Keep source rows unchanged. Use references and formulas for derived numeric outputs when supported. Label any generated narrative as a draft that needs refreshing after source changes. Verify counts against the underlying IDs before finishing.

## Steps
1. Create an Action Follow-up output sheet with the as-of date. Exclude Completed actions from the open-action workload, but retain a count of all source actions for reconciliation.
2. Classify open actions: Unknown due date when the date is blank or invalid; Overdue when due date is before as-of; Due today when equal; Upcoming when after as-of through as-of plus seven days; Later for other future dates. These categories must be mutually exclusive.
3. Add Days overdue as MAX(0,as-of minus due date) only for valid dates. Keep unknown dates blank and explicitly flagged. A due-today item has zero days overdue.
4. Flag missing owners independently of due category. Do not infer an owner from a related milestone. Group known-owner follow-ups by owner; route unassigned items to the project-lead role for assignment.
5. Sort overdue items by days overdue descending, then High, Medium, Low priority. Keep unknown due dates and missing owners visible in a separate attention section, not buried at the bottom of a future-due list.
6. Draft an email subject and body for each owner needing follow-up. Include action IDs, action text, original due dates and a request for status, evidence and a revised date where needed. Do not invent recipients' email addresses or new commitments. Do not send the drafts.
7. Verify that due-category counts reconcile to the open-action total. An unassigned action remains in exactly one due category and may also carry a missing-owner flag.
