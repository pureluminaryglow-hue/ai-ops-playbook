# 🤖 AI-Powered Team Management Automation Suite

> A collection of 22 platform-agnostic AI automation skills built for leadership and operations management. Each skill is a production-tested prompt that runs on **any AI assistant** — Claude, ChatGPT, Amazon Quick, Gemini, Copilot, or any LLM-powered platform.

## Author

**Tanita Vermeulen** — AI & Automation Operations Manager  
Built and refined in a live Amazon Customer Service Team Manager environment, managing a 20-person team with full operational accountability.

## What This Is

Each folder contains a **transferable automation skill** — a structured system prompt that turns any AI assistant into a specialised operations tool. These aren't theoretical templates. Every skill was built to solve a real operational problem and has run in production.

## Skills by Category

### 📊 Team Performance Management
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 01 | [Daily Operations Briefing](./01_daily_operations_briefing/) | Pre-shift summary combining calendar, actions, team health, and comms | Weekdays, before shift |
| 02 | [Team Health Dashboard](./02_team_health_dashboard/) | RAG-status team performance snapshot with prioritised action checklist | Weekdays, at shift start |
| 05 | [Manager Status Update](./05_manager_status_update/) | Automated daily upward report to your manager via chat | Weekdays, 1-2hr after start |
| 07 | [Weekly Coaching Notes](./07_weekly_coaching_notes/) | One structured coaching note per team member from real data | Weekly |
| 08 | [Team Member Data Refresh](./08_team_member_data_refresh/) | Auto-updates team member profiles from email, chat, and data sources | Every 2-3 hours |

### 📬 Communications & Triage
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 03 | [Communications Triage](./03_comms_triage/) | Monitors chat for items needing your attention, classifies by urgency | Every 15 minutes |
| 04 | [Email Classification & Routing](./04_email_triage/) | Classifies, tags, and routes inbox emails by category and priority | Twice daily |
| 15 | [Chat Channel Digest](./15_slack_channel_digest/) | Daily summary of channel decisions, action items, and blockers | Daily |
| 16 | [Team Email Monitor](./16_team_email_monitor/) | Surfaces team-relevant emails from shared mailboxes | Every 30 minutes |

### 🤝 Coaching & Development
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 06 | [1:1 Meeting Prep](./06_1on1_meeting_prep/) | Auto-generates prep brief when a 1:1 is 30 minutes away | Every 15 minutes |
| 07 | [Weekly Coaching Notes](./07_weekly_coaching_notes/) | Structured coaching documentation per team member | Weekly |

### 🏥 Attendance & Leave Management
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 09 | [Absence Scanner](./09_absence_scanner/) | Detects unplanned absences from chat and email | Daily, shift start |
| 10 | [Leave Case Monitor](./10_leave_case_monitor/) | Tracks leave/disability cases and flags RTW documentation needs | Weekdays |
| 14 | [Attendance Tracker Reminder](./14_attendance_tracker_reminder/) | Daily nudge to update attendance records | Weekdays |

### 🔍 Monitoring & Alerts
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 11 | [Ticket Monitor](./11_ticket_monitor/) | Watches a specific ticket until resolved, then alerts | Every 15 minutes |
| 12 | [Workflow Error Monitor](./12_workflow_error_monitor/) | Detects automation failures and suggests fixes | Every 15 minutes |

### 📁 Data Sync & Management
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 17 | [Local-to-Cloud File Sync](./17_folder_sync/) | Mirrors local folders to a cloud workspace | Weekdays |
| 18 | [Hourly Data Sync](./18_hourly_data_sync/) | High-frequency sync of local files and email attachments | Every 60 minutes |
| 19 | [Report File Sync](./19_acq_mining_file_sync/) | Extracts, converts, and files email report attachments | Weekly |
| 20 | [Full Daily Team Sync](./20_full_daily_team_sync/) | Consolidated daily sync: folders + email + profiles | Daily |

### 📋 Reporting & Compliance
| # | Skill | What It Does | Schedule |
|---|-------|-------------|----------|
| 13 | [Weekly Admin Checklist](./13_monday_admin_checklist/) | Sends structured admin checklist before weekly admin block | Weekly |
| 21 | [Weekly Tracker Report](./21_acq_mining_weekly_report/) | Parses a tracker file and generates a status report with metrics | Weekly |
| 22 | [ER/HR Interaction Tracker](./22_er_hr_interaction_capture/) | Auditable log of all HR/ER interactions across channels | Every 60 minutes |

## How to Use Any Skill

1. **Open the skill folder** → read `README.md` for context
2. **Copy `PROMPT.md`** → paste into your AI platform as a system prompt
3. **Replace `[PLACEHOLDERS]`** → swap in your team names, emails, file paths
4. **Run it** → manually or on your platform's schedule

## Platform Compatibility

| Platform | How to Use |
|----------|-----------|
| **Claude** | Projects → System Prompt |
| **ChatGPT** | Custom GPT → Instructions |
| **Amazon Quick** | Agent → Instructions, or Skill → SKILL.md |
| **Gemini** | Gems → Instructions |
| **Copilot** | Custom Copilot → System Message |
| **Any LLM API** | Pass as `system` message |

## Architecture Philosophy

These automations follow a consistent pattern:

```
┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│  Data Layer  │────▶│  AI Process  │────▶│   Output    │
│  (Sources)   │     │  (Classify,  │     │  (Alert,    │
│  Email/Chat/ │     │   Analyse,   │     │   Report,   │
│  Files/APIs  │     │   Synthesise)│     │   Update)   │
└─────────────┘     └──────────────┘     └─────────────┘
```

**Key principles:**
- **Evidence-based**: Never fabricate data. State "data unavailable" when sources are empty.
- **Actionable output**: Every output includes a clear next action, owner, and timeframe.
- **Least privilege**: Each automation only accesses what it needs.
- **Idempotent**: Safe to re-run. Won't duplicate notifications or corrupt data.

## License

MIT — free to use, modify, and distribute.

---

*Built with ❤️ by Tanita Vermeulen — proving that AI automation isn't about replacing leaders, it's about giving them superpowers.*
