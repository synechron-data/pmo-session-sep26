# M365 Copilot for PMOs — Quick Reference (Copilot Chat, No Office Add-in)

Use this if you do **not** see a Copilot icon inside Word, Excel, or PowerPoint. You'll do the same work through the **Microsoft 365 Copilot Chat** window instead, then copy the result into your document.

## Set this once (do this first)

In Copilot Chat, open Settings → Personalization → Custom instructions → Edit instructions, and paste:

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

Once this is set, you can drop Role and Tone from your prompts below, Copilot already knows those.

## Where to find Copilot Chat

- Browser: copilot.cloud.microsoft (sign in with your work account)
- Or the Copilot app / Teams Copilot Chat tab

## The 4-step workflow (every time)

1. Open Copilot Chat.
2. Click **Add content** in the compose box.
3. Choose **Upload images and files** (from your device) or **Attach cloud files** (from OneDrive/SharePoint), then select your file, e.g. the resource allocation or status sheet.
4. Type your prompt using the RTCFT formula below, and hit Send.

You can also type `/` in the compose box to reference a file already saved in OneDrive or SharePoint, without a full upload.

## The RTCFT prompt formula

| Part | Ask yourself |
|---|---|
| **R**ole | Who should Copilot act as? |
| **T**ask | What's the one thing I need done? |
| **C**ontext | Mention the file you just attached |
| **F**ormat | Table, bullets, email, slide text? |
| **T**one | Executive, factual, transparent? |

## Ready-to-use prompts (after attaching the file)

### Resource allocation
> "I've attached our allocation trend summary. Role: resource manager. Task: list everyone whose Wk4 total is above 100%, and separately, who's trending upward even if not over yet. Format: two short tables. Tone: factual."

### Status reporting and budget
> "I've attached our project status sheet. Role: PMO analyst. Task: write a status summary grouped by RAG status, one line per project, and flag any project with Budget Variance % above 20%. Format: headed sections (Red / Amber / Green). Tone: executive."

### Governance
> "I've attached our RAID log. Role: PMO lead. Task: summarize all Open, High-impact items by project in plain business language. Format: short paragraph per item. Tone: neutral."

### Stakeholder email
> "I've attached our project status and RAID sheets. Role: PMO lead. Task: draft an email to the sponsor about the Red status and the top risk. Format: 3 short paragraphs, end with a clear ask. Tone: transparent."

## Getting the result into your document

Copilot Chat gives you text in the chat window, it does not write into your Word, Excel, or PowerPoint file directly. Copy the response and paste it into your document, then adjust formatting as needed.

## Tips

- You can upload up to 20 files in one conversation, keep it to just the file(s) you need.
- Stay in the same chat thread to refine an answer, don't start a new chat for each tweak.
- Always double-check names, numbers, and dates against your source file before sending anything to a stakeholder.
