# Architecture

## High-level design

```mermaid
flowchart LR
  U[User / Telegram / Web Dashboard] --> H[Hermes Agent Runtime]
  H --> T[Tool Layer]
  T --> B[Visible Browser Automation]
  T --> G[Google Sheets / Gmail Workflows]
  T --> N[NotebookLM-style Research Extraction]
  T --> S[System Monitoring Scripts]
  H --> C[Scheduled Agents / Cron]
  C --> R[Reports and Alerts]
  R --> U
  H --> M[Persistent Memory / Skills / Session Store]
```

## Components

- **Linux VPS host:** Runs the self-hosted automation environment.
- **Hermes Agent runtime:** Core agent layer for tool-enabled tasks, scheduled jobs, sessions, and memory/skills.
- **Telegram interface:** Main delivery channel for reports, alerts, and task interaction.
- **Web dashboard:** Operational visibility for sessions, cron jobs, logs, models, usage, and system status.
- **Visible browser automation:** Used for workflows where web UI state matters and evidence is needed.
- **Google workflows:** Sheets/Gmail integration for tracking and operational data.
- **Research extraction:** YouTube/source review workflows using transcript/fulltext extraction and summarization.

## Engineering themes

- Human-in-the-loop operations where needed.
- Evidence-based automation: logs, screenshots, visible QA, and status reports.
- Token/cost awareness via summarization, session history, and scheduled workflows.
- Safe public/private separation: repo contains patterns and documentation, not private config.
