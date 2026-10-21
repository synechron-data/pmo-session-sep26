# M365 Copilot for PMOs — Quick Reference (Full Copilot in Word / Excel / PowerPoint)

Use this if you see the Copilot icon inside Word, Excel, and PowerPoint. Your prompts run directly against the open file, no need to paste data.

## Set this once (do this first)

Go to Copilot Settings → Personalization → Custom instructions → Edit instructions, and paste:

```
I work in a non-technical PMO role covering project governance, resource
allocation, status reporting, and stakeholder communication. I do not manage
code or technical architecture.

Act as an experienced PMO analyst or PMO lead unless I name another role.
Keep responses executive-ready: clear, factual, no technical jargon. Default
to tables for data, short bullets for lists, short paragraphs for emails.
Use RAG (Red/Amber/Green) language naturally. Lead with the most urgent item
first. If a number or date isn't in the data I gave you, say so.
```

In Excel specifically, there's a separate Personalization option, add:

```
Show analysis results in the chat pane rather than creating a new worksheet,
unless I ask you to add one. Use INR currency formatting with thousands
separators. Prefer tables over PivotTables unless I ask by name.
```

Once this is set, you can drop Role and Tone from your prompts below, Copilot already knows those.

## The RTCFT prompt formula

| Part | Ask yourself |
|---|---|
| **R**ole | Who should Copilot act as? |
| **T**ask | What's the one thing I need done? |
| **C**ontext | What data or text should it use? |
| **F**ormat | Table, bullets, email, slide? |
| **T**one | Executive, factual, transparent? |

## Where to find Copilot

- **Excel**: Home tab → Copilot icon → opens a chat pane on the right. Ask questions about the open sheet. Ask it to show answers **in the chat pane**, not a new worksheet, unless you actually want a new tab.
- **Word**: Home tab → Copilot icon, or right-click selected text → Copilot.
- **PowerPoint**: Home tab → Copilot icon → can build slides from a Word doc, Excel sheet, or your own prompt.

## Ready-to-use prompts

### Resource allocation (Excel — Allocation Trend Summary sheet)
> "Role: resource manager. Task: list everyone whose Wk4 Total % is above 100, and separately who's trending upward even if not over yet. Format: two short tables. Tone: factual."

### Status reporting and budget (PowerPoint / Excel — Project Status sheet)
> "Role: PMO analyst. Task: turn this into a one-slide steering committee update and flag any project with Budget Variance % above 20%. Format: table with RAG colors, one line per project. Tone: executive, concise."

### Governance (Word)
> "Role: PMO lead. Task: draft a RAID summary for the governance pack, only Open and High-impact items. Format: short paragraph per item, grouped by project. Tone: neutral."

### Stakeholder email (Word / Outlook)
> "Role: PMO lead. Task: draft an email to the project sponsor about the Red status and the key risk. Format: 3 short paragraphs, end with a clear ask. Tone: transparent, solution-forward."

## Tips

- Keep the Copilot pane open and refine your prompt rather than starting over.
- Always check names, numbers, and dates it gives you against the source data before sending anything out.
- If the output isn't right, add more Context or be more specific about Format, that fixes most misses.
