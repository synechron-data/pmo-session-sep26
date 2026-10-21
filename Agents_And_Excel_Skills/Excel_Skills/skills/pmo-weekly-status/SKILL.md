---
name: pmo-weekly-status
description: Create a weekly PMO status report from milestone, action and RAID tables, including achievements, overdue work, upcoming milestones and data-quality questions.
---

# Weekly PMO status

Use the active workbook's Milestones, Actions and RAID tables. Read the as-of date from Milestones!B3 and flag inconsistent as-of dates on other sheets. Use real date values and calendar days. For this training workbook the reporting week starts four calendar days before the as-of date and ends on the as-of date. If required fields or sheets are missing, identify them before producing affected results.
Preserve source values and table names. Never replace reported status or RAG with an inference. Use IDs as stable keys and exclude repeated IDs from counts only after reporting the duplicate and asking which record is authoritative. Flag missing owners and dates rather than treating them as zero. Do not invent explanations, completion dates, trends or overall progress weights. Do not send messages or claim to update external systems.
Write outputs to a new worksheet. If the proposed output sheet already exists, ask whether to replace it or create a dated version. Keep source rows unchanged. Use references and formulas for derived numeric outputs when supported. Label any generated narrative as a draft that needs refreshing after source changes. Verify counts against the underlying IDs before finishing.

## Steps
1. Identify the reporting week and as-of date. Display both at the top of a new Weekly Status sheet.
2. Summarize unique project and milestone counts by source status. Completed-this-week requires Completed Date within the inclusive reporting week and Status equal to Completed. Flag inconsistent completion dates and status.
3. List overdue milestones: non-Completed with Due Date strictly before as-of. List due-today items separately. Upcoming means after as-of and no later than as-of plus seven days. Do not include completed records in these attention lists.
4. List open RAID entries and show Type, Impact, Owner, Review Date and Response. Keep issues, risks, assumptions and dependencies distinguishable. Do not count related records as independent blockers without checking their milestone links.
5. Include overdue actions, excluding Completed status. Show missing owners, missing due dates and milestone updates older than seven calendar days. Missing update dates are separate data-quality issues.
6. Draft a short executive summary, achievements, blockers, next steps and decisions needed. Cite source sheet and record IDs. Keep suggested actions separate from recorded commitments. Do not compute project RAG unless rules are supplied.
7. Format readable tables with filters, explicit date formats, wrapped long text, and a clear heading. Show the calculation basis for counts and verify representative records against source rows.
