---
name: customer-briefing
description: Write a one-page briefing to prepare a meeting with a customer, using only the wiki, with a wikilink for every claim. Use when the user asks to prepare a customer meeting, asks for a customer briefing, or writes "/customer-briefing <customer>".
---

# Customer briefing

Prepares me (CEO) for a meeting with a customer. Uses only the wiki. Never contacts the customer and never formulates commitments.

When the user asks for a briefing on a customer:

1. Read `wiki/_index.md`, then the customer's entity page and every page that mentions the customer (sources, projects, products, people).
2. If the customer has no page in the wiki: say so, list the sources in `raw/` that mention the customer and are not yet ingested, and stop.
3. Write a one-page briefing with these parts:
   - **Customer at a glance** – who they are, contact persons with role, products and contracts (e.g., AlpPick, AlpCare), fleet size if known.
   - **What happened recently** – the last events, newest first, each with date and wikilink.
   - **Open points and commitments** – what is open, what we have committed to (only if a source says so explicitly), who owns it, by when.
   - **Conflicts, contradictions, risks** – flagged, not resolved (e.g., `[!warning] Contradiction` or `[!warning] Outdated`).
   - **What the customer will probably ask** – maximum 5 questions, each with the current status from the wiki.
   - **Do not say or promise** – topics where nothing is decided (prices, dates, credit notes, compensation, service levels). Name what is open and who decides.
   - **Suggested goals for the meeting** – clearly marked as the agent's suggestion, not a fact.
4. Every statement has a wikilink; numbers always with date and source.
5. State what the wiki does **not** know about the customer, and name non-ingested sources in `raw/` that could close the gap.
6. Show the briefing in the chat and ask whether to save it as `wiki/syntheses/<YYYY-MM-DD>-customer-briefing-<customer>.md`. Save only after a yes.
7. Append an entry to `wiki/_log.md`: date, "briefing", customer.

## Boundaries

- Draft wording for the meeting is always marked as a draft. Never phrase it as a commitment.
- Do not treat proposals, drafts or emails as decisions.
- No confidential or personal data beyond names and roles.
