# Employee Onboarding Automation (2)

## Overview
This comprehensive n8n workflow entirely automates the employee onboarding process. When a new hire is added to the system, AI tools evaluate the user's role and coordinate everything from creating an IT Jira ticket to booking orientation events, making pages on Notion, and notifying specific teams via Slack.

## Nodes Used
- **Webhook**: Entry point for a new employee being logged.
- **AI Agent / Chat Open AI**: Evaluates role requirements and required onboarding steps.
- **Jira**: Generates an IT equipment and setup ticket.
- **Slack (Multiple Notifications)**: Updates IT, Finance, HR Alerts, and Facilities (office setup / shipping equipment).
- **Google Calendar**: Creates an orientation or welcome event.
- **Notion**: Dynamically generates onboarding pages and checklists.
- **Gmail**: Sends welcome/manager emails.
- **Google Sheets**: Logs onboarding status tracking.
- **IF nodes & Merge**: Branching logic for office locations and aggregating flow branches.

## Setup Requirements
- OpenAI / AI tooling credentials
- Jira credentials
- Slack credentials
- Google OAuth (Gmail, Sheets, Calendar)
- Notion credentials
