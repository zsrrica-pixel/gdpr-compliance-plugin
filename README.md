# gdpr-compliance

A Claude Code plugin for GDPR work. Outputs are working drafts, not legal advice.

Skills: `dpia`, `ropa`, `privacy-policy-review`, `cookie-tracker-audit`, `dpa-review`, `breach-response`, `dsar-response`
Commands: `/gdpr-compliance:gdpr-check <path>`, `/gdpr-compliance:breach <incident>`

Test locally: `claude --plugin-dir ./gdpr-compliance`

## Install

From a local path:
```
/plugin marketplace add "C:/Users/zirlandia/OneDrive/Desktop/Business concept project/gdpr-compliance"
/plugin install gdpr-compliance@gdprgard-plugins
```
From GitHub (after pushing this folder as its own repo): `/plugin marketplace add <user>/<repo>`
