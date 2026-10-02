---
title: Agentic AI in service (pilot)
type: project
created: 2026-10-02
updated: 2026-10-02
sources: [raw/alpstein/2026-05-05-strategy-memo-service-first.md, raw/alpstein/2026-07-30-q2-report-excerpt.md, raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md]
tags: [service, ai, pilot]
---

# Agentic AI in service (pilot)

Initiative of the [[service-first-strategy]]: an AI agent classifies service tickets automatically, resolves standard cases directly and hands complex cases over to humans. (Source: [[2026-05-05-strategy-memo-service-first]])

## Status (as of 5 May 2026)

- Goal: response time under 10 minutes in the standard case. (Source: [[2026-05-05-strategy-memo-service-first]])
- Pilot from August 2026; requested budget CHF 180,000 – outdated, see below. (Source: [[2026-05-05-strategy-memo-service-first]])
- Responsible: [[jonas-weber]] with [[priya-raman]]. (Source: [[2026-05-05-strategy-memo-service-first]])

## Risks

- Liability: if the agent makes a wrong commitment in service, Alpstein is liable; clear rules are needed for what the agent may do. (Source: [[2026-05-05-strategy-memo-service-first]])

> [!note] Uncertain
> The memo is a **draft for discussion** at the EB meeting of 7 May 2026. The wiki does not yet contain the outcome of that meeting; nothing in it counts as decided.

## From the Q2 report of 30 July 2026

- **Budget of CHF 180,000 approved**; kickoff in August 2026. (Source: [[2026-07-30-q2-report-excerpt]])
- Risk lies less in the technology than in the rules: what may the agent commit to toward customers? (Source: [[2026-07-30-q2-report-excerpt]])

## From the kickoff notes of 21 August 2026

- Kickoff on 21 August 2026; project lead [[jonas-weber]], technology [[priya-raman]], Service Desk [[nadia-frei]], software [[lukas-amrein]]. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Pilot duration **September to November 2026**; budget CHF 180,000 (approved). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- The agent ("service triage agent") reads tickets from [[alpmind]] and the email mailbox and classifies them as fault, maintenance, question or complaint. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Response time today 3 hours on average; goal under 10 minutes in the standard case. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Architecture: one agent; knowledge base from service manuals and the last 2,000 resolved tickets; every action is logged; a checker agent is planned for the second stage. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

### What the agent may do – first draft

| Action | Allowed? | Comment |
|---|---|---|
| Read and categorize ticket | yes | – |
| Suggest an answer from the knowledge base | yes | A human approves |
| Send an answer directly to customers | **no** (pilot phase) | to be decided after the pilot |
| Give price information | no | Price questions always go to Sales |
| Promise a credit note or compensation | **never** | Lesson from the Bergland case |
| Trigger a technician call-out | suggestion only | Dispatch decides |
| Close ticket | no | – |

(Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

> [!note] Uncertain
> The rule set "What the agent may do" is a **first draft** (21 August 2026). It was to be finalized by [[jonas-weber]] and [[nadia-frei]] by 5 September 2026; the final version is not in the wiki. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

> [!warning] Outdated
> The strategy memo of 5 May 2026 gives "pilot from August 2026" and a **requested** budget of CHF 180,000 ([[2026-05-05-strategy-memo-service-first]]). Newer status: budget **approved** ([[2026-07-30-q2-report-excerpt]], confirmed in the kickoff notes); kickoff on 21 August 2026, pilot duration **September to November 2026** (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]]).

### Open questions

- Responsibility for misclassification ([[marco-steiner]]); quality measurement (10% sample, [[nadia-frei]]); data protection for customer data by 15 September 2026; fallback to today's process. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Status report to the [[executive-board]] by 30 September 2026. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
