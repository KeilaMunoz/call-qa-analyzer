# QA Scoring Rubric — Call Center Quality Analysis
**Version 1.0 · Keila Muñoz · Oct 2026**

---

## Overview

This rubric defines the scoring dimensions used by the Call QA Analyzer tool.
Each dimension carries a maximum point value. The tool scores each call against
these criteria and outputs a structured report with findings and coaching priorities.

Dimensions and point values are configurable. This version is a starting point
built on standard call center QA practices.

---

## How Tone Is Detected

Tone detection works by scanning for linguistic markers — specific word patterns
that signal how the agent is showing up emotionally.

**Warm and empathetic signals:**
Phrases like *"I understand how frustrating"*, *"I sincerely apologize"*,
*"I appreciate your patience"*, *"I'm happy to help"* — these are explicit
acknowledgments that the agent sees the customer as a person, not a ticket.

**Professional and accountable signals:**
Active ownership language like *"I will take care of this"*,
*"Let me fix that for you"*, *"I'm going to escalate this right now"* —
these show the agent is driving the resolution, not deflecting it.

**Flat or defensive signals (what we flag as absent):**
Passive constructions like *"this will be reviewed"*, generic closes with no
warmth, or zero empathy language across the entire call — these don't necessarily
mean the agent was rude, but they do indicate a missed opportunity to build trust.

The tool doesn't read tone the way a human does. It identifies the vocabulary
that QA reviewers look for manually — and surfaces the calls where those
markers are missing.

---

## Scoring Dimensions

### 1. Opening & Verification — 15 pts
Did the agent identify themselves, greet the customer professionally,
and verify the account before accessing any information?

| Criteria | Points |
|---|---|
| Agent stated their name on opening | 4 |
| Agent used a professional greeting | 5 |
| Agent requested account number or verified identity | 6 |

---

### 2. Empathy & Tone — 20 pts
Did the agent acknowledge the customer's situation and maintain
a respectful, human tone throughout the call?

| Criteria | Points |
|---|---|
| Baseline professional tone maintained | 8 |
| Explicit empathy language used | up to 9 |
| Customer explicitly acknowledged as valued | 3 |

---

### 3. Issue Resolution — 25 pts
Did the agent identify the problem, offer a concrete solution,
and follow through with confirmation?

| Criteria | Points |
|---|---|
| Concrete solution offered | 10 |
| Proactive recovery offered without customer demanding it | 10 |
| Written or verbal confirmation provided | 5 |

---

### 4. Compliance & Disclosures — 20 pts
Did the agent follow required procedural steps and close the interaction properly?

| Criteria | Points |
|---|---|
| Baseline procedural compliance | 10 |
| Confirmed next steps in writing or verbally | 6 |
| Soft close used before ending the call | 4 |

---

### 5. Call Closing — 10 pts
Did the agent close the call with a professional farewell and appreciation statement?

| Criteria | Points |
|---|---|
| Warm farewell used | 5 |
| Explicit appreciation statement | 5 |

---

### 6. Handle Time & Efficiency — 10 pts *(optional — off by default)*
Did the agent manage the call without unnecessary elaboration or dead air?

| Criteria | Points |
|---|---|
| Agent word count within expected range | 10 |

---

## Scoring Thresholds

| Score | Result |
|---|---|
| 85 – 100 | Excellent — Above Standard |
| 70 – 84 | Meets Standard — Review flagged items |
| Below 70 | Below Standard — Coaching required |

---

## A Note on Customization

This rubric is a starting point. The dimensions, criteria, and point values
are designed to be adjusted based on the specific processes, standards, and
behaviors your team wants to reinforce or flag.

If the team decides to move forward with a pilot, the next step would be a
short working session to align the scoring criteria with your actual QA
standards and call types. The tool adapts to the rubric — not the other way around.

For questions or collaboration, connect with me on LinkedIn.
