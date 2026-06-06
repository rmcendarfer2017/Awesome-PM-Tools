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

### [Backlog Groomer](https://github.com/rmcendarfer2017/backlog-groomer)

An AI-powered backlog grooming tool that connects to your Jira backlog, scores every ticket using a structured prioritization framework, and surfaces the housekeeping work — duplicates, stale tickets, enrichment gaps — that quietly degrades backlog quality over time.

**What it does:**
- Fetches your Jira backlog and runs a housekeeping sweep: merge candidates, stale tickets, enrichment rewrites, and theme orphans
- Scores every ticket across four dimensions — quality, freshness, theme alignment, and similarity — and produces a ranked priority table
- Surfaces coordination flags (compliance, security, legal, partner dependencies) alongside scores without deflating them
- Provides an interactive table sortable by any scoring dimension with hover-to-expand score breakdowns

**Key features:**
- Jira REST API integration — connect with an API token, no plugins required
- Demo mode — load 12 pre-built tickets to explore the full feature set without a Jira account
- Layer 1 scoring — composite priority score with visible dimension breakdown so every ranking has a reason
- Coordination flags — Light / Moderate / Significant overhead flags shown separately from the score
- Claude.ai skill — also available as a `/backlog-groomer` slash command for teams already using Claude Chat with Jira connected

**Also available as a Claude.ai skill:** For PMs already using Claude.ai with Jira MCP connected, the `skill/` folder contains a custom slash command that delivers the same housekeeping sweep and scoring directly in a Claude Chat conversation — no separate app required.

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
