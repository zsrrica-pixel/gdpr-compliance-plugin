---
name: ropa
description: Build or review a Record of Processing Activities (GDPR Art. 30). Use when the user wants to document processing activities, create a ROPA, or audit an existing one.
---

# Record of Processing Activities

For each processing activity capture: name and purpose; controller/joint controller/DPO contact; categories of data subjects; categories of personal data (flag special-category data); lawful basis (Art. 6, plus Art. 9 condition if relevant); recipients and processors; third-country transfers and safeguards; retention period; security measures (Art. 32).

Output as a table (or CSV if asked). When reviewing an existing record, list gaps: missing lawful basis, undefined retention, processors without DPAs, transfers without a mechanism. Ask the user about anything you cannot infer rather than guessing.

## Handling unknowns and sources
- Record the evidence source for each row (policy page, code, contract). Mark unknowns **OPEN** and collect them in an "Open questions" list at the end; in a non-interactive run, do not stop to ask.
- Include one row per distinct purpose, including consent/cookie-driven processing (ads, pixels, analytics), payments, and rights handling. Mark inferred rows "inferred".
- Finish with a "Gaps" list: processors without a DPA, transfers without a mechanism or TIA, missing lawful basis or retention, joint-controller questions (e.g. ad pixels), and anything that contradicts the privacy policy.
