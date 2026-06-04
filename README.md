# Awesome PM Tools

A curated collection of open-source tools built for Product Managers.

---

## Tools

### [Feedback-Synthesis](https://github.com/rmcendarfer2017/Feedback-Synthesis)

A local AI-powered tool for synthesizing user feedback from Obsidian vaults using Claude.

**What it does:**
- Scans a folder of Obsidian markdown notes and organizes them into vaults
- Filters feedback by source type, date range, and tags
- Sends filtered notes to Claude and streams back a structured synthesis report with themes, sentiment, recommendations, and evidence quotes

**Key features:**
- Source filter — narrow to `user-interview`, `nps`, `support-ticket`, `sales-call`, or `survey`
- Date range filter — scope synthesis to a specific time window
- Tag filter — focus on specific topic areas
- Guided onboarding — walks you through API key setup, vault connection, and note structure
- Works with any Obsidian vault — no plugins required

**Note structure:** Notes use YAML frontmatter to unlock filtering:
```markdown
---
date: 2026-05-14
source: user-interview
sentiment: 2
tags: [onboarding, mobile]
participant: "SMB / 12 seats"
---
Your note body here.
```

---

## Getting Started

Each tool lives in its own subdirectory as an independent repository. Clone with submodules to get everything:

```bash
git clone --recurse-submodules https://github.com/rmcendarfer2017/Awesome-PM-Tools.git
```

Or if you already cloned without submodules:

```bash
git submodule update --init --recursive
```

Then follow the setup instructions in each tool's own README.

---

## Contributing

Have a PM tool to add? Open a PR or file an issue.
