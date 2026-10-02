---
title: Kickoff notes pilot "Agentic AI in service", 21 August 2026
type: source
created: 2026-10-02
updated: 2026-10-02
sources: [raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md]
tags: [service, ai, pilot, governance]
---

# Kickoff notes pilot "Agentic AI in service", 21 August 2026

**Original:** `raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md` · **Type:** meeting notes · **Date:** 21 August 2026, 14:00–15:30 · **Notes:** [[lukas-amrein]]
**Participants:** [[jonas-weber]] (project lead), [[priya-raman]] (technology), [[nadia-frei]] (Service Desk, team lead), [[lukas-amrein]] (software development), [[marco-steiner]] (guest, finance)

## Summary

The kickoff defines the [[agentic-ai-service-pilot]]: a "service triage agent" reads service tickets from [[alpmind]] and the email mailbox, classifies them, resolves standard cases with an answer from the knowledge base and forwards everything else to a human. Goal: response time under 10 minutes in the standard case (today 3 hours on average). The pilot runs from September to November 2026 with an approved budget of CHF 180,000. A first-draft rule set limits the agent to suggesting; it may never promise a credit note or compensation – a lesson from the [[bergland-logistik-ag]] case. Open questions concern responsibility for misclassification, quality measurement, data protection and fallback.

## Key points

- Ticket categories: fault, maintenance, question, complaint.
- Response time today: **3 hours on average**; goal: **under 10 minutes** in the standard case (as of 21 August 2026).
- Pilot duration: **September to November 2026**; budget **CHF 180,000 (approved)**.
- Nadia Frei: "The agent may suggest, not promise."
- Architecture ([[priya-raman]]): one agent, no multi-agent solution in the pilot; knowledge base = service manuals plus the last 2,000 resolved tickets, prepared as a wiki; every action is logged; second stage after the pilot: a checker agent that checks suggestions against the rules before a human sees them.

## What the agent may do – first draft

| Action | Allowed? | Comment |
|---|---|---|
| Read and categorize ticket | yes | – |
| Suggest an answer from the knowledge base | yes | A human approves |
| Send an answer directly to customers | **no** (pilot phase) | to be decided after the pilot |
| Give price information | no | Price questions always go to Sales |
| Promise a credit note or compensation | **never** | Lesson from the Bergland case |
| Trigger a technician call-out | suggestion only | Dispatch decides |
| Close ticket | no | – |

> [!note] Uncertain
> The rule set "What the agent may do" is a **first draft** (21 August 2026). It was to be finalized by [[jonas-weber]] and [[nadia-frei]] by 5 September 2026; the final version is not in the wiki. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## Open questions

1. Who is responsible if the agent misclassifies a ticket and a downtime lasts longer as a result? ([[marco-steiner]])
2. How is quality measured, not just speed? Proposal by [[nadia-frei]]: a 10% sample of tickets reviewed by the team.
3. May customer data from tickets go into the language model? To be clarified with data protection by 15 September 2026.
4. What happens if the agent fails? Falling back to today's process must be possible at any time.

## Next steps

| What | Who | By |
|---|---|---|
| Finalize the rule set "What the agent may do" | [[jonas-weber]], [[nadia-frei]] | 5 September 2026 |
| Build the knowledge base | [[lukas-amrein]] | 19 September 2026 |
| Data protection clarification | [[priya-raman]] | 15 September 2026 |
| Quality measurement concept | [[nadia-frei]] | 12 September 2026 |
| Status report to the Executive Board | [[jonas-weber]] | 30 September 2026 |

## People and organizations involved

- [[jonas-weber]], [[priya-raman]], [[nadia-frei]], [[lukas-amrein]], [[marco-steiner]]
- [[alpstein-robotics-ag]], [[bergland-logistik-ag]] (as lesson)

## Open points

- Final rule set, data protection clarification, quality concept: due in September 2026; results not in the wiki.
- Status report to the EB of 30 September 2026: not in the wiki.
