# Quick Start — Chief of Staff to Steve Zanco

You have an AI Chief of Staff. This guide gets you up and running in 10 minutes.

---

## What This System Is

This is not a task manager. Not a note-taking app. Not another productivity system that you'll use for 3 weeks and abandon.

This is an operating system for your professional life — one that connects your role performance, your promotion path, your relationships, and your intelligence across 8 life domains. The AI knows your context. It holds the history. It connects the dots you don't have time to connect yourself.

**The Chief of Staff's job:** Surface what matters, challenge your thinking, hold you accountable, and make sure you're never caught unprepared.

**Your job:** Show up, be honest in your inputs, and use the commands consistently.

---

## Starting Each Day — /briefing

Every morning, before you open email, run:

```
/briefing
```

You'll get:
- **Top 3 priorities** — sorted by urgency x importance from your task list
- **Stale contacts** — anyone you haven't touched in longer than their tier threshold
- **Intelligence summary** — the most relevant recent items from your background research
- **Today's meetings** — with prep notes and what matters in each one
- **A challenge question** — something worth sitting with before the day starts

This takes 5 minutes to read. It replaces 30 minutes of scattered mental preparation.

**Pro tip:** Run /briefing before checking any other communication. Context before reaction.

---

## Ending Each Day — /debrief

Every evening (or after a significant event), run:

```
/debrief
```

You'll be asked:
1. What happened today that matters?
2. What decisions did you make or witness?
3. Who did you connect with?
4. What should be remembered for next time?
5. Any wins? Any misses?

The Chief of Staff then:
- Updates contact records for anyone you mentioned
- Logs decisions to decisions.json
- Captures meeting outcomes
- Flags patterns ("This is the third time you've mentioned this tension...")

**Why this is the most important habit in the system:** The evidence file for your Director promotion builds in /debrief. Decisions logged, relationships tracked, outcomes captured. Over 18 months, that's your promotion case.

Even a 5-minute /debrief is better than skipping it.

---

## Adding Tasks — /add-task

When something comes up that needs to happen:

```
/add-task [brief description]
```

You'll be prompted for:
- Which of the 8 domains it belongs to
- Urgency (1–5) and importance (1–5)
- Due date
- Related contacts or intel

Tasks are sorted by urgency x importance. The 5/5 tasks always surface first in your briefing. The 1/1 tasks sit in the list until you're ready.

**The rule:** If it matters, it goes in the system. If it's in your head only, it competes with everything else in your head.

---

## Adding Intelligence — /add-intel

When you read something, hear something, or learn something worth remembering:

```
/add-intel [topic] [what you learned]
```

The system captures the source, tags it by domain, and cross-references it. If it's construction market news, it'll flag any stale Tier 1 customers who should hear about it. If it's a competitor move, it'll connect it to any related open tasks.

**Background research runs automatically** (construction market every 3 days, sales leadership every 7 days, career opportunities every 14 days) and adds items to the intelligence file. You'll see the summary in your morning /briefing.

---

## Reviewing a Domain — /domain-review

When you want to go deep on one area of your life:

```
/domain-review inside-sales
/domain-review career-growth
/domain-review leadership-team
/domain-review side-projects
/domain-review health-wellness
/domain-review learning-development
/domain-review family-relationships
/domain-review finance-investments
```

You'll get a full picture: current tasks, recent decisions, key contacts and their status, recent intelligence, and suggested next actions. Closes with an accountability question you should answer honestly.

Run one domain review per week minimum. The domains you avoid reviewing are usually the ones that need it most.

---

## The Dashboard — /dashboard

For the weekly review or when you want the full picture:

```
/dashboard
```

Shows you:
- Task health by domain (open, in-progress, overdue)
- Contact health by tier (how many stale in each tier)
- Intelligence items from the last 7 days
- Decisions logged in the last 30 days
- Domain health summary — green/yellow/red with a one-liner for each

Run this every Monday morning or at the end of the week to calibrate.

---

## Data Files Explained

Your data lives in the `/data` directory. **This directory is gitignored — it never gets committed.** It's your private operational data.

| File | What it holds |
|------|--------------|
| `tasks.json` | All tasks across all domains |
| `contacts.json` | Every contact with tier, last touch, relationship notes |
| `decisions.json` | Every logged decision with context and outcomes |
| `meetings.json` | Meeting records with prep notes and outcomes |
| `intelligence.json` | Market intel, research, conversation captures |

**Why gitignored:** This data is sensitive. Customer names, internal decisions, personal financial notes — none of that belongs in version control. The code (CLAUDE.md, domain files, frameworks) is safe to commit. The data is not.

**Backing up your data:** Copy the `/data` directory to a secure location regularly. If you lose it, you lose your history.

---

## Contact Tiers — How They Work

Every contact in contacts.json has a tier. The tier determines how often the Chief of Staff flags them as stale.

| Tier | Staleness Threshold | Who Belongs Here |
|------|--------------------|--------------------|
| 1 | 14 days | Boss, boss's boss, exec sponsors, top customers, key internal partners |
| 2 | 30 days | Important customers, peer managers, warm prospects, mentors |
| 3 | 60 days | Past customers, network contacts, industry connections, references |

**The key insight:** Being "stale" doesn't mean the relationship is bad. It means enough time has passed that you should reach out. The system catches the drift before it becomes a dead relationship.

**Adding a contact:**
```
/debrief
```
When you mention someone you spoke to, the Chief of Staff prompts you to add or update them in contacts.json.

---

## The 8 Domains

Your life is organized into 8 domains. Every task, contact, and piece of intelligence belongs to at least one.

| Domain | What It Covers |
|--------|---------------|
| `inside-sales` | Day job performance, team results, pipeline |
| `career-growth` | Promotion path, skills, executive visibility |
| `leadership-team` | Boss, peers, exec stakeholders, your team's health |
| `side-projects` | Skatepark Respect + consulting work |
| `health-wellness` | Energy, fitness, sleep, stress management |
| `learning-development` | Reading, courses, skill-building |
| `family-relationships` | Commitments, presence, important dates |
| `finance-investments` | Income, investments, financial goals |

The domain structure prevents the problem where work consumes everything and you only notice you've neglected other areas when the damage is done.

---

## Getting the Most Out of the System

**Do these things:**
- Run /briefing every morning before email
- Run /debrief every evening, even if it's just 5 minutes
- Log every significant decision in /debrief (they become your promotion case)
- Add contacts as you meet people — don't let them fall out of the system
- Log intel when you read or hear something relevant — it compounds

**Avoid these failure modes:**
- Running /briefing but not acting on what it surfaces
- Skipping /debrief when the day was hard (those are the most important ones to capture)
- Letting the intelligence file fill up without reviewing it
- Using this as a to-do list instead of an operating system (strategy > task management)

**The system gets smarter as you use it.** The more you put in — decisions, contacts, intel — the more it can cross-reference and surface connections you wouldn't catch on your own.

---

## Framework Files

The `/frameworks` directory has four frameworks to help Steve operate at a higher level:

| File | What It's For |
|------|--------------|
| `ai-evaluation.md` | Scoring matrix for evaluating AI tools and vendors |
| `stakeholder-communication.md` | How to communicate with each audience type |
| `executive-narrative.md` | Building and deploying the Director promotion case |
| `team-capability-matrix.md` | Assessing and developing sales reps |

These aren't reference documents to read once. They're operational tools. Open `executive-narrative.md` before every performance review. Open `team-capability-matrix.md` at the start of each quarter.

---

## Domain Files

The `/domains` directory has a file for each of Steve's 8 life areas. These contain:
- Role overview and success criteria
- Key metrics to track
- Current priorities and quarterly objectives
- Frameworks for common decisions in that domain
- Notes section for ongoing observations

Review the relevant domain file before any major conversation, meeting, or decision in that area.

---

## One Last Thing

The most important thing about this system is also the simplest: **use it consistently.**

The Chief of Staff can't surface patterns from data that wasn't captured. It can't cross-reference contacts you didn't add. It can't flag a stale relationship you never logged.

The daily investment is small — 5 minutes for /briefing, 5-10 minutes for /debrief. The compounding return over 18 months is the promotion case, the relationship history, the decision record, and the market intelligence that makes Steve the most prepared person in any room.

Start today.

---

*Questions about what to enter somewhere? Just describe what happened and the system will help you route it.*
