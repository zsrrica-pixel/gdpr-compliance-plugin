---
name: privacy-policy-review
description: Review a privacy policy or notice against GDPR Arts. 12-14 transparency requirements. Use when the user shares a privacy policy, website, or notice to check.
---

# Privacy policy review

Check the document for each Art. 13/14 element and mark Present / Weak / Missing:

- Controller identity and contact, DPO contact
- Purposes and lawful basis for each purpose; legitimate interests explained
- Recipients or categories of recipients
- International transfers and safeguards
- Retention periods (or criteria)
- Data subject rights (access, rectification, erasure, restriction, portability, objection, withdraw consent) and right to complain to a supervisory authority
- Whether providing data is mandatory; consequences of not providing
- Automated decision-making/profiling information
- Source of data (if not collected from the subject)

Also check plain language, easy accessibility, cookie/tracking disclosures, and date/version. Output a findings table and suggested replacement wording for each gap.

## Method and format
- **Read the verbatim text.** For a URL use a browser tool and read the page text (not a summarising fetch); if only a summary is available, say so and treat every "Missing" as "verify on the live page".
- **Status:** Present = element stated clearly. Weak = stated but vague, wrong basis, or incomplete (e.g. legitimate interest named but not explained). Missing = absent.
- **Also check ePrivacy/cookie disclosures** (cookie-by-cookie table, withdrawal route) and cross-check the policy against what the site actually loads (see `cookie-tracker-audit`) and what it sells or collects (payments, forms, AI tools).
- **Output:** table (element, status, finding, priority High/Medium/Low), then replacement wording per gap with `[placeholders]` only where a fact is unknown.
