# gdpr-compliance

A [Claude Code](https://claude.com/claude-code) plugin for everyday GDPR work, from the team behind [GDPRGard](https://gdprgard.eu).

> **Not legal advice.** The skills produce working drafts and checklists to help you prepare and review. They are a summary of GDPR requirements, not a substitute for your DPO or a qualified lawyer. Check outputs before relying on them.

## Skills

| Skill | What it does |
|---|---|
| `dpia` | Screens whether a DPIA is needed (Art. 35) and drafts one |
| `ropa` | Builds or audits a Record of Processing Activities (Art. 30) |
| `privacy-policy-review` | Checks a privacy policy against Arts. 12-14 |
| `cookie-tracker-audit` | Audits a site's cookies, trackers and consent banner (ePrivacy Art. 5(3)) |
| `dpa-review` | Reviews a processor agreement against Art. 28 and drafts redlines |
| `breach-response` | Guides breach handling and the 72-hour notification (Arts. 33-34) |
| `dsar-response` | Handles data subject requests (Arts. 15-22) |

## Commands

- `/gdpr-compliance:gdpr-check <path or description>` - prioritised compliance review
- `/gdpr-compliance:breach <incident>` - start a breach response

## Install

```
/plugin marketplace add zsrrica-pixel/gdpr-compliance-plugin
/plugin install gdpr-compliance@gdprgard-plugins
```

Restart Claude Code (or run `/reload-plugins`) after installing. To try it without installing, clone the repo and run `claude --plugin-dir <path-to-clone>`.

## More

Free GDPR tools, guides and templates: [gdprgard.eu](https://gdprgard.eu)

## License

[MIT](LICENSE)
