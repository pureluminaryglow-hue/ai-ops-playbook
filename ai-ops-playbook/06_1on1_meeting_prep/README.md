# 1:1 Meeting Prep Engine

> **Category:** Coaching & Development  
> **Schedule:** Every 15 minutes (triggers when a 1:1 is 30 minutes away)  
> **Platform:** Any AI assistant (Claude, ChatGPT, Amazon Quick, Gemini, Copilot, etc.)

## What It Does

Detects upcoming 1:1 meetings from the calendar and generates a prep brief from the team member's performance data, coaching history, and recent interactions.

## Who It's For

Managers with multiple direct reports who need contextual prep briefs before every 1:1 — automatically, without manual lookup.

## How to Use

### On Any AI Platform
1. Copy the contents of `PROMPT.md`
2. Paste it as a system prompt / custom instructions in your AI platform of choice
3. Replace all `[PLACEHOLDER]` values with your actual details (team names, email addresses, file paths, etc.)
4. Run manually or configure your platform's scheduling feature

### Placeholder Reference

| Placeholder | Description | Example |
|------------|-------------|---------|
| `[YOUR_NAME]` | Your full name | Jane Smith |
| `[YOUR_ALIAS]` | Your username/login | jsmith |
| `[YOUR_EMAIL]` | Your email address | jsmith@company.com |
| `[MANAGER_NAME]` | Your direct manager's name | John Doe |
| `[MANAGER_EMAIL]` | Your manager's email | jdoe@company.com |
| `[MANAGER_ALIAS]` | Your manager's username | jdoe |
| `[TEAM_NAME]` | Your team's name | Alpha Squad |
| `[TEAM_MEMBERS]` | Comma-separated list of team member usernames | alice, bob, charlie |
| `[CHANNEL_ID]` | Chat channel identifier | #team-general |
| `[DM_CHANNEL_ID]` | Direct message channel ID | DM with manager |
| `[LOCAL_FILE_PATH]` | Path to local data files | /Users/you/Documents/data/ |
| `[YOUR_WORKSPACE_ID]` | Cloud workspace/space ID | your-workspace-id |
| `[QUEUE_NAME]` | Your team's queue or workgroup | Support Queue A |
| `[BUSINESS_UNIT]` | Your business unit/org | Operations - EMEA |
| `[SITE_LOCATION]` | Your site or office location | London Office |

## Adapting This Skill

This skill was designed for a **Customer Service Team Manager** but the pattern is transferable to any leadership role:

- **Sales Leaders**: Replace performance metrics with pipeline/quota data
- **Engineering Leads**: Replace with sprint velocity, incident, and deployment data  
- **Operations Managers**: Replace with throughput, SLA, and capacity data
- **HR Business Partners**: Replace with headcount, attrition, and engagement data

## Files

| File | Purpose |
|------|---------|
| `README.md` | This file — overview and setup guide |
| `PROMPT.md` | The system prompt — copy into any AI platform |

## License

MIT — free to use, modify, and distribute.

---

*Originally built by [Tanita Vermeulen](https://github.com/YOUR_GITHUB) as part of an AI-powered Team Management automation suite.*
