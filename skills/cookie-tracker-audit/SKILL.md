---
name: cookie-tracker-audit
description: Audit a website's cookies, trackers and third-party scripts for GDPR/ePrivacy compliance. Use when the user gives a URL or site source and asks about cookies, consent banners, analytics, pixels or tracking.
---

# Cookie and tracker audit

1. **Collect evidence.** For a URL, load it with a browser tool if available (or fetch the HTML) and list: cookies set, localStorage keys, third-party domains, scripts, iframes, pixels, fonts and embeds. For local source, grep for `gtag`, `analytics`, `fbq`, `pixel`, `hotjar`, `clarity`, `<script src=`, `<iframe`, `document.cookie`, `localStorage`. Record what loads **before** any consent interaction separately from what loads after.
2. **Classify** each item: strictly necessary / preferences / statistics / marketing, with vendor and country of processing (flag non-EEA transfers).
3. **Check compliance** (ePrivacy Art. 5(3), GDPR Arts. 6-7, EDPB/CNIL guidance):
   - Non-essential items must not fire before opt-in.
   - Banner offers Reject as easily as Accept; no pre-ticked boxes; no cookie walls.
   - Granular choices per purpose; consent can be withdrawn as easily as given.
   - Cookie policy lists each cookie, purpose, duration and vendor.
   - Third-party embeds (YouTube, Maps, fonts) loaded without consent.
   - Consent records kept; retention of cookies reasonable (typically <= 13 months).
4. **Report** a table: item, category, fires pre-consent (Y/N), issue, fix. Then a prioritised fix list (High/Medium/Low).

State limits: a static check cannot prove behaviour after consent choices; say what was and was not tested. Working draft, not legal advice.

## Edge cases
- Local source with no consent logic (or a banner whose buttons have no handlers): treat everything non-essential as firing pre-consent and say so.
- Include non-item rows (banner, missing cookie policy) with "n/a" in the pre-consent column; mark uncertain results "Y (probable)" and explain (e.g. broken or stubbed snippets).
- Country of processing: from source alone, state the vendor's known entity and mark transfers "likely US" rather than asserting; unknown items are "Unclassified".
