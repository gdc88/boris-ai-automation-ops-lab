# Sanitized case studies

## 1. Job-search operations assistant

Problem: Job search across multiple sources creates duplicate tracking, missed updates, and repetitive manual checking.

Approach:

- Scheduled scans and source checks.
- Candidate extraction and manual-verification status.
- Google Sheet tracker as source of truth.
- Telegram reports with clickable role URLs and next actions.

Value:

- Less manual scanning.
- Better audit trail.
- Faster review of promising roles.

## 2. Personal radar / research briefing

Problem: Important AI, relocation, job-market, and infrastructure signals are spread across many sources.

Approach:

- Scheduled source monitoring.
- Summary reports grouped by actionability.
- Telegram delivery.
- Optional deep extraction for long videos/articles.

Value:

- Converts noisy information streams into practical actions.

## 3. Visible-browser QA and web workflows

Problem: Some tasks cannot be validated only from API text; visible browser state matters.

Approach:

- Browser interaction with screenshots/recording when needed.
- Contact-sheet review and visible-state verification.
- Reports listing what was visibly proven and what was not.

Value:

- Better reliability for authenticated web workflows and UI-dependent tasks.

## 4. Infrastructure monitoring and maintenance

Problem: VPS-hosted automation needs monitoring and cautious updates.

Approach:

- Health reports for disk, services, processes, dashboard status.
- Guarded update workflow with verification before and after changes.
- Service restart discipline and failure reporting.

Value:

- Automation remains useful without becoming fragile.
