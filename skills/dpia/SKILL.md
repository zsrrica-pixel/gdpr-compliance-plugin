---
name: dpia
description: Conduct a Data Protection Impact Assessment (GDPR Art. 35) for a processing activity, product feature, or system. Use when the user asks whether a DPIA is needed or wants one drafted.
---

# DPIA

1. Gather: purpose, data categories, data subjects, recipients, transfers outside the EEA, retention, technology used (especially AI/profiling). Ask for anything missing.
2. Screening: check against the Art. 35(3) triggers and the EDPB's nine criteria (scoring, automated decisions, systematic monitoring, sensitive data, large scale, matching datasets, vulnerable subjects, new technology, blocking rights). Two or more criteria usually means a DPIA is required. State the verdict and why.
3. Draft the DPIA with these sections: systematic description; necessity and proportionality (lawful basis, minimisation, retention); risk assessment (likelihood x severity per risk to data subjects); mitigation measures; residual risk; DPO advice; Art. 36 prior consultation if residual risk stays high.
4. Mark any assumption clearly. This is a working draft for the controller or DPO to review, not legal advice.

## Scale and conflicts
- Rating scale: Likelihood and Severity each Low/Medium/High; level = the higher of the two unless both are Low. State that ratings are assumptions for the DPO to confirm.
- Borderline screening that hinges on unknown facts (e.g. "large scale", uploaded content): recommend treating the DPIA as required until answered, and list the deciding questions.
- When sources conflict (privacy notice vs. widget text vs. code), do not pick one: list each claim, its source, and mark it a transparency risk. Read relevant local source (backend function, widget) but cap the review to the data flow in question.
- End with open questions for the controller; do not invent facts.
