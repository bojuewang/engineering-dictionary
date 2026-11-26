# Architecture

## Architectural principle

Keep meaning, normative rules, and reusable forms separate. A canonical concept has one authoritative home within the repository; other documents reference it.

```text
engineering-dictionary/
├── README.md
├── AGENTS.md
├── ARCHITECTURE.md
├── SPECIFICATION.md
├── CHANGELOG.md
├── dictionary/
│   └── engineering-terms.md
├── protocols/
│   ├── file-naming.md
│   ├── directory-naming.md
│   └── versioning.md
└── templates/
    ├── term.md
    └── protocol.md
```

| Layer | Question | Location |
| --- | --- | --- |
| Vocabulary | What does it mean? | `dictionary/` |
| Normative rules | What must or should we do? | `protocols/` |
| Reusable forms | How do we record an instance? | `templates/` |

The intended dependency is terminology → protocols → templates/usage. Root governance documents explain scope and link to the canonical files. Start with a consolidated glossary; split it into topic files when it becomes difficult to navigate. Add a machine-readable schema or automated checks only when there is a concrete consumer and an agreed data model. Git stores history; avoid parallel copies for ordinary versions.
