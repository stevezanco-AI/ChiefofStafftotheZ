# Tool 1: Team Chief of Staff
**Tagline:** Every rep on your team gets the same AI-powered support system you use — personalized to their role, goals, and development.

---

## What It Is

A scaled version of Steve's own Chief of Staff system, deployed for each of the 19 team members. Each rep gets an AI system that:
- Tracks their personal goals and development areas
- Surfaces coaching prompts before 1:1s
- Captures wins and challenges in real time
- Helps them prepare for customer calls and difficult conversations
- Gives Steve a consistent view of team health across all 19 people

**This is not generic AI.** Each instance is personalized: the rep's role, their current performance focus, their development stage, their career goals.

---

## Why This Matters

**For Gallup:** Employee engagement rises when people feel seen, supported, and developed. A rep who has a tool that helps them grow — one their manager built specifically for them — feels invested in.

**For Steve:** 19 reps across a large territory is hard to coach consistently at depth. This system creates coaching leverage — each rep is getting structured development between 1:1s, not just during them.

**For the business:** Reps who develop faster perform faster. The team's operational metrics (NPS, order accuracy, call answer rate) improve when reps are better prepared and more confident.

---

## How It Works

### For Each Rep — What They Get

A personal CLAUDE.md-style profile containing:
- Their role and current responsibilities
- Performance focus areas (what they're working on this quarter)
- Development goals (skill they're building)
- Communication style and coaching preferences
- Current challenges and wins log

**Daily use pattern:**
```
Rep: "Help me prep for my call with [customer] at 2pm"
AI: [Pulls context on the customer, surfaces relevant talking points, flags any open issues]

Rep: "I just had a tough conversation with a customer — here's what happened"
AI: [Captures the debrief, surfaces the lesson, notes it for their development log]

Rep: "What should I focus on this week?"
AI: [Surfaces their goals, open items, upcoming priorities]
```

### For Steve — What He Gets

Before every 1:1, a prep brief for each rep:
- What they've been working on since last touch
- Wins to recognize (specifically)
- Development focus to coach on
- Any flags (stale customers, open challenges, mood signals)

This means Steve's 1:1s are substantive every time — not "what's going on?" but "I see you closed the Hendricks account — what made that work?"

---

## Build Approach

**Phase 1 — Foundation (2 weeks)**
- Create template CLAUDE.md profile structure for a rep (simpler than Steve's — role-focused, not 8 domains)
- Build for 2-3 pilot reps who are already engaged and growth-oriented
- Steve onboards them personally — this is a coaching conversation, not a tech rollout

**Phase 2 — Data structure (1 week)**
- Simple JSON files per rep: goals, wins_log, challenges_log, customer_contacts
- Gitignored (private per rep)
- Steve has read access to summary view; full files belong to the rep

**Phase 3 — Team rollout (2-3 weeks)**
- Roll out to full team of 19, one cohort at a time
- Pair rollout with a team meeting on "how we use AI to grow"
- Frame it as a development investment, not a monitoring tool

**Phase 4 — 1:1 intelligence layer (ongoing)**
- Steve's pre-1:1 brief auto-generates from each rep's recent entries
- Pattern flags: rep hasn't logged in 5+ days, rep is only logging challenges (no wins), etc.

---

## Files to Build

```
/team-cos/
  template/
    CLAUDE.md          ← Rep-facing AI profile template
    goals.json         ← Development goals structure
    log.json           ← Wins/challenges capture structure
  reps/
    [rep-name]/        ← One folder per rep (gitignored)
      CLAUDE.md        ← Personalized profile
      goals.json
      log.json
  steve-view/
    1on1-prep.md       ← Auto-generated pre-1:1 brief format
```

---

## Success Metrics

| Metric | Baseline | Target | Timeline |
|--------|---------|--------|----------|
| Gallup engagement score | [Current] | +X points | Q4 2026 |
| Rep-reported development clarity | [Survey] | Improved | 90 days |
| 1:1 quality (Steve's assessment) | Subjective | Measurably more substantive | 60 days |
| Rep performance on focus skill | [Baseline] | Measurable improvement | 90 days |

---

## The Pitch to Zack

> "I'm building a personalized AI development system for each of my 19 reps — the same kind of system I use to manage my own priorities. It gives every person on the team a consistent coaching experience between 1:1s, and it makes my 1:1s dramatically more effective. I think it directly addresses our Gallup engagement goals and our development gaps."
